# Comparing `tmp/checkpoint_tool-0.3.0.tar.gz` & `tmp/checkpoint_tool-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpoint_tool-0.3.0.tar", max compression
+gzip compressed data, was "checkpoint_tool-0.3.1.tar", max compression
```

## Comparing `checkpoint_tool-0.3.0.tar` & `checkpoint_tool-0.3.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3308 2023-04-27 00:24:50.167733 checkpoint_tool-0.3.0/README.md
--rw-r--r--   0        0        0    15489 2023-04-27 00:45:24.936478 checkpoint_tool-0.3.0/checkpoint.py
--rw-r--r--   0        0        0      644 2023-04-27 00:46:57.918529 checkpoint_tool-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4087 1970-01-01 00:00:00.000000 checkpoint_tool-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3319 2023-04-28 05:20:08.672000 checkpoint_tool-0.3.1/README.md
+-rw-r--r--   0        0        0    15938 2023-04-28 13:15:25.736513 checkpoint_tool-0.3.1/checkpoint.py
+-rw-r--r--   0        0        0      662 2023-04-28 13:19:26.337203 checkpoint_tool-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4135 1970-01-01 00:00:00.000000 checkpoint_tool-0.3.1/PKG-INFO
```

### Comparing `checkpoint_tool-0.3.0/README.md` & `checkpoint_tool-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Checkpoint-tool
 A lightweight workflow management tool written in pure Python.
 
-Internally, it depends on `DiskCache`, `cloudpickle` and `concurrent.futures`.
+Internally, it depends on `DiskCache`, `cloudpickle` `networkx` and `concurrent.futures`.
 
 
 ### Installation
 ```
 pip install checkpoint-tool
 ```
```

### Comparing `checkpoint_tool-0.3.0/checkpoint.py` & `checkpoint_tool-0.3.1/checkpoint.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,37 @@
+""" A lightweight workflow management tool.
+
+TODO:
+    - Priority-based scheduling
+"""
 from __future__ import annotations
+from typing import Callable, ClassVar, Generic, NewType, TypeVar, Any, cast, overload
+from typing_extensions import ParamSpec, Concatenate, Self
+from collections import defaultdict
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Callable, Generic, NewType, Type, TypeVar, Any, cast, overload
-from typing_extensions import ParamSpec, Concatenate, Self
-import os
 from pathlib import Path
-import copy
-
-import logging
-import cloudpickle
-import zlib
-import diskcache as dc
-
 from concurrent.futures import ProcessPoolExecutor, Future, wait, FIRST_COMPLETED, Executor
 from functools import wraps
+import os
+import logging
 import inspect
 import json
 
+import cloudpickle
+import zlib
+import diskcache as dc
+import networkx as nx
+
 
 CHECKPOINT_PATH = Path(os.getenv('CP_CACHE_DIR', './.cache')) / 'checkpoint'
 CHECKPOINT_PATH.mkdir(parents=True, exist_ok=True)
 
 
-LOGGER = logging.getLogger(__file__)
+LOGGER = logging.getLogger(__name__)
 
 
 Json = NewType('Json', str)
 
 
 K = TypeVar('K')
 T = TypeVar('T')
@@ -37,40 +42,42 @@
 
 Serializer = tuple[Callable[[Any], bytes], Callable[[bytes], Any]]
 DEFAULT_SERIALIZER: Serializer = (cloudpickle.dumps, cloudpickle.loads)
 
 
 @dataclass(frozen=True)
 class Database(Generic[T, D]):
-    path: str
+    name: str
     compress_level: int
     result_cache: dc.Cache
     timestamp_cache: dc.Cache
     serializer: Serializer = DEFAULT_SERIALIZER
 
     @classmethod
-    def make(cls, path: str, compress_level: int) -> Self:
+    def make(cls, name: str, compress_level: int) -> Self:
+        base_path = str(CHECKPOINT_PATH / name)
         return Database(
-                path=path,
+                name=name,
                 compress_level=compress_level,
-                result_cache=dc.Cache(path + '/result'),
-                timestamp_cache=dc.Cache(path + '/timestamp'),
+                result_cache=dc.Cache(base_path + '/result'),
+                timestamp_cache=dc.Cache(base_path + '/timestamp'),
                 )
 
     def _dumps(self, obj: Any) -> bytes:
         dumps, _ = self.serializer
         return zlib.compress(dumps(obj), level=self.compress_level)
 
     def _loads(self, data: bytes) -> Any:
         _, loads = self.serializer
         return loads(zlib.decompress(data))
 
     def save(self, key: Json, obj: T) -> datetime:
+        data = self._dumps(obj)
         with self.result_cache as ref:
-            ref[key] = self._dumps(obj)
+            ref[key] = data
 
         timestamp = datetime.now()
         with self.timestamp_cache as ref:
             ref[key] = timestamp.timestamp()
         return timestamp
 
     def load(self, key: Json) -> T:
@@ -104,69 +111,94 @@
                 del ref[key]
 
 
 Runner = Callable[[], R]  # Delayed computation
 RunnerFactory = Callable[P, Runner[R]]
 
 
+TaskKey = tuple[str, Json]
+
+
 @dataclass(frozen=True)
-class Task(Generic[R]):
-    """ Runner with cache """
-    runner: Runner[R]
+class TaskSkeleton(Generic[R]):
     task_factory: TaskFactory[..., R]
     key: Json
-    timestamp: datetime | None
 
-    def set_result(self) -> None:
-        db = self.task_factory.db
-        out = self.runner()
-        db.save(self.key, out)
+    _register: ClassVar[dict[TaskKey, Runner[Any]]] = dict()
+
+    def to_tuple(self) -> TaskKey:
+        return self.task_factory.get_db_name(), self.key
 
     def get_result(self) -> R:
         db = self.task_factory.db
         return db.load(self.key)
 
+    def clear(self) -> None:
+        db = self.task_factory.db
+        db.delete(self.key)
+
+    def peek_timestamp(self) -> datetime | None:
+        try:
+            return self.task_factory.db.load_timestamp(self.key)
+        except KeyError:
+            return None
+
+    def load_content(self, loader: RunnerFactory[[], R]) -> Task[R]:
+        is_root = not self._register
+
+        key = self.to_tuple()
+        runner = self._register.get(key, None)
+        if runner is None:
+            runner = loader()
+            self._register[key] = runner
+        task = Task(task_factory=self.task_factory, key=self.key, runner=runner)
+
+        if is_root:
+            self._register.clear()
+        return task
+
+
+@dataclass(frozen=True)
+class Task(TaskSkeleton[R]):
+    """ Runner with cache """
+    runner: Runner[R]
+
+    def set_result(self) -> None:
+        db = self.task_factory.db
+        out = self.runner()
+        db.save(self.key, out)
+
     def run(self, *, executor: Executor | None = None) -> R:
         return self.run_with_info(executor=executor)[0]
 
     def run_with_info(self, *, executor: Executor | None = None, dump_generations: bool = False) -> tuple[R, dict[str, Any]]:
-        graph = Graph.build(self)
+        graph = TaskGraph.build_from(self)
         if executor is None:
             executor = ProcessPoolExecutor()
         info = run_task_graph(graph=graph, executor=executor, dump_generations=dump_generations)
         return self.get_result(), info
 
-    def clear(self) -> None:
-        db = self.task_factory.db
-        db.delete(self.key)
-
-    def to_tuple(self) -> tuple[str, Json]:
-        return self.task_factory.get_db_path(), self.key
-
 
 @dataclass
 class TaskFactory(Generic[P, R]):
     runner_factory: RunnerFactory[P, R]
     db: Database
     max_concurrency: int | None
+    is_building_graph: ClassVar[bool] = False
 
-    def get_db_path(self) -> str:
-        return self.db.path
+    def get_db_name(self) -> str:
+        return self.db.name
 
     def clear(self) -> None:
         self.db.clear()
 
     def __call__(self, *args: P.args, **kwargs: P.kwargs) -> Task[R]:
-        runner = self.runner_factory(*args, **kwargs)
         key = _serialize_arguments(self.runner_factory, *args, **kwargs)
-        try:
-            timestamp = self.db.load_timestamp(key)
-        except KeyError:
-            timestamp = None
-        return Task(runner, task_factory=self, key=key, timestamp=timestamp)
+        dummy = TaskSkeleton(task_factory=self, key=key)
+        return dummy.load_content(loader=lambda: self.runner_factory(*args, **kwargs))
 
 
 @overload
 def task(fn: RunnerFactory[P, R]) -> TaskFactory[P, R]: ...
 @overload
 def task(*, compress_level: int = 0, max_concurrency: int | None = None) -> Callable[[RunnerFactory[P, R]], TaskFactory[P, R]]: ...
 def task(*args, **kwargs) -> Any:
@@ -179,19 +211,20 @@
 
 def _task(
         *, compress_level: int = 0, max_concurrency: int | None = None
         ) -> Callable[[RunnerFactory[P, R]], TaskFactory[P, R]]:
     """ Convert a runner factory into a task factory. """
 
     def decorator(fn: RunnerFactory[P, R]) -> TaskFactory[P, R]:
-        db_path = str(CHECKPOINT_PATH / _serialize_function(fn))
-        db = Database.make(path=db_path, compress_level=compress_level)
-        return wraps(fn)(
-                TaskFactory(runner_factory=fn, db=db, max_concurrency=max_concurrency)
-                )
+        name = _serialize_function(fn)
+        db = Database.make(name=name, compress_level=compress_level)
+        return wraps(fn)(TaskFactory(
+            runner_factory=fn, db=db,
+            max_concurrency=max_concurrency
+            ))
     return decorator
 
 
 def _serialize_function(fn: Callable[..., Any]) -> str:
     return f'{fn.__module__}.{fn.__qualname__}'
 
 
@@ -287,182 +320,185 @@
 def requires_dict(tasks: dict[K, Task[T]]) -> Connector[dict[K, T], P, R]:
     """ Register a task dependency """
     def decorator(fn: Callable[Concatenate[dict[K, T], P], R]) -> Callable[P, R]:
         return DictConnected(tasks, fn)
     return decorator
 
 
-def get_upstream(task: AnyTask) -> list[AnyTask]:
+def get_prerequisite_tasks(task: AnyTask) -> list[AnyTask]:
     deps: list[Task[Any]] = []
     task_fn = task.runner
     while isinstance(task_fn, (Connected, ListConnected, DictConnected)):
         deps.extend(task_fn.get_tasks())
         task_fn = task_fn.fn
     return deps
 
 
 @dataclass
-class Graph:
-    root: Task[Any]
-    timestamp: datetime | None  # None indicate update is needed.
-    downstream: Task[Any] | None
-    upstream_graphs: list[Graph]
+class TaskGraph:
+    G: nx.DiGraph
 
     @classmethod
-    def build(cls, task: Task[Any], downstream: Task[Any] | None = None) -> Self:
-        upstream_graphs = [Graph.build(t, downstream=task) for t in get_upstream(task)]
-        timestamp = task.timestamp
-        if timestamp is not None:
-            upstream_timestamps = [ug.timestamp for ug in upstream_graphs]
-            need_update = any(uts is None or timestamp < uts for uts in upstream_timestamps)
-            if need_update:
-                timestamp = None
-
-        out = Graph(
-                root=task,
-                timestamp=timestamp,
-                downstream=downstream,
-                upstream_graphs=upstream_graphs,
-                )
+    def build_from(cls, root: AnyTask) -> Self:
+        G = nx.DiGraph()
+        seen: set[TaskKey] = set()
+        to_expand = [root]
+        while to_expand:
+            task = to_expand.pop()
+            x = task.to_tuple()
+            if x not in seen:
+                seen.add(x)
+                prerequisite_tasks = get_prerequisite_tasks(task)
+                to_expand.extend(prerequisite_tasks)
+                G.add_node(x, task=task, timestamp=task.peek_timestamp())
+                G.add_edges_from([(p.to_tuple(), x) for p in prerequisite_tasks])
+        out = TaskGraph(G)
+        out.trim()
         return out
 
-
-def walk_subgraph_to_update(graph: Graph) -> list[Graph]:
-    out: list[Graph] = []
-    to_expand: list[Graph] = [graph]
-    while to_expand:
-        g = to_expand.pop()
-        if g.timestamp is None:
-            out.append(g)
-            to_expand.extend(g.upstream_graphs)
-    return out
+    @property
+    def size(self) -> int:
+        return len(self.G)
+
+    def get_task(self, key: TaskKey) -> AnyTask:
+        return self.G.nodes[key]['task']
+
+    def trim(self) -> None:
+        self._mark_fresh_nodes()
+        self._remove_fresh_nodes()
+        self._transitive_reduction()
+
+    def _mark_fresh_nodes(self) -> None:
+        for x in nx.topological_sort(self.G):
+            ts0 = self.G.nodes[x]['timestamp']
+            if ts0 is None:
+                self.G.add_node(x, fresh=False)
+                continue
+            for y in self.G.predecessors(x):
+                fresh_y = self.G.nodes[y]['fresh']
+                ts = self.G.nodes[y]['timestamp']
+                if not fresh_y or ts is None or ts > ts0:
+                    self.G.add_node(x, fresh=False)
+                    break
+            else:
+                self.G.add_node(x, fresh=True)
+
+    def _remove_fresh_nodes(self) -> None:
+        to_remove = [x for x, attr in self.G.nodes.items() if attr['fresh']]
+        for x in to_remove:
+            self.G.remove_node(x)
+
+    def _transitive_reduction(self) -> None:
+        TR = nx.transitive_reduction(self.G)
+        TR.add_nodes_from(self.G.nodes(data=True))
+        self.G = TR
+
+    def get_task_factories(self) -> dict[str, TaskFactory[..., Any]]:
+        return dict((path, attr['task'].task_factory) for (path, _), attr in self.G.nodes.items())
+
+    def get_initial_tasks(self) -> list[TaskKey]:
+        return [x for x in self.G if self.G.in_degree(x) == 0]
+
+    def pop_with_new_leaves(self, x: TaskKey, disallow_non_leaf: bool = True) -> list[TaskKey]:
+        if disallow_non_leaf:
+            assert not list(self.G.predecessors(x))
+
+        new_leaves: list[TaskKey] = []
+        for y in self.G.successors(x):
+            if self.G.in_degree(y) == 1:
+                new_leaves.append(y)
+
+        self.G.remove_node(x)
+        return new_leaves
+
+    def get_grouped_nodes(self) -> dict[str, list[Json]]:
+        out: dict[str, list[Json]] = defaultdict(list)
+        for x in self.G:
+            path, args = x
+            out[path].append(args)
+        return dict(out)
+
+
+def _group_nodes_by_db(tasks: list[TaskKey]) -> dict[str, list[TaskKey]]:
+    out = defaultdict(list)
+    for x in tasks:
+        db, _ = x
+        out[db].append(x)
+    return dict(out)
 
 
-def run_task_graph(graph: Graph, executor: Executor, dump_generations: bool = False) -> dict[str, Any]:
+def run_task_graph(graph: TaskGraph, executor: Executor, dump_generations: bool = False) -> dict[str, Any]:
     """ Consume task graph concurrently.
     """
-    info = {'stats': {}, 'generations': []}
-
-    active_subgraphs = walk_subgraph_to_update(graph)
-
-    # Parse graph in a flat format
-    Key = tuple[str, Json]
-    nodes: dict[Key, AnyTask] = {g.root.to_tuple(): g.root for g in active_subgraphs}
-    task_factories: dict[str, TaskFactory[..., Any]] = {k[0]: nodes[k].task_factory for k in nodes}
-
-    descendants: dict[Key, set[Key]] = {}
-    precedents: dict[Key, set[Key]] = {}
-    node_groups: dict[str, set[Json]] = {}
-    for g in active_subgraphs:
-        root_key = g.root.to_tuple()
-        assert nodes[root_key].to_tuple() == root_key
-        assert task_factories[g.root.task_factory.get_db_path()] is g.root.task_factory
-
-        # Aggregate downsteram
-        downstream_keys = set() if g.downstream is None else {g.downstream.to_tuple()}.intersection(nodes)
-        if root_key not in descendants:
-            descendants[root_key] = downstream_keys
-        else:
-            descendants[root_key].update(downstream_keys)
-
-        # Upstream should be the same if the root is the same
-        upstream_keys = set(ug.root.to_tuple() for ug in g.upstream_graphs).intersection(nodes)
-        if root_key not in precedents:
-            precedents[root_key] = upstream_keys
-        else:
-            assert precedents[root_key] == upstream_keys, 'Same tasks have to have the same upstream'
-
-        # Group nodes by db_path
-        path, arg_key = root_key
-        if path not in node_groups:
-            node_groups[path] = {arg_key}
-        else:
-            node_groups[path].add(arg_key)
-
-    stats = {k: len(args) for k, args in node_groups.items()}
+    stats = {k: len(args) for k, args in graph.get_grouped_nodes().items()}
     LOGGER.info(f'Following tasks will be called: {stats}')
-    info['stats'] = stats
+    info = {'stats': stats, 'generations': []}
 
     # Read concurrency budgets
     budgets: dict[str, int] = {}
     occupied: dict[str, int] = {}
-    for path in node_groups:
-        mc = task_factories[path].max_concurrency
+    for path, fac in graph.get_task_factories().items():
+        mc = fac.max_concurrency
         if mc is not None:
             budgets[path] = mc
             occupied[path] = 0
 
-    # Collect leaf nodes by groups
-    leaves: dict[str, list[Json]] = {
-            path: [k for k in keys if not precedents[path, k]]
-            for path, keys in node_groups.items()
-            }
-
     # Execute tasks
+    standby = _group_nodes_by_db(graph.get_initial_tasks())
+    in_process: set[Future[TaskKey]] = set()
     with executor as executor:
-        in_process: set[Future[Key]] = set()
-        while leaves or in_process:
+        while standby or in_process:
             # Log some stats
             LOGGER.info(
-                    f'nodes: {len(nodes)}, desc: {len(descendants)}, prec: {len(precedents)}, leaves: {len(leaves)}, in_process: {len(in_process)}'
+                    f'nodes: {graph.size}, '
+                    f'standby: {len(standby)}, '
+                    f'in_process: {len(in_process)}'
                     )
             if dump_generations:
-                info['generations'].append(copy.deepcopy(node_groups))
+                info['generations'].append(graph.get_grouped_nodes())
 
             # Submit all leaf tasks
-            leftover: dict[str, list[Json]] = {}
-            for path, keys in leaves.items():
+            leftover: dict[str, list[TaskKey]] = {}
+            for path, keys in standby.items():
                 if path in budgets:
                     free = budgets[path] - occupied[path]
                     to_submit, to_hold = keys[:free], keys[free:]
                     occupied[path] += len(to_submit)
                     if to_hold:
                         leftover[path] = to_hold
                 else:
                     to_submit = keys
 
                 for key in to_submit:
-                    future = executor.submit(_run_task, cloudpickle.dumps(nodes[path, key]))
+                    future = executor.submit(_run_task, cloudpickle.dumps(graph.get_task(key)))
                     in_process.add(future)
 
             # Wait for the first tasks to complete
             done, in_process = wait(in_process, return_when=FIRST_COMPLETED)
 
             # Update graph
-            leaves = leftover
+            standby = defaultdict(list, leftover)
             for done_future in done:
-                done_task = done_future.result()
+                x_done = done_future.result()
 
                 # Update occupied
-                path = done_task[0]
+                path = x_done[0]
                 if path in occupied:
                     occupied[path] -= 1
                     assert occupied[path] >= 0
 
                 # Remove node from graph
-                nodes.pop(done_task)
-                node_groups[path].remove(done_task[1])
-                if not node_groups[path]:
-                    del node_groups[path]
-                assert not precedents.pop(done_task)
-                next_tasks = descendants.pop(done_task)
-
-                # Update leaves
-                for next_task in next_tasks:
-                    precs = precedents[next_task]
-                    precs.remove(done_task)
-                    if not precs:
-                        path_next, key_next = next_task
-                        if path_next not in leaves:
-                            leaves[path_next] = [key_next]
-                        else:
-                            leaves[path_next].append(key_next)
+                ys = graph.pop_with_new_leaves(x_done)
+
+                # Update standby
+                for y in ys:
+                    standby[y[0]].append(y)
 
     # Sanity check
-    assert not nodes and not descendants and not precedents and not node_groups, f'Graph is not empty. Should not happen.'
+    assert graph.size == 0, f'Graph is not empty. Should not happen.'
     assert all(n == 0 for n in occupied.values()), 'Incorrect task count. Should not happen.'
     return info
 
 
 def _run_task(task_data: bytes) -> tuple[str, Json]:
     task = cloudpickle.loads(task_data)
     assert isinstance(task, Task)
```

### Comparing `checkpoint_tool-0.3.0/pyproject.toml` & `checkpoint_tool-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "checkpoint-tool"
-version = "0.3.0"
+version = "0.3.1"
 description = "A lightweight workflow management tool written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/checkpoint"
 repository = "https://github.com/koheimiya/checkpoint"
 readme = "README.md"
 packages = [{include = "checkpoint.py"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typing-extensions = "^4.5.0"
 diskcache = "^5.6.1"
 cloudpickle = "^2.2.1"
+networkx = "^3.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `checkpoint_tool-0.3.0/PKG-INFO` & `checkpoint_tool-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: checkpoint-tool
-Version: 0.3.0
+Version: 0.3.1
 Summary: A lightweight workflow management tool written in pure Python
 Home-page: https://github.com/koheimiya/checkpoint
 License: MIT
 Author: Kohei Miyaguchi
 Author-email: koheimiyaguchi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
+Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/koheimiya/checkpoint
 Description-Content-Type: text/markdown
 
 # Checkpoint-tool
 A lightweight workflow management tool written in pure Python.
 
-Internally, it depends on `DiskCache`, `cloudpickle` and `concurrent.futures`.
+Internally, it depends on `DiskCache`, `cloudpickle` `networkx` and `concurrent.futures`.
 
 
 ### Installation
 ```
 pip install checkpoint-tool
 ```
```


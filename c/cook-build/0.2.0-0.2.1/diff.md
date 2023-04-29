# Comparing `tmp/cook-build-0.2.0.tar.gz` & `tmp/cook-build-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cook-build-0.2.0.tar", last modified: Tue Apr  4 19:44:51 2023, max compression
+gzip compressed data, was "cook-build-0.2.1.tar", last modified: Sat Apr 29 00:26:26 2023, max compression
```

## Comparing `cook-build-0.2.0.tar` & `cook-build-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:44:51.344965 cook-build-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-04 19:44:04.000000 cook-build-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-04 19:44:51.344965 cook-build-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-04 19:44:04.000000 cook-build-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:44:51.340965 cook-build-0.2.0/cook/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-04 19:44:04.000000 cook-build-0.2.0/cook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-04 19:44:04.000000 cook-build-0.2.0/cook/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-04 19:44:04.000000 cook-build-0.2.0/cook/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-04 19:44:04.000000 cook-build-0.2.0/cook/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-04-04 19:44:04.000000 cook-build-0.2.0/cook/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-04 19:44:04.000000 cook-build-0.2.0/cook/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-04 19:44:04.000000 cook-build-0.2.0/cook/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-04 19:44:04.000000 cook-build-0.2.0/cook/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:44:51.344965 cook-build-0.2.0/cook_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-04 19:44:51.000000 cook-build-0.2.0/cook_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-04 19:44:51.000000 cook-build-0.2.0/cook_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:44:51.000000 cook-build-0.2.0/cook_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 19:44:51.000000 cook-build-0.2.0/cook_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-04 19:44:51.000000 cook-build-0.2.0/cook_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-04 19:44:51.000000 cook-build-0.2.0/cook_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-04 19:44:51.344965 cook-build-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-04 19:44:04.000000 cook-build-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:26:26.662414 cook-build-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-29 00:26:04.000000 cook-build-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-29 00:26:26.662414 cook-build-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-29 00:26:04.000000 cook-build-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:26:26.662414 cook-build-0.2.1/cook/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:26:26.662414 cook-build-0.2.1/cook_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-29 00:26:26.000000 cook-build-0.2.1/cook_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-29 00:26:26.000000 cook-build-0.2.1/cook_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:26:26.000000 cook-build-0.2.1/cook_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-29 00:26:26.000000 cook-build-0.2.1/cook_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 00:26:26.000000 cook-build-0.2.1/cook_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 00:26:26.000000 cook-build-0.2.1/cook_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-29 00:26:26.662414 cook-build-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-29 00:26:04.000000 cook-build-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:26:26.662414 cook-build-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-29 00:26:04.000000 cook-build-0.2.1/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-29 00:26:04.000000 cook-build-0.2.1/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-29 00:26:04.000000 cook-build-0.2.1/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-29 00:26:04.000000 cook-build-0.2.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-29 00:26:04.000000 cook-build-0.2.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-29 00:26:04.000000 cook-build-0.2.1/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-29 00:26:04.000000 cook-build-0.2.1/tests/test_util.py
```

### Comparing `cook-build-0.2.0/LICENSE` & `cook-build-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.0/README.rst` & `cook-build-0.2.1/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -21,48 +21,53 @@
     ...             action="echo 'int main() { return 0; }' > hello.c")  # doctest: +IGNORE_RESULT
     >>> create_task("cc", dependencies=["hello.c"], targets=["hello"],
     ...             action="cc -o hello hello.c")  # doctest: +IGNORE_RESULT
     >>> create_task("hello", dependencies=["hello"], action="./hello")  # doctest: +IGNORE_RESULT
 
 Running :code:`cook ls` from the command line lists all known tasks, e.g.,
 
-.. code-block:: bash
+.. shtest::
+    :cwd: examples/getting_started
 
     $ cook ls
     <task `src` @ /.../recipe.py:3>
-    <task `cc` @ /.../recipe.py:5>
-    <task `hello` @ /.../recipe.py:7>
+    <task `cc` @ /.../recipe.py:4>
+    <task `hello` @ /.../recipe.py:5>
 
 Running :code:`cook exec hello` creates the source file, compile it, and executes the binary. We use :code:`--log-level=debug` to provide additional information here.
 
-.. code-block:: bash
+.. shtest::
+    :cwd: examples/getting_started
+    :stderr:
 
     $ cook --log-level=debug exec hello
-    DEBUG: <task `src` @ ...> is stale because one of its targets is missing
-    DEBUG: started <task `src` @ ...>
-    DEBUG: completed <task `src` @ ...> in ... seconds
-    DEBUG: `<task `src` @ ...>` created `hello.c`
-
-    DEBUG: <task `cc` @ ...> is stale because its dependency `hello.c` does not have a hash entry
-    DEBUG: started <task `cc` @ ...>
-    DEBUG: completed <task `cc` @ ...> in ... seconds
-    DEBUG: `<task `cc` @ ...>` created `hello`
-
-    DEBUG: <task `hello` @ ...> is "stale" because it has no targets
-    DEBUG: started <task `hello` @ ...>
-    DEBUG: completed <task `hello` @ ...> in ... seconds
+    DEBUG: <task `src` @ .../recipe.py:3> is stale because one of its targets is missing
+    DEBUG: started <task `src` @ .../recipe.py:3>
+    DEBUG: completed <task `src` @ .../recipe.py:3> in ... seconds
+    DEBUG: <task `src` @ .../recipe.py:3> created `hello.c`
+    DEBUG: <task `cc` @ .../recipe.py:4> is stale because one of its targets is missing
+    DEBUG: started <task `cc` @ .../recipe.py:4>
+    DEBUG: completed <task `cc` @ .../recipe.py:4> in ... seconds
+    DEBUG: <task `cc` @ .../recipe.py:4> created `hello`
+    DEBUG: <task `hello` @ .../recipe.py:5> is "stale" because it has no targets
+    DEBUG: started <task `hello` @ .../recipe.py:5>
+    DEBUG: completed <task `hello` @ .../recipe.py:5> in ... seconds
 
 To rerun a task, tell Cook to reset it.
 
-.. code-block:: bash
+.. shtest::
+    :cwd: examples/getting_started
+    :stderr:
 
     $ cook reset cc
     INFO: reset 1 task
 
-The full set of available commands can be explored using :code:`cook --help`.
+The full set of available commands can be explored using :code:`cook --help` as shown below.
+
+.. sh:: cook --help
 
 Tasks Are Dumb; Contexts Are Smart
 ----------------------------------
 
 :class:`~cook.task.Task`\ s do not provide any functionality beyond storing metadata, including
 
 - :code:`targets`, the files generated by the task,
```

### Comparing `cook-build-0.2.0/cook/__main__.py` & `cook-build-0.2.1/cook/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,29 +59,33 @@
     def execute(self, controller: Controller, args: argparse.Namespace) -> None:
         raise NotImplementedError
 
 
 class ExecArgs(argparse.Namespace):
     tasks: Iterable[re.Pattern]
     re: bool
+    jobs: int
 
 
 class ExecCommand(Command):
     """
     Execute one or more tasks.
     """
     NAME = "exec"
 
     def configure_parser(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument("--re", "-r", action="store_true",
                             help="use regular expressions for pattern matching instead of glob")
+        parser.add_argument("--jobs", "-j", help="number of concurrent jobs", type=int, default=1)
         parser.add_argument("tasks", nargs="+",
                             help="task or tasks to execute as regular expressions")
 
     def execute(self, controller: Controller, args: ExecArgs) -> None:
+        # Monkeypatch the controller semaphore.
+        controller.num_concurrent = args.jobs
         tasks = discover_tasks(controller.manager, args.tasks, args.re)
         controller.execute_sync(*tasks)
 
 
 class LsArgs(argparse.Namespace):
     tasks: Iterable[re.Pattern]
     all: bool
```

### Comparing `cook-build-0.2.0/cook/actions.py` & `cook-build-0.2.1/cook/actions.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.0/cook/contexts.py` & `cook-build-0.2.1/cook/contexts.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.0/cook/controller.py` & `cook-build-0.2.1/cook/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import logging
 import os
 from pathlib import Path
 from sqlite3 import Connection
+import sys
 from typing import Dict, Iterable, Optional, Set, Tuple, TYPE_CHECKING, Union
 from . import util
 
 if TYPE_CHECKING:
     from .manager import Manager
     from .task import Task
 
@@ -37,15 +38,25 @@
     def __init__(self, manager: "Manager", connection: Connection, num_concurrent: int = 1) -> None:
         self.manager = manager
         self.connection = connection
         self.dependencies = manager.resolve_dependencies()
         self.status: Dict[Task, bool] = {}
         self.futures: Dict[Task, asyncio.Future] = {}
         self.size_digest: Dict[str, Tuple[int, str]] = {}
-        self.semaphore = asyncio.Semaphore(num_concurrent)
+        self.num_concurrent = num_concurrent
+        self._semaphore = None
+        self.cancelled = False
+
+    @property
+    def semaphore(self) -> asyncio.Semaphore:
+        # Create the semaphore upon first use for python 3.9 and below (see
+        # https://stackoverflow.com/a/55918049/1150961 for details).
+        if self._semaphore is None:
+            self._semaphore = asyncio.Semaphore(self.num_concurrent)
+        return self._semaphore
 
     def resolve_stale_tasks(self, tasks: Optional[Iterable["Task"]] = None) -> Set["Task"]:
         tasks = tasks or self.manager.tasks.values()
         for task in tasks:
             self.is_stale(task)
         return {task for task, is_stale in self.status.items() if is_stale}
 
@@ -111,14 +122,17 @@
         dependents = [self.is_stale(dependent) for dependent in self.dependencies.get(task, [])]
         if any(dependents):
             return self.status.setdefault(task, True)
 
         return self.status.setdefault(task, self._is_self_stale(task))
 
     async def execute(self, task: "Task") -> None:
+        if self.cancelled:  # pragma: no cover
+            return
+
         # If there already is a future, just wait for it and return.
         if future := self.futures.get(task):
             await future
             return
 
         # Create a new future and add it to the lookup.
         future = self.futures.setdefault(task, asyncio.Future())
@@ -136,15 +150,15 @@
                         await task.execute()
                     LOGGER.debug("completed %s in %.3f seconds", task, timer.duration)
 
                 # Validate that all desired targets exist.
                 for target in task.targets:
                     if not target.is_file():
                         raise FileNotFoundError(f"`{task}` did not create `{target}`")
-                    LOGGER.debug("`%s` created `%s`", task, target)
+                    LOGGER.debug("%s created `%s`", task, target)
 
                 # Update the state and write to the database.
                 self.status[task] = False
                 records = []
                 for dependency in task.dependencies:
                     size, digest = self.evaluate_size_digest(dependency)
                     records.append({
@@ -155,18 +169,25 @@
                 self.connection.executemany(QUERIES["upsert"], records)
         except Exception as ex:
             message = f"failed to execute {task}: {ex}"
             LOGGER.exception(message)
             error = util.FailedTaskError(message, task=task)
             error.__cause__ = ex
             future.set_exception(error)
+            # Cancel all other futures.
+            self.cancelled = True
+            for future in self.futures.values():
+                future.cancel(message) if sys.version_info[:2] > (3, 8) else future.cancel()
         else:
             future.set_result(None)
 
-        await future
+        try:
+            await future
+        except asyncio.CancelledError:  # pragma: no cover
+            pass
 
     def execute_sync(self, *tasks: "Task") -> None:
         util.run_until_complete(*(self.execute(task) for task in tasks))
 
     def reset(self, *tasks: "Task") -> None:
         names = []
         for task in tasks:
```

### Comparing `cook-build-0.2.0/cook/manager.py` & `cook-build-0.2.1/cook/manager.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.0/cook/task.py` & `cook-build-0.2.1/cook/task.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.0/cook/util.py` & `cook-build-0.2.1/cook/util.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.0/setup.py` & `cook-build-0.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from setuptools import find_packages, setup
 
 
 with open("README.rst") as fp:
     long_description = fp.read()
 long_description = long_description \
     .replace(":func:", ":code:") \
-    .replace(".. doctest::", ".. code-block::") \
+    .replace(".. doctest::", ".. code-block::\n") \
+    .replace(".. shtest::", ".. code-block::\n") \
     .replace(":class:", ":code:") \
-    .replace(".. toctree::", "..")
+    .replace(".. toctree::", "..") \
+    .replace(".. sh::", "..")
 
 
 setup(
     name="cook-build",
-    version="0.2.0",
+    version="0.2.1",
     long_description=long_description,
     long_description_content_type="text/x-rst",
+    python_requires=">=3.8",
     install_requires=[
         "colorama",
     ],
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "cook = cook.__main__:__main__",
```


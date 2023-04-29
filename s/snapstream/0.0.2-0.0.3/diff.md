# Comparing `tmp/snapstream-0.0.2.tar.gz` & `tmp/snapstream-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapstream-0.0.2.tar", max compression
+gzip compressed data, was "snapstream-0.0.3.tar", max compression
```

## Comparing `snapstream-0.0.2.tar` & `snapstream-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-04-17 13:31:07.558570 snapstream-0.0.2/LICENSE
--rw-r--r--   0        0        0     2064 2023-04-17 13:31:07.558570 snapstream-0.0.2/README.md
--rw-r--r--   0        0        0     1265 2023-04-17 13:31:20.466662 snapstream-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1673 2023-04-17 13:31:07.562570 snapstream-0.0.2/snapstream/__init__.py
--rw-r--r--   0        0        0     9660 2023-04-17 13:31:07.562570 snapstream-0.0.2/snapstream/caching.py
--rw-r--r--   0        0        0     2538 2023-04-17 13:31:07.562570 snapstream-0.0.2/snapstream/codecs.py
--rw-r--r--   0        0        0     8531 2023-04-17 13:31:07.562570 snapstream-0.0.2/snapstream/core.py
--rw-r--r--   0        0        0     1033 2023-04-17 13:31:07.562570 snapstream-0.0.2/snapstream/utils.py
--rw-r--r--   0        0        0     3214 1970-01-01 00:00:00.000000 snapstream-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-29 18:13:55.378851 snapstream-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2236 2023-04-29 18:13:55.378851 snapstream-0.0.3/README.md
+-rw-r--r--   0        0        0     1350 2023-04-29 18:14:09.463051 snapstream-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2181 2023-04-29 18:13:55.382851 snapstream-0.0.3/snapstream/__init__.py
+-rw-r--r--   0        0        0     7580 2023-04-29 18:13:55.382851 snapstream-0.0.3/snapstream/__main__.py
+-rw-r--r--   0        0        0     9509 2023-04-29 18:13:55.382851 snapstream-0.0.3/snapstream/caching.py
+-rw-r--r--   0        0        0     2538 2023-04-29 18:13:55.382851 snapstream-0.0.3/snapstream/codecs.py
+-rw-r--r--   0        0        0     8531 2023-04-29 18:13:55.382851 snapstream-0.0.3/snapstream/core.py
+-rw-r--r--   0        0        0     3241 2023-04-29 18:13:55.382851 snapstream-0.0.3/snapstream/utils.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 snapstream-0.0.3/PKG-INFO
```

### Comparing `snapstream-0.0.2/LICENSE` & `snapstream-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.2/README.md` & `snapstream-0.0.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 We pass the callable `print` to print out the return value. Multiple iterables and sinks can be passed.
 
 ```py
 from snapstream import snap, stream
 
 @snap(range(5), sink=[print])
 def handler(msg):
-    return f'Hello {msg}'
+    yield f'Hello {msg}'
 
 stream()
 ```
 
 ```sh
 Hello 0
 Hello 1
@@ -40,14 +40,27 @@
 
 To try it out for yourself, spin up a local kafka broker with [docker-compose.yml](docker-compose.yml), using `localhost:29091` to connect:
 
 ```sh
 docker compose up broker -d
 ```
 
+Use the cli tool to inspect Topic/Cache:
+
+```sh
+snapstream topic emoji --offset -2
+```
+
+```
+>>> timestamp: 2023-04-28T17:31:51.775000+00:00
+>>> offset: 0
+>>> key:
+🏆
+```
+
 ## Features
 
 - [`snapstream.snap`](snapstream/__init__.py): bind streams (iterables) and sinks (callables) to user defined handler functions
 - [`snapstream.stream`](snapstream/__init__.py): start streaming
 - [`snapstream.Topic`](snapstream/core.py): consume from (iterable) and produce to (callable) kafka using [**confluent-kafka**](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html)
 - [`snapstream.Cache`](snapstream/caching.py): store data to disk using [**rocksdict**](https://congyuwang.github.io/RocksDict/rocksdict.html)
 - [`snapstream.Conf`](snapstream/core.py): set global kafka configuration (can be overridden per topic)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snapstream-0.0.2/pyproject.toml` & `snapstream-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [tool.poetry]
 name = "snapstream"
-version = "0.0.2"
+version = "0.0.3"
 description = "Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions."
 authors = ["Menziess <stefan_schenk@hotmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Menziess/snapstream"
 license = "MIT"
 keywords = ["kafka", "pubsub"]
 
+[tool.poetry.scripts]
+snapstream = 'snapstream.__main__:main'
+
 [tool.poetry.dependencies]
 python = "^3.8.1"
 confluent-kafka = "^2.0.2"
 rocksdict = "^0.3.10"
 pypubsub = "^4.0.3"
 avro = "^1.11.1"
 toolz = "^0.12.0"
@@ -23,14 +26,15 @@
 pyright = "^1.1.300"
 flake8 = "^6.0.0"
 bandit = "^1.7.5"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pre-commit = "^3.2.1"
 pytest-mock = "^3.10.0"
+ipykernel = "^6.22.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 include = ["snapstream"]
```

### Comparing `snapstream-0.0.2/snapstream/__init__.py` & `snapstream-0.0.3/snapstream/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Snapstream public objects."""
 
-from typing import Iterable
+from inspect import signature
+from typing import Any, Callable, Generator, Iterable
 
 from pubsub import pub
 
 from snapstream.caching import Cache
 from snapstream.core import READ_FROM_END, READ_FROM_START, Conf, Topic
 
 __all__ = [
@@ -14,61 +15,74 @@
     'Topic',
     'Cache',
     'READ_FROM_START',
     'READ_FROM_END',
 ]
 
 
+def _sink_output(s: Callable[..., None], output: Any) -> None:
+    if not isinstance(output, tuple) and isinstance(s, (Cache)):
+        raise ValueError('Cache sink expects: Tuple[key, val].')
+    elif isinstance(output, tuple) and isinstance(s, (Cache, Topic)):
+        key, val = output
+        s(key=key, val=val)
+    else:
+        s(output)
+
+
+def _handle_generator_or_function(
+    sink: Iterable[Callable[..., None]],
+    output: Any
+) -> None:
+    if isinstance(output, Generator):
+        for val in output:
+            for s in sink:
+                _sink_output(s, val)
+    else:
+        for s in sink:
+            _sink_output(s, output)
+
+
 def snap(
     *iterable: Iterable,
-    sink: Iterable = []
+    sink: Iterable[Callable[..., None]] = []
 ):
     """Snaps function to stream.
 
     Ex:
-        >> topic = Topic('demo')
-        >> cache = Cache('state/demo')
+        >>> topic = Topic('demo')               # doctest: +SKIP
+        >>> cache = Cache('state/demo')         # doctest: +SKIP
 
-        >> @snap(topic, sink=[print, cache])
-        .. def handler(msg, **kwargs):
-        ..     return msg.key(), msg.value()
+        >>> @snap(topic, sink=[print, cache])   # doctest: +SKIP
+        ... def handler(msg, **kwargs):
+        ...     return msg.key(), msg.value()
     """
     c = Conf()
 
-    def sink_output(s, output):
-        if not isinstance(output, tuple) and isinstance(s, (Cache)):
-            # Sink requires Tuple[key, val]
-            raise ValueError('Cache sink expects: Tuple[key, val].')
-        elif isinstance(output, tuple) and isinstance(s, (Cache, Topic)):
-            key, val = output
-            s(key=key, val=val)
-        else:
-            s(output)
-
     def _deco(f):
         def _handler(msg, kwargs):
-            try:
+            parameters = signature(f).parameters.values()
+            if any(p.kind == p.VAR_KEYWORD for p in parameters):
                 output = f(msg, **kwargs)
-            except TypeError:
+            else:
                 output = f(msg)
-            for s in sink:
-                sink_output(s, output)
+            _handle_generator_or_function(sink, output)
 
         for it in iterable:
             iterable_key = str(id(it))
             c.register_iterables((iterable_key, it))
             pub.subscribe(_handler, iterable_key)
         return _handler
 
     return _deco
 
 
 def stream(**kwargs):
     """Start the streams.
 
     Ex:
-        >> args = {
-        ..     'env': 'DEV',
-        .. }
-        >> stream(**args)
+        >>> args = {
+        ...     'env': 'DEV',
+        ... }
+        >>> stream(**args)
     """
     Conf().start(**kwargs)
```

### Comparing `snapstream-0.0.2/snapstream/caching.py` & `snapstream-0.0.3/snapstream/caching.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,21 @@
     """A Rocksdb instance."""
 
     def __init__(
         self,
         path: str,
         options: Union[Options, None] = None,
         column_families: Union[Dict[str, Options], None] = None,
-        access_type=AccessType.with_ttl(4 * 24 * 60 * MINUTES),
+        access_type=AccessType.read_write(),
         target_table_size=25 * MB
     ) -> None:
         """Create instance that holds rocksdb reference.
 
         This configuration setup optimizes for low disk usage (25mb per table/cf).
-        TTL is set to 4 days, older records may be removed during compaction.
-        When 25mb (target_table_size) is reached, the oldest file gets
-        deleted (the first records go out).
+        The oldest records may be removed during compaction.
 
         https://congyuwang.github.io/RocksDict/rocksdict.html
         """
         self.name = path
         options = options or self._default_options(target_table_size)
         column_families = column_families or {
             key: options
```

### Comparing `snapstream-0.0.2/snapstream/codecs.py` & `snapstream-0.0.3/snapstream/codecs.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.2/snapstream/core.py` & `snapstream-0.0.3/snapstream/core.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.2/PKG-INFO` & `snapstream-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapstream
-Version: 0.0.2
+Version: 0.0.3
 Summary: Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions.
 Home-page: https://github.com/Menziess/snapstream
 License: MIT
 Keywords: kafka,pubsub
 Author: Menziess
 Author-email: stefan_schenk@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -45,15 +45,15 @@
 We pass the callable `print` to print out the return value. Multiple iterables and sinks can be passed.
 
 ```py
 from snapstream import snap, stream
 
 @snap(range(5), sink=[print])
 def handler(msg):
-    return f'Hello {msg}'
+    yield f'Hello {msg}'
 
 stream()
 ```
 
 ```sh
 Hello 0
 Hello 1
@@ -64,14 +64,27 @@
 
 To try it out for yourself, spin up a local kafka broker with [docker-compose.yml](docker-compose.yml), using `localhost:29091` to connect:
 
 ```sh
 docker compose up broker -d
 ```
 
+Use the cli tool to inspect Topic/Cache:
+
+```sh
+snapstream topic emoji --offset -2
+```
+
+```
+>>> timestamp: 2023-04-28T17:31:51.775000+00:00
+>>> offset: 0
+>>> key:
+🏆
+```
+
 ## Features
 
 - [`snapstream.snap`](snapstream/__init__.py): bind streams (iterables) and sinks (callables) to user defined handler functions
 - [`snapstream.stream`](snapstream/__init__.py): start streaming
 - [`snapstream.Topic`](snapstream/core.py): consume from (iterable) and produce to (callable) kafka using [**confluent-kafka**](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html)
 - [`snapstream.Cache`](snapstream/caching.py): store data to disk using [**rocksdict**](https://congyuwang.github.io/RocksDict/rocksdict.html)
 - [`snapstream.Conf`](snapstream/core.py): set global kafka configuration (can be overridden per topic)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


# Comparing `tmp/irisml-0.0.8.tar.gz` & `tmp/irisml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-0.0.8.tar", last modified: Mon Sep 12 20:35:51 2022, max compression
+gzip compressed data, was "irisml-0.0.9.tar", last modified: Tue Sep 13 00:45:56 2022, max compression
```

## Comparing `irisml-0.0.8.tar` & `irisml-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 20:35:51.336495 irisml-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-09-12 20:34:57.000000 irisml-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6281 2022-09-12 20:35:51.336495 irisml-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6032 2022-09-12 20:34:57.000000 irisml-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 20:35:51.332495 irisml-0.0.8/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 20:35:51.332495 irisml-0.0.8/irisml/core/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-09-12 20:34:57.000000 irisml-0.0.8/irisml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9070 2022-09-12 20:34:57.000000 irisml-0.0.8/irisml/core/cache_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 20:35:51.336495 irisml-0.0.8/irisml/core/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     2873 2022-09-12 20:34:57.000000 irisml-0.0.8/irisml/core/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-09-12 20:34:57.000000 irisml-0.0.8/irisml/core/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-09-12 20:34:57.000000 irisml-0.0.8/irisml/core/commands/run_task.py
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-09-12 20:34:57.000000 irisml-0.0.8/irisml/core/commands/show.py
--rw-r--r--   0 runner    (1001) docker     (121)     3670 2022-09-12 20:34:57.000000 irisml-0.0.8/irisml/core/context.py
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-12 20:34:57.000000 irisml-0.0.8/irisml/core/description.py
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-09-12 20:34:57.000000 irisml-0.0.8/irisml/core/hash_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-09-12 20:34:57.000000 irisml-0.0.8/irisml/core/job.py
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-09-12 20:34:57.000000 irisml-0.0.8/irisml/core/job_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     9626 2022-09-12 20:34:57.000000 irisml-0.0.8/irisml/core/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-09-12 20:34:57.000000 irisml-0.0.8/irisml/core/task_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3423 2022-09-12 20:34:57.000000 irisml-0.0.8/irisml/core/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 20:35:51.332495 irisml-0.0.8/irisml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6281 2022-09-12 20:35:51.000000 irisml-0.0.8/irisml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-09-12 20:35:51.000000 irisml-0.0.8/irisml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 20:35:51.000000 irisml-0.0.8/irisml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-09-12 20:35:51.000000 irisml-0.0.8/irisml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-12 20:35:51.000000 irisml-0.0.8/irisml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-12 20:35:51.000000 irisml-0.0.8/irisml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-12 20:34:57.000000 irisml-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-09-12 20:35:51.336495 irisml-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 20:35:51.336495 irisml-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)     5922 2022-09-12 20:34:57.000000 irisml-0.0.8/test/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-09-12 20:34:57.000000 irisml-0.0.8/test/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-09-12 20:34:57.000000 irisml-0.0.8/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-09-12 20:34:57.000000 irisml-0.0.8/test/test_task.py
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-09-12 20:34:57.000000 irisml-0.0.8/test/test_variable.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 00:45:56.902457 irisml-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-09-13 00:44:50.000000 irisml-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     6281 2022-09-13 00:45:56.902457 irisml-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6032 2022-09-13 00:44:50.000000 irisml-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 00:45:56.894457 irisml-0.0.9/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 00:45:56.902457 irisml-0.0.9/irisml/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-09-13 00:44:50.000000 irisml-0.0.9/irisml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9070 2022-09-13 00:44:50.000000 irisml-0.0.9/irisml/core/cache_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 00:45:56.902457 irisml-0.0.9/irisml/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     2873 2022-09-13 00:44:50.000000 irisml-0.0.9/irisml/core/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-09-13 00:44:50.000000 irisml-0.0.9/irisml/core/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-09-13 00:44:50.000000 irisml-0.0.9/irisml/core/commands/run_task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-09-13 00:44:50.000000 irisml-0.0.9/irisml/core/commands/show.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3670 2022-09-13 00:44:50.000000 irisml-0.0.9/irisml/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-13 00:44:50.000000 irisml-0.0.9/irisml/core/description.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-09-13 00:44:50.000000 irisml-0.0.9/irisml/core/hash_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-09-13 00:44:50.000000 irisml-0.0.9/irisml/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-09-13 00:44:50.000000 irisml-0.0.9/irisml/core/job_runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9626 2022-09-13 00:44:50.000000 irisml-0.0.9/irisml/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-09-13 00:44:50.000000 irisml-0.0.9/irisml/core/task_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3423 2022-09-13 00:44:50.000000 irisml-0.0.9/irisml/core/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 00:45:56.898457 irisml-0.0.9/irisml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6281 2022-09-13 00:45:56.000000 irisml-0.0.9/irisml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2022-09-13 00:45:56.000000 irisml-0.0.9/irisml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 00:45:56.000000 irisml-0.0.9/irisml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-09-13 00:45:56.000000 irisml-0.0.9/irisml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-13 00:45:56.000000 irisml-0.0.9/irisml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-13 00:45:56.000000 irisml-0.0.9/irisml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-13 00:44:50.000000 irisml-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2022-09-13 00:45:56.902457 irisml-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 00:45:56.902457 irisml-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     6505 2022-09-13 00:44:50.000000 irisml-0.0.9/test/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-09-13 00:44:50.000000 irisml-0.0.9/test/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-09-13 00:44:50.000000 irisml-0.0.9/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-09-13 00:44:50.000000 irisml-0.0.9/test/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-09-13 00:44:50.000000 irisml-0.0.9/test/test_variable.py
```

### Comparing `irisml-0.0.8/LICENSE` & `irisml-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/PKG-INFO` & `irisml-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple ML pipeline platform
 Home-page: https://github.com/microsoft/irisml
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-0.0.8/README.md` & `irisml-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/irisml/core/cache_manager.py` & `irisml-0.0.9/irisml/core/cache_manager.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/irisml/core/commands/common.py` & `irisml-0.0.9/irisml/core/commands/common.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/irisml/core/commands/run.py` & `irisml-0.0.9/irisml/core/commands/run.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/irisml/core/commands/run_task.py` & `irisml-0.0.9/irisml/core/commands/run_task.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/irisml/core/commands/show.py` & `irisml-0.0.9/irisml/core/commands/show.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/irisml/core/context.py` & `irisml-0.0.9/irisml/core/context.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/irisml/core/description.py` & `irisml-0.0.9/irisml/core/description.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/irisml/core/hash_generator.py` & `irisml-0.0.9/irisml/core/hash_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,47 @@
-import copyreg
 import dataclasses
 import hashlib
-import io
 import json
 import pickle
 import torch
 
 
-def _reduce_tensor(tensor):
-    """__reduce__ for torch.Tensor.
-
-    Since pickle.dumps(tensor) is not deterministic, we convert torch.Tensor to numpy array.
-    """
-    return torch.Tensor, (tensor.cpu().numpy(),)
-
-
-class HashPickler(pickle.Pickler):
-    """Pickler to calculate hash.
-
-    Note that it's not guaranteed that the loads(dumps(obj)) will create the same object.
-    """
-    dispatch_table = copyreg.dispatch_table.copy()
-    dispatch_table[torch.Tensor] = _reduce_tensor
-
-
 class HashGenerator:
     """Calculate hash for the given object.
 
     Note that we cannot simply hashlib.sha1(pickle.dumps(obj)) since some of the contents might be cached on remote. For nested objects, we calculate hash for each child element recursively.
     """
     @classmethod
     def calculate_hash(cls, value, context=None):
-        from .variable import Variable
-
         def get_hash(value):
+            from .variable import Variable
             if isinstance(value, dict):
-                value = json.dumps({k: get_hash(v) for k, v in sorted(value.items())}).encode('utf-8')
+                value = json.dumps({k: get_hash(v) for k, v in sorted(value.items())})
             elif isinstance(value, (list, tuple)):
-                value = json.dumps([get_hash(v) for v in value]).encode('utf-8')
+                value = json.dumps([get_hash(v) for v in value])
             elif dataclasses.is_dataclass(value):
-                value = json.dumps({k: get_hash(v) for k, v in sorted(dataclasses.asdict(value).items())}).encode('utf-8')
+                value = json.dumps({k: get_hash(v) for k, v in sorted(dataclasses.asdict(value).items())})
             elif isinstance(value, Variable):
                 return value.get_hash(context)
-            elif isinstance(value, bytes):
+            elif isinstance(value, (str, bytes)):
                 pass
             elif isinstance(value, torch.Tensor):
                 value = value.cpu().detach().numpy().tobytes()
             elif hasattr(value, '__getstate__'):
                 return get_hash(value.__getstate__())
-            elif hasattr(value, '__dict__'):
-                value = json.dumps([str(value.__class__), get_hash(value.__dict__)]).encode('utf-8')
-            else:
-                f = io.BytesIO()
-                p = HashPickler(f)
-                p.dump(value)
-                value = f.getbuffer()
+            elif hasattr(value, '__reduce__'):
+                try:
+                    states = value.__reduce__()
+                    value = json.dumps([str(value.__class__), get_hash((states[1:3]))])
+                except TypeError:
+                    pass
+
+            if isinstance(value, str):
+                value = value.encode('utf-8')
+
+            if not isinstance(value, bytes):
+                # Fall back to pickle.
+                value = pickle.dumps(value)
 
             return hashlib.sha1(value).hexdigest()
 
         return get_hash(value)
```

### Comparing `irisml-0.0.8/irisml/core/job.py` & `irisml-0.0.9/irisml/core/job.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/irisml/core/job_runner.py` & `irisml-0.0.9/irisml/core/job_runner.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/irisml/core/task.py` & `irisml-0.0.9/irisml/core/task.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/irisml/core/task_base.py` & `irisml-0.0.9/irisml/core/task_base.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/irisml/core/variable.py` & `irisml-0.0.9/irisml/core/variable.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/irisml.egg-info/PKG-INFO` & `irisml-0.0.9/irisml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple ML pipeline platform
 Home-page: https://github.com/microsoft/irisml
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-0.0.8/irisml.egg-info/SOURCES.txt` & `irisml-0.0.9/irisml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/setup.cfg` & `irisml-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = irisml
-version = 0.0.8
+version = 0.0.9
 description = Simple ML pipeline platform
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = irisdev
 license = MIT
 url = https://github.com/microsoft/irisml
```

### Comparing `irisml-0.0.8/test/test_cache.py` & `irisml-0.0.9/test/test_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import collections
 import dataclasses
 import pickle
+import threading
 import typing
 import unittest
 import torch
 from irisml.core.cache_manager import CachedOutputs, StorageManager
 from irisml.core.hash_generator import HashGenerator
 from irisml.core.variable import Variable
 
@@ -96,14 +97,29 @@
 
     def test_torch_in_class(self):
         dummy_instance = Dummy(torch.tensor([1, 2, 3]))
         dummy_instance2 = Dummy(torch.tensor([1, 2, 3]))
 
         self.assertEqual(HashGenerator.calculate_hash(dummy_instance), HashGenerator.calculate_hash(dummy_instance2))
 
+    def test_instance_with_unpickleable(self):
+        class Dummy:
+            def __init__(self, number):
+                self._value = threading.Lock()
+                self._number = number
+
+            def __reduce__(self):
+                return (self.__class__, (self._number))
+
+        dummy = Dummy(1)
+        dummy2 = Dummy(1)
+        dummy3 = Dummy(2)
+        self.assertEqual(HashGenerator.calculate_hash(dummy), HashGenerator.calculate_hash(dummy2))
+        self.assertNotEqual(HashGenerator.calculate_hash(dummy), HashGenerator.calculate_hash(dummy3))
+
     def _assert_same_hash(self, a, b):
         self.assertEqual(HashGenerator.calculate_hash(a), HashGenerator.calculate_hash(b))
 
 
 class FakeStorageManager(StorageManager):
     def __init__(self, data=None):
         self._data = data or {}
```

### Comparing `irisml-0.0.8/test/test_context.py` & `irisml-0.0.9/test/test_context.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/test/test_job.py` & `irisml-0.0.9/test/test_job.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/test/test_task.py` & `irisml-0.0.9/test/test_task.py`

 * *Files identical despite different names*

### Comparing `irisml-0.0.8/test/test_variable.py` & `irisml-0.0.9/test/test_variable.py`

 * *Files identical despite different names*


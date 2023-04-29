# Comparing `tmp/envoy.base.utils-0.4.3.tar.gz` & `tmp/envoy.base.utils-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envoy.base.utils-0.4.3.tar", last modified: Sat Apr 29 11:47:01 2023, max compression
+gzip compressed data, was "envoy.base.utils-0.4.4.tar", last modified: Sat Apr 29 13:59:38 2023, max compression
```

## Comparing `envoy.base.utils-0.4.3.tar` & `envoy.base.utils-0.4.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:47:01.174293 envoy.base.utils-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-29 11:47:01.174293 envoy.base.utils-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:47:01.170293 envoy.base.utils-0.4.3/envoy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:47:01.170293 envoy.base.utils-0.4.3/envoy/base/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:47:01.170293 envoy.base.utils-0.4.3/envoy/base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:47:01.174293 envoy.base.utils-0.4.3/envoy/base/utils/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:47:01.174293 envoy.base.utils-0.4.3/envoy/base/utils/abstract/project/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/abstract/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/abstract/project/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/abstract/project/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/abstract/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/abstract/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/data_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/data_env_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/jinja_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/jinja_env_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/parallel_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/parallel_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/project_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/project_data_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/project_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/envoy/base/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:47:01.170293 envoy.base.utils-0.4.3/envoy.base.utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-29 11:47:01.000000 envoy.base.utils-0.4.3/envoy.base.utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-29 11:47:01.000000 envoy.base.utils-0.4.3/envoy.base.utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 11:47:01.000000 envoy.base.utils-0.4.3/envoy.base.utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 11:47:01.000000 envoy.base.utils-0.4.3/envoy.base.utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 11:47:01.000000 envoy.base.utils-0.4.3/envoy.base.utils.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-29 11:47:01.000000 envoy.base.utils-0.4.3/envoy.base.utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 11:47:01.000000 envoy.base.utils-0.4.3/envoy.base.utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 11:47:01.174293 envoy.base.utils-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-29 11:47:00.000000 envoy.base.utils-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.758401 envoy.base.utils-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-29 13:59:38.758401 envoy.base.utils-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.750400 envoy.base.utils-0.4.4/envoy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.750400 envoy.base.utils-0.4.4/envoy/base/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.758401 envoy.base.utils-0.4.4/envoy/base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.758401 envoy.base.utils-0.4.4/envoy/base/utils/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.758401 envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/abstract/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/data_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/data_env_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/jinja_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/jinja_env_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/parallel_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/parallel_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/project_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/project_data_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/project_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy/base/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:38.754401 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/envoy.base.utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 13:59:38.758401 envoy.base.utils-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-29 13:59:38.000000 envoy.base.utils-0.4.4/setup.py
```

### Comparing `envoy.base.utils-0.4.3/backend_shim.py` & `envoy.base.utils-0.4.4/backend_shim.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/__init__.py` & `envoy.base.utils-0.4.4/envoy/base/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/abstract/project/changelog.py` & `envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/changelog.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/abstract/project/inventory.py` & `envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/inventory.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/abstract/project/project.py` & `envoy.base.utils-0.4.4/envoy/base/utils/abstract/project/project.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/abstract/protobuf.py` & `envoy.base.utils-0.4.4/envoy/base/utils/abstract/protobuf.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/data_env.py` & `envoy.base.utils-0.4.4/envoy/base/utils/data_env.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/interface.py` & `envoy.base.utils-0.4.4/envoy/base/utils/interface.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/jinja_env.py` & `envoy.base.utils-0.4.4/envoy/base/utils/jinja_env.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/parallel_runner.py` & `envoy.base.utils-0.4.4/envoy/base/utils/parallel_runner.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/project.py` & `envoy.base.utils-0.4.4/envoy/base/utils/project.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/project_runner.py` & `envoy.base.utils-0.4.4/envoy/base/utils/project_runner.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/tar.py` & `envoy.base.utils-0.4.4/envoy/base/utils/tar.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,17 +118,17 @@
     for src, dest in (mappings or {}).items():
         src_path = path.joinpath(src)
         dest_path = path.joinpath(dest)
         dest_path.parent.mkdir(exist_ok=True, parents=True)
         shutil.move(src_path, dest_path)
 
 
-def _open(path: pathlib.Path | str) -> ContextManager[
-        tuple[str, tarfile.TarFile]
-        | tarfile.TarFile]:
+def _open(
+        path: pathlib.Path | str) -> (
+            ContextManager[tuple[str, tarfile.TarFile]]):
     """For a given tarball path if it contains `:` split prefix, path,
     otherwise prefix is empty.
 
     If the tarfile is `tar.zst` use zstd to decompress.
 
     Return prefix, and opened tarfile for path.
     """
@@ -153,22 +153,17 @@
     outfile.seek(0)
     return tarfile.open(fileobj=outfile)
 
 
 @contextlib.contextmanager
 def _opener(
         tarball: tarfile.TarFile,
-        prefix: str = "") -> Iterator[
-            tuple[str, tarfile.TarFile]
-            | tarfile.TarFile]:
+        prefix: str = "") -> Iterator[tuple[str, tarfile.TarFile]]:
     with tarball as t:
-        yield (
-            (prefix, t)
-            if prefix
-            else t)
+        yield prefix, t
 
 
 def _rm_paths(path: pathlib.Path, matching: Optional[Pattern[str]]):
     if not matching:
         return
     for sub in path.glob("*"):
         if not matching.match(sub.name):
```

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/typing.py` & `envoy.base.utils-0.4.4/envoy/base/utils/typing.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/utils.py` & `envoy.base.utils-0.4.4/envoy/base/utils/utils.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy/base/utils/yaml.py` & `envoy.base.utils-0.4.4/envoy/base/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/envoy.base.utils.egg-info/SOURCES.txt` & `envoy.base.utils-0.4.4/envoy.base.utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `envoy.base.utils-0.4.3/setup.py` & `envoy.base.utils-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,9 +53,9 @@
     'packages': (
         'envoy.base.utils',
         'envoy.base.utils.abstract',
         'envoy.base.utils.abstract.project',
     ),
     'python_requires': '>=3.10.0',
     'url': 'https://github.com/envoyproxy/pytooling/tree/main/envoy.base.utils',
-    'version': '0.4.3',
+    'version': '0.4.4',
 })
```


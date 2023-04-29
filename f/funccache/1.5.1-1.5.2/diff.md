# Comparing `tmp/funccache-1.5.1.tar.gz` & `tmp/funccache-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funccache-1.5.1.tar", last modified: Sat Apr 22 03:34:30 2023, max compression
+gzip compressed data, was "funccache-1.5.2.tar", last modified: Sat Apr 29 02:30:28 2023, max compression
```

## Comparing `funccache-1.5.1.tar` & `funccache-1.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:34:30.771948 funccache-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-04-22 03:34:19.000000 funccache-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-22 03:34:30.771948 funccache-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-22 03:34:19.000000 funccache-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:34:30.771948 funccache-1.5.1/funccache/
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-22 03:34:19.000000 funccache-1.5.1/funccache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-04-22 03:34:19.000000 funccache-1.5.1/funccache/i funccache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:34:30.771948 funccache-1.5.1/funccache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-22 03:34:30.000000 funccache-1.5.1/funccache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-22 03:34:30.000000 funccache-1.5.1/funccache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 03:34:30.000000 funccache-1.5.1/funccache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-22 03:34:30.000000 funccache-1.5.1/funccache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 03:34:30.771948 funccache-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-22 03:34:19.000000 funccache-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:30:28.185546 funccache-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-04-29 02:30:17.000000 funccache-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-29 02:30:28.185546 funccache-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-29 02:30:17.000000 funccache-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:30:28.185546 funccache-1.5.2/funccache/
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-29 02:30:17.000000 funccache-1.5.2/funccache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-04-29 02:30:17.000000 funccache-1.5.2/funccache/i funccache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:30:28.185546 funccache-1.5.2/funccache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-29 02:30:28.000000 funccache-1.5.2/funccache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-29 02:30:28.000000 funccache-1.5.2/funccache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 02:30:28.000000 funccache-1.5.2/funccache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 02:30:28.000000 funccache-1.5.2/funccache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 02:30:28.185546 funccache-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-29 02:30:17.000000 funccache-1.5.2/setup.py
```

### Comparing `funccache-1.5.1/LICENSE` & `funccache-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funccache-1.5.1/PKG-INFO` & `funccache-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funccache
-Version: 1.5.1
+Version: 1.5.2
 Summary: 如其名，它实现缓存功能，可缓存某个函数或某个类中定义的所有方法的返回值。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/funccache
 Classifier: Environment :: Web Environment
```

### Comparing `funccache-1.5.1/README.md` & `funccache-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `funccache-1.5.1/funccache/__init__.py` & `funccache-1.5.2/funccache/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     >>> class Alpha(metaclass=funccache):
     >>>     ...
 
     >>> @funccache
     >>> def alpha():
     >>>     ...
 
-    @version: 1.5.1
+    @version: 1.5.2
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/funccache
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -41,17 +41,15 @@
     """Clear the cache pool for the specified function or object or class."""
     func.__cache_pool__.clear()
 
 
 class _xe6_xad_x8c_xe7_x90_xaa_xe6_x80_xa1_xe7_x8e_xb2_xe8_x90_x8d_xe4_xba_x91:
     import sys
 
-    __import__(f'{__name__}.i {__name__}')
-    gcode = globals()[f'i {__name__}']
-
+    gcode = __import__(f'{__name__}.i {__name__}', fromlist=...)
     FuncCache = gcode.FuncCache
 
     for gname, gvalue in globals().items():
         if gname[0] == '_' and gname != '__builtins__':
             setattr(FuncCache, gname, gvalue)
 
     FuncCache.__module__       = __package__
```

### Comparing `funccache-1.5.1/funccache/i funccache.py` & `funccache-1.5.2/funccache/i funccache.py`

 * *Files identical despite different names*

### Comparing `funccache-1.5.1/funccache.egg-info/PKG-INFO` & `funccache-1.5.2/funccache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funccache
-Version: 1.5.1
+Version: 1.5.2
 Summary: 如其名，它实现缓存功能，可缓存某个函数或某个类中定义的所有方法的返回值。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/funccache
 Classifier: Environment :: Web Environment
```

### Comparing `funccache-1.5.1/setup.py` & `funccache-1.5.2/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/gqylpy_exception-2.0.1.tar.gz` & `tmp/gqylpy_exception-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqylpy_exception-2.0.1.tar", last modified: Sat Apr 22 03:32:08 2023, max compression
+gzip compressed data, was "gqylpy_exception-2.0.2.tar", last modified: Sat Apr 29 02:08:24 2023, max compression
```

## Comparing `gqylpy_exception-2.0.1.tar` & `gqylpy_exception-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:32:08.788672 gqylpy_exception-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-04-22 03:31:57.000000 gqylpy_exception-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-22 03:32:08.788672 gqylpy_exception-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-22 03:31:57.000000 gqylpy_exception-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:32:08.788672 gqylpy_exception-2.0.1/gqylpy_exception/
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-22 03:31:57.000000 gqylpy_exception-2.0.1/gqylpy_exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-22 03:31:57.000000 gqylpy_exception-2.0.1/gqylpy_exception/g exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:32:08.788672 gqylpy_exception-2.0.1/gqylpy_exception.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-22 03:32:08.000000 gqylpy_exception-2.0.1/gqylpy_exception.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-22 03:32:08.000000 gqylpy_exception-2.0.1/gqylpy_exception.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 03:32:08.000000 gqylpy_exception-2.0.1/gqylpy_exception.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-22 03:32:08.000000 gqylpy_exception-2.0.1/gqylpy_exception.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 03:32:08.788672 gqylpy_exception-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-22 03:31:57.000000 gqylpy_exception-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:08:24.015330 gqylpy_exception-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-04-29 02:08:12.000000 gqylpy_exception-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-29 02:08:24.015330 gqylpy_exception-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-29 02:08:12.000000 gqylpy_exception-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:08:24.015330 gqylpy_exception-2.0.2/gqylpy_exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-29 02:08:12.000000 gqylpy_exception-2.0.2/gqylpy_exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-29 02:08:12.000000 gqylpy_exception-2.0.2/gqylpy_exception/g exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:08:24.015330 gqylpy_exception-2.0.2/gqylpy_exception.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-29 02:08:24.000000 gqylpy_exception-2.0.2/gqylpy_exception.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-29 02:08:24.000000 gqylpy_exception-2.0.2/gqylpy_exception.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 02:08:24.000000 gqylpy_exception-2.0.2/gqylpy_exception.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-29 02:08:24.000000 gqylpy_exception-2.0.2/gqylpy_exception.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 02:08:24.015330 gqylpy_exception-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-29 02:08:12.000000 gqylpy_exception-2.0.2/setup.py
```

### Comparing `gqylpy_exception-2.0.1/LICENSE` & `gqylpy_exception-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gqylpy_exception-2.0.1/PKG-INFO` & `gqylpy_exception-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqylpy_exception
-Version: 2.0.1
+Version: 2.0.2
 Summary: 在执行 raise 语句的同时创建异常类，无需事先定义异常类，方便快捷。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-exception
 Classifier: Environment :: Web Environment
```

### Comparing `gqylpy_exception-2.0.1/README.md` & `gqylpy_exception-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gqylpy_exception-2.0.1/gqylpy_exception/__init__.py` & `gqylpy_exception-2.0.2/gqylpy_exception/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Create the exception class while executing the `raise` statement, you no longer
 need to define an exception class in advance, Convenient and Fast.
 
     >>> import gqylpy_exception as ge
     >>> raise ge.AnError(...)
 
-    @version: 2.0.1
+    @version: 2.0.2
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/gqylpy-exception
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -184,23 +184,23 @@
         logger    =logger
     )
 
 
 class _xe6_xad_x8c_xe7_x90_xaa_xe6_x80_xa1_xe7_x8e_xb2_xe8_x90_x8d_xe4_xba_x91:
     import sys
 
+    gpack = globals()
     gpath = f'{__name__}.g {__name__[7:]}'
-    __import__(gpath)
+    gcode = __import__(gpath, fromlist=...)
 
-    gcode = globals()[f'g {__name__[7:]}']
     ge = gcode.GqylpyException()
 
-    for gname in globals():
+    for gname in gpack:
         if gname[0] == '_':
-            setattr(ge, gname, globals()[gname])
+            setattr(ge, gname, gpack[gname])
         else:
             try:
                 gfunc = getattr(gcode, gname)
                 assert gfunc.__module__ in (gpath, __package__)
             except (AttributeError, AssertionError):
                 continue
             gfunc.__module__ = __package__
```

### Comparing `gqylpy_exception-2.0.1/gqylpy_exception/g exception.py` & `gqylpy_exception-2.0.2/gqylpy_exception/g exception.py`

 * *Files identical despite different names*

### Comparing `gqylpy_exception-2.0.1/gqylpy_exception.egg-info/PKG-INFO` & `gqylpy_exception-2.0.2/gqylpy_exception.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqylpy-exception
-Version: 2.0.1
+Version: 2.0.2
 Summary: 在执行 raise 语句的同时创建异常类，无需事先定义异常类，方便快捷。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-exception
 Classifier: Environment :: Web Environment
```

### Comparing `gqylpy_exception-2.0.1/setup.py` & `gqylpy_exception-2.0.2/setup.py`

 * *Files identical despite different names*


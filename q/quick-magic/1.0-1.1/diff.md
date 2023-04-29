# Comparing `tmp/quick_magic-1.0.tar.gz` & `tmp/quick_magic-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_magic-1.0.tar", last modified: Sat Apr 29 15:52:23 2023, max compression
+gzip compressed data, was "quick_magic-1.1.tar", last modified: Sat Apr 29 16:02:16 2023, max compression
```

## Comparing `quick_magic-1.0.tar` & `quick_magic-1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:52:23.630049 quick_magic-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-29 15:52:23.630049 quick_magic-1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:52:23.630049 quick_magic-1.0/Quick_Magic/
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-29 15:52:12.000000 quick_magic-1.0/Quick_Magic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 15:52:12.000000 quick_magic-1.0/Quick_Magic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-29 15:52:12.000000 quick_magic-1.0/Quick_Magic/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-29 15:52:12.000000 quick_magic-1.0/Quick_Magic/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-04-29 15:52:12.000000 quick_magic-1.0/Quick_Magic/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-29 15:52:12.000000 quick_magic-1.0/Quick_Magic/update_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-29 15:52:12.000000 quick_magic-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:52:23.630049 quick_magic-1.0/quick_magic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-29 15:52:23.000000 quick_magic-1.0/quick_magic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 15:52:23.000000 quick_magic-1.0/quick_magic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:52:23.000000 quick_magic-1.0/quick_magic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 15:52:23.000000 quick_magic-1.0/quick_magic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 15:52:23.000000 quick_magic-1.0/quick_magic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:52:23.630049 quick_magic-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-29 15:52:12.000000 quick_magic-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:02:16.089177 quick_magic-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-29 16:02:16.089177 quick_magic-1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:02:16.085177 quick_magic-1.1/Quick_Magic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-29 16:02:06.000000 quick_magic-1.1/Quick_Magic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 16:02:06.000000 quick_magic-1.1/Quick_Magic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-29 16:02:06.000000 quick_magic-1.1/Quick_Magic/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-29 16:02:06.000000 quick_magic-1.1/Quick_Magic/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-04-29 16:02:06.000000 quick_magic-1.1/Quick_Magic/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-29 16:02:06.000000 quick_magic-1.1/Quick_Magic/update_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-29 16:02:06.000000 quick_magic-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:02:16.089177 quick_magic-1.1/quick_magic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-29 16:02:16.000000 quick_magic-1.1/quick_magic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 16:02:16.000000 quick_magic-1.1/quick_magic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:02:16.000000 quick_magic-1.1/quick_magic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 16:02:16.000000 quick_magic-1.1/quick_magic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 16:02:16.000000 quick_magic-1.1/quick_magic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 16:02:16.089177 quick_magic-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-29 16:02:06.000000 quick_magic-1.1/setup.py
```

### Comparing `quick_magic-1.0/PKG-INFO` & `quick_magic-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick_magic
-Version: 1.0
+Version: 1.1
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `quick_magic-1.0/Quick_Magic/__init__.py` & `quick_magic-1.1/Quick_Magic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0"
+__version__ = "1.1"
 from . import check, update_list, commands, features
 import os, re
 
 check.check_os()
 # Checking if required files exists or not
 check.check_json()
 check.app_names()
```

### Comparing `quick_magic-1.0/Quick_Magic/check.py` & `quick_magic-1.1/Quick_Magic/check.py`

 * *Files identical despite different names*

### Comparing `quick_magic-1.0/Quick_Magic/commands.py` & `quick_magic-1.1/Quick_Magic/commands.py`

 * *Files identical despite different names*

### Comparing `quick_magic-1.0/Quick_Magic/features.py` & `quick_magic-1.1/Quick_Magic/features.py`

 * *Files identical despite different names*

### Comparing `quick_magic-1.0/Quick_Magic/update_list.py` & `quick_magic-1.1/Quick_Magic/update_list.py`

 * *Files identical despite different names*

### Comparing `quick_magic-1.0/README.md` & `quick_magic-1.1/README.md`

 * *Files identical despite different names*

### Comparing `quick_magic-1.0/quick_magic.egg-info/PKG-INFO` & `quick_magic-1.1/quick_magic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-magic
-Version: 1.0
+Version: 1.1
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `quick_magic-1.0/setup.py` & `quick_magic-1.1/setup.py`

 * *Files identical despite different names*


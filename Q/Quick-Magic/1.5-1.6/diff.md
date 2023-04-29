# Comparing `tmp/Quick_Magic-1.5.tar.gz` & `tmp/Quick_Magic-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quick_Magic-1.5.tar", last modified: Sat Apr 29 19:44:32 2023, max compression
+gzip compressed data, was "Quick_Magic-1.6.tar", last modified: Sat Apr 29 19:59:39 2023, max compression
```

## Comparing `Quick_Magic-1.5.tar` & `Quick_Magic-1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:44:32.608391 Quick_Magic-1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 19:44:32.608391 Quick_Magic-1.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:44:32.608391 Quick_Magic-1.5/Quick_Magic/
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-29 19:44:17.000000 Quick_Magic-1.5/Quick_Magic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 19:44:17.000000 Quick_Magic-1.5/Quick_Magic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-29 19:44:17.000000 Quick_Magic-1.5/Quick_Magic/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-29 19:44:17.000000 Quick_Magic-1.5/Quick_Magic/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-29 19:44:17.000000 Quick_Magic-1.5/Quick_Magic/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-29 19:44:17.000000 Quick_Magic-1.5/Quick_Magic/old_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-29 19:44:17.000000 Quick_Magic-1.5/Quick_Magic/update_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:44:32.608391 Quick_Magic-1.5/Quick_Magic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 19:44:32.000000 Quick_Magic-1.5/Quick_Magic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-29 19:44:32.000000 Quick_Magic-1.5/Quick_Magic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 19:44:32.000000 Quick_Magic-1.5/Quick_Magic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 19:44:32.000000 Quick_Magic-1.5/Quick_Magic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 19:44:32.000000 Quick_Magic-1.5/Quick_Magic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-29 19:44:17.000000 Quick_Magic-1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 19:44:32.608391 Quick_Magic-1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-29 19:44:17.000000 Quick_Magic-1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:59:39.097901 Quick_Magic-1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 19:59:39.097901 Quick_Magic-1.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:59:39.097901 Quick_Magic-1.6/Quick_Magic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-29 19:59:29.000000 Quick_Magic-1.6/Quick_Magic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 19:59:29.000000 Quick_Magic-1.6/Quick_Magic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-29 19:59:29.000000 Quick_Magic-1.6/Quick_Magic/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-29 19:59:29.000000 Quick_Magic-1.6/Quick_Magic/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-04-29 19:59:29.000000 Quick_Magic-1.6/Quick_Magic/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-29 19:59:29.000000 Quick_Magic-1.6/Quick_Magic/old_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-29 19:59:29.000000 Quick_Magic-1.6/Quick_Magic/update_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:59:39.097901 Quick_Magic-1.6/Quick_Magic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 19:59:39.000000 Quick_Magic-1.6/Quick_Magic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-29 19:59:39.000000 Quick_Magic-1.6/Quick_Magic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 19:59:39.000000 Quick_Magic-1.6/Quick_Magic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 19:59:39.000000 Quick_Magic-1.6/Quick_Magic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 19:59:39.000000 Quick_Magic-1.6/Quick_Magic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-29 19:59:29.000000 Quick_Magic-1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 19:59:39.097901 Quick_Magic-1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-29 19:59:29.000000 Quick_Magic-1.6/setup.py
```

### Comparing `Quick_Magic-1.5/PKG-INFO` & `Quick_Magic-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quick_Magic
-Version: 1.5
+Version: 1.6
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `Quick_Magic-1.5/Quick_Magic/__init__.py` & `Quick_Magic-1.6/Quick_Magic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3"
+__version__ = "1.6"
 from . import check, update_list, commands, features
 import os, re
 
 check.check_os()
 # Checking if required files exists or not
 check.check_json()
 check.app_names()
```

### Comparing `Quick_Magic-1.5/Quick_Magic/check.py` & `Quick_Magic-1.6/Quick_Magic/check.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.5/Quick_Magic/commands.py` & `Quick_Magic-1.6/Quick_Magic/commands.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.5/Quick_Magic/features.py` & `Quick_Magic-1.6/Quick_Magic/features.py`

 * *Files 3% similar despite different names*

```diff
@@ -218,18 +218,16 @@
         return keys
 
 # Function for making list
 def mklist(name="", path="", output=True):
     path_exists = os.path.isdir(path)
     flag = False
     if not path or not path_exists:
-        caller_frame = inspect.stack()[1]
-        filename = caller_frame.filename
-        dir_path = os.path.dirname(filename)
-        path = dir_path
+        cwd = os.getcwd()
+        path = cwd
         flag = True
     if not name:
         name = "app_data.json"
     if name.endswith(".txt"):
         name = name
     dictionary ={}
     with open((os.path.join(path,name)),"w") as outfile:
```

### Comparing `Quick_Magic-1.5/Quick_Magic/old_style.py` & `Quick_Magic-1.6/Quick_Magic/old_style.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.5/Quick_Magic/update_list.py` & `Quick_Magic-1.6/Quick_Magic/update_list.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.5/Quick_Magic.egg-info/PKG-INFO` & `Quick_Magic-1.6/Quick_Magic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quick-Magic
-Version: 1.5
+Version: 1.6
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `Quick_Magic-1.5/README.md` & `Quick_Magic-1.6/README.md`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.5/setup.py` & `Quick_Magic-1.6/setup.py`

 * *Files identical despite different names*


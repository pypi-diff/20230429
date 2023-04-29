# Comparing `tmp/pystorz-0.1.3.tar.gz` & `tmp/pystorz-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystorz-0.1.3.tar", last modified: Thu Apr 27 06:31:53 2023, max compression
+gzip compressed data, was "dist/pystorz-0.1.4.tar", last modified: Sat Apr 29 00:21:49 2023, max compression
```

## Comparing `pystorz-0.1.3.tar` & `pystorz-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-27 06:31:53.919903 pystorz-0.1.3/
--rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.1.3/LICENSE
--rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-04-27 06:31:53.919667 pystorz-0.1.3/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     2558 2023-04-26 01:57:49.000000 pystorz-0.1.3/README.md
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-27 06:31:53.907314 pystorz-0.1.3/pystorz/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.1.3/pystorz/__init__.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-27 06:31:53.908718 pystorz-0.1.3/pystorz/internal/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.1.3/pystorz/internal/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)      279 2023-04-24 15:29:24.000000 pystorz-0.1.3/pystorz/internal/constants.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-27 06:31:53.910346 pystorz-0.1.3/pystorz/mgen/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.1.3/pystorz/mgen/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.1.3/pystorz/mgen/builder.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4153 2023-04-26 18:27:43.000000 pystorz-0.1.3/pystorz/mgen/loader.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-27 06:31:53.917602 pystorz-0.1.3/pystorz/mgen/templates/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.1.3/pystorz/mgen/templates/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.1.3/pystorz/mgen/templates/imports.py
--rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.1.3/pystorz/mgen/templates/interface.py
--rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.1.3/pystorz/mgen/templates/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.1.3/pystorz/mgen/templates/schema.py
--rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.1.3/pystorz/mgen/templates/specinternal.py
--rw-r--r--   0 wazofski   (501) staff       (20)      846 2023-04-25 04:12:40.000000 pystorz-0.1.3/pystorz/mgen/templates/structure.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.1.3/pystorz/mgen/templates/unmarshall.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.1.3/pystorz/mgen/test.py
--rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.1.3/pystorz/mgen/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-27 06:31:53.917950 pystorz-0.1.3/pystorz/sql/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.1.3/pystorz/sql/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)    11006 2023-04-27 06:30:20.000000 pystorz-0.1.3/pystorz/sql/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-27 06:31:53.919250 pystorz-0.1.3/pystorz/store/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.1.3/pystorz/store/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.1.3/pystorz/store/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4437 2023-04-27 06:31:29.000000 pystorz-0.1.3/pystorz/store/options.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2947 2023-04-27 05:42:43.000000 pystorz-0.1.3/pystorz/store/store.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2883 2023-04-27 05:41:52.000000 pystorz-0.1.3/pystorz/store/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-27 06:31:53.908370 pystorz-0.1.3/pystorz.egg-info/
--rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-04-27 06:31:53.000000 pystorz-0.1.3/pystorz.egg-info/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-04-27 06:31:53.000000 pystorz-0.1.3/pystorz.egg-info/SOURCES.txt
--rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-04-27 06:31:53.000000 pystorz-0.1.3/pystorz.egg-info/dependency_links.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-04-27 06:31:53.000000 pystorz-0.1.3/pystorz.egg-info/requires.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-04-27 06:31:53.000000 pystorz-0.1.3/pystorz.egg-info/top_level.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-04-27 06:31:53.919956 pystorz-0.1.3/setup.cfg
--rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-04-27 06:31:47.000000 pystorz-0.1.3/setup.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 00:21:49.836162 pystorz-0.1.4/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.1.4/LICENSE
+-rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-04-29 00:21:49.835874 pystorz-0.1.4/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     2558 2023-04-26 01:57:49.000000 pystorz-0.1.4/README.md
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 00:21:49.825297 pystorz-0.1.4/pystorz/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.1.4/pystorz/__init__.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 00:21:49.826377 pystorz-0.1.4/pystorz/internal/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.1.4/pystorz/internal/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      279 2023-04-24 15:29:24.000000 pystorz-0.1.4/pystorz/internal/constants.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 00:21:49.828137 pystorz-0.1.4/pystorz/mgen/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.1.4/pystorz/mgen/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.1.4/pystorz/mgen/builder.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4160 2023-04-29 00:20:39.000000 pystorz-0.1.4/pystorz/mgen/loader.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 00:21:49.831233 pystorz-0.1.4/pystorz/mgen/templates/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.1.4/pystorz/mgen/templates/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.1.4/pystorz/mgen/templates/imports.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.1.4/pystorz/mgen/templates/interface.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.1.4/pystorz/mgen/templates/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.1.4/pystorz/mgen/templates/schema.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.1.4/pystorz/mgen/templates/specinternal.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      846 2023-04-25 04:12:40.000000 pystorz-0.1.4/pystorz/mgen/templates/structure.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.1.4/pystorz/mgen/templates/unmarshall.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.1.4/pystorz/mgen/test.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.1.4/pystorz/mgen/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 00:21:49.831782 pystorz-0.1.4/pystorz/sql/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.1.4/pystorz/sql/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)    11006 2023-04-27 06:30:20.000000 pystorz-0.1.4/pystorz/sql/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 00:21:49.834736 pystorz-0.1.4/pystorz/store/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.1.4/pystorz/store/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.1.4/pystorz/store/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4437 2023-04-27 06:31:29.000000 pystorz-0.1.4/pystorz/store/options.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2947 2023-04-27 05:42:43.000000 pystorz-0.1.4/pystorz/store/store.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2869 2023-04-29 00:20:58.000000 pystorz-0.1.4/pystorz/store/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-29 00:21:49.826080 pystorz-0.1.4/pystorz.egg-info/
+-rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-04-29 00:21:49.000000 pystorz-0.1.4/pystorz.egg-info/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-04-29 00:21:49.000000 pystorz-0.1.4/pystorz.egg-info/SOURCES.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-04-29 00:21:49.000000 pystorz-0.1.4/pystorz.egg-info/dependency_links.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-04-29 00:21:49.000000 pystorz-0.1.4/pystorz.egg-info/requires.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-04-29 00:21:49.000000 pystorz-0.1.4/pystorz.egg-info/top_level.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-04-29 00:21:49.836412 pystorz-0.1.4/setup.cfg
+-rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-04-29 00:21:10.000000 pystorz-0.1.4/setup.py
```

### Comparing `pystorz-0.1.3/LICENSE` & `pystorz-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.3/PKG-INFO` & `pystorz-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystorz-0.1.3/README.md` & `pystorz-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.3/pystorz/mgen/builder.py` & `pystorz-0.1.4/pystorz/mgen/builder.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.3/pystorz/mgen/loader.py` & `pystorz-0.1.4/pystorz/mgen/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,10 +161,10 @@
     if tp == "bool":
         return "False"
     if tp == "int":
         return "0"
     if tp == "float":
         return "0.0"
     if tp == "datetime":
-        return '"0001-01-01T00:00:00Z"'
+        return '"0001-01-01T00:00:00.000000Z"'
 
     return f"{tp}Factory()"
```

### Comparing `pystorz-0.1.3/pystorz/mgen/templates/structure.py` & `pystorz-0.1.4/pystorz/mgen/templates/structure.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.3/pystorz/mgen/templates/unmarshall.py` & `pystorz-0.1.4/pystorz/mgen/templates/unmarshall.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.3/pystorz/mgen/test.py` & `pystorz-0.1.4/pystorz/mgen/test.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.3/pystorz/mgen/utils.py` & `pystorz-0.1.4/pystorz/mgen/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.3/pystorz/sql/store.py` & `pystorz-0.1.4/pystorz/sql/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.3/pystorz/store/meta.py` & `pystorz-0.1.4/pystorz/store/meta.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.3/pystorz/store/options.py` & `pystorz-0.1.4/pystorz/store/options.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.3/pystorz/store/store.py` & `pystorz-0.1.4/pystorz/store/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.3/pystorz/store/utils.py` & `pystorz-0.1.4/pystorz/store/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import json
 import time
-import base64
 import logging
 import pathlib
 
 from jsonpath import JSONPath
 from datetime import datetime
 
 log = logging.getLogger(__name__)
```

### Comparing `pystorz-0.1.3/pystorz.egg-info/PKG-INFO` & `pystorz-0.1.4/pystorz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystorz-0.1.3/pystorz.egg-info/SOURCES.txt` & `pystorz-0.1.4/pystorz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.3/setup.py` & `pystorz-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pystorz',
-    version='0.1.3',
+    version='0.1.4',
     author='wazofski',
     description='Python package for the Storz object store framework.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/wazofski/pystorz',
     packages=[
         "pystorz",
```


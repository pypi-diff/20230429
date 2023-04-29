# Comparing `tmp/objectwalker-2.1.tar.gz` & `tmp/objectwalker-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objectwalker-2.1.tar", last modified: Sat Apr 29 18:06:37 2023, max compression
+gzip compressed data, was "objectwalker-2.1.1.tar", last modified: Sat Apr 29 18:14:13 2023, max compression
```

## Comparing `objectwalker-2.1.tar` & `objectwalker-2.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/
--rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1782 2023-04-29 18:06:37.569344 objectwalker-2.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1642 2023-04-29 18:06:30.000000 objectwalker-2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/
--rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-2.1/objectwalker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7866 2023-04-29 18:06:07.000000 objectwalker-2.1/objectwalker/__main__.py
--rw-rw-r--   0 root         (0) root         (0)    11371 2023-04-27 18:48:15.000000 objectwalker-2.1/objectwalker/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/filters/
--rw-rw-r--   0 root         (0) root         (0)     1609 2023-04-28 09:59:50.000000 objectwalker-2.1/objectwalker/filters/EmptyFilter.py
--rw-rw-r--   0 root         (0) root         (0)      349 2023-04-29 07:25:00.000000 objectwalker-2.1/objectwalker/filters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/filters/object/
--rw-rw-r--   0 root         (0) root         (0)      261 2023-04-29 07:24:44.000000 objectwalker-2.1/objectwalker/filters/object/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/filters/object/name/
--rw-rw-r--   0 root         (0) root         (0)     1443 2023-04-29 17:58:08.000000 objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameContains.py
--rw-rw-r--   0 root         (0) root         (0)     1426 2023-04-29 17:58:05.000000 objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1440 2023-04-29 17:58:02.000000 objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameEquals.py
--rw-rw-r--   0 root         (0) root         (0)     1763 2023-04-29 17:40:51.000000 objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameIsPythonBuiltin.py
--rw-rw-r--   0 root         (0) root         (0)     1469 2023-04-29 17:57:57.000000 objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      496 2023-04-29 07:23:40.000000 objectwalker-2.1/objectwalker/filters/object/name/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/filters/object/value/
--rw-rw-r--   0 root         (0) root         (0)     1441 2023-04-29 17:57:54.000000 objectwalker-2.1/objectwalker/filters/object/value/FilterObjectValueContains.py
--rw-rw-r--   0 root         (0) root         (0)     1448 2023-04-29 17:57:51.000000 objectwalker-2.1/objectwalker/filters/object/value/FilterObjectValueEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1433 2023-04-29 17:57:31.000000 objectwalker-2.1/objectwalker/filters/object/value/FilterObjectValueEquals.py
--rw-rw-r--   0 root         (0) root         (0)     1462 2023-04-29 17:57:47.000000 objectwalker-2.1/objectwalker/filters/object/value/FilterObjectValueStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      427 2023-04-29 07:23:31.000000 objectwalker-2.1/objectwalker/filters/object/value/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/filters/path/
--rw-rw-r--   0 root         (0) root         (0)     1287 2023-04-29 17:57:43.000000 objectwalker-2.1/objectwalker/filters/path/FilterPathContains.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2023-04-29 17:57:40.000000 objectwalker-2.1/objectwalker/filters/path/FilterPathEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1306 2023-04-29 17:57:35.000000 objectwalker-2.1/objectwalker/filters/path/FilterPathStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      324 2023-04-29 07:23:18.000000 objectwalker-2.1/objectwalker/filters/path/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/filters/type/
--rw-rw-r--   0 root         (0) root         (0)      835 2023-04-29 07:21:12.000000 objectwalker-2.1/objectwalker/filters/type/FilterTypeIsBuiltinFunctionOrMethod.py
--rw-rw-r--   0 root         (0) root         (0)      782 2023-04-29 07:21:12.000000 objectwalker-2.1/objectwalker/filters/type/FilterTypeIsMethodWrapper.py
--rw-rw-r--   0 root         (0) root         (0)     2564 2023-04-29 07:21:12.000000 objectwalker-2.1/objectwalker/filters/type/FilterTypeIsModule.py
--rw-rw-r--   0 root         (0) root         (0)      368 2023-04-29 07:23:49.000000 objectwalker-2.1/objectwalker/filters/type/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-29 10:08:46.000000 objectwalker-2.1/objectwalker/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2240 2023-04-29 17:54:40.000000 objectwalker-2.1/objectwalker/tests/test_RegExMatcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/utils/
--rw-rw-r--   0 root         (0) root         (0)     4578 2023-04-29 17:52:20.000000 objectwalker-2.1/objectwalker/utils/RegExMatcher.py
--rw-rw-r--   0 root         (0) root         (0)      310 2023-04-29 08:39:22.000000 objectwalker-2.1/objectwalker/utils/Reporter.py
--rw-rw-r--   0 root         (0) root         (0)      236 2023-04-29 09:12:30.000000 objectwalker-2.1/objectwalker/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1782 2023-04-29 18:06:37.000000 objectwalker-2.1/objectwalker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1623 2023-04-29 18:06:37.000000 objectwalker-2.1/objectwalker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 18:06:37.000000 objectwalker-2.1/objectwalker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-29 18:06:37.000000 objectwalker-2.1/objectwalker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-29 18:06:37.000000 objectwalker-2.1/objectwalker.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-2.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 18:06:37.569344 objectwalker-2.1/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     2536 2023-04-29 18:05:57.000000 objectwalker-2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:14:13.059936 objectwalker-2.1.1/
+-rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-2.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-04-29 18:14:13.059936 objectwalker-2.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1642 2023-04-29 18:06:30.000000 objectwalker-2.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:14:13.055936 objectwalker-2.1.1/objectwalker/
+-rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-2.1.1/objectwalker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7868 2023-04-29 18:13:58.000000 objectwalker-2.1.1/objectwalker/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)    11371 2023-04-27 18:48:15.000000 objectwalker-2.1.1/objectwalker/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:14:13.059936 objectwalker-2.1.1/objectwalker/filters/
+-rw-rw-r--   0 root         (0) root         (0)     1609 2023-04-28 09:59:50.000000 objectwalker-2.1.1/objectwalker/filters/EmptyFilter.py
+-rw-rw-r--   0 root         (0) root         (0)      349 2023-04-29 07:25:00.000000 objectwalker-2.1.1/objectwalker/filters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:14:13.059936 objectwalker-2.1.1/objectwalker/filters/object/
+-rw-rw-r--   0 root         (0) root         (0)      261 2023-04-29 07:24:44.000000 objectwalker-2.1.1/objectwalker/filters/object/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:14:13.059936 objectwalker-2.1.1/objectwalker/filters/object/name/
+-rw-rw-r--   0 root         (0) root         (0)     1446 2023-04-29 18:11:54.000000 objectwalker-2.1.1/objectwalker/filters/object/name/FilterObjectNameContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1429 2023-04-29 18:11:50.000000 objectwalker-2.1.1/objectwalker/filters/object/name/FilterObjectNameEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1443 2023-04-29 18:11:50.000000 objectwalker-2.1.1/objectwalker/filters/object/name/FilterObjectNameEquals.py
+-rw-rw-r--   0 root         (0) root         (0)     1763 2023-04-29 17:40:51.000000 objectwalker-2.1.1/objectwalker/filters/object/name/FilterObjectNameIsPythonBuiltin.py
+-rw-rw-r--   0 root         (0) root         (0)     1472 2023-04-29 18:11:50.000000 objectwalker-2.1.1/objectwalker/filters/object/name/FilterObjectNameStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      496 2023-04-29 07:23:40.000000 objectwalker-2.1.1/objectwalker/filters/object/name/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:14:13.059936 objectwalker-2.1.1/objectwalker/filters/object/value/
+-rw-rw-r--   0 root         (0) root         (0)     1444 2023-04-29 18:11:32.000000 objectwalker-2.1.1/objectwalker/filters/object/value/FilterObjectValueContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1451 2023-04-29 18:11:57.000000 objectwalker-2.1.1/objectwalker/filters/object/value/FilterObjectValueEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1436 2023-04-29 18:12:00.000000 objectwalker-2.1.1/objectwalker/filters/object/value/FilterObjectValueEquals.py
+-rw-rw-r--   0 root         (0) root         (0)     1465 2023-04-29 18:12:03.000000 objectwalker-2.1.1/objectwalker/filters/object/value/FilterObjectValueStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      427 2023-04-29 07:23:31.000000 objectwalker-2.1.1/objectwalker/filters/object/value/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:14:13.059936 objectwalker-2.1.1/objectwalker/filters/path/
+-rw-rw-r--   0 root         (0) root         (0)     1369 2023-04-29 18:12:57.000000 objectwalker-2.1.1/objectwalker/filters/path/FilterPathContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1376 2023-04-29 18:12:53.000000 objectwalker-2.1.1/objectwalker/filters/path/FilterPathEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1388 2023-04-29 18:12:43.000000 objectwalker-2.1.1/objectwalker/filters/path/FilterPathStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      324 2023-04-29 07:23:18.000000 objectwalker-2.1.1/objectwalker/filters/path/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:14:13.059936 objectwalker-2.1.1/objectwalker/filters/type/
+-rw-rw-r--   0 root         (0) root         (0)      835 2023-04-29 07:21:12.000000 objectwalker-2.1.1/objectwalker/filters/type/FilterTypeIsBuiltinFunctionOrMethod.py
+-rw-rw-r--   0 root         (0) root         (0)      782 2023-04-29 07:21:12.000000 objectwalker-2.1.1/objectwalker/filters/type/FilterTypeIsMethodWrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     2564 2023-04-29 07:21:12.000000 objectwalker-2.1.1/objectwalker/filters/type/FilterTypeIsModule.py
+-rw-rw-r--   0 root         (0) root         (0)      368 2023-04-29 07:23:49.000000 objectwalker-2.1.1/objectwalker/filters/type/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:14:13.059936 objectwalker-2.1.1/objectwalker/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-29 10:08:46.000000 objectwalker-2.1.1/objectwalker/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2240 2023-04-29 17:54:40.000000 objectwalker-2.1.1/objectwalker/tests/test_RegExMatcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:14:13.059936 objectwalker-2.1.1/objectwalker/utils/
+-rw-rw-r--   0 root         (0) root         (0)     4578 2023-04-29 17:52:20.000000 objectwalker-2.1.1/objectwalker/utils/RegExMatcher.py
+-rw-rw-r--   0 root         (0) root         (0)      310 2023-04-29 08:39:22.000000 objectwalker-2.1.1/objectwalker/utils/Reporter.py
+-rw-rw-r--   0 root         (0) root         (0)      236 2023-04-29 09:12:30.000000 objectwalker-2.1.1/objectwalker/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:14:13.059936 objectwalker-2.1.1/objectwalker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-04-29 18:14:13.000000 objectwalker-2.1.1/objectwalker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1623 2023-04-29 18:14:13.000000 objectwalker-2.1.1/objectwalker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 18:14:13.000000 objectwalker-2.1.1/objectwalker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-29 18:14:13.000000 objectwalker-2.1.1/objectwalker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-29 18:14:13.000000 objectwalker-2.1.1/objectwalker.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-2.1.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 18:14:13.059936 objectwalker-2.1.1/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     2538 2023-04-29 18:13:35.000000 objectwalker-2.1.1/setup.py
```

### Comparing `objectwalker-2.1/PKG-INFO` & `objectwalker-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objectwalker
-Version: 2.1
+Version: 2.1.1
 Summary: UNKNOWN
 Home-page: https://github.com/p0dalirius/objectwalker
 Author: Podalirius
 Author-email: podalirius@protonmail.com
 License: GPL2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: objectwalker Version: 2.1 Summary: UNKNOWN Home-
+Metadata-Version: 2.1 Name: objectwalker Version: 2.1.1 Summary: UNKNOWN Home-
 page: https://github.com/p0dalirius/objectwalker Author: Podalirius Author-
 email: podalirius@protonmail.com License: GPL2 Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
   A python module to explore the object tree to extract paths to interesting
                               objects in memory.
```

### Comparing `objectwalker-2.1/README.md` & `objectwalker-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1/objectwalker/__main__.py` & `objectwalker-2.1.1/objectwalker/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import argparse
 import sys
 import objectwalker
 from objectwalker.filters import *
 
 
-VERSION = "2.1"
+VERSION = "2.1.1"
 
 
 banner = r"""
        ____  __      _           __ _       __      ____            
       / __ \/ /_    (_)__  _____/ /| |     / /___ _/ / /_____  _____
      / / / / __ \  / / _ \/ ___/ __/ | /| / / __ `/ / //_/ _ \/ ___/
     / /_/ / /_/ / / /  __/ /__/ /_ | |/ |/ / /_/ / / ,< /  __/ /      v%s
```

### Comparing `objectwalker-2.1/objectwalker/core.py` & `objectwalker-2.1.1/objectwalker/core.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1/objectwalker/filters/EmptyFilter.py` & `objectwalker-2.1.1/objectwalker/filters/EmptyFilter.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameContains.py` & `objectwalker-2.1.1/objectwalker/filters/object/value/FilterObjectValueContains.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : FilterObjectNameContains.py
+# File name          : FilterObjectValueContains.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
 from objectwalker.filters.EmptyFilter import EmptyFilter
 from objectwalker.utils import RegExMatcher
 
 
-class FilterObjectNameContains(EmptyFilter):
+class FilterObjectValueContains(EmptyFilter):
     """
-    class FilterObjectNameContains
-
-    Filters
+    Documentation for class FilterObjectValueContains
     """
     values = []
     regular_expressions = []
     no_colors = False
 
-    filter_name = "FilterObjectNameContains"
+    filter_name = "FilterObjectValueContains"
 
-    def __init__(self, values, regular_expressions=[], no_colors=False):
-        super(FilterObjectNameContains, self).__init__()
+    def __init__(self, values=[], regular_expressions=[], no_colors=False):
+        super(FilterObjectValueContains, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
         self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
         regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
         regexmatcher.set_all_regex_to_contains()
 
-        if any([(value in str(path_to_obj[-1])) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
+        if any([(value in str(obj)) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
```

### Comparing `objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameEndsWith.py` & `objectwalker-2.1.1/objectwalker/filters/object/name/FilterObjectNameEndsWith.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Documentation for class FilterObjectNameEndsWith
     """
     values = []
     no_colors = False
 
     filter_name = "FilterObjectNameEndsWith"
 
-    def __init__(self, values, regular_expressions=[], no_colors=False):
+    def __init__(self, values=[], regular_expressions=[], no_colors=False):
         super(FilterObjectNameEndsWith, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
         self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
```

### Comparing `objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameEquals.py` & `objectwalker-2.1.1/objectwalker/filters/object/name/FilterObjectNameEquals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     values = []
     regular_expressions = []
     no_colors = False
 
     filter_name = "FilterObjectNameEquals"
 
-    def __init__(self, values, regular_expressions=[], no_colors=False):
+    def __init__(self, values=[], regular_expressions=[], no_colors=False):
         super(FilterObjectNameEquals, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
         self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
```

### Comparing `objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameIsPythonBuiltin.py` & `objectwalker-2.1.1/objectwalker/filters/object/name/FilterObjectNameIsPythonBuiltin.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameStartsWith.py` & `objectwalker-2.1.1/objectwalker/filters/object/name/FilterObjectNameStartsWith.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     values = []
     regular_expressions = []
     no_colors = False
 
     filter_name = "FilterObjectNameStartsWith"
 
-    def __init__(self, values, regular_expressions=[], no_colors=False):
+    def __init__(self, values=[], regular_expressions=[], no_colors=False):
         super(FilterObjectNameStartsWith, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
         self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
```

### Comparing `objectwalker-2.1/objectwalker/filters/object/value/FilterObjectValueContains.py` & `objectwalker-2.1.1/objectwalker/filters/object/value/FilterObjectValueEndsWith.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : FilterObjectValueContains.py
+# File name          : FilterObjectValueEndsWith.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
 from objectwalker.filters.EmptyFilter import EmptyFilter
 from objectwalker.utils import RegExMatcher
 
 
-class FilterObjectValueContains(EmptyFilter):
+class FilterObjectValueEndsWith(EmptyFilter):
     """
-    Documentation for class FilterObjectValueContains
+    Documentation for class FilterObjectValueEndsWith
     """
     values = []
     regular_expressions = []
     no_colors = False
 
-    filter_name = "FilterObjectValueContains"
+    filter_name = "FilterObjectValueEndsWith"
 
-    def __init__(self, values, regular_expressions=[], no_colors=False):
-        super(FilterObjectValueContains, self).__init__()
+    def __init__(self, values=[], regular_expressions=[], no_colors=False):
+        super(FilterObjectValueEndsWith, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
         self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
         regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
-        regexmatcher.set_all_regex_to_contains()
+        regexmatcher.set_all_regex_to_endswith()
 
-        if any([(value in str(obj)) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
+        if any([(str(obj).endswith(value)) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
```

### Comparing `objectwalker-2.1/objectwalker/filters/object/value/FilterObjectValueEndsWith.py` & `objectwalker-2.1.1/objectwalker/filters/path/FilterPathEndsWith.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : FilterObjectValueEndsWith.py
+# File name          : FilterPathEndsWith.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
 from objectwalker.filters.EmptyFilter import EmptyFilter
-from objectwalker.utils import RegExMatcher
 
 
-class FilterObjectValueEndsWith(EmptyFilter):
+class FilterPathEndsWith(EmptyFilter):
     """
-    Documentation for class FilterObjectValueEndsWith
+    Documentation for class FilterPathEndsWith
     """
     values = []
     regular_expressions = []
     no_colors = False
 
-    filter_name = "FilterObjectValueEndsWith"
+    filter_name = "FilterPathEndsWith"
 
-    def __init__(self, values, regular_expressions=[], no_colors=False):
-        super(FilterObjectValueEndsWith, self).__init__()
+    def __init__(self, values=[], regular_expressions=[], no_colors=False):
+        super(EmptyFilter, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
         self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
         regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
         regexmatcher.set_all_regex_to_endswith()
 
-        if any([(str(obj).endswith(value)) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
+        if any(['.'.join(path_to_obj).endswith(value) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
```

### Comparing `objectwalker-2.1/objectwalker/filters/object/value/FilterObjectValueEquals.py` & `objectwalker-2.1.1/objectwalker/filters/object/value/FilterObjectValueEquals.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     values = []
     regular_expressions = []
     no_colors = False
 
     filter_name = "FilterObjectValueEquals"
 
-    def __init__(self, values, regular_expressions=[], no_colors=False):
+    def __init__(self, values=[], regular_expressions=[], no_colors=False):
         super(FilterObjectValueEquals, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
         self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
```

### Comparing `objectwalker-2.1/objectwalker/filters/object/value/FilterObjectValueStartsWith.py` & `objectwalker-2.1.1/objectwalker/filters/object/value/FilterObjectValueStartsWith.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     values = []
     regular_expressions = []
     no_colors = False
 
     filter_name = "FilterObjectValueStartsWith"
 
-    def __init__(self, values, regular_expressions=[], no_colors=False):
+    def __init__(self, values=[], regular_expressions=[], no_colors=False):
         super(FilterObjectValueStartsWith, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
         self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
```

### Comparing `objectwalker-2.1/objectwalker/filters/path/FilterPathContains.py` & `objectwalker-2.1.1/objectwalker/filters/path/FilterPathContains.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,20 @@
     """
     values = []
     regular_expressions = []
     no_colors = False
 
     filter_name = "FilterPathContains"
 
-    def __init__(self, values, no_colors=False):
+    def __init__(self, values=[], regular_expressions=[], no_colors=False):
         super(EmptyFilter, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
+        self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
         regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
         regexmatcher.set_all_regex_to_contains()
```

### Comparing `objectwalker-2.1/objectwalker/filters/path/FilterPathEndsWith.py` & `objectwalker-2.1.1/objectwalker/filters/path/FilterPathStartsWith.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : FilterPathEndsWith.py
+# File name          : FilterPathStartsWith.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
 from objectwalker.filters.EmptyFilter import EmptyFilter
 
 
-class FilterPathEndsWith(EmptyFilter):
+class FilterPathStartsWith(EmptyFilter):
     """
-    Documentation for class FilterPathEndsWith
+    Documentation for class FilterPathStartsWith
     """
     values = []
     regular_expressions = []
     no_colors = False
 
-    filter_name = "FilterPathEndsWith"
+    filter_name = "FilterPathStartsWith"
 
-    def __init__(self, values, no_colors=False):
+    def __init__(self, values=[], regular_expressions=[], no_colors=False):
         super(EmptyFilter, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
+        self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
         regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
-        regexmatcher.set_all_regex_to_endswith()
+        regexmatcher.set_all_regex_to_startswith()
 
-        if any(['.'.join(path_to_obj).endswith(value) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
+        if any(['.'.join(path_to_obj).startswith(value) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
```

### Comparing `objectwalker-2.1/objectwalker/filters/path/FilterPathStartsWith.py` & `objectwalker-2.1.1/objectwalker/filters/object/name/FilterObjectNameContains.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : FilterPathStartsWith.py
+# File name          : FilterObjectNameContains.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
 from objectwalker.filters.EmptyFilter import EmptyFilter
+from objectwalker.utils import RegExMatcher
 
 
-class FilterPathStartsWith(EmptyFilter):
+class FilterObjectNameContains(EmptyFilter):
     """
-    Documentation for class FilterPathStartsWith
+    class FilterObjectNameContains
+
+    Filters
     """
     values = []
     regular_expressions = []
     no_colors = False
 
-    filter_name = "FilterPathStartsWith"
+    filter_name = "FilterObjectNameContains"
 
-    def __init__(self, values, no_colors=False):
-        super(EmptyFilter, self).__init__()
+    def __init__(self, values=[], regular_expressions=[], no_colors=False):
+        super(FilterObjectNameContains, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
+        self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
         regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
-        regexmatcher.set_all_regex_to_startswith()
+        regexmatcher.set_all_regex_to_contains()
 
-        if any(['.'.join(path_to_obj).startswith(value) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
+        if any([(value in str(path_to_obj[-1])) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
```

### Comparing `objectwalker-2.1/objectwalker/filters/type/FilterTypeIsBuiltinFunctionOrMethod.py` & `objectwalker-2.1.1/objectwalker/filters/type/FilterTypeIsBuiltinFunctionOrMethod.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1/objectwalker/filters/type/FilterTypeIsMethodWrapper.py` & `objectwalker-2.1.1/objectwalker/filters/type/FilterTypeIsMethodWrapper.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1/objectwalker/filters/type/FilterTypeIsModule.py` & `objectwalker-2.1.1/objectwalker/filters/type/FilterTypeIsModule.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1/objectwalker/tests/test_RegExMatcher.py` & `objectwalker-2.1.1/objectwalker/tests/test_RegExMatcher.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1/objectwalker/utils/RegExMatcher.py` & `objectwalker-2.1.1/objectwalker/utils/RegExMatcher.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1/objectwalker.egg-info/PKG-INFO` & `objectwalker-2.1.1/objectwalker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objectwalker
-Version: 2.1
+Version: 2.1.1
 Summary: UNKNOWN
 Home-page: https://github.com/p0dalirius/objectwalker
 Author: Podalirius
 Author-email: podalirius@protonmail.com
 License: GPL2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: objectwalker Version: 2.1 Summary: UNKNOWN Home-
+Metadata-Version: 2.1 Name: objectwalker Version: 2.1.1 Summary: UNKNOWN Home-
 page: https://github.com/p0dalirius/objectwalker Author: Podalirius Author-
 email: podalirius@protonmail.com License: GPL2 Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
   A python module to explore the object tree to extract paths to interesting
                               objects in memory.
```

### Comparing `objectwalker-2.1/objectwalker.egg-info/SOURCES.txt` & `objectwalker-2.1.1/objectwalker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1/setup.py` & `objectwalker-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 """
 
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = [x.strip() for x in f.readlines()]
 
 setuptools.setup(
     name="objectwalker",
-    version="2.1",
+    version="2.1.1",
     description="",
     url="https://github.com/p0dalirius/objectwalker",
     author="Podalirius",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="podalirius@protonmail.com",
     packages=["objectwalker", "objectwalker.filters"],
```


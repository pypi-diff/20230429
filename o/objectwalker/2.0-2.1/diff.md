# Comparing `tmp/objectwalker-2.0.tar.gz` & `tmp/objectwalker-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objectwalker-2.0.tar", last modified: Fri Apr 28 12:10:26 2023, max compression
+gzip compressed data, was "objectwalker-2.1.tar", last modified: Sat Apr 29 18:06:37 2023, max compression
```

## Comparing `objectwalker-2.0.tar` & `objectwalker-2.1.tar`

### file list

```diff
@@ -1,35 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:10:26.030876 objectwalker-2.0/
--rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1782 2023-04-28 12:10:26.030876 objectwalker-2.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1642 2023-04-26 14:54:45.000000 objectwalker-2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:10:26.026876 objectwalker-2.0/objectwalker/
--rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-2.0/objectwalker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7866 2023-04-28 12:02:50.000000 objectwalker-2.0/objectwalker/__main__.py
--rw-rw-r--   0 root         (0) root         (0)    11371 2023-04-27 18:48:15.000000 objectwalker-2.0/objectwalker/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:10:26.030876 objectwalker-2.0/objectwalker/filters/
--rw-rw-r--   0 root         (0) root         (0)     1609 2023-04-28 09:59:50.000000 objectwalker-2.0/objectwalker/filters/EmptyFilter.py
--rw-rw-r--   0 root         (0) root         (0)     1049 2023-04-28 10:21:25.000000 objectwalker-2.0/objectwalker/filters/FilterObjectNameContains.py
--rw-rw-r--   0 root         (0) root         (0)     1061 2023-04-27 10:44:22.000000 objectwalker-2.0/objectwalker/filters/FilterObjectNameEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1044 2023-04-27 10:44:25.000000 objectwalker-2.0/objectwalker/filters/FilterObjectNameEquals.py
--rw-rw-r--   0 root         (0) root         (0)     1742 2023-04-27 11:37:42.000000 objectwalker-2.0/objectwalker/filters/FilterObjectNameIsPythonBuiltin.py
--rw-rw-r--   0 root         (0) root         (0)     1073 2023-04-27 10:44:32.000000 objectwalker-2.0/objectwalker/filters/FilterObjectNameStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1047 2023-04-27 10:44:35.000000 objectwalker-2.0/objectwalker/filters/FilterObjectValueContains.py
--rw-rw-r--   0 root         (0) root         (0)     1054 2023-04-27 10:44:38.000000 objectwalker-2.0/objectwalker/filters/FilterObjectValueEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1037 2023-04-27 10:44:41.000000 objectwalker-2.0/objectwalker/filters/FilterObjectValueEquals.py
--rw-rw-r--   0 root         (0) root         (0)     1066 2023-04-27 10:44:44.000000 objectwalker-2.0/objectwalker/filters/FilterObjectValueStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1016 2023-04-27 10:44:47.000000 objectwalker-2.0/objectwalker/filters/FilterPathContains.py
--rw-rw-r--   0 root         (0) root         (0)     1023 2023-04-27 10:44:05.000000 objectwalker-2.0/objectwalker/filters/FilterPathEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1033 2023-04-27 10:44:53.000000 objectwalker-2.0/objectwalker/filters/FilterPathStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      815 2023-04-27 10:35:32.000000 objectwalker-2.0/objectwalker/filters/FilterTypeIsBuiltinFunctionOrMethod.py
--rw-rw-r--   0 root         (0) root         (0)      762 2023-04-27 10:35:30.000000 objectwalker-2.0/objectwalker/filters/FilterTypeIsMethodWrapper.py
--rw-rw-r--   0 root         (0) root         (0)     2544 2023-04-27 10:45:04.000000 objectwalker-2.0/objectwalker/filters/FilterTypeIsModule.py
--rw-rw-r--   0 root         (0) root         (0)     1267 2023-04-27 10:23:43.000000 objectwalker-2.0/objectwalker/filters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:10:26.030876 objectwalker-2.0/objectwalker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1782 2023-04-28 12:10:26.000000 objectwalker-2.0/objectwalker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1106 2023-04-28 12:10:26.000000 objectwalker-2.0/objectwalker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 12:10:26.000000 objectwalker-2.0/objectwalker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-28 12:10:26.000000 objectwalker-2.0/objectwalker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 12:10:26.000000 objectwalker-2.0/objectwalker.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-2.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 12:10:26.030876 objectwalker-2.0/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     2490 2023-04-28 12:09:48.000000 objectwalker-2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/
+-rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-04-29 18:06:37.569344 objectwalker-2.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1642 2023-04-29 18:06:30.000000 objectwalker-2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/
+-rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-2.1/objectwalker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7866 2023-04-29 18:06:07.000000 objectwalker-2.1/objectwalker/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)    11371 2023-04-27 18:48:15.000000 objectwalker-2.1/objectwalker/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/filters/
+-rw-rw-r--   0 root         (0) root         (0)     1609 2023-04-28 09:59:50.000000 objectwalker-2.1/objectwalker/filters/EmptyFilter.py
+-rw-rw-r--   0 root         (0) root         (0)      349 2023-04-29 07:25:00.000000 objectwalker-2.1/objectwalker/filters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/filters/object/
+-rw-rw-r--   0 root         (0) root         (0)      261 2023-04-29 07:24:44.000000 objectwalker-2.1/objectwalker/filters/object/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/filters/object/name/
+-rw-rw-r--   0 root         (0) root         (0)     1443 2023-04-29 17:58:08.000000 objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1426 2023-04-29 17:58:05.000000 objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1440 2023-04-29 17:58:02.000000 objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameEquals.py
+-rw-rw-r--   0 root         (0) root         (0)     1763 2023-04-29 17:40:51.000000 objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameIsPythonBuiltin.py
+-rw-rw-r--   0 root         (0) root         (0)     1469 2023-04-29 17:57:57.000000 objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      496 2023-04-29 07:23:40.000000 objectwalker-2.1/objectwalker/filters/object/name/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/filters/object/value/
+-rw-rw-r--   0 root         (0) root         (0)     1441 2023-04-29 17:57:54.000000 objectwalker-2.1/objectwalker/filters/object/value/FilterObjectValueContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1448 2023-04-29 17:57:51.000000 objectwalker-2.1/objectwalker/filters/object/value/FilterObjectValueEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1433 2023-04-29 17:57:31.000000 objectwalker-2.1/objectwalker/filters/object/value/FilterObjectValueEquals.py
+-rw-rw-r--   0 root         (0) root         (0)     1462 2023-04-29 17:57:47.000000 objectwalker-2.1/objectwalker/filters/object/value/FilterObjectValueStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      427 2023-04-29 07:23:31.000000 objectwalker-2.1/objectwalker/filters/object/value/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/filters/path/
+-rw-rw-r--   0 root         (0) root         (0)     1287 2023-04-29 17:57:43.000000 objectwalker-2.1/objectwalker/filters/path/FilterPathContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-04-29 17:57:40.000000 objectwalker-2.1/objectwalker/filters/path/FilterPathEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1306 2023-04-29 17:57:35.000000 objectwalker-2.1/objectwalker/filters/path/FilterPathStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      324 2023-04-29 07:23:18.000000 objectwalker-2.1/objectwalker/filters/path/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/filters/type/
+-rw-rw-r--   0 root         (0) root         (0)      835 2023-04-29 07:21:12.000000 objectwalker-2.1/objectwalker/filters/type/FilterTypeIsBuiltinFunctionOrMethod.py
+-rw-rw-r--   0 root         (0) root         (0)      782 2023-04-29 07:21:12.000000 objectwalker-2.1/objectwalker/filters/type/FilterTypeIsMethodWrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     2564 2023-04-29 07:21:12.000000 objectwalker-2.1/objectwalker/filters/type/FilterTypeIsModule.py
+-rw-rw-r--   0 root         (0) root         (0)      368 2023-04-29 07:23:49.000000 objectwalker-2.1/objectwalker/filters/type/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-29 10:08:46.000000 objectwalker-2.1/objectwalker/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2240 2023-04-29 17:54:40.000000 objectwalker-2.1/objectwalker/tests/test_RegExMatcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker/utils/
+-rw-rw-r--   0 root         (0) root         (0)     4578 2023-04-29 17:52:20.000000 objectwalker-2.1/objectwalker/utils/RegExMatcher.py
+-rw-rw-r--   0 root         (0) root         (0)      310 2023-04-29 08:39:22.000000 objectwalker-2.1/objectwalker/utils/Reporter.py
+-rw-rw-r--   0 root         (0) root         (0)      236 2023-04-29 09:12:30.000000 objectwalker-2.1/objectwalker/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:06:37.569344 objectwalker-2.1/objectwalker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-04-29 18:06:37.000000 objectwalker-2.1/objectwalker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1623 2023-04-29 18:06:37.000000 objectwalker-2.1/objectwalker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 18:06:37.000000 objectwalker-2.1/objectwalker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-29 18:06:37.000000 objectwalker-2.1/objectwalker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-29 18:06:37.000000 objectwalker-2.1/objectwalker.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-2.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 18:06:37.569344 objectwalker-2.1/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     2536 2023-04-29 18:05:57.000000 objectwalker-2.1/setup.py
```

### Comparing `objectwalker-2.0/PKG-INFO` & `objectwalker-2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objectwalker
-Version: 2.0
+Version: 2.1
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
-Metadata-Version: 2.1 Name: objectwalker Version: 2.0 Summary: UNKNOWN Home-
+Metadata-Version: 2.1 Name: objectwalker Version: 2.1 Summary: UNKNOWN Home-
 page: https://github.com/p0dalirius/objectwalker Author: Podalirius Author-
 email: podalirius@protonmail.com License: GPL2 Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
   A python module to explore the object tree to extract paths to interesting
                               objects in memory.
```

### Comparing `objectwalker-2.0/README.md` & `objectwalker-2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  - [x] Python module to use in pdb after a `breakpoint()`.
  - [x] Standalone tool to explore paths in python modules.
  - [x] Multiple built-in filters.
  - [x] Possibility to implement custom filters and pass them to ObjectWalker().
 
 ## Demonstration
 
-https://user-images.githubusercontent.com/79218792/234614877-19b5e5b8-a52b-4f4d-a4aa-4cda0b7ddf96.mp4
+https://user-images.githubusercontent.com/79218792/235144127-189d536c-b51c-495c-bcab-f803d806e90b.mp4
 
 ## Installation
 
 You can now install it from pypi (latest version is <img alt="PyPI" src="https://img.shields.io/pypi/v/objectwalker">) with this command:
 
 ```
 sudo python3 -m pip install objectwalker
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
                               objects in memory.
    [GitHub release (latest by date)] [https://img.shields.io/twitter/follow/
    podalirius_?label=Podalirius&style=social] [YouTube_Channel_Subscribers]
 ## Features - [x] Python module to use in pdb after a `breakpoint()`. - [x]
 Standalone tool to explore paths in python modules. - [x] Multiple built-in
 filters. - [x] Possibility to implement custom filters and pass them to
 ObjectWalker(). ## Demonstration https://user-images.githubusercontent.com/
-79218792/234614877-19b5e5b8-a52b-4f4d-a4aa-4cda0b7ddf96.mp4 ## Installation You
+79218792/235144127-189d536c-b51c-495c-bcab-f803d806e90b.mp4 ## Installation You
 can now install it from pypi (latest version is [PyPI]) with this command: ```
 sudo python3 -m pip install objectwalker ``` ## Example commands + We want to
 find all the paths to the `os` module in the module `jinja2`: ``` objectwalker
 -m jinja2 --filter-object-is-module os --max-depth 15 ``` We get the following
 output: ![](./.github/find_module_os_in_jinja2.png) ## Contributing Pull
 requests are welcome. Feel free to open an issue if you want to add other
 features.
```

### Comparing `objectwalker-2.0/objectwalker/__main__.py` & `objectwalker-2.1/objectwalker/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import argparse
 import sys
 import objectwalker
 from objectwalker.filters import *
 
 
-VERSION = "2.0"
+VERSION = "2.1"
 
 
 banner = r"""
        ____  __      _           __ _       __      ____            
       / __ \/ /_    (_)__  _____/ /| |     / /___ _/ / /_____  _____
      / / / / __ \  / / _ \/ ___/ __/ | /| / / __ `/ / //_/ _ \/ ___/
     / /_/ / /_/ / / /  __/ /__/ /_ | |/ |/ / /_/ / / ,< /  __/ /      v%s
```

### Comparing `objectwalker-2.0/objectwalker/core.py` & `objectwalker-2.1/objectwalker/core.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.0/objectwalker/filters/EmptyFilter.py` & `objectwalker-2.1/objectwalker/filters/EmptyFilter.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.0/objectwalker/filters/FilterObjectNameEndsWith.py` & `objectwalker-2.1/objectwalker/filters/type/FilterTypeIsBuiltinFunctionOrMethod.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : FilterObjectNameEndsWith.py
+# File name          : FilterTypeIsBuiltinFunctionOrMethod.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
-from .EmptyFilter import EmptyFilter
+from objectwalker.filters.EmptyFilter import EmptyFilter
 
 
-class FilterObjectNameEndsWith(EmptyFilter):
+class FilterTypeIsBuiltinFunctionOrMethod(EmptyFilter):
     """
-    Documentation for class FilterObjectNameEndsWith
+    Documentation for class FilterTypeIsBuiltinFunctionOrMethod
     """
-    values = []
-    no_colors = False
 
-    filter_name = "FilterObjectNameEndsWith"
-
-    def __init__(self, values, no_colors=False):
-        super(FilterObjectNameEndsWith, self).__init__()
-        self.callback = self.print_result
-        self.no_colors = no_colors
-        self.values = values
+    filter_name = "FilterTypeIsBuiltinFunctionOrMethod"
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
-        if any([(str(path_to_obj[-1]).endswith(value)) for value in self.values]):
+        if str(type(obj)) == "<class 'builtin_function_or_method'>":
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
 
     def __repr__(self):
-        return "<%s values=%s>" % (self.filter_name, self.values)
+        return "<%s>" % self.filter_name
```

### Comparing `objectwalker-2.0/objectwalker/filters/FilterObjectNameEquals.py` & `objectwalker-2.1/objectwalker/filters/path/FilterPathContains.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : FilterObjectNameEquals.py
+# File name          : FilterPathContains.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
-from .EmptyFilter import EmptyFilter
+from objectwalker.filters.EmptyFilter import EmptyFilter
 
 
-class FilterObjectNameEquals(EmptyFilter):
+class FilterPathContains(EmptyFilter):
     """
-    Documentation for class FilterObjectNameEquals
+    Documentation for class FilterPathContains
     """
     values = []
+    regular_expressions = []
     no_colors = False
 
-    filter_name = "FilterObjectNameEquals"
+    filter_name = "FilterPathContains"
 
     def __init__(self, values, no_colors=False):
-        super(FilterObjectNameEquals, self).__init__()
+        super(EmptyFilter, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
-        if any([(str(path_to_obj[-1]) == value) for value in self.values]):
+        regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
+        regexmatcher.set_all_regex_to_contains()
+
+        if any([value in '.'.join(path_to_obj) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
 
     def __repr__(self):
-        return "<%s values=%s>" % (self.filter_name, self.values)
+        return "<%s values=%s regular_expressions=%s>" % (self.filter_name, self.values, self.regular_expressions)
```

### Comparing `objectwalker-2.0/objectwalker/filters/FilterObjectNameIsPythonBuiltin.py` & `objectwalker-2.1/objectwalker/filters/object/name/FilterObjectNameIsPythonBuiltin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # File name          : FilterObjectNameIsPythonBuiltin.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
-from .EmptyFilter import EmptyFilter
+from objectwalker.filters.EmptyFilter import EmptyFilter
+
 
 class DummyEmptyClass(object):
     pass
 
 def DummyEmptyFunction():
     pass
```

### Comparing `objectwalker-2.0/objectwalker/filters/FilterObjectNameStartsWith.py` & `objectwalker-2.1/objectwalker/filters/type/FilterTypeIsMethodWrapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : FilterObjectNameStartsWith.py
+# File name          : FilterTypeIsMethodWrapper.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
-from .EmptyFilter import EmptyFilter
+from objectwalker.filters.EmptyFilter import EmptyFilter
 
-
-class FilterObjectNameStartsWith(EmptyFilter):
+class FilterTypeIsMethodWrapper(EmptyFilter):
     """
-    Documentation for class FilterObjectNameStartsWith
+    Documentation for class FilterTypeIsMethodWrapper
     """
-    values = []
-    no_colors = False
-
-    filter_name = "FilterObjectNameStartsWith"
 
-    def __init__(self, values, no_colors=False):
-        super(FilterObjectNameStartsWith, self).__init__()
-        self.callback = self.print_result
-        self.no_colors = no_colors
-        self.values = values
+    filter_name = "FilterTypeIsMethodWrapper"
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
-        if any([(str(path_to_obj[-1]).startswith(value)) for value in self.values]):
+        if str(type(obj)) == "<class 'method-wrapper'>":
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
 
     def __repr__(self):
-        return "<%s values=%s>" % (self.filter_name, self.values)
+        return "<%s>" % self.filter_name
```

### Comparing `objectwalker-2.0/objectwalker/filters/FilterObjectValueContains.py` & `objectwalker-2.1/objectwalker/filters/object/value/FilterObjectValueContains.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # File name          : FilterObjectValueContains.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
-from .EmptyFilter import EmptyFilter
+from objectwalker.filters.EmptyFilter import EmptyFilter
+from objectwalker.utils import RegExMatcher
 
 
 class FilterObjectValueContains(EmptyFilter):
     """
     Documentation for class FilterObjectValueContains
     """
     values = []
+    regular_expressions = []
     no_colors = False
 
     filter_name = "FilterObjectValueContains"
 
-    def __init__(self, values, no_colors=False):
+    def __init__(self, values, regular_expressions=[], no_colors=False):
         super(FilterObjectValueContains, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
+        self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
-        if any([(value in str(obj)) for value in self.values]):
+        regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
+        regexmatcher.set_all_regex_to_contains()
+
+        if any([(value in str(obj)) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
 
     def __repr__(self):
-        return "<%s values=%s>" % (self.filter_name, self.values)
+        return "<%s values=%s regular_expressions=%s>" % (self.filter_name, self.values, self.regular_expressions)
```

### Comparing `objectwalker-2.0/objectwalker/filters/FilterPathContains.py` & `objectwalker-2.1/objectwalker/filters/object/value/FilterObjectValueEquals.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : FilterPathContains.py
+# File name          : FilterObjectValueEquals.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
-from .EmptyFilter import EmptyFilter
+from objectwalker.filters.EmptyFilter import EmptyFilter
+from objectwalker.utils import RegExMatcher
 
 
-class FilterPathContains(EmptyFilter):
+class FilterObjectValueEquals(EmptyFilter):
     """
-    Documentation for class FilterPathContains
+    Documentation for class FilterObjectValueEquals
     """
     values = []
+    regular_expressions = []
     no_colors = False
 
-    filter_name = "FilterPathContains"
+    filter_name = "FilterObjectValueEquals"
 
-    def __init__(self, values, no_colors=False):
-        super(EmptyFilter, self).__init__()
+    def __init__(self, values, regular_expressions=[], no_colors=False):
+        super(FilterObjectValueEquals, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
+        self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
-        if any([value in '.'.join(path_to_obj) for value in self.values]):
+        regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
+        regexmatcher.set_all_regex_to_exactmatch()
+
+        if any([(str(obj) == value) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
 
     def __repr__(self):
-        return "<%s values=%s>" % (self.filter_name, self.values)
+        return "<%s values=%s regular_expressions=%s>" % (self.filter_name, self.values, self.regular_expressions)
```

### Comparing `objectwalker-2.0/objectwalker/filters/FilterTypeIsModule.py` & `objectwalker-2.1/objectwalker/filters/type/FilterTypeIsModule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # File name          : FilterTypeIsModule.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
 import re
-from .EmptyFilter import EmptyFilter
+from objectwalker.filters.EmptyFilter import EmptyFilter
 
 
 class FilterTypeIsModule(EmptyFilter):
     """
     Documentation for class FilterTypeIsModule
     """
```

### Comparing `objectwalker-2.0/objectwalker.egg-info/PKG-INFO` & `objectwalker-2.1/objectwalker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objectwalker
-Version: 2.0
+Version: 2.1
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
-Metadata-Version: 2.1 Name: objectwalker Version: 2.0 Summary: UNKNOWN Home-
+Metadata-Version: 2.1 Name: objectwalker Version: 2.1 Summary: UNKNOWN Home-
 page: https://github.com/p0dalirius/objectwalker Author: Podalirius Author-
 email: podalirius@protonmail.com License: GPL2 Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
   A python module to explore the object tree to extract paths to interesting
                               objects in memory.
```

### Comparing `objectwalker-2.0/setup.py` & `objectwalker-2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,23 +44,23 @@
 """
 
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = [x.strip() for x in f.readlines()]
 
 setuptools.setup(
     name="objectwalker",
-    version="2.0",
+    version="2.1",
     description="",
     url="https://github.com/p0dalirius/objectwalker",
     author="Podalirius",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="podalirius@protonmail.com",
     packages=["objectwalker", "objectwalker.filters"],
-    package_data={'objectwalker': ['objectwalker/', 'objectwalker/filters/']},
+    package_data={'objectwalker': ['objectwalker/', 'objectwalker/filters/', 'objectwalker/utils/', 'objectwalker/tests/']},
     include_package_data=True,
     license="GPL2",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Operating System :: OS Independent",
     ],
```


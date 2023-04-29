# Comparing `tmp/objectwalker-2.1.2.tar.gz` & `tmp/objectwalker-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objectwalker-2.1.2.tar", last modified: Sat Apr 29 18:20:37 2023, max compression
+gzip compressed data, was "objectwalker-2.1.3.tar", last modified: Sat Apr 29 18:47:14 2023, max compression
```

## Comparing `objectwalker-2.1.2.tar` & `objectwalker-2.1.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:20:37.156898 objectwalker-2.1.2/
--rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-2.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1784 2023-04-29 18:20:37.156898 objectwalker-2.1.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1642 2023-04-29 18:06:30.000000 objectwalker-2.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:20:37.156898 objectwalker-2.1.2/objectwalker/
--rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-2.1.2/objectwalker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7868 2023-04-29 18:20:02.000000 objectwalker-2.1.2/objectwalker/__main__.py
--rw-rw-r--   0 root         (0) root         (0)    11371 2023-04-27 18:48:15.000000 objectwalker-2.1.2/objectwalker/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:20:37.156898 objectwalker-2.1.2/objectwalker/filters/
--rw-rw-r--   0 root         (0) root         (0)     1609 2023-04-28 09:59:50.000000 objectwalker-2.1.2/objectwalker/filters/EmptyFilter.py
--rw-rw-r--   0 root         (0) root         (0)      349 2023-04-29 07:25:00.000000 objectwalker-2.1.2/objectwalker/filters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:20:37.156898 objectwalker-2.1.2/objectwalker/filters/object/
--rw-rw-r--   0 root         (0) root         (0)      261 2023-04-29 07:24:44.000000 objectwalker-2.1.2/objectwalker/filters/object/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:20:37.156898 objectwalker-2.1.2/objectwalker/filters/object/name/
--rw-rw-r--   0 root         (0) root         (0)     1446 2023-04-29 18:11:54.000000 objectwalker-2.1.2/objectwalker/filters/object/name/FilterObjectNameContains.py
--rw-rw-r--   0 root         (0) root         (0)     1429 2023-04-29 18:11:50.000000 objectwalker-2.1.2/objectwalker/filters/object/name/FilterObjectNameEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1443 2023-04-29 18:11:50.000000 objectwalker-2.1.2/objectwalker/filters/object/name/FilterObjectNameEquals.py
--rw-rw-r--   0 root         (0) root         (0)     1763 2023-04-29 17:40:51.000000 objectwalker-2.1.2/objectwalker/filters/object/name/FilterObjectNameIsPythonBuiltin.py
--rw-rw-r--   0 root         (0) root         (0)     1472 2023-04-29 18:11:50.000000 objectwalker-2.1.2/objectwalker/filters/object/name/FilterObjectNameStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      496 2023-04-29 07:23:40.000000 objectwalker-2.1.2/objectwalker/filters/object/name/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:20:37.156898 objectwalker-2.1.2/objectwalker/filters/object/value/
--rw-rw-r--   0 root         (0) root         (0)     1444 2023-04-29 18:11:32.000000 objectwalker-2.1.2/objectwalker/filters/object/value/FilterObjectValueContains.py
--rw-rw-r--   0 root         (0) root         (0)     1451 2023-04-29 18:11:57.000000 objectwalker-2.1.2/objectwalker/filters/object/value/FilterObjectValueEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1436 2023-04-29 18:12:00.000000 objectwalker-2.1.2/objectwalker/filters/object/value/FilterObjectValueEquals.py
--rw-rw-r--   0 root         (0) root         (0)     1465 2023-04-29 18:12:03.000000 objectwalker-2.1.2/objectwalker/filters/object/value/FilterObjectValueStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      427 2023-04-29 07:23:31.000000 objectwalker-2.1.2/objectwalker/filters/object/value/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:20:37.156898 objectwalker-2.1.2/objectwalker/filters/path/
--rw-rw-r--   0 root         (0) root         (0)     1369 2023-04-29 18:12:57.000000 objectwalker-2.1.2/objectwalker/filters/path/FilterPathContains.py
--rw-rw-r--   0 root         (0) root         (0)     1376 2023-04-29 18:12:53.000000 objectwalker-2.1.2/objectwalker/filters/path/FilterPathEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1388 2023-04-29 18:12:43.000000 objectwalker-2.1.2/objectwalker/filters/path/FilterPathStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      324 2023-04-29 07:23:18.000000 objectwalker-2.1.2/objectwalker/filters/path/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:20:37.156898 objectwalker-2.1.2/objectwalker/filters/type/
--rw-rw-r--   0 root         (0) root         (0)      835 2023-04-29 07:21:12.000000 objectwalker-2.1.2/objectwalker/filters/type/FilterTypeIsBuiltinFunctionOrMethod.py
--rw-rw-r--   0 root         (0) root         (0)      782 2023-04-29 07:21:12.000000 objectwalker-2.1.2/objectwalker/filters/type/FilterTypeIsMethodWrapper.py
--rw-rw-r--   0 root         (0) root         (0)     2564 2023-04-29 07:21:12.000000 objectwalker-2.1.2/objectwalker/filters/type/FilterTypeIsModule.py
--rw-rw-r--   0 root         (0) root         (0)      368 2023-04-29 07:23:49.000000 objectwalker-2.1.2/objectwalker/filters/type/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:20:37.156898 objectwalker-2.1.2/objectwalker/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-29 10:08:46.000000 objectwalker-2.1.2/objectwalker/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2240 2023-04-29 17:54:40.000000 objectwalker-2.1.2/objectwalker/tests/test_RegExMatcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:20:37.156898 objectwalker-2.1.2/objectwalker/utils/
--rw-rw-r--   0 root         (0) root         (0)     4651 2023-04-29 18:19:05.000000 objectwalker-2.1.2/objectwalker/utils/RegExMatcher.py
--rw-rw-r--   0 root         (0) root         (0)      310 2023-04-29 08:39:22.000000 objectwalker-2.1.2/objectwalker/utils/Reporter.py
--rw-rw-r--   0 root         (0) root         (0)      236 2023-04-29 09:12:30.000000 objectwalker-2.1.2/objectwalker/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:20:37.156898 objectwalker-2.1.2/objectwalker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1784 2023-04-29 18:20:37.000000 objectwalker-2.1.2/objectwalker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1623 2023-04-29 18:20:37.000000 objectwalker-2.1.2/objectwalker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 18:20:37.000000 objectwalker-2.1.2/objectwalker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-29 18:20:37.000000 objectwalker-2.1.2/objectwalker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-29 18:20:37.000000 objectwalker-2.1.2/objectwalker.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-2.1.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 18:20:37.156898 objectwalker-2.1.2/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     2538 2023-04-29 18:20:14.000000 objectwalker-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/
+-rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-2.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-04-29 18:47:14.470241 objectwalker-2.1.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1642 2023-04-29 18:06:30.000000 objectwalker-2.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.466241 objectwalker-2.1.3/objectwalker/
+-rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-2.1.3/objectwalker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7868 2023-04-29 18:46:55.000000 objectwalker-2.1.3/objectwalker/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)    13288 2023-04-29 18:35:53.000000 objectwalker-2.1.3/objectwalker/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/filters/
+-rw-rw-r--   0 root         (0) root         (0)     1609 2023-04-28 09:59:50.000000 objectwalker-2.1.3/objectwalker/filters/EmptyFilter.py
+-rw-rw-r--   0 root         (0) root         (0)      349 2023-04-29 07:25:00.000000 objectwalker-2.1.3/objectwalker/filters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/filters/object/
+-rw-rw-r--   0 root         (0) root         (0)      261 2023-04-29 07:24:44.000000 objectwalker-2.1.3/objectwalker/filters/object/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/filters/object/name/
+-rw-rw-r--   0 root         (0) root         (0)     1446 2023-04-29 18:11:54.000000 objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1429 2023-04-29 18:11:50.000000 objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1443 2023-04-29 18:11:50.000000 objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameEquals.py
+-rw-rw-r--   0 root         (0) root         (0)     1763 2023-04-29 17:40:51.000000 objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameIsPythonBuiltin.py
+-rw-rw-r--   0 root         (0) root         (0)     1472 2023-04-29 18:11:50.000000 objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      496 2023-04-29 07:23:40.000000 objectwalker-2.1.3/objectwalker/filters/object/name/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/filters/object/value/
+-rw-rw-r--   0 root         (0) root         (0)     1437 2023-04-29 18:22:54.000000 objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1444 2023-04-29 18:22:54.000000 objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1429 2023-04-29 18:22:54.000000 objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueEquals.py
+-rw-rw-r--   0 root         (0) root         (0)     1458 2023-04-29 18:22:54.000000 objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      427 2023-04-29 07:23:31.000000 objectwalker-2.1.3/objectwalker/filters/object/value/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/filters/path/
+-rw-rw-r--   0 root         (0) root         (0)     1419 2023-04-29 18:23:37.000000 objectwalker-2.1.3/objectwalker/filters/path/FilterPathContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1426 2023-04-29 18:23:37.000000 objectwalker-2.1.3/objectwalker/filters/path/FilterPathEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1438 2023-04-29 18:23:37.000000 objectwalker-2.1.3/objectwalker/filters/path/FilterPathStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      324 2023-04-29 07:23:18.000000 objectwalker-2.1.3/objectwalker/filters/path/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/filters/type/
+-rw-rw-r--   0 root         (0) root         (0)      835 2023-04-29 07:21:12.000000 objectwalker-2.1.3/objectwalker/filters/type/FilterTypeIsBuiltinFunctionOrMethod.py
+-rw-rw-r--   0 root         (0) root         (0)      782 2023-04-29 07:21:12.000000 objectwalker-2.1.3/objectwalker/filters/type/FilterTypeIsMethodWrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     2564 2023-04-29 07:21:12.000000 objectwalker-2.1.3/objectwalker/filters/type/FilterTypeIsModule.py
+-rw-rw-r--   0 root         (0) root         (0)      368 2023-04-29 07:23:49.000000 objectwalker-2.1.3/objectwalker/filters/type/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-29 10:08:46.000000 objectwalker-2.1.3/objectwalker/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2240 2023-04-29 17:54:40.000000 objectwalker-2.1.3/objectwalker/tests/test_RegExMatcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/utils/
+-rw-rw-r--   0 root         (0) root         (0)     4651 2023-04-29 18:19:05.000000 objectwalker-2.1.3/objectwalker/utils/RegExMatcher.py
+-rw-rw-r--   0 root         (0) root         (0)      310 2023-04-29 08:39:22.000000 objectwalker-2.1.3/objectwalker/utils/Reporter.py
+-rw-rw-r--   0 root         (0) root         (0)      236 2023-04-29 09:12:30.000000 objectwalker-2.1.3/objectwalker/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.466241 objectwalker-2.1.3/objectwalker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-04-29 18:47:14.000000 objectwalker-2.1.3/objectwalker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1623 2023-04-29 18:47:14.000000 objectwalker-2.1.3/objectwalker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 18:47:14.000000 objectwalker-2.1.3/objectwalker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-29 18:47:14.000000 objectwalker-2.1.3/objectwalker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-29 18:47:14.000000 objectwalker-2.1.3/objectwalker.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-2.1.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 18:47:14.470241 objectwalker-2.1.3/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     2538 2023-04-29 18:46:55.000000 objectwalker-2.1.3/setup.py
```

### Comparing `objectwalker-2.1.2/PKG-INFO` & `objectwalker-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objectwalker
-Version: 2.1.2
+Version: 2.1.3
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
-Metadata-Version: 2.1 Name: objectwalker Version: 2.1.2 Summary: UNKNOWN Home-
+Metadata-Version: 2.1 Name: objectwalker Version: 2.1.3 Summary: UNKNOWN Home-
 page: https://github.com/p0dalirius/objectwalker Author: Podalirius Author-
 email: podalirius@protonmail.com License: GPL2 Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
   A python module to explore the object tree to extract paths to interesting
                               objects in memory.
```

### Comparing `objectwalker-2.1.2/README.md` & `objectwalker-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.2/objectwalker/__main__.py` & `objectwalker-2.1.3/objectwalker/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import argparse
 import sys
 import objectwalker
 from objectwalker.filters import *
 
 
-VERSION = "2.1.2"
+VERSION = "2.1.3"
 
 
 banner = r"""
        ____  __      _           __ _       __      ____            
       / __ \/ /_    (_)__  _____/ /| |     / /___ _/ / /_____  _____
      / / / / __ \  / / _ \/ ___/ __/ | /| / / __ `/ / //_/ _ \/ ___/
     / /_/ / /_/ / / /  __/ /__/ /_ | |/ |/ / /_/ / / ,< /  __/ /      v%s
```

### Comparing `objectwalker-2.1.2/objectwalker/core.py` & `objectwalker-2.1.3/objectwalker/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,19 +8,27 @@
 
 
 class ObjectWalker(object):
     """
     Documentation for class ObjectWalker
     """
 
-    def __init__(self, filters_accept=[], filters_reject=[], filters_skip_exploration=[], callback=None, verbose=False, no_colors=False):
+    def __init__(self, filters_accept=[], filters_reject=[], filters_skip_exploration=[], matchmode_accept="any", matchmode_reject="any", matchmode_skip_exploration="any", callback=None, verbose=False, no_colors=False):
         super(ObjectWalker, self).__init__()
         self.verbose = verbose
         self.no_colors = no_colors
 
+        # Matchmode
+        self.filter_matchmode_accept = any
+        self.set_filter_matchmode_accept(matchmode_accept)
+        self.filter_matchmode_reject = any
+        self.set_filter_matchmode_reject(matchmode_reject)
+        self.filter_matchmode_skip_exploration = any
+        self.set_filter_matchmode_skip_exploration(matchmode_skip_exploration)
+
         # Filters
         self.filters_accept = filters_accept
         self.filters_reject = filters_reject
         self.filters_skip_exploration = filters_skip_exploration
         if len(self.filters_accept) == 0 and len(self.filters_reject) == 0:
             self.filters_accept = [EmptyFilter()]
 
@@ -88,21 +96,21 @@
                                 subobj = eval('obj["%s"]' % subkey, {"obj": obj})
                             else:
                                 path_to_obj[-1] += '["%s"]' % subkey
                                 subobj = eval('obj["%s"]' % subkey, {"obj": obj})
                         except (SyntaxError, ValueError, KeyError, TypeError) as e:
                             continue
 
-                        if any([f.check(subobj, path_to_obj) for f in self.filters_accept]) and not any([f.check(subobj, path_to_obj) for f in self.filters_reject]):
+                        if self.filter_matchmode_accept([f.check(subobj, path_to_obj) for f in self.filters_accept]) and not self.filter_matchmode_reject([f.check(subobj, path_to_obj) for f in self.filters_reject]):
                             # Save the found path
                             found.append(path_to_obj)
                             input()
 
                         # Explore further
-                        if not any([f.check(subobj, path_to_obj) for f in self.filters_skip_exploration]):
+                        if not self.filter_matchmode_skip_exploration([f.check(subobj, path_to_obj) for f in self.filters_skip_exploration]):
                             if int(id(subobj)) not in self.knownids and False:
                                 self.knownids.append(int(id(subobj)))
                                 found = self.walk_depth_first(obj=subobj, found=found, path=path_to_obj, depth=(depth+1), maxdepth=maxdepth, verbose=verbose)
 
                     except AttributeError as e:
                         pass
 
@@ -141,24 +149,26 @@
                     try:
                         try:
                             path_to_obj = path + [subkey]
                             subobj = eval("obj.%s" % subkey, {"obj": obj})
                         except (SyntaxError, ValueError, KeyError, TypeError) as e:
                             continue
 
-                        if any([f.check(subobj, path_to_obj) for f in self.filters_accept]) and not any([f.check(subobj, path_to_obj) for f in self.filters_reject]):
-                            # Save the found path
-                            found.append(path_to_obj)
-                            input()
+                        # Save the found path if it matches filters (accept, and not reject)
+                        if not self.filter_matchmode_accept([f.check(subobj, path_to_obj) for f in self.filters_reject]):
+                            if self.filter_matchmode_reject([f.check(subobj, path_to_obj) for f in self.filters_accept]):
+                                found.append(path_to_obj)
+                        else:
+                            # Save id of explored object
+                            if int(id(subobj)) not in self.knownids:
+                                self.knownids.append(int(id(subobj)))
 
                         # Explore further
                         if not any([f.check(subobj, path_to_obj) for f in self.filters_skip_exploration]):
-                            if int(id(subobj)) not in self.knownids and False:
-                                self.knownids.append(int(id(subobj)))
-                                found = self.walk_depth_first(obj=subobj, found=found, path=path_to_obj, depth=(depth+1), maxdepth=maxdepth, verbose=verbose)
+                            found = self.walk_depth_first(obj=subobj, found=found, path=path_to_obj, depth=(depth+1), maxdepth=maxdepth, verbose=verbose)
 
                     except AttributeError as e:
                         pass
         return found
 
     def walk_breadth_first(self, obj, found=[], path=[], depth=0, maxdepth=3, verbose=False):
         to_explore = []
@@ -204,24 +214,24 @@
                         elif type(obj) == list:
                             path_to_obj.append("[%d]" % subkey)
                         # All other types
                         else:
                             path_to_obj.append(subkey)
 
                         # Save the found path if it matches filters (accept, and not reject)
-                        if not any([f.check(subobj, path_to_obj) for f in self.filters_reject]):
-                            if any([f.check(subobj, path_to_obj) for f in self.filters_accept]):
+                        if not self.filter_matchmode_accept([f.check(subobj, path_to_obj) for f in self.filters_reject]):
+                            if self.filter_matchmode_reject([f.check(subobj, path_to_obj) for f in self.filters_accept]):
                                 found.append(path_to_obj)
                         else:
                             # Save id of explored object
                             if int(id(subobj)) not in self.knownids:
                                 self.knownids.append(int(id(subobj)))
 
                         # Explore further if filters allow it
-                        if not any([f.check(subobj, path_to_obj) for f in self.filters_skip_exploration]):
+                        if not self.filter_matchmode_skip_exploration([f.check(subobj, path_to_obj) for f in self.filters_skip_exploration]):
                             to_explore.append((subobj, path_to_obj, depth))
 
                 except AttributeError as e:
                     pass
 
         if depth == 0:
             # Explore one more in depth, but only in top level function
@@ -249,7 +259,41 @@
     def get_callback(self):
         return self.callback
     
     def set_callback(self, fcallback):
         self.callback = fcallback
         for f in self.filters_accept:
             f.set_callback(fcallback)
+
+
+    def get_filter_matchmode_accept(self):
+        return self.filter_matchmode_accept
+
+    def set_filter_matchmode_accept(self, matchmode):
+        if matchmode == "any":
+            self.filter_matchmode_accept = any
+        elif matchmode == "all":
+            self.filter_matchmode_accept = all
+        else:
+            self.filter_matchmode_accept = any
+
+    def get_filter_matchmode_reject(self):
+        return self.filter_matchmode_reject
+
+    def set_filter_matchmode_reject(self, matchmode):
+        if matchmode == "any":
+            self.filter_matchmode_reject = any
+        elif matchmode == "all":
+            self.filter_matchmode_reject = all
+        else:
+            self.filter_matchmode_reject = any
+
+    def get_filter_matchmode_skip_exploration(self):
+        return self.filter_matchmode_skip_exploration
+
+    def set_filter_matchmode_skip_exploration(self, matchmode):
+        if matchmode == "any":
+            self.filter_matchmode_skip_exploration = any
+        elif matchmode == "all":
+            self.filter_matchmode_skip_exploration = all
+        else:
+            self.filter_matchmode_skip_exploration = any
```

### Comparing `objectwalker-2.1.2/objectwalker/filters/EmptyFilter.py` & `objectwalker-2.1.3/objectwalker/filters/EmptyFilter.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.2/objectwalker/filters/object/name/FilterObjectNameContains.py` & `objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameContains.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.2/objectwalker/filters/object/name/FilterObjectNameEndsWith.py` & `objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameEndsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.2/objectwalker/filters/object/name/FilterObjectNameEquals.py` & `objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameEquals.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.2/objectwalker/filters/object/name/FilterObjectNameIsPythonBuiltin.py` & `objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameIsPythonBuiltin.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.2/objectwalker/filters/object/name/FilterObjectNameStartsWith.py` & `objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameStartsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.2/objectwalker/filters/object/value/FilterObjectValueContains.py` & `objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueContains.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
         regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
         regexmatcher.set_all_regex_to_contains()
 
-        if any([(value in str(obj)) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
+        if any([(value in str(obj)) for value in self.values]) or (regexmatcher.match(str(obj))):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
```

### Comparing `objectwalker-2.1.2/objectwalker/filters/object/value/FilterObjectValueEndsWith.py` & `objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueEndsWith.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
         regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
         regexmatcher.set_all_regex_to_endswith()
 
-        if any([(str(obj).endswith(value)) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
+        if any([(str(obj).endswith(value)) for value in self.values]) or (regexmatcher.match(str(obj))):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
```

### Comparing `objectwalker-2.1.2/objectwalker/filters/object/value/FilterObjectValueEquals.py` & `objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueEquals.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
         regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
         regexmatcher.set_all_regex_to_exactmatch()
 
-        if any([(str(obj) == value) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
+        if any([(str(obj) == value) for value in self.values]) or (regexmatcher.match(str(obj))):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
```

### Comparing `objectwalker-2.1.2/objectwalker/filters/object/value/FilterObjectValueStartsWith.py` & `objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueStartsWith.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
         regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
         regexmatcher.set_all_regex_to_startswith()
 
-        if any([(str(obj).startswith(value)) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
+        if any([(str(obj).startswith(value)) for value in self.values]) or (regexmatcher.match(str(obj))):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
```

### Comparing `objectwalker-2.1.2/objectwalker/filters/path/FilterPathContains.py` & `objectwalker-2.1.3/objectwalker/filters/path/FilterPathEndsWith.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : FilterPathContains.py
+# File name          : FilterPathEndsWith.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
 from objectwalker.filters.EmptyFilter import EmptyFilter
+from objectwalker.utils import RegExMatcher
 
 
-class FilterPathContains(EmptyFilter):
+class FilterPathEndsWith(EmptyFilter):
     """
-    Documentation for class FilterPathContains
+    Documentation for class FilterPathEndsWith
     """
     values = []
     regular_expressions = []
     no_colors = False
 
-    filter_name = "FilterPathContains"
+    filter_name = "FilterPathEndsWith"
 
     def __init__(self, values=[], regular_expressions=[], no_colors=False):
         super(EmptyFilter, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
         self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
         regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
-        regexmatcher.set_all_regex_to_contains()
+        regexmatcher.set_all_regex_to_endswith()
 
-        if any([value in '.'.join(path_to_obj) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
+        if any(['.'.join(path_to_obj).endswith(value) for value in self.values]) or (regexmatcher.match('.'.join(path_to_obj))):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
```

### Comparing `objectwalker-2.1.2/objectwalker/filters/path/FilterPathEndsWith.py` & `objectwalker-2.1.3/objectwalker/filters/path/FilterPathStartsWith.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : FilterPathEndsWith.py
+# File name          : FilterPathStartsWith.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
 from objectwalker.filters.EmptyFilter import EmptyFilter
+from objectwalker.utils import RegExMatcher
 
 
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
 
     def __init__(self, values=[], regular_expressions=[], no_colors=False):
         super(EmptyFilter, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
         self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
         regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
-        regexmatcher.set_all_regex_to_endswith()
+        regexmatcher.set_all_regex_to_startswith()
 
-        if any(['.'.join(path_to_obj).endswith(value) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
+        if any(['.'.join(path_to_obj).startswith(value) for value in self.values]) or (regexmatcher.match('.'.join(path_to_obj))):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
```

### Comparing `objectwalker-2.1.2/objectwalker/filters/path/FilterPathStartsWith.py` & `objectwalker-2.1.3/objectwalker/filters/path/FilterPathContains.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : FilterPathStartsWith.py
+# File name          : FilterPathContains.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
 from objectwalker.filters.EmptyFilter import EmptyFilter
+from objectwalker.utils import RegExMatcher
 
 
-class FilterPathStartsWith(EmptyFilter):
+class FilterPathContains(EmptyFilter):
     """
-    Documentation for class FilterPathStartsWith
+    Documentation for class FilterPathContains
     """
     values = []
     regular_expressions = []
     no_colors = False
 
-    filter_name = "FilterPathStartsWith"
+    filter_name = "FilterPathContains"
 
     def __init__(self, values=[], regular_expressions=[], no_colors=False):
         super(EmptyFilter, self).__init__()
         self.callback = self.print_result
         self.no_colors = no_colors
         self.values = values
         self.regular_expressions = regular_expressions
 
     def check(self, obj, path_to_obj):
         matches_filter = False
 
         regexmatcher = RegExMatcher(regular_expressions=self.regular_expressions)
-        regexmatcher.set_all_regex_to_startswith()
+        regexmatcher.set_all_regex_to_contains()
 
-        if any(['.'.join(path_to_obj).startswith(value) for value in self.values]) or (regexmatcher.match(path_to_obj[-1])):
+        if any([value in '.'.join(path_to_obj) for value in self.values]) or (regexmatcher.match('.'.join(path_to_obj))):
             matches_filter = True
 
         if matches_filter:
             if self.callback is not None:
                 self.callback(obj, path_to_obj)
 
         return matches_filter
```

### Comparing `objectwalker-2.1.2/objectwalker/filters/type/FilterTypeIsBuiltinFunctionOrMethod.py` & `objectwalker-2.1.3/objectwalker/filters/type/FilterTypeIsBuiltinFunctionOrMethod.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.2/objectwalker/filters/type/FilterTypeIsMethodWrapper.py` & `objectwalker-2.1.3/objectwalker/filters/type/FilterTypeIsMethodWrapper.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.2/objectwalker/filters/type/FilterTypeIsModule.py` & `objectwalker-2.1.3/objectwalker/filters/type/FilterTypeIsModule.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.2/objectwalker/tests/test_RegExMatcher.py` & `objectwalker-2.1.3/objectwalker/tests/test_RegExMatcher.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.2/objectwalker/utils/RegExMatcher.py` & `objectwalker-2.1.3/objectwalker/utils/RegExMatcher.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.2/objectwalker.egg-info/PKG-INFO` & `objectwalker-2.1.3/objectwalker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objectwalker
-Version: 2.1.2
+Version: 2.1.3
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
-Metadata-Version: 2.1 Name: objectwalker Version: 2.1.2 Summary: UNKNOWN Home-
+Metadata-Version: 2.1 Name: objectwalker Version: 2.1.3 Summary: UNKNOWN Home-
 page: https://github.com/p0dalirius/objectwalker Author: Podalirius Author-
 email: podalirius@protonmail.com License: GPL2 Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
   A python module to explore the object tree to extract paths to interesting
                               objects in memory.
```

### Comparing `objectwalker-2.1.2/objectwalker.egg-info/SOURCES.txt` & `objectwalker-2.1.3/objectwalker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.2/setup.py` & `objectwalker-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 """
 
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = [x.strip() for x in f.readlines()]
 
 setuptools.setup(
     name="objectwalker",
-    version="2.1.2",
+    version="2.1.3",
     description="",
     url="https://github.com/p0dalirius/objectwalker",
     author="Podalirius",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="podalirius@protonmail.com",
     packages=["objectwalker", "objectwalker.filters"],
```


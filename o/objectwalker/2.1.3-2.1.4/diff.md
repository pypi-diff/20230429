# Comparing `tmp/objectwalker-2.1.3.tar.gz` & `tmp/objectwalker-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objectwalker-2.1.3.tar", last modified: Sat Apr 29 18:47:14 2023, max compression
+gzip compressed data, was "objectwalker-2.1.4.tar", last modified: Sat Apr 29 18:59:43 2023, max compression
```

## Comparing `objectwalker-2.1.3.tar` & `objectwalker-2.1.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/
--rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-2.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1784 2023-04-29 18:47:14.470241 objectwalker-2.1.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1642 2023-04-29 18:06:30.000000 objectwalker-2.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.466241 objectwalker-2.1.3/objectwalker/
--rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-2.1.3/objectwalker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7868 2023-04-29 18:46:55.000000 objectwalker-2.1.3/objectwalker/__main__.py
--rw-rw-r--   0 root         (0) root         (0)    13288 2023-04-29 18:35:53.000000 objectwalker-2.1.3/objectwalker/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/filters/
--rw-rw-r--   0 root         (0) root         (0)     1609 2023-04-28 09:59:50.000000 objectwalker-2.1.3/objectwalker/filters/EmptyFilter.py
--rw-rw-r--   0 root         (0) root         (0)      349 2023-04-29 07:25:00.000000 objectwalker-2.1.3/objectwalker/filters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/filters/object/
--rw-rw-r--   0 root         (0) root         (0)      261 2023-04-29 07:24:44.000000 objectwalker-2.1.3/objectwalker/filters/object/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/filters/object/name/
--rw-rw-r--   0 root         (0) root         (0)     1446 2023-04-29 18:11:54.000000 objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameContains.py
--rw-rw-r--   0 root         (0) root         (0)     1429 2023-04-29 18:11:50.000000 objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1443 2023-04-29 18:11:50.000000 objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameEquals.py
--rw-rw-r--   0 root         (0) root         (0)     1763 2023-04-29 17:40:51.000000 objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameIsPythonBuiltin.py
--rw-rw-r--   0 root         (0) root         (0)     1472 2023-04-29 18:11:50.000000 objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      496 2023-04-29 07:23:40.000000 objectwalker-2.1.3/objectwalker/filters/object/name/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/filters/object/value/
--rw-rw-r--   0 root         (0) root         (0)     1437 2023-04-29 18:22:54.000000 objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueContains.py
--rw-rw-r--   0 root         (0) root         (0)     1444 2023-04-29 18:22:54.000000 objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1429 2023-04-29 18:22:54.000000 objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueEquals.py
--rw-rw-r--   0 root         (0) root         (0)     1458 2023-04-29 18:22:54.000000 objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      427 2023-04-29 07:23:31.000000 objectwalker-2.1.3/objectwalker/filters/object/value/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/filters/path/
--rw-rw-r--   0 root         (0) root         (0)     1419 2023-04-29 18:23:37.000000 objectwalker-2.1.3/objectwalker/filters/path/FilterPathContains.py
--rw-rw-r--   0 root         (0) root         (0)     1426 2023-04-29 18:23:37.000000 objectwalker-2.1.3/objectwalker/filters/path/FilterPathEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)     1438 2023-04-29 18:23:37.000000 objectwalker-2.1.3/objectwalker/filters/path/FilterPathStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      324 2023-04-29 07:23:18.000000 objectwalker-2.1.3/objectwalker/filters/path/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/filters/type/
--rw-rw-r--   0 root         (0) root         (0)      835 2023-04-29 07:21:12.000000 objectwalker-2.1.3/objectwalker/filters/type/FilterTypeIsBuiltinFunctionOrMethod.py
--rw-rw-r--   0 root         (0) root         (0)      782 2023-04-29 07:21:12.000000 objectwalker-2.1.3/objectwalker/filters/type/FilterTypeIsMethodWrapper.py
--rw-rw-r--   0 root         (0) root         (0)     2564 2023-04-29 07:21:12.000000 objectwalker-2.1.3/objectwalker/filters/type/FilterTypeIsModule.py
--rw-rw-r--   0 root         (0) root         (0)      368 2023-04-29 07:23:49.000000 objectwalker-2.1.3/objectwalker/filters/type/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-29 10:08:46.000000 objectwalker-2.1.3/objectwalker/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2240 2023-04-29 17:54:40.000000 objectwalker-2.1.3/objectwalker/tests/test_RegExMatcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.470241 objectwalker-2.1.3/objectwalker/utils/
--rw-rw-r--   0 root         (0) root         (0)     4651 2023-04-29 18:19:05.000000 objectwalker-2.1.3/objectwalker/utils/RegExMatcher.py
--rw-rw-r--   0 root         (0) root         (0)      310 2023-04-29 08:39:22.000000 objectwalker-2.1.3/objectwalker/utils/Reporter.py
--rw-rw-r--   0 root         (0) root         (0)      236 2023-04-29 09:12:30.000000 objectwalker-2.1.3/objectwalker/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:47:14.466241 objectwalker-2.1.3/objectwalker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1784 2023-04-29 18:47:14.000000 objectwalker-2.1.3/objectwalker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1623 2023-04-29 18:47:14.000000 objectwalker-2.1.3/objectwalker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 18:47:14.000000 objectwalker-2.1.3/objectwalker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-29 18:47:14.000000 objectwalker-2.1.3/objectwalker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-29 18:47:14.000000 objectwalker-2.1.3/objectwalker.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-2.1.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 18:47:14.470241 objectwalker-2.1.3/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     2538 2023-04-29 18:46:55.000000 objectwalker-2.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:59:43.264521 objectwalker-2.1.4/
+-rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-2.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-04-29 18:59:43.264521 objectwalker-2.1.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1642 2023-04-29 18:06:30.000000 objectwalker-2.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:59:43.264521 objectwalker-2.1.4/objectwalker/
+-rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-2.1.4/objectwalker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7868 2023-04-29 18:58:26.000000 objectwalker-2.1.4/objectwalker/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)    13288 2023-04-29 18:55:48.000000 objectwalker-2.1.4/objectwalker/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:59:43.264521 objectwalker-2.1.4/objectwalker/filters/
+-rw-rw-r--   0 root         (0) root         (0)     1609 2023-04-28 09:59:50.000000 objectwalker-2.1.4/objectwalker/filters/EmptyFilter.py
+-rw-rw-r--   0 root         (0) root         (0)      349 2023-04-29 07:25:00.000000 objectwalker-2.1.4/objectwalker/filters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:59:43.264521 objectwalker-2.1.4/objectwalker/filters/object/
+-rw-rw-r--   0 root         (0) root         (0)      261 2023-04-29 07:24:44.000000 objectwalker-2.1.4/objectwalker/filters/object/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:59:43.264521 objectwalker-2.1.4/objectwalker/filters/object/name/
+-rw-rw-r--   0 root         (0) root         (0)     1446 2023-04-29 18:11:54.000000 objectwalker-2.1.4/objectwalker/filters/object/name/FilterObjectNameContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1429 2023-04-29 18:11:50.000000 objectwalker-2.1.4/objectwalker/filters/object/name/FilterObjectNameEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1443 2023-04-29 18:11:50.000000 objectwalker-2.1.4/objectwalker/filters/object/name/FilterObjectNameEquals.py
+-rw-rw-r--   0 root         (0) root         (0)     1763 2023-04-29 17:40:51.000000 objectwalker-2.1.4/objectwalker/filters/object/name/FilterObjectNameIsPythonBuiltin.py
+-rw-rw-r--   0 root         (0) root         (0)     1472 2023-04-29 18:11:50.000000 objectwalker-2.1.4/objectwalker/filters/object/name/FilterObjectNameStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      496 2023-04-29 07:23:40.000000 objectwalker-2.1.4/objectwalker/filters/object/name/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:59:43.264521 objectwalker-2.1.4/objectwalker/filters/object/value/
+-rw-rw-r--   0 root         (0) root         (0)     1437 2023-04-29 18:22:54.000000 objectwalker-2.1.4/objectwalker/filters/object/value/FilterObjectValueContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1444 2023-04-29 18:22:54.000000 objectwalker-2.1.4/objectwalker/filters/object/value/FilterObjectValueEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1429 2023-04-29 18:22:54.000000 objectwalker-2.1.4/objectwalker/filters/object/value/FilterObjectValueEquals.py
+-rw-rw-r--   0 root         (0) root         (0)     1458 2023-04-29 18:22:54.000000 objectwalker-2.1.4/objectwalker/filters/object/value/FilterObjectValueStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      427 2023-04-29 07:23:31.000000 objectwalker-2.1.4/objectwalker/filters/object/value/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:59:43.264521 objectwalker-2.1.4/objectwalker/filters/path/
+-rw-rw-r--   0 root         (0) root         (0)     1419 2023-04-29 18:23:37.000000 objectwalker-2.1.4/objectwalker/filters/path/FilterPathContains.py
+-rw-rw-r--   0 root         (0) root         (0)     1426 2023-04-29 18:23:37.000000 objectwalker-2.1.4/objectwalker/filters/path/FilterPathEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)     1438 2023-04-29 18:23:37.000000 objectwalker-2.1.4/objectwalker/filters/path/FilterPathStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      324 2023-04-29 07:23:18.000000 objectwalker-2.1.4/objectwalker/filters/path/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:59:43.264521 objectwalker-2.1.4/objectwalker/filters/type/
+-rw-rw-r--   0 root         (0) root         (0)      835 2023-04-29 07:21:12.000000 objectwalker-2.1.4/objectwalker/filters/type/FilterTypeIsBuiltinFunctionOrMethod.py
+-rw-rw-r--   0 root         (0) root         (0)      782 2023-04-29 07:21:12.000000 objectwalker-2.1.4/objectwalker/filters/type/FilterTypeIsMethodWrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     2564 2023-04-29 07:21:12.000000 objectwalker-2.1.4/objectwalker/filters/type/FilterTypeIsModule.py
+-rw-rw-r--   0 root         (0) root         (0)      368 2023-04-29 07:23:49.000000 objectwalker-2.1.4/objectwalker/filters/type/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:59:43.264521 objectwalker-2.1.4/objectwalker/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-29 10:08:46.000000 objectwalker-2.1.4/objectwalker/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2240 2023-04-29 17:54:40.000000 objectwalker-2.1.4/objectwalker/tests/test_RegExMatcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:59:43.264521 objectwalker-2.1.4/objectwalker/utils/
+-rw-rw-r--   0 root         (0) root         (0)     4651 2023-04-29 18:19:05.000000 objectwalker-2.1.4/objectwalker/utils/RegExMatcher.py
+-rw-rw-r--   0 root         (0) root         (0)      310 2023-04-29 08:39:22.000000 objectwalker-2.1.4/objectwalker/utils/Reporter.py
+-rw-rw-r--   0 root         (0) root         (0)      236 2023-04-29 09:12:30.000000 objectwalker-2.1.4/objectwalker/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:59:43.264521 objectwalker-2.1.4/objectwalker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-04-29 18:59:43.000000 objectwalker-2.1.4/objectwalker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1623 2023-04-29 18:59:43.000000 objectwalker-2.1.4/objectwalker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 18:59:43.000000 objectwalker-2.1.4/objectwalker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-29 18:59:43.000000 objectwalker-2.1.4/objectwalker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-29 18:59:43.000000 objectwalker-2.1.4/objectwalker.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-2.1.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 18:59:43.264521 objectwalker-2.1.4/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     2538 2023-04-29 18:58:29.000000 objectwalker-2.1.4/setup.py
```

### Comparing `objectwalker-2.1.3/PKG-INFO` & `objectwalker-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objectwalker
-Version: 2.1.3
+Version: 2.1.4
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
-Metadata-Version: 2.1 Name: objectwalker Version: 2.1.3 Summary: UNKNOWN Home-
+Metadata-Version: 2.1 Name: objectwalker Version: 2.1.4 Summary: UNKNOWN Home-
 page: https://github.com/p0dalirius/objectwalker Author: Podalirius Author-
 email: podalirius@protonmail.com License: GPL2 Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
   A python module to explore the object tree to extract paths to interesting
                               objects in memory.
```

### Comparing `objectwalker-2.1.3/README.md` & `objectwalker-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/__main__.py` & `objectwalker-2.1.4/objectwalker/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import argparse
 import sys
 import objectwalker
 from objectwalker.filters import *
 
 
-VERSION = "2.1.3"
+VERSION = "2.1.4"
 
 
 banner = r"""
        ____  __      _           __ _       __      ____            
       / __ \/ /_    (_)__  _____/ /| |     / /___ _/ / /_____  _____
      / / / / __ \  / / _ \/ ___/ __/ | /| / / __ `/ / //_/ _ \/ ___/
     / /_/ / /_/ / / /  __/ /__/ /_ | |/ |/ / /_/ / / ,< /  __/ /      v%s
```

### Comparing `objectwalker-2.1.3/objectwalker/core.py` & `objectwalker-2.1.4/objectwalker/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,16 +150,16 @@
                         try:
                             path_to_obj = path + [subkey]
                             subobj = eval("obj.%s" % subkey, {"obj": obj})
                         except (SyntaxError, ValueError, KeyError, TypeError) as e:
                             continue
 
                         # Save the found path if it matches filters (accept, and not reject)
-                        if not self.filter_matchmode_accept([f.check(subobj, path_to_obj) for f in self.filters_reject]):
-                            if self.filter_matchmode_reject([f.check(subobj, path_to_obj) for f in self.filters_accept]):
+                        if not self.filter_matchmode_accept([f.check(subobj, path_to_obj) for f in self.filters_accept]):
+                            if self.filter_matchmode_reject([f.check(subobj, path_to_obj) for f in self.filters_reject]):
                                 found.append(path_to_obj)
                         else:
                             # Save id of explored object
                             if int(id(subobj)) not in self.knownids:
                                 self.knownids.append(int(id(subobj)))
 
                         # Explore further
@@ -214,16 +214,16 @@
                         elif type(obj) == list:
                             path_to_obj.append("[%d]" % subkey)
                         # All other types
                         else:
                             path_to_obj.append(subkey)
 
                         # Save the found path if it matches filters (accept, and not reject)
-                        if not self.filter_matchmode_accept([f.check(subobj, path_to_obj) for f in self.filters_reject]):
-                            if self.filter_matchmode_reject([f.check(subobj, path_to_obj) for f in self.filters_accept]):
+                        if not self.filter_matchmode_accept([f.check(subobj, path_to_obj) for f in self.filters_accept]):
+                            if self.filter_matchmode_reject([f.check(subobj, path_to_obj) for f in self.filters_reject]):
                                 found.append(path_to_obj)
                         else:
                             # Save id of explored object
                             if int(id(subobj)) not in self.knownids:
                                 self.knownids.append(int(id(subobj)))
 
                         # Explore further if filters allow it
```

### Comparing `objectwalker-2.1.3/objectwalker/filters/EmptyFilter.py` & `objectwalker-2.1.4/objectwalker/filters/EmptyFilter.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameContains.py` & `objectwalker-2.1.4/objectwalker/filters/object/name/FilterObjectNameContains.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameEndsWith.py` & `objectwalker-2.1.4/objectwalker/filters/object/name/FilterObjectNameEndsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameEquals.py` & `objectwalker-2.1.4/objectwalker/filters/object/name/FilterObjectNameEquals.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameIsPythonBuiltin.py` & `objectwalker-2.1.4/objectwalker/filters/object/name/FilterObjectNameIsPythonBuiltin.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/object/name/FilterObjectNameStartsWith.py` & `objectwalker-2.1.4/objectwalker/filters/object/name/FilterObjectNameStartsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueContains.py` & `objectwalker-2.1.4/objectwalker/filters/object/value/FilterObjectValueContains.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueEndsWith.py` & `objectwalker-2.1.4/objectwalker/filters/object/value/FilterObjectValueEndsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueEquals.py` & `objectwalker-2.1.4/objectwalker/filters/object/value/FilterObjectValueEquals.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/object/value/FilterObjectValueStartsWith.py` & `objectwalker-2.1.4/objectwalker/filters/object/value/FilterObjectValueStartsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/path/FilterPathContains.py` & `objectwalker-2.1.4/objectwalker/filters/path/FilterPathContains.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/path/FilterPathEndsWith.py` & `objectwalker-2.1.4/objectwalker/filters/path/FilterPathEndsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/path/FilterPathStartsWith.py` & `objectwalker-2.1.4/objectwalker/filters/path/FilterPathStartsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/type/FilterTypeIsBuiltinFunctionOrMethod.py` & `objectwalker-2.1.4/objectwalker/filters/type/FilterTypeIsBuiltinFunctionOrMethod.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/type/FilterTypeIsMethodWrapper.py` & `objectwalker-2.1.4/objectwalker/filters/type/FilterTypeIsMethodWrapper.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/filters/type/FilterTypeIsModule.py` & `objectwalker-2.1.4/objectwalker/filters/type/FilterTypeIsModule.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/tests/test_RegExMatcher.py` & `objectwalker-2.1.4/objectwalker/tests/test_RegExMatcher.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker/utils/RegExMatcher.py` & `objectwalker-2.1.4/objectwalker/utils/RegExMatcher.py`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/objectwalker.egg-info/PKG-INFO` & `objectwalker-2.1.4/objectwalker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objectwalker
-Version: 2.1.3
+Version: 2.1.4
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
-Metadata-Version: 2.1 Name: objectwalker Version: 2.1.3 Summary: UNKNOWN Home-
+Metadata-Version: 2.1 Name: objectwalker Version: 2.1.4 Summary: UNKNOWN Home-
 page: https://github.com/p0dalirius/objectwalker Author: Podalirius Author-
 email: podalirius@protonmail.com License: GPL2 Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
   A python module to explore the object tree to extract paths to interesting
                               objects in memory.
```

### Comparing `objectwalker-2.1.3/objectwalker.egg-info/SOURCES.txt` & `objectwalker-2.1.4/objectwalker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `objectwalker-2.1.3/setup.py` & `objectwalker-2.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 """
 
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = [x.strip() for x in f.readlines()]
 
 setuptools.setup(
     name="objectwalker",
-    version="2.1.3",
+    version="2.1.4",
     description="",
     url="https://github.com/p0dalirius/objectwalker",
     author="Podalirius",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="podalirius@protonmail.com",
     packages=["objectwalker", "objectwalker.filters"],
```


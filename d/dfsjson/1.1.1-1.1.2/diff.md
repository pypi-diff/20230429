# Comparing `tmp/dfsjson-1.1.1.tar.gz` & `tmp/dfsjson-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfsjson-1.1.1.tar", max compression
+gzip compressed data, was "dfsjson-1.1.2.tar", max compression
```

## Comparing `dfsjson-1.1.1.tar` & `dfsjson-1.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-04-21 10:30:21.167494 dfsjson-1.1.1/LICENSE
--rw-r--r--   0        0        0      972 2023-04-22 09:47:28.532993 dfsjson-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-21 10:14:31.990972 dfsjson-1.1.1/dfsjson/__init__.py
--rw-r--r--   0        0        0       28 2023-04-21 13:40:54.294586 dfsjson-1.1.1/dfsjson/src/__init__.py
--rw-r--r--   0        0        0     3344 2023-04-22 09:35:38.005165 dfsjson-1.1.1/dfsjson/src/dfsjson.py
--rw-r--r--   0        0        0      499 2023-04-22 09:48:10.937282 dfsjson-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 dfsjson-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-21 10:30:21.167494 dfsjson-1.1.2/LICENSE
+-rw-r--r--   0        0        0      972 2023-04-22 09:47:28.532993 dfsjson-1.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 10:14:31.990972 dfsjson-1.1.2/dfsjson/__init__.py
+-rw-r--r--   0        0        0       28 2023-04-21 13:40:54.294586 dfsjson-1.1.2/dfsjson/src/__init__.py
+-rw-r--r--   0        0        0     3362 2023-04-29 09:46:58.350747 dfsjson-1.1.2/dfsjson/src/dfsjson.py
+-rw-r--r--   0        0        0      499 2023-04-29 09:48:31.848041 dfsjson-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 dfsjson-1.1.2/PKG-INFO
```

### Comparing `dfsjson-1.1.1/LICENSE` & `dfsjson-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dfsjson-1.1.1/README.md` & `dfsjson-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dfsjson-1.1.1/dfsjson/src/dfsjson.py` & `dfsjson-1.1.2/dfsjson/src/dfsjson.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 import json
 import re
 
 
 class DFSJson:
-    def __init__(self, max_depth=100, max_diff=5):
+    def __init__(self, max_depth=200, max_diff=10):
         self.max_depth = max_depth
         self.max_diff = max_diff
         self.search_pattern = r'([\[\]\(\)\{\}\,\"\'])'
-        self.replace_characters = """\"\',+ }{()]"""
+        self.replace_characters = """\"\',+ }{()[]"""
         return
 
     @staticmethod
     def dump(*args):
         return json.dump(*args)
 
     @staticmethod
@@ -69,15 +69,15 @@
             cur_fitness = self.fitness(string)
         if max_depth < 0:
             return string, 0
         if cur_fitness == int(1e8):
             return string, cur_fitness
         best_fitness = cur_fitness
         best_string = string
-        indexes = [cur_fitness] + [
+        indexes = [0, len(string), cur_fitness] + [
             r.span()[0]
             for r in re.finditer(self.search_pattern, string)
         ]
         diff = -self.max_diff
 
         for index in indexes:
             for m in self.replace_characters:
```

### Comparing `dfsjson-1.1.1/PKG-INFO` & `dfsjson-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfsjson
-Version: 1.1.1
+Version: 1.1.2
 Summary: A robust JSON encoder that fixes errors by utilizing DFS algorithm.
 Home-page: https://github.com/AutomaticHourglass/dfsjson
 Keywords: JSON,JSON Serialize,DFS,Error correcting JSON
 Author: Unsal Gokdag
 Author-email: unsal.gokdag@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/joern_lib-0.6.5.tar.gz` & `tmp/joern_lib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joern_lib-0.6.5.tar", max compression
+gzip compressed data, was "joern_lib-0.7.0.tar", max compression
```

## Comparing `joern_lib-0.6.5.tar` & `joern_lib-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-04-28 20:22:45.955128 joern_lib-0.6.5/LICENSE
--rw-r--r--   0        0        0     3102 2023-04-28 20:22:45.959128 joern_lib-0.6.5/README.md
--rw-r--r--   0        0        0        0 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/__init__.py
--rw-r--r--   0        0        0     6605 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/client.py
--rw-r--r--   0        0        0        0 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/detectors/__init__.py
--rw-r--r--   0        0        0      627 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/detectors/c.py
--rw-r--r--   0        0        0     4132 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/detectors/common.py
--rw-r--r--   0        0        0     3914 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/detectors/js.py
--rw-r--r--   0        0        0     2060 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/utils.py
--rw-r--r--   0        0        0     4535 2023-04-28 20:22:45.979129 joern_lib-0.6.5/joern_lib/workspace.py
--rw-r--r--   0        0        0     1185 2023-04-28 20:22:45.979129 joern_lib-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     4443 1970-01-01 00:00:00.000000 joern_lib-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-29 00:44:10.997535 joern_lib-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3102 2023-04-29 00:44:10.997535 joern_lib-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-29 00:44:11.017536 joern_lib-0.7.0/joern_lib/__init__.py
+-rw-r--r--   0        0        0     6685 2023-04-29 00:44:11.017536 joern_lib-0.7.0/joern_lib/client.py
+-rw-r--r--   0        0        0        0 2023-04-29 00:44:11.017536 joern_lib-0.7.0/joern_lib/detectors/__init__.py
+-rw-r--r--   0        0        0      627 2023-04-29 00:44:11.017536 joern_lib-0.7.0/joern_lib/detectors/c.py
+-rw-r--r--   0        0        0     6184 2023-04-29 00:44:11.021535 joern_lib-0.7.0/joern_lib/detectors/common.py
+-rw-r--r--   0        0        0     3914 2023-04-29 00:44:11.021535 joern_lib-0.7.0/joern_lib/detectors/js.py
+-rw-r--r--   0        0        0     2800 2023-04-29 00:44:11.021535 joern_lib-0.7.0/joern_lib/utils.py
+-rw-r--r--   0        0        0     4535 2023-04-29 00:44:11.021535 joern_lib-0.7.0/joern_lib/workspace.py
+-rw-r--r--   0        0        0     1185 2023-04-29 00:44:11.021535 joern_lib-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4443 1970-01-01 00:00:00.000000 joern_lib-0.7.0/PKG-INFO
```

### Comparing `joern_lib-0.6.5/LICENSE` & `joern_lib-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joern_lib-0.6.5/README.md` & `joern_lib-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `joern_lib-0.6.5/joern_lib/client.py` & `joern_lib-0.7.0/joern_lib/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
+import os
 
 import httpx
-import os
 import orjson
 import uvloop
 
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
 import websockets
 
@@ -86,14 +86,16 @@
         query_str = query_str.replace("\\.", "\\\\.")
     if (
         query_str.startswith("cpg.")
         or query_str.startswith("({cpg.")
         and ".toJson" not in query_str
         and ".plotDot" not in query_str
         and not query_str.endswith(".p")
+        and "def" not in query_str
+        and "printCallTree" not in query_str
     ):
         query_str = f"{query_str}.toJsonPretty"
     return query_str
 
 
 def parse_error(serr):
     if "No projects loaded" in serr:
```

### Comparing `joern_lib-0.6.5/joern_lib/detectors/c.py` & `joern_lib-0.7.0/joern_lib/detectors/c.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.6.5/joern_lib/detectors/js.py` & `joern_lib-0.7.0/joern_lib/detectors/js.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.6.5/joern_lib/utils.py` & `joern_lib-0.7.0/joern_lib/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 
 from rich.console import Console
 from rich.syntax import Syntax
 from rich.table import Table
+from rich.tree import Tree
 
 console = Console(
     log_time=False,
     log_path=False,
     color_system="auto",
     width=int(os.getenv("COLUMNS", 280)),
 )
@@ -58,7 +59,29 @@
 
 
 def print_md(result):
     if isinstance(result, dict) and result.get("response"):
         console.print(result.get("response"))
     else:
         console.print(result)
+
+
+def walk_tree(paths, tree, level_branches):
+    for path in paths:
+        level = path.count("|    ")
+        if level == 0:
+            branch = tree
+        elif level_branches.get(level - 1):
+            branch = level_branches.get(level - 1)
+            if not level_branches.get(level):
+                level_branches[level] = branch
+        branch.add(path.replace("+--- ", ""))
+
+
+def print_tree(result, guide_style="bold bright_blue"):
+    result = result.split("\n")
+    if result:
+        tree = Tree(result[0].replace("+--- ", ""), guide_style=guide_style)
+        level_branches = {0: tree}
+        if len(result) > 1:
+            walk_tree(result[1:], tree, level_branches)
+    console.print(tree)
```

### Comparing `joern_lib-0.6.5/joern_lib/workspace.py` & `joern_lib-0.7.0/joern_lib/workspace.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.6.5/pyproject.toml` & `joern_lib-0.7.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "joern-lib"
-version = "0.6.5"
+version = "0.7.0"
 description = "Python library to interact with Joern server"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "joern_lib"}]
 homepage = "https://github.com/AppThreat/joern-lib"
 repository = "https://github.com/AppThreat/joern-lib"
```

### Comparing `joern_lib-0.6.5/PKG-INFO` & `joern_lib-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joern-lib
-Version: 0.6.5
+Version: 0.7.0
 Summary: Python library to interact with Joern server
 Home-page: https://github.com/AppThreat/joern-lib
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.7,<3.11
```


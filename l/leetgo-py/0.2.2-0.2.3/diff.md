# Comparing `tmp/leetgo-py-0.2.2.tar.gz` & `tmp/leetgo_py-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leetgo-py-0.2.2.tar", max compression
+gzip compressed data, was "leetgo_py-0.2.3.tar", max compression
```

## Comparing `leetgo-py-0.2.2.tar` & `leetgo_py-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      515 2023-04-27 02:41:41.571155 leetgo-py-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      288 2023-04-27 02:41:41.571917 leetgo-py-0.2.2/src/leetgo_py/__init__.py
--rw-r--r--   0        0        0      735 2023-04-18 12:56:19.579341 leetgo-py-0.2.2/src/leetgo_py/list.py
--rw-r--r--   0        0        0     1415 2023-04-18 12:56:19.579909 leetgo-py-0.2.2/src/leetgo_py/parse.py
--rw-r--r--   0        0        0     1224 2023-04-18 12:56:19.580506 leetgo-py-0.2.2/src/leetgo_py/tree.py
--rw-r--r--   0        0        0      179 2023-04-18 12:56:19.581019 leetgo-py-0.2.2/src/leetgo_py/utils.py
--rw-r--r--   0        0        0      626 2023-04-27 02:42:16.636208 leetgo-py-0.2.2/setup.py
--rw-r--r--   0        0        0      665 2023-04-27 02:42:16.636442 leetgo-py-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      515 2023-04-29 13:55:04.647529 leetgo_py-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-04-28 08:33:48.881220 leetgo_py-0.2.3/src/leetgo_py/__init__.py
+-rw-r--r--   0        0        0      735 2023-04-18 15:36:24.716681 leetgo_py-0.2.3/src/leetgo_py/list.py
+-rw-r--r--   0        0        0     1415 2023-04-29 13:55:04.647529 leetgo_py-0.2.3/src/leetgo_py/parse.py
+-rw-r--r--   0        0        0     1224 2023-04-18 15:36:24.717797 leetgo_py-0.2.3/src/leetgo_py/tree.py
+-rw-r--r--   0        0        0      179 2023-04-18 15:36:24.718797 leetgo_py-0.2.3/src/leetgo_py/utils.py
+-rw-r--r--   0        0        0      632 1970-01-01 00:00:00.000000 leetgo_py-0.2.3/setup.py
+-rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 leetgo_py-0.2.3/PKG-INFO
```

### Comparing `leetgo-py-0.2.2/pyproject.toml` & `leetgo_py-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "leetgo-py"
-version = "0.2.2"
+version = "0.2.3"
 description = "Python test utils for leetgo"
 authors = ["j178 <10510431+j178@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://github.com/j178/leetgo"
 repository = "https://github.com/j178/leetgo"
 keywords = ["leetcode"]
```

### Comparing `leetgo-py-0.2.2/src/leetgo_py/list.py` & `leetgo_py-0.2.3/src/leetgo_py/list.py`

 * *Files identical despite different names*

### Comparing `leetgo-py-0.2.2/src/leetgo_py/parse.py` & `leetgo_py-0.2.3/src/leetgo_py/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
     splits = json.loads(s)
     res = [json.dumps(split) for split in splits]
     return res
 
 
 def serialize(val: Any) -> str:
-    if isinstance(val, int):
+    if isinstance(val, bool):
+        return "true" if val else "false"
+    elif isinstance(val, int):
         return str(val)
     elif isinstance(val, float):
         return str(val)
     elif isinstance(val, str):
         return '"' + val + '"'
-    elif isinstance(val, bool):
-        return "true" if val else "false"
     elif isinstance(val, list):
         return "[" + ",".join(serialize(v) for v in val) + "]"
     elif isinstance(val, (ListNode, TreeNode)):
         return val.serialize()
     else:
         raise Exception("Unknown type: " + str(type(val)))
```

### Comparing `leetgo-py-0.2.2/src/leetgo_py/tree.py` & `leetgo_py-0.2.3/src/leetgo_py/tree.py`

 * *Files identical despite different names*

### Comparing `leetgo-py-0.2.2/setup.py` & `leetgo_py-0.2.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 ['leetgo_py']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'leetgo-py',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Python test utils for leetgo',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'j178',
     'author_email': '10510431+j178@users.noreply.github.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/j178/leetgo',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.6,<4.0',
 }
```

### Comparing `leetgo-py-0.2.2/PKG-INFO` & `leetgo_py-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: leetgo-py
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python test utils for leetgo
 Home-page: https://github.com/j178/leetgo
 License: MIT
 Keywords: leetcode
 Author: j178
 Author-email: 10510431+j178@users.noreply.github.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/j178/leetgo
```


# Comparing `tmp/hkkang_utils-0.1.8.tar.gz` & `tmp/hkkang_utils-0.1.9.tar.gz`

## Comparing `hkkang_utils-0.1.8.tar` & `hkkang_utils-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,18 @@
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.8/src/hkkang_utils/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 hkkang_utils-0.1.8/src/hkkang_utils/file.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hkkang_utils-0.1.8/src/hkkang_utils/list.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.8/src/hkkang_utils/sql.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 hkkang_utils-0.1.8/src/hkkang_utils/string.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 hkkang_utils-0.1.8/src/hkkang_utils/tensor.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.8/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.8/LICENSE
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hkkang_utils-0.1.8/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hkkang_utils-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 hkkang_utils-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/.vscode/settings.json
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/src/hkkang_utils/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/src/hkkang_utils/file.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/src/hkkang_utils/list.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/src/hkkang_utils/misc.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/src/hkkang_utils/sql.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/src/hkkang_utils/string.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/src/hkkang_utils/tensor.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/tests/test_file.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/tests/test_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/tests/test_sql.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/tests/test_string.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/tests/test_tensor.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/LICENSE
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/PKG-INFO
```

### Comparing `hkkang_utils-0.1.8/src/hkkang_utils/sql.py` & `hkkang_utils-0.1.9/src/hkkang_utils/sql.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.8/src/hkkang_utils/string.py` & `hkkang_utils-0.1.9/src/hkkang_utils/string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.8/src/hkkang_utils/tensor.py` & `hkkang_utils-0.1.9/src/hkkang_utils/tensor.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.8/.gitignore` & `hkkang_utils-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.8/LICENSE` & `hkkang_utils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.8/pyproject.toml` & `hkkang_utils-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hkkang_utils"
-version = "0.1.8"
+version = "0.1.9"
 authors = [{name="Hyukkyu Kang", email="hyukkyukang@gmail.com"}]
 description = "A collection of useful util functions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `hkkang_utils-0.1.8/PKG-INFO` & `hkkang_utils-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkkang_utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collection of useful util functions
 Project-URL: Homepage, https://github.com/hyukkyukang/python_utils
 Project-URL: Bug Tracker, https://github.com/hyukkyukang/python_utils/issues
 Author-email: Hyukkyu Kang <hyukkyukang@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,7 +15,12 @@
 Requires-Dist: pglast>=3.17
 Requires-Dist: torch>=1.13
 Description-Content-Type: text/markdown
 
 # Python util funcs
 
 This is a collection of python functions that I use in my projects.
+
+To install [the package](https://pypi.org/project/hkkang-utils/):
+```bash
+pip install hkkang_utils
+```
```


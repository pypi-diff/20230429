# Comparing `tmp/llm_generation_server-0.0.5.tar.gz` & `tmp/llm_generation_server-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_generation_server-0.0.5.tar", last modified: Sat Apr 29 13:59:16 2023, max compression
+gzip compressed data, was "llm_generation_server-0.0.6.tar", last modified: Sat Apr 29 14:25:04 2023, max compression
```

## Comparing `llm_generation_server-0.0.5.tar` & `llm_generation_server-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:16.060130 llm_generation_server-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-29 13:59:16.060130 llm_generation_server-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-29 13:59:08.000000 llm_generation_server-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:16.056130 llm_generation_server-0.0.5/llm_generation_server/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/component_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:16.056130 llm_generation_server-0.0.5/llm_generation_server/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:16.060130 llm_generation_server-0.0.5/llm_generation_server/elements/
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/elements/barchart_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/elements/element_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/elements/plain_text_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/elements/selector_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/elements/table_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/elements/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:16.056130 llm_generation_server-0.0.5/llm_generation_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-29 13:59:16.000000 llm_generation_server-0.0.5/llm_generation_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-29 13:59:16.000000 llm_generation_server-0.0.5/llm_generation_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:59:16.000000 llm_generation_server-0.0.5/llm_generation_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-29 13:59:16.000000 llm_generation_server-0.0.5/llm_generation_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 13:59:16.000000 llm_generation_server-0.0.5/llm_generation_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-29 13:59:08.000000 llm_generation_server-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 13:59:16.060130 llm_generation_server-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:25:04.612775 llm_generation_server-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 14:24:50.000000 llm_generation_server-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-29 14:24:50.000000 llm_generation_server-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-29 14:25:04.612775 llm_generation_server-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-29 14:24:56.000000 llm_generation_server-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:25:04.608775 llm_generation_server-0.0.6/llm_generation_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-29 14:24:50.000000 llm_generation_server-0.0.6/llm_generation_server/component_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:25:04.608775 llm_generation_server-0.0.6/llm_generation_server/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-29 14:24:50.000000 llm_generation_server-0.0.6/llm_generation_server/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-29 14:24:50.000000 llm_generation_server-0.0.6/llm_generation_server/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:25:04.612775 llm_generation_server-0.0.6/llm_generation_server/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-29 14:24:50.000000 llm_generation_server-0.0.6/llm_generation_server/elements/barchart_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-29 14:24:50.000000 llm_generation_server-0.0.6/llm_generation_server/elements/element_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-29 14:24:50.000000 llm_generation_server-0.0.6/llm_generation_server/elements/plain_text_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-29 14:24:50.000000 llm_generation_server-0.0.6/llm_generation_server/elements/selector_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-29 14:24:50.000000 llm_generation_server-0.0.6/llm_generation_server/elements/table_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-29 14:24:50.000000 llm_generation_server-0.0.6/llm_generation_server/elements/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-29 14:24:50.000000 llm_generation_server-0.0.6/llm_generation_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:25:04.608775 llm_generation_server-0.0.6/llm_generation_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-29 14:25:04.000000 llm_generation_server-0.0.6/llm_generation_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-29 14:25:04.000000 llm_generation_server-0.0.6/llm_generation_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 14:25:04.000000 llm_generation_server-0.0.6/llm_generation_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-29 14:25:04.000000 llm_generation_server-0.0.6/llm_generation_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 14:25:04.000000 llm_generation_server-0.0.6/llm_generation_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-29 14:24:56.000000 llm_generation_server-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 14:25:04.612775 llm_generation_server-0.0.6/setup.cfg
```

### Comparing `llm_generation_server-0.0.5/LICENSE` & `llm_generation_server-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.5/PKG-INFO` & `llm_generation_server-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: llm_generation_server
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple full stack app for displaying distribution of next token.
 Author-email: "Frantisek Trebuna (gortibaldik)" <ferotre@gmail.com>
 Project-URL: Homepage, https://github.com/gortibaldik/visualize_llm_generation
 Project-URL: Bug Tracker, https://github.com/gortibaldik/visualize_llm_generation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.0.5`
+## VERSION: `0.0.6`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
```

### Comparing `llm_generation_server-0.0.5/README.md` & `llm_generation_server-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.0.5`
+## VERSION: `0.0.6`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
```

### Comparing `llm_generation_server-0.0.5/llm_generation_server/component_base.py` & `llm_generation_server-0.0.6/llm_generation_server/component_base.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.5/llm_generation_server/dist/favicon.ico` & `llm_generation_server-0.0.6/llm_generation_server/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.5/llm_generation_server/elements/barchart_element.py` & `llm_generation_server-0.0.6/llm_generation_server/elements/barchart_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.5/llm_generation_server/elements/element_base.py` & `llm_generation_server-0.0.6/llm_generation_server/elements/element_base.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.5/llm_generation_server/elements/plain_text_element.py` & `llm_generation_server-0.0.6/llm_generation_server/elements/plain_text_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.5/llm_generation_server/elements/selector_element.py` & `llm_generation_server-0.0.6/llm_generation_server/elements/selector_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.5/llm_generation_server/elements/table_element.py` & `llm_generation_server-0.0.6/llm_generation_server/elements/table_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.5/llm_generation_server/elements/utils.py` & `llm_generation_server-0.0.6/llm_generation_server/elements/utils.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.5/llm_generation_server/server.py` & `llm_generation_server-0.0.6/llm_generation_server/server.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.5/llm_generation_server.egg-info/PKG-INFO` & `llm_generation_server-0.0.6/llm_generation_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: llm-generation-server
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple full stack app for displaying distribution of next token.
 Author-email: "Frantisek Trebuna (gortibaldik)" <ferotre@gmail.com>
 Project-URL: Homepage, https://github.com/gortibaldik/visualize_llm_generation
 Project-URL: Bug Tracker, https://github.com/gortibaldik/visualize_llm_generation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.0.5`
+## VERSION: `0.0.6`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
```

### Comparing `llm_generation_server-0.0.5/llm_generation_server.egg-info/SOURCES.txt` & `llm_generation_server-0.0.6/llm_generation_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.5/pyproject.toml` & `llm_generation_server-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm_generation_server"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Frantisek Trebuna (gortibaldik)", email="ferotre@gmail.com" },
 ]
 description = "Simple full stack app for displaying distribution of next token."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -31,15 +31,15 @@
 [tool.setuptools.package-dir]
 llm_generation_server = "llm_generation_server"
 
 [tool.isort]
 profile = "black"
 
 [tool.bumpver]
-current_version = "0.0.5"
+current_version = "0.0.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```


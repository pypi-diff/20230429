# Comparing `tmp/llm_generation_server-0.0.3.tar.gz` & `tmp/llm_generation_server-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_generation_server-0.0.3.tar", last modified: Sat Apr 29 12:08:06 2023, max compression
+gzip compressed data, was "llm_generation_server-0.0.5.tar", last modified: Sat Apr 29 13:59:16 2023, max compression
```

## Comparing `llm_generation_server-0.0.3.tar` & `llm_generation_server-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:08:06.651881 llm_generation_server-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 12:07:33.000000 llm_generation_server-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-29 12:07:33.000000 llm_generation_server-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-29 12:08:06.651881 llm_generation_server-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-29 12:07:54.000000 llm_generation_server-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:08:06.647881 llm_generation_server-0.0.3/llm_generation_server/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-29 12:07:33.000000 llm_generation_server-0.0.3/llm_generation_server/component_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:08:06.647881 llm_generation_server-0.0.3/llm_generation_server/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-29 12:07:33.000000 llm_generation_server-0.0.3/llm_generation_server/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-29 12:07:33.000000 llm_generation_server-0.0.3/llm_generation_server/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:08:06.651881 llm_generation_server-0.0.3/llm_generation_server/elements/
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-29 12:07:33.000000 llm_generation_server-0.0.3/llm_generation_server/elements/barchart_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-29 12:07:33.000000 llm_generation_server-0.0.3/llm_generation_server/elements/element_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-29 12:07:33.000000 llm_generation_server-0.0.3/llm_generation_server/elements/plain_text_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-29 12:07:33.000000 llm_generation_server-0.0.3/llm_generation_server/elements/selector_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-29 12:07:33.000000 llm_generation_server-0.0.3/llm_generation_server/elements/table_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-29 12:07:33.000000 llm_generation_server-0.0.3/llm_generation_server/elements/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-29 12:07:33.000000 llm_generation_server-0.0.3/llm_generation_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:08:06.647881 llm_generation_server-0.0.3/llm_generation_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-29 12:08:06.000000 llm_generation_server-0.0.3/llm_generation_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-29 12:08:06.000000 llm_generation_server-0.0.3/llm_generation_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 12:08:06.000000 llm_generation_server-0.0.3/llm_generation_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-29 12:08:06.000000 llm_generation_server-0.0.3/llm_generation_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 12:08:06.000000 llm_generation_server-0.0.3/llm_generation_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-29 12:07:54.000000 llm_generation_server-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 12:08:06.651881 llm_generation_server-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:16.060130 llm_generation_server-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-29 13:59:16.060130 llm_generation_server-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-29 13:59:08.000000 llm_generation_server-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:16.056130 llm_generation_server-0.0.5/llm_generation_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/component_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:16.056130 llm_generation_server-0.0.5/llm_generation_server/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:16.060130 llm_generation_server-0.0.5/llm_generation_server/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/elements/barchart_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/elements/element_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/elements/plain_text_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/elements/selector_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/elements/table_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/elements/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-29 13:59:01.000000 llm_generation_server-0.0.5/llm_generation_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:59:16.056130 llm_generation_server-0.0.5/llm_generation_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-29 13:59:16.000000 llm_generation_server-0.0.5/llm_generation_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-29 13:59:16.000000 llm_generation_server-0.0.5/llm_generation_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:59:16.000000 llm_generation_server-0.0.5/llm_generation_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-29 13:59:16.000000 llm_generation_server-0.0.5/llm_generation_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 13:59:16.000000 llm_generation_server-0.0.5/llm_generation_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-29 13:59:08.000000 llm_generation_server-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 13:59:16.060130 llm_generation_server-0.0.5/setup.cfg
```

### Comparing `llm_generation_server-0.0.3/LICENSE` & `llm_generation_server-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.3/PKG-INFO` & `llm_generation_server-0.0.5/llm_generation_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
-Name: llm_generation_server
-Version: 0.0.3
+Name: llm-generation-server
+Version: 0.0.5
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
 
-## VERSION: `0.0.3`
+## VERSION: `0.0.5`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
 
-- right now only installation right from the git is supported, however I plan to deploy the package also to PyPi
-- `pip install git+https://github.com/gortibaldik/visualize_llm_generation#egg=llm_generation_server`
+- install from pypi:
+  - `pip install llm-generation-server`
+- install directly from git:
+  - `pip install git+https://github.com/gortibaldik/visualize_llm_generation#egg=llm_generation_server`
 
 ## Usage
 
 The library is composed of three parts:
 
 1. Server - `llm_generation_server.server.Server`
 2. Component - `llm_generation_server.component_base.ComponentBase`
@@ -214,15 +216,15 @@
 def _initialize_vocab(self):
     word_site = "https://www.mit.edu/~ecprice/wordlist.10000"
     response = requests.get(word_site)
     self.word_vocab = [x.decode("utf-8") for x in response.content.splitlines()]
     self.ix_arr = list(range(len(self.word_vocab)))
 ```
 
-![barchart_page](./readme_images/softmax.png)
+![barchart_page ](./readme_images/softmax.png)
 
 ## More Elaborate Example
 
-More elaborate example can be found in [`app.py`](./app.py) and [`examples_py/*`](./examples_py/). The example frontend generated by such an application is shown below.
+More elaborate example can be found in [`app.py`](https://github.com/gortibaldik/visualize_llm_generation/app.py) and [`examples_py/*`](https://github.com/gortibaldik/visualize_llm_generation/examples_py/). The example frontend generated by such an application is shown below.
 
 ![next_token_page](./readme_images/example_next_token.png)
 ![example_multi_tables](./readme_images/example_dialogue.png)
```

### Comparing `llm_generation_server-0.0.3/README.md` & `llm_generation_server-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.0.3`
+## VERSION: `0.0.5`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
 
-- right now only installation right from the git is supported, however I plan to deploy the package also to PyPi
-- `pip install git+https://github.com/gortibaldik/visualize_llm_generation#egg=llm_generation_server`
+- install from pypi:
+  - `pip install llm-generation-server`
+- install directly from git:
+  - `pip install git+https://github.com/gortibaldik/visualize_llm_generation#egg=llm_generation_server`
 
 ## Usage
 
 The library is composed of three parts:
 
 1. Server - `llm_generation_server.server.Server`
 2. Component - `llm_generation_server.component_base.ComponentBase`
@@ -200,15 +202,15 @@
 def _initialize_vocab(self):
     word_site = "https://www.mit.edu/~ecprice/wordlist.10000"
     response = requests.get(word_site)
     self.word_vocab = [x.decode("utf-8") for x in response.content.splitlines()]
     self.ix_arr = list(range(len(self.word_vocab)))
 ```
 
-![barchart_page](./readme_images/softmax.png)
+![barchart_page ](./readme_images/softmax.png)
 
 ## More Elaborate Example
 
-More elaborate example can be found in [`app.py`](./app.py) and [`examples_py/*`](./examples_py/). The example frontend generated by such an application is shown below.
+More elaborate example can be found in [`app.py`](https://github.com/gortibaldik/visualize_llm_generation/app.py) and [`examples_py/*`](https://github.com/gortibaldik/visualize_llm_generation/examples_py/). The example frontend generated by such an application is shown below.
 
 ![next_token_page](./readme_images/example_next_token.png)
 ![example_multi_tables](./readme_images/example_dialogue.png)
```

### Comparing `llm_generation_server-0.0.3/llm_generation_server/component_base.py` & `llm_generation_server-0.0.5/llm_generation_server/component_base.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.3/llm_generation_server/dist/favicon.ico` & `llm_generation_server-0.0.5/llm_generation_server/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.3/llm_generation_server/elements/barchart_element.py` & `llm_generation_server-0.0.5/llm_generation_server/elements/barchart_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.3/llm_generation_server/elements/element_base.py` & `llm_generation_server-0.0.5/llm_generation_server/elements/element_base.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.3/llm_generation_server/elements/plain_text_element.py` & `llm_generation_server-0.0.5/llm_generation_server/elements/plain_text_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.3/llm_generation_server/elements/selector_element.py` & `llm_generation_server-0.0.5/llm_generation_server/elements/selector_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.3/llm_generation_server/elements/table_element.py` & `llm_generation_server-0.0.5/llm_generation_server/elements/table_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.3/llm_generation_server/elements/utils.py` & `llm_generation_server-0.0.5/llm_generation_server/elements/utils.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.3/llm_generation_server/server.py` & `llm_generation_server-0.0.5/llm_generation_server/server.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.3/llm_generation_server.egg-info/PKG-INFO` & `llm_generation_server-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
-Name: llm-generation-server
-Version: 0.0.3
+Name: llm_generation_server
+Version: 0.0.5
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
 
-## VERSION: `0.0.3`
+## VERSION: `0.0.5`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
 
-- right now only installation right from the git is supported, however I plan to deploy the package also to PyPi
-- `pip install git+https://github.com/gortibaldik/visualize_llm_generation#egg=llm_generation_server`
+- install from pypi:
+  - `pip install llm-generation-server`
+- install directly from git:
+  - `pip install git+https://github.com/gortibaldik/visualize_llm_generation#egg=llm_generation_server`
 
 ## Usage
 
 The library is composed of three parts:
 
 1. Server - `llm_generation_server.server.Server`
 2. Component - `llm_generation_server.component_base.ComponentBase`
@@ -214,15 +216,15 @@
 def _initialize_vocab(self):
     word_site = "https://www.mit.edu/~ecprice/wordlist.10000"
     response = requests.get(word_site)
     self.word_vocab = [x.decode("utf-8") for x in response.content.splitlines()]
     self.ix_arr = list(range(len(self.word_vocab)))
 ```
 
-![barchart_page](./readme_images/softmax.png)
+![barchart_page ](./readme_images/softmax.png)
 
 ## More Elaborate Example
 
-More elaborate example can be found in [`app.py`](./app.py) and [`examples_py/*`](./examples_py/). The example frontend generated by such an application is shown below.
+More elaborate example can be found in [`app.py`](https://github.com/gortibaldik/visualize_llm_generation/app.py) and [`examples_py/*`](https://github.com/gortibaldik/visualize_llm_generation/examples_py/). The example frontend generated by such an application is shown below.
 
 ![next_token_page](./readme_images/example_next_token.png)
 ![example_multi_tables](./readme_images/example_dialogue.png)
```

### Comparing `llm_generation_server-0.0.3/llm_generation_server.egg-info/SOURCES.txt` & `llm_generation_server-0.0.5/llm_generation_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.3/pyproject.toml` & `llm_generation_server-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm_generation_server"
-version = "0.0.3"
+version = "0.0.5"
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
-current_version = "0.0.3"
+current_version = "0.0.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```


# Comparing `tmp/semantra-0.1.5.tar.gz` & `tmp/semantra-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantra-0.1.5.tar", last modified: Thu Apr 27 04:42:35 2023, max compression
+gzip compressed data, was "semantra-0.1.6.tar", last modified: Sat Apr 29 15:53:21 2023, max compression
```

## Comparing `semantra-0.1.5.tar` & `semantra-0.1.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:42:35.888933 semantra-0.1.5/
--rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.1.5/LICENSE
--rw-r--r--   0 freedmand   (501) staff       (20)    10618 2023-04-27 04:42:35.886173 semantra-0.1.5/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)    10075 2023-04-26 12:51:15.000000 semantra-0.1.5/README.md
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:42:35.876965 semantra-0.1.5/client/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:42:35.878836 semantra-0.1.5/client/public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:42:35.879673 semantra-0.1.5/client/public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-04-27 04:42:09.000000 semantra-0.1.5/client/public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449103 2023-04-27 04:42:09.000000 semantra-0.1.5/client/public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495745 2023-04-27 04:42:09.000000 semantra-0.1.5/client/public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.5/client/public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.5/client/public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-27 04:38:40.000000 semantra-0.1.5/client/public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)     1020 2023-04-27 04:42:07.000000 semantra-0.1.5/pyproject.toml
--rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-27 04:42:35.888982 semantra-0.1.5/setup.cfg
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:42:35.877224 semantra-0.1.5/src/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:42:35.881480 semantra-0.1.5/src/semantra/
--rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.1.5/src/semantra/__init__.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:42:35.883584 semantra-0.1.5/src/semantra/__pycache__/
--rw-r--r--   0 freedmand   (501) staff       (20)      148 2023-04-23 04:39:41.000000 semantra-0.1.5/src/semantra/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)    10961 2023-04-23 04:37:57.000000 semantra-0.1.5/src/semantra/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)     3086 2023-04-23 04:37:58.000000 semantra-0.1.5/src/semantra/__pycache__/pdf.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)    19561 2023-04-23 12:15:19.000000 semantra-0.1.5/src/semantra/__pycache__/semantra.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)     4744 2023-04-23 04:37:58.000000 semantra-0.1.5/src/semantra/__pycache__/util.cpython-39.pyc
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:42:35.884045 semantra-0.1.5/src/semantra/client_public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:42:35.885047 semantra-0.1.5/src/semantra/client_public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-04-27 04:42:09.000000 semantra-0.1.5/src/semantra/client_public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449103 2023-04-27 04:42:09.000000 semantra-0.1.5/src/semantra/client_public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495745 2023-04-27 04:42:09.000000 semantra-0.1.5/src/semantra/client_public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.5/src/semantra/client_public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.5/src/semantra/client_public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-27 04:38:40.000000 semantra-0.1.5/src/semantra/client_public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)    11501 2023-04-27 04:38:40.000000 semantra-0.1.5/src/semantra/models.py
--rw-r--r--   0 freedmand   (501) staff       (20)     3325 2023-04-27 04:38:40.000000 semantra-0.1.5/src/semantra/pdf.py
--rw-r--r--   0 freedmand   (501) staff       (20)    28701 2023-04-27 04:38:40.000000 semantra-0.1.5/src/semantra/semantra.py
--rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-04-27 04:38:40.000000 semantra-0.1.5/src/semantra/util.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-27 04:42:35.882232 semantra-0.1.5/src/semantra.egg-info/
--rw-r--r--   0 freedmand   (501) staff       (20)    10618 2023-04-27 04:42:35.000000 semantra-0.1.5/src/semantra.egg-info/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)     1018 2023-04-27 04:42:35.000000 semantra-0.1.5/src/semantra.egg-info/SOURCES.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-27 04:42:35.000000 semantra-0.1.5/src/semantra.egg-info/dependency_links.txt
--rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-04-27 04:42:35.000000 semantra-0.1.5/src/semantra.egg-info/entry_points.txt
--rw-r--r--   0 freedmand   (501) staff       (20)      176 2023-04-27 04:42:35.000000 semantra-0.1.5/src/semantra.egg-info/requires.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-27 04:42:35.000000 semantra-0.1.5/src/semantra.egg-info/top_level.txt
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.553142 semantra-0.1.6/
+-rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.1.6/LICENSE
+-rw-r--r--   0 freedmand   (501) staff       (20)    10690 2023-04-29 15:53:21.550984 semantra-0.1.6/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)    10147 2023-04-29 15:53:11.000000 semantra-0.1.6/README.md
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.529888 semantra-0.1.6/client/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.531758 semantra-0.1.6/client/public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.534017 semantra-0.1.6/client/public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-04-29 13:52:26.000000 semantra-0.1.6/client/public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449103 2023-04-29 13:52:26.000000 semantra-0.1.6/client/public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495745 2023-04-29 13:52:26.000000 semantra-0.1.6/client/public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.6/client/public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.6/client/public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-29 13:52:21.000000 semantra-0.1.6/client/public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)     1020 2023-04-29 15:53:11.000000 semantra-0.1.6/pyproject.toml
+-rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-29 15:53:21.553207 semantra-0.1.6/setup.cfg
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.530149 semantra-0.1.6/src/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.539080 semantra-0.1.6/src/semantra/
+-rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.1.6/src/semantra/__init__.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.542379 semantra-0.1.6/src/semantra/__pycache__/
+-rw-r--r--   0 freedmand   (501) staff       (20)      148 2023-04-23 04:39:41.000000 semantra-0.1.6/src/semantra/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)    10961 2023-04-23 04:37:57.000000 semantra-0.1.6/src/semantra/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)     3086 2023-04-23 04:37:58.000000 semantra-0.1.6/src/semantra/__pycache__/pdf.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)    19561 2023-04-23 12:15:19.000000 semantra-0.1.6/src/semantra/__pycache__/semantra.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)     4744 2023-04-23 04:37:58.000000 semantra-0.1.6/src/semantra/__pycache__/util.cpython-39.pyc
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.543121 semantra-0.1.6/src/semantra/client_public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.546116 semantra-0.1.6/src/semantra/client_public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-04-29 13:52:26.000000 semantra-0.1.6/src/semantra/client_public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449103 2023-04-29 13:52:26.000000 semantra-0.1.6/src/semantra/client_public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495745 2023-04-29 13:52:26.000000 semantra-0.1.6/src/semantra/client_public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.6/src/semantra/client_public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.6/src/semantra/client_public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-29 13:52:21.000000 semantra-0.1.6/src/semantra/client_public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)    11501 2023-04-29 13:52:21.000000 semantra-0.1.6/src/semantra/models.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     3325 2023-04-29 13:52:21.000000 semantra-0.1.6/src/semantra/pdf.py
+-rw-r--r--   0 freedmand   (501) staff       (20)    29168 2023-04-29 15:53:11.000000 semantra-0.1.6/src/semantra/semantra.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-04-29 13:52:21.000000 semantra-0.1.6/src/semantra/util.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-29 15:53:21.540312 semantra-0.1.6/src/semantra.egg-info/
+-rw-r--r--   0 freedmand   (501) staff       (20)    10690 2023-04-29 15:53:21.000000 semantra-0.1.6/src/semantra.egg-info/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)     1018 2023-04-29 15:53:21.000000 semantra-0.1.6/src/semantra.egg-info/SOURCES.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-29 15:53:21.000000 semantra-0.1.6/src/semantra.egg-info/dependency_links.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-04-29 15:53:21.000000 semantra-0.1.6/src/semantra.egg-info/entry_points.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)      176 2023-04-29 15:53:21.000000 semantra-0.1.6/src/semantra.egg-info/requires.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-29 15:53:21.000000 semantra-0.1.6/src/semantra.egg-info/top_level.txt
```

### Comparing `semantra-0.1.5/LICENSE` & `semantra-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/PKG-INFO` & `semantra-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.1.5
+Version: 0.1.6
 Summary: A semantic search CLI tool
 Author-email: Dylan Freedman <freedmand@gmail.com>
 Project-URL: Homepage, https://github.com/freedmand/semantra
 Project-URL: Repository, https://github.com/freedmand/semantra
 Project-URL: Bug Tracker, https://github.com/freedmand/semantra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -119,14 +119,15 @@
 ```
 
 ## Options
 
 - `--model [openai|minilm|mpnet|sgpt|sgpt-1.3B]`: Preset model to use for embedding. See [the models guide](docs/guide_models.md) for more info (default: mpnet)
 - `--transformer-model TEXT`: Custom Huggingface transformers model name to use for embedding (only one of `--model` and `--transformer-model` should be specified). See [the models guide](docs/guide_models.md) for more info
 - `--windows TEXT`: Embedding windows to extract. A comma-separated list of the format "size[\_offset=0][_rewind=0]. A window with size 128, offset 0, and rewind of 16 (128_0_16) will embed the document in chunks of 128 tokens which partially overlap by 16. Only the first window is used for search. See the [windows concept doc](docs/concept_windows.md) for more information (default: 128_0_16)
+- `--encoding`: Encoding to use for reading text files [default: utf-8]
 - `--no-server`: Do not start the UI server (only process)
 - `--port INTEGER`: Port to use for embedding server (default: 8080)
 - `--host TEXT`: Host to use for embedding server (default: 0.0.0.0)
 - `--pool-size INTEGER`: Max number of embedding tokens to pool together in requests
 - `--pool-count INTEGER`: Max number of embeddings to pool together in requests
 - `--doc-token-pre TEXT`: Token to prepend to each document in transformer models (default: None)
 - `--doc-token-post TEXT`: Token to append to each document in transformer models (default: None)
```

### Comparing `semantra-0.1.5/README.md` & `semantra-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 ```
 
 ## Options
 
 - `--model [openai|minilm|mpnet|sgpt|sgpt-1.3B]`: Preset model to use for embedding. See [the models guide](docs/guide_models.md) for more info (default: mpnet)
 - `--transformer-model TEXT`: Custom Huggingface transformers model name to use for embedding (only one of `--model` and `--transformer-model` should be specified). See [the models guide](docs/guide_models.md) for more info
 - `--windows TEXT`: Embedding windows to extract. A comma-separated list of the format "size[\_offset=0][_rewind=0]. A window with size 128, offset 0, and rewind of 16 (128_0_16) will embed the document in chunks of 128 tokens which partially overlap by 16. Only the first window is used for search. See the [windows concept doc](docs/concept_windows.md) for more information (default: 128_0_16)
+- `--encoding`: Encoding to use for reading text files [default: utf-8]
 - `--no-server`: Do not start the UI server (only process)
 - `--port INTEGER`: Port to use for embedding server (default: 8080)
 - `--host TEXT`: Host to use for embedding server (default: 0.0.0.0)
 - `--pool-size INTEGER`: Max number of embedding tokens to pool together in requests
 - `--pool-count INTEGER`: Max number of embeddings to pool together in requests
 - `--doc-token-pre TEXT`: Token to prepend to each document in transformer models (default: None)
 - `--doc-token-post TEXT`: Token to append to each document in transformer models (default: None)
```

### Comparing `semantra-0.1.5/client/public/build/bundle.css` & `semantra-0.1.6/client/public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/client/public/build/bundle.js` & `semantra-0.1.6/client/public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/client/public/build/bundle.js.map` & `semantra-0.1.6/client/public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/client/public/favicon.png` & `semantra-0.1.6/client/public/favicon.png`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/client/public/global.css` & `semantra-0.1.6/client/public/global.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/pyproject.toml` & `semantra-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "semantra"
-version = "0.1.5"
+version = "0.1.6"
 description = "A semantic search CLI tool"
 authors = [{name = "Dylan Freedman", email = "freedmand@gmail.com"}]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `semantra-0.1.5/src/semantra/__pycache__/models.cpython-39.pyc` & `semantra-0.1.6/src/semantra/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/src/semantra/__pycache__/pdf.cpython-39.pyc` & `semantra-0.1.6/src/semantra/__pycache__/pdf.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/src/semantra/__pycache__/semantra.cpython-39.pyc` & `semantra-0.1.6/src/semantra/__pycache__/semantra.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/src/semantra/__pycache__/util.cpython-39.pyc` & `semantra-0.1.6/src/semantra/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/src/semantra/client_public/build/bundle.css` & `semantra-0.1.6/src/semantra/client_public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/src/semantra/client_public/build/bundle.js` & `semantra-0.1.6/src/semantra/client_public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/src/semantra/client_public/build/bundle.js.map` & `semantra-0.1.6/src/semantra/client_public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/src/semantra/client_public/favicon.png` & `semantra-0.1.6/src/semantra/client_public/favicon.png`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/src/semantra/client_public/global.css` & `semantra-0.1.6/src/semantra/client_public/global.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/src/semantra/models.py` & `semantra-0.1.6/src/semantra/models.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/src/semantra/pdf.py` & `semantra-0.1.6/src/semantra/pdf.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/src/semantra/semantra.py` & `semantra-0.1.6/src/semantra/semantra.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,30 +25,31 @@
     load_annoy_db,
     sort_results,
     HASH_LENGTH,
 )
 import pkg_resources
 
 VERSION = pkg_resources.require("semantra")[0].version
+DEFAULT_ENCODING = "utf-8"
 
 package_directory = os.path.dirname(os.path.abspath(__file__))
 
 
 class Content:
     def __init__(self, rawtext, filename):
         self.rawtext = rawtext
         self.filename = filename
         self.filetype = "text"
 
 
-def get_text_content(md5, filename, semantra_dir, force, silent):
+def get_text_content(md5, filename, semantra_dir, force, silent, encoding):
     if filename.endswith(".pdf"):
         return get_pdf_content(md5, filename, semantra_dir, force, silent)
 
-    with open(filename, "r", encoding="utf-8", errors="ignore") as f:
+    with open(filename, "r", encoding=encoding, errors="ignore") as f:
         rawtext = f.read()
         return Content(rawtext, filename)
 
 
 TRANSFORMER_POOL_DEFAULT = 15000
 
 
@@ -63,31 +64,35 @@
         embeddings_filenames,
         use_annoy,
         annoy_filenames,
         windows,
         offsets,
         tokens_filename,
         num_dimensions,
+        encoding,
     ):
         self.filename = filename
         self.md5 = md5
         self.semantra_dir = semantra_dir
         self.base_filename = base_filename
         self.config = config
         self.embeddings_filenames = embeddings_filenames
         self.use_annoy = use_annoy
         self.annoy_filenames = annoy_filenames
         self.windows = windows
         self.offsets = offsets
         self.tokens_filename = tokens_filename
         self.num_dimensions = num_dimensions
+        self.encoding = encoding
 
     @property
     def content(self):
-        return get_text_content(self.md5, self.filename, self.semantra_dir, False, True)
+        return get_text_content(
+            self.md5, self.filename, self.semantra_dir, False, True, self.encoding
+        )
 
     @property
     def text_chunks(self):
         with open(self.tokens_filename, "r") as f:
             return json.loads(f.read())
 
     @property
@@ -121,33 +126,36 @@
     windows,
     cost_per_token,
     pool_count,
     pool_size,
     force,
     silent,
     no_confirm,
+    encoding,
 ):
     # Check if semantra dir exists
     if not os.path.exists(semantra_dir):
         os.makedirs(semantra_dir)
 
     # Get the md5 and config
     md5 = file_md5(filename)
     base_filename = os.path.basename(filename)
     config = model.get_config()
+    if encoding != DEFAULT_ENCODING:
+        config["encoding"] = encoding
     config_hash = hashlib.shake_256(json.dumps(config).encode()).hexdigest(HASH_LENGTH)
 
     # File names
     tokens_filename = os.path.join(semantra_dir, get_tokens_filename(md5, config_hash))
     config_filename = os.path.join(semantra_dir, get_config_filename(md5, config_hash))
 
     should_calculate_tokens = True
     if force or not os.path.exists(tokens_filename):
         # Calculate tokens to get text chunks
-        content = get_text_content(md5, filename, semantra_dir, force, silent)
+        content = get_text_content(md5, filename, semantra_dir, force, silent, encoding)
         text = content.rawtext
         tokens = model.get_tokens(text)
         should_calculate_tokens = False
         text_chunks = model.get_text_chunks(text, tokens)
         with open(tokens_filename, "w") as f:
             f.write(json.dumps(text_chunks))
     else:
@@ -312,14 +320,15 @@
         embeddings_filenames=embeddings_filenames,
         use_annoy=use_annoy,
         annoy_filenames=annoy_filenames,
         windows=windows,
         offsets=offsets,
         tokens_filename=tokens_filename,
         num_dimensions=num_dimensions,
+        encoding=encoding,
     )
 
 
 def process_windows(windows: str) -> "list[tuple[int, int, int]]":
     for window in windows.split(","):
         if "_" in window:
             # One or two occurrences?
@@ -339,14 +348,21 @@
     "--model",
     type=click.Choice(models.keys(), case_sensitive=True),
     default="mpnet",
     show_default=True,
     help="Preset model to use for embedding",
 )
 @click.option(
+    "--encoding",
+    type=str,
+    default=DEFAULT_ENCODING,
+    show_default=True,
+    help="Encoding to use for reading text files",
+)
+@click.option(
     "--transformer-model",
     type=str,
     help="Custom Huggingface transformers model name to use for embedding",
 )
 @click.option(
     "--windows",
     type=str,
@@ -516,14 +532,15 @@
     pool_count=None,
     doc_token_pre=None,
     doc_token_post=None,
     query_token_pre=None,
     query_token_post=None,
     model="mpnet",
     transformer_model=None,
+    encoding=DEFAULT_ENCODING,
     num_annoy_trees=100,
     num_results=10,
     annoy=True,
     svm=False,
     svm_c=1.0,
     explain_split_count=9,
     explain_split_divide=6,
@@ -601,14 +618,15 @@
             windows=processed_windows,
             cost_per_token=cost_per_token,
             pool_count=pool_count,
             pool_size=pool_size,
             force=force,
             silent=silent,
             no_confirm=no_confirm,
+            encoding=encoding,
         )
 
     cached_content = None
     cached_content_filename = None
 
     def get_content(filename):
         nonlocal cached_content, cached_content_filename
```

### Comparing `semantra-0.1.5/src/semantra/util.py` & `semantra-0.1.6/src/semantra/util.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.5/src/semantra.egg-info/PKG-INFO` & `semantra-0.1.6/src/semantra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.1.5
+Version: 0.1.6
 Summary: A semantic search CLI tool
 Author-email: Dylan Freedman <freedmand@gmail.com>
 Project-URL: Homepage, https://github.com/freedmand/semantra
 Project-URL: Repository, https://github.com/freedmand/semantra
 Project-URL: Bug Tracker, https://github.com/freedmand/semantra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -119,14 +119,15 @@
 ```
 
 ## Options
 
 - `--model [openai|minilm|mpnet|sgpt|sgpt-1.3B]`: Preset model to use for embedding. See [the models guide](docs/guide_models.md) for more info (default: mpnet)
 - `--transformer-model TEXT`: Custom Huggingface transformers model name to use for embedding (only one of `--model` and `--transformer-model` should be specified). See [the models guide](docs/guide_models.md) for more info
 - `--windows TEXT`: Embedding windows to extract. A comma-separated list of the format "size[\_offset=0][_rewind=0]. A window with size 128, offset 0, and rewind of 16 (128_0_16) will embed the document in chunks of 128 tokens which partially overlap by 16. Only the first window is used for search. See the [windows concept doc](docs/concept_windows.md) for more information (default: 128_0_16)
+- `--encoding`: Encoding to use for reading text files [default: utf-8]
 - `--no-server`: Do not start the UI server (only process)
 - `--port INTEGER`: Port to use for embedding server (default: 8080)
 - `--host TEXT`: Host to use for embedding server (default: 0.0.0.0)
 - `--pool-size INTEGER`: Max number of embedding tokens to pool together in requests
 - `--pool-count INTEGER`: Max number of embeddings to pool together in requests
 - `--doc-token-pre TEXT`: Token to prepend to each document in transformer models (default: None)
 - `--doc-token-post TEXT`: Token to append to each document in transformer models (default: None)
```

### Comparing `semantra-0.1.5/src/semantra.egg-info/SOURCES.txt` & `semantra-0.1.6/src/semantra.egg-info/SOURCES.txt`

 * *Files identical despite different names*


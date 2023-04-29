# Comparing `tmp/cdktf-surreal-backend-1.0.93.tar.gz` & `tmp/cdktf-surreal-backend-1.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-surreal-backend-1.0.93.tar", last modified: Fri Apr 28 00:19:35 2023, max compression
+gzip compressed data, was "cdktf-surreal-backend-1.0.94.tar", last modified: Sat Apr 29 00:18:36 2023, max compression
```

## Comparing `cdktf-surreal-backend-1.0.93.tar` & `cdktf-surreal-backend-1.0.94.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:19:35.388793 cdktf-surreal-backend-1.0.93/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-28 00:19:23.000000 cdktf-surreal-backend-1.0.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 00:19:23.000000 cdktf-surreal-backend-1.0.93/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-28 00:19:35.384792 cdktf-surreal-backend-1.0.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-28 00:19:23.000000 cdktf-surreal-backend-1.0.93/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-28 00:19:23.000000 cdktf-surreal-backend-1.0.93/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:19:35.388793 cdktf-surreal-backend-1.0.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-28 00:19:23.000000 cdktf-surreal-backend-1.0.93/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:19:35.384792 cdktf-surreal-backend-1.0.93/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:19:35.384792 cdktf-surreal-backend-1.0.93/src/cdktf_surreal-backend/
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-28 00:19:23.000000 cdktf-surreal-backend-1.0.93/src/cdktf_surreal-backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:19:35.384792 cdktf-surreal-backend-1.0.93/src/cdktf_surreal-backend/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-28 00:19:23.000000 cdktf-surreal-backend-1.0.93/src/cdktf_surreal-backend/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-04-28 00:19:23.000000 cdktf-surreal-backend-1.0.93/src/cdktf_surreal-backend/_jsii/cdktf-surreal-backend@1.0.93.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:19:23.000000 cdktf-surreal-backend-1.0.93/src/cdktf_surreal-backend/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:19:35.384792 cdktf-surreal-backend-1.0.93/src/cdktf_surreal_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-28 00:19:35.000000 cdktf-surreal-backend-1.0.93/src/cdktf_surreal_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-28 00:19:35.000000 cdktf-surreal-backend-1.0.93/src/cdktf_surreal_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:19:35.000000 cdktf-surreal-backend-1.0.93/src/cdktf_surreal_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-28 00:19:35.000000 cdktf-surreal-backend-1.0.93/src/cdktf_surreal_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 00:19:35.000000 cdktf-surreal-backend-1.0.93/src/cdktf_surreal_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:18:36.708625 cdktf-surreal-backend-1.0.94/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-29 00:18:22.000000 cdktf-surreal-backend-1.0.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-29 00:18:22.000000 cdktf-surreal-backend-1.0.94/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-29 00:18:36.708625 cdktf-surreal-backend-1.0.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-29 00:18:22.000000 cdktf-surreal-backend-1.0.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-29 00:18:22.000000 cdktf-surreal-backend-1.0.94/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 00:18:36.708625 cdktf-surreal-backend-1.0.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-29 00:18:22.000000 cdktf-surreal-backend-1.0.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:18:36.708625 cdktf-surreal-backend-1.0.94/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:18:36.708625 cdktf-surreal-backend-1.0.94/src/cdktf_surreal-backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-29 00:18:22.000000 cdktf-surreal-backend-1.0.94/src/cdktf_surreal-backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:18:36.708625 cdktf-surreal-backend-1.0.94/src/cdktf_surreal-backend/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-29 00:18:22.000000 cdktf-surreal-backend-1.0.94/src/cdktf_surreal-backend/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-04-29 00:18:22.000000 cdktf-surreal-backend-1.0.94/src/cdktf_surreal-backend/_jsii/cdktf-surreal-backend@1.0.94.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:18:22.000000 cdktf-surreal-backend-1.0.94/src/cdktf_surreal-backend/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:18:36.708625 cdktf-surreal-backend-1.0.94/src/cdktf_surreal_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-29 00:18:36.000000 cdktf-surreal-backend-1.0.94/src/cdktf_surreal_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-29 00:18:36.000000 cdktf-surreal-backend-1.0.94/src/cdktf_surreal_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:18:36.000000 cdktf-surreal-backend-1.0.94/src/cdktf_surreal_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-29 00:18:36.000000 cdktf-surreal-backend-1.0.94/src/cdktf_surreal_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 00:18:36.000000 cdktf-surreal-backend-1.0.94/src/cdktf_surreal_backend.egg-info/top_level.txt
```

### Comparing `cdktf-surreal-backend-1.0.93/LICENSE` & `cdktf-surreal-backend-1.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-surreal-backend-1.0.93/PKG-INFO` & `cdktf-surreal-backend-1.0.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-surreal-backend
-Version: 1.0.93
+Version: 1.0.94
 Summary: A package that vends a construct to setup the surreal backend in CDKTF
 Home-page: https://github.com/awlsring/cdktf-surreal-backend.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-surreal-backend.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-surreal-backend-1.0.93/README.md` & `cdktf-surreal-backend-1.0.94/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-surreal-backend-1.0.93/setup.py` & `cdktf-surreal-backend-1.0.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-surreal-backend",
-    "version": "1.0.93",
+    "version": "1.0.94",
     "description": "A package that vends a construct to setup the surreal backend in CDKTF",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdktf-surreal-backend.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdktf_surreal-backend",
         "cdktf_surreal-backend._jsii"
     ],
     "package_data": {
         "cdktf_surreal-backend._jsii": [
-            "cdktf-surreal-backend@1.0.93.jsii.tgz"
+            "cdktf-surreal-backend@1.0.94.jsii.tgz"
         ],
         "cdktf_surreal-backend": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-surreal-backend-1.0.93/src/cdktf_surreal-backend/__init__.py` & `cdktf-surreal-backend-1.0.94/src/cdktf_surreal-backend/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-surreal-backend-1.0.93/src/cdktf_surreal_backend.egg-info/PKG-INFO` & `cdktf-surreal-backend-1.0.94/src/cdktf_surreal_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-surreal-backend
-Version: 1.0.93
+Version: 1.0.94
 Summary: A package that vends a construct to setup the surreal backend in CDKTF
 Home-page: https://github.com/awlsring/cdktf-surreal-backend.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-surreal-backend.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```


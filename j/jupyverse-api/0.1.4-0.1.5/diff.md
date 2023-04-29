# Comparing `tmp/jupyverse_api-0.1.4.tar.gz` & `tmp/jupyverse_api-0.1.5.tar.gz`

## Comparing `jupyverse_api-0.1.4.tar` & `jupyverse_api-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/cli.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/py.typed
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/README.md
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/retrolab/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/README.md
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 jupyverse_api-0.1.5/PKG-INFO
```

### Comparing `jupyverse_api-0.1.4/jupyverse_api/__init__.py` & `jupyverse_api-0.1.5/jupyverse_api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 
 from pydantic import BaseModel, Extra
 
 from .app import App
 
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
```

### Comparing `jupyverse_api-0.1.4/jupyverse_api/cli.py` & `jupyverse_api-0.1.5/jupyverse_api/cli.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/jupyverse_api/app/__init__.py` & `jupyverse_api-0.1.5/jupyverse_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/jupyverse_api/auth/__init__.py` & `jupyverse_api-0.1.5/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/jupyverse_api/contents/__init__.py` & `jupyverse_api-0.1.5/jupyverse_api/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/jupyverse_api/contents/models.py` & `jupyverse_api-0.1.5/jupyverse_api/contents/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/jupyverse_api/jupyterlab/__init__.py` & `jupyverse_api-0.1.5/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/jupyverse_api/kernels/__init__.py` & `jupyverse_api-0.1.5/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/jupyverse_api/kernels/models.py` & `jupyverse_api-0.1.5/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/jupyverse_api/lab/__init__.py` & `jupyverse_api-0.1.5/jupyverse_api/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/jupyverse_api/main/__init__.py` & `jupyverse_api-0.1.5/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/jupyverse_api/nbconvert/__init__.py` & `jupyverse_api-0.1.5/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/jupyverse_api/resource_usage/__init__.py` & `jupyverse_api-0.1.5/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/jupyverse_api/retrolab/__init__.py` & `jupyverse_api-0.1.5/jupyverse_api/retrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/jupyverse_api/terminals/__init__.py` & `jupyverse_api-0.1.5/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/jupyverse_api/yjs/__init__.py` & `jupyverse_api-0.1.5/jupyverse_api/yjs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/.gitignore` & `jupyverse_api-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/COPYING.md` & `jupyverse_api-0.1.5/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/pyproject.toml` & `jupyverse_api-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.4/PKG-INFO` & `jupyverse_api-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyverse_api
-Version: 0.1.4
+Version: 0.1.5
 Summary: The public API for Jupyverse
 Project-URL: Source, https://github.com/jupyter-server/jupyverse/jupyverse_api
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: api,jupyverse
 Classifier: Development Status :: 4 - Beta
```


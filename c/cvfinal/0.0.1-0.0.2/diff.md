# Comparing `tmp/cvfinal-0.0.1.tar.gz` & `tmp/cvfinal-0.0.2.tar.gz`

## Comparing `cvfinal-0.0.1.tar` & `cvfinal-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cvfinal-0.0.1/src/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 cvfinal-0.0.1/src/aaa.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 cvfinal-0.0.1/src/cvfinal.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cvfinal-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 cvfinal-0.0.1/README.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 cvfinal-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 cvfinal-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 cvfinal-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cvfinal-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 cvfinal-0.0.2/src/aaa.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 cvfinal-0.0.2/src/cvfinal.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cvfinal-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 cvfinal-0.0.2/README.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 cvfinal-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 cvfinal-0.0.2/PKG-INFO
```

### Comparing `cvfinal-0.0.1/src/cvfinal.py` & `cvfinal-0.0.2/src/cvfinal.py`

 * *Files identical despite different names*

### Comparing `cvfinal-0.0.1/LICENSE.txt` & `cvfinal-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvfinal-0.0.1/pyproject.toml` & `cvfinal-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cvfinal"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="7017_1", email="nsysu.ee.7017.1@gamil.com" },
 ]
 description = "A final project package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```


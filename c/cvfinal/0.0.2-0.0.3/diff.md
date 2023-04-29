# Comparing `tmp/cvfinal-0.0.2.tar.gz` & `tmp/cvfinal-0.0.3.tar.gz`

## Comparing `cvfinal-0.0.2.tar` & `cvfinal-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 cvfinal-0.0.2/PKG-INFO
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cvfinal-0.0.2/src/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 cvfinal-0.0.2/src/aaa.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 cvfinal-0.0.2/src/cvfinal.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cvfinal-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 cvfinal-0.0.2/README.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 cvfinal-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 cvfinal-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 cvfinal-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cvfinal-0.0.3/src/cvfinal/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 cvfinal-0.0.3/src/cvfinal/aaa.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 cvfinal-0.0.3/src/cvfinal/cvfinal.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cvfinal-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 cvfinal-0.0.3/README.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 cvfinal-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 cvfinal-0.0.3/PKG-INFO
```

### Comparing `cvfinal-0.0.2/src/cvfinal.py` & `cvfinal-0.0.3/src/cvfinal/cvfinal.py`

 * *Files identical despite different names*

### Comparing `cvfinal-0.0.2/LICENSE.txt` & `cvfinal-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvfinal-0.0.2/pyproject.toml` & `cvfinal-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cvfinal"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="7017_1", email="nsysu.ee.7017.1@gamil.com" },
 ]
 description = "A final project package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```


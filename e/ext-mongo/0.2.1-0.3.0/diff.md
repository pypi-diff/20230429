# Comparing `tmp/ext-mongo-0.2.1.tar.gz` & `tmp/ext-mongo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ext-mongo-0.2.1.tar", last modified: Sat Apr 29 12:46:13 2023, max compression
+gzip compressed data, was "ext-mongo-0.3.0.tar", last modified: Sat Apr 29 17:26:34 2023, max compression
```

## Comparing `ext-mongo-0.2.1.tar` & `ext-mongo-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      395 2023-04-29 12:07:25.855827 ext-mongo-0.2.1/mongo/__init__.py
--rw-r--r--   0        0        0      453 2023-04-29 10:30:44.699476 ext-mongo-0.2.1/mongo/connect.py
--rw-r--r--   0        0        0       60 2023-04-29 10:01:06.786503 ext-mongo-0.2.1/mongo/deps.py
--rw-r--r--   0        0        0      795 2023-04-29 12:25:07.701795 ext-mongo-0.2.1/mongo/document.py
--rw-r--r--   0        0        0     1557 2023-04-29 12:41:58.626422 ext-mongo-0.2.1/mongo/document_meta.py
--rw-r--r--   0        0        0      613 2023-04-29 12:46:07.877362 ext-mongo-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1091 2023-04-29 12:44:30.408958 ext-mongo-0.2.1/README.md
--rw-r--r--   0        0        0      874 2023-04-29 12:42:46.025658 ext-mongo-0.2.1/tests/__main__.py
--rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 ext-mongo-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      395 2023-04-29 12:07:25.855827 ext-mongo-0.3.0/mongo/__init__.py
+-rw-r--r--   0        0        0      453 2023-04-29 10:30:44.699476 ext-mongo-0.3.0/mongo/connect.py
+-rw-r--r--   0        0        0       60 2023-04-29 10:01:06.786503 ext-mongo-0.3.0/mongo/deps.py
+-rw-r--r--   0        0        0      795 2023-04-29 12:25:07.701795 ext-mongo-0.3.0/mongo/document.py
+-rw-r--r--   0        0        0     1557 2023-04-29 12:41:58.626422 ext-mongo-0.3.0/mongo/document_meta.py
+-rw-r--r--   0        0        0      541 2023-04-29 17:26:19.862938 ext-mongo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1091 2023-04-29 12:44:30.408958 ext-mongo-0.3.0/README.md
+-rw-r--r--   0        0        0      874 2023-04-29 12:42:46.025658 ext-mongo-0.3.0/tests/__main__.py
+-rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 ext-mongo-0.3.0/PKG-INFO
```

### Comparing `ext-mongo-0.2.1/mongo/document.py` & `ext-mongo-0.3.0/mongo/document.py`

 * *Files identical despite different names*

### Comparing `ext-mongo-0.2.1/mongo/document_meta.py` & `ext-mongo-0.3.0/mongo/document_meta.py`

 * *Files identical despite different names*

### Comparing `ext-mongo-0.2.1/pyproject.toml` & `ext-mongo-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ext-mongo"
-version = "0.2.1"
+version = "0.3.0"
 description = "Extended mongoengine"
 authors = [
     { name = "levch", email = "levchenko.d.a1998@gmail.com" },
 ]
 dependencies = [
     "mongoengine>=0.27.0",
     "parsenv>=0.1.4",
@@ -21,17 +21,13 @@
 ]
 build-backend = "pdm.pep517.api"
 
 [tool.pdm.scripts]
 black = "black . -q"
 ruff = "ruff ."
 test = "python tests"
-test2 = "python tests/test2.py"
-
-[tool.pdm.scripts._]
-env_file = ".env"
 
 [tool.pdm.scripts.lint]
 composite = [
     "black",
     "ruff",
 ]
```

### Comparing `ext-mongo-0.2.1/README.md` & `ext-mongo-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ext-mongo-0.2.1/tests/__main__.py` & `ext-mongo-0.3.0/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `ext-mongo-0.2.1/PKG-INFO` & `ext-mongo-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ext-mongo
-Version: 0.2.1
+Version: 0.3.0
 Summary: Extended mongoengine
 License: MIT
 Author-email: levch <levchenko.d.a1998@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ### Depends on environment variables:
```


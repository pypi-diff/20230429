# Comparing `tmp/starter_py-0.0.3.tar.gz` & `tmp/starter_py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starter_py-0.0.3.tar", max compression
+gzip compressed data, was "starter_py-0.0.4.tar", max compression
```

## Comparing `starter_py-0.0.3.tar` & `starter_py-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1061 2023-04-29 15:13:14.072620 starter_py-0.0.3/LICENSE
--rw-r--r--   0        0        0      543 2023-04-29 15:13:14.072620 starter_py-0.0.3/README.md
--rw-r--r--   0        0        0      525 2023-04-29 15:13:14.072620 starter_py-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       20 2023-04-29 15:13:14.072620 starter_py-0.0.3/starter_py/__init__.py
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 starter_py-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-29 15:43:03.683197 starter_py-0.0.4/LICENSE
+-rw-r--r--   0        0        0      543 2023-04-29 15:43:03.683197 starter_py-0.0.4/README.md
+-rw-r--r--   0        0        0      750 2023-04-29 15:43:03.683197 starter_py-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-04-29 15:43:03.683197 starter_py-0.0.4/starter_py/__init__.py
+-rw-r--r--   0        0        0     1383 1970-01-01 00:00:00.000000 starter_py-0.0.4/PKG-INFO
```

### Comparing `starter_py-0.0.3/LICENSE` & `starter_py-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `starter_py-0.0.3/README.md` & `starter_py-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `starter_py-0.0.3/pyproject.toml` & `starter_py-0.0.4/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 [tool.poetry]
 name = "starter-py"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python3 Starter"
 readme = "README.md"
 authors = ["Dup4 <lyuzhi.pan@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Topic :: Software Development :: Build Tools",
-    "Topic :: Software Development :: Libraries :: Python Modules"
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
```


# Comparing `tmp/parsenv-0.2.0.tar.gz` & `tmp/parsenv-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsenv-0.2.0.tar", last modified: Sat Apr 29 17:08:36 2023, max compression
+gzip compressed data, was "parsenv-0.2.1.tar", last modified: Sat Apr 29 17:10:21 2023, max compression
```

## Comparing `parsenv-0.2.0.tar` & `parsenv-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      242 2023-04-29 16:54:02.050035 parsenv-0.2.0/env/__init__.py
--rw-r--r--   0        0        0      114 2023-04-29 16:54:02.080416 parsenv-0.2.0/env/core.py
--rw-r--r--   0        0        0     1379 2023-04-29 16:54:01.987250 parsenv-0.2.0/env/main.py
--rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 parsenv-0.2.0/env/py.typed
--rw-r--r--   0        0        0      451 2023-04-29 16:51:16.468378 parsenv-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      950 2023-04-29 17:07:52.520578 parsenv-0.2.0/README.md
--rw-r--r--   0        0        0      778 2023-04-29 16:55:03.344368 parsenv-0.2.0/tests/__main__.py
--rw-r--r--   0        0        0     1093 1970-01-01 00:00:00.000000 parsenv-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      242 2023-04-29 16:54:02.050035 parsenv-0.2.1/env/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-29 16:54:02.080416 parsenv-0.2.1/env/core.py
+-rw-r--r--   0        0        0     1379 2023-04-29 16:54:01.987250 parsenv-0.2.1/env/main.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 parsenv-0.2.1/env/py.typed
+-rw-r--r--   0        0        0      451 2023-04-29 17:10:16.739713 parsenv-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-04-29 17:10:16.708983 parsenv-0.2.1/README.md
+-rw-r--r--   0        0        0      778 2023-04-29 16:55:03.344368 parsenv-0.2.1/tests/__main__.py
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 parsenv-0.2.1/PKG-INFO
```

### Comparing `parsenv-0.2.0/env/main.py` & `parsenv-0.2.1/env/main.py`

 * *Files identical despite different names*

### Comparing `parsenv-0.2.0/README.md` & `parsenv-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### Getting Started
 
-Use `pip install parsenv`
+Use `pip install parsenv`.
 
-Reads `.env` file on import, then reads other env-files from `$ENVPATH` (comma separated)
+Reads `.env` file on import, then reads other env-files from `$ENVPATH` (comma separated).
 
 ### Example
 
 ```py
 import env
 
 assert env.get("TOKEN") == "abc123"
```

### Comparing `parsenv-0.2.0/tests/__main__.py` & `parsenv-0.2.1/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `parsenv-0.2.0/PKG-INFO` & `parsenv-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: parsenv
-Version: 0.2.0
+Version: 0.2.1
 License: MIT
 Author-email: levch <levchenko.d.a1998@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ### Getting Started
 
-Use `pip install parsenv`
+Use `pip install parsenv`.
 
-Reads `.env` file on import, then reads other env-files from `$ENVPATH` (comma separated)
+Reads `.env` file on import, then reads other env-files from `$ENVPATH` (comma separated).
 
 ### Example
 
 ```py
 import env
 
 assert env.get("TOKEN") == "abc123"
```


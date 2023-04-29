# Comparing `tmp/fastapi_sql-0.1.6.tar.gz` & `tmp/fastapi_sql-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sql-0.1.6.tar", max compression
+gzip compressed data, was "fastapi_sql-0.2.0.tar", max compression
```

## Comparing `fastapi_sql-0.1.6.tar` & `fastapi_sql-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2651 2023-04-27 19:49:11.547995 fastapi_sql-0.1.6/fastapi_sql/__init__.py
--rw-r--r--   0        0        0      366 2023-04-27 19:45:25.220252 fastapi_sql-0.1.6/fastapi_sql/middleware.py
--rw-r--r--   0        0        0      933 2023-04-26 16:52:03.910855 fastapi_sql-0.1.6/fastapi_sql/migrate.py
--rw-r--r--   0        0        0     5135 2023-04-27 18:51:50.354029 fastapi_sql-0.1.6/fastapi_sql/model.py
--rw-r--r--   0        0        0      359 2023-04-27 19:49:43.701276 fastapi_sql-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 fastapi_sql-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2651 2023-04-28 14:00:06.315737 fastapi_sql-0.2.0/fastapi_sql/__init__.py
+-rw-r--r--   0        0        0      799 2023-04-28 14:16:59.302509 fastapi_sql-0.2.0/fastapi_sql/middleware.py
+-rw-r--r--   0        0        0      933 2023-04-26 16:52:03.910855 fastapi_sql-0.2.0/fastapi_sql/migrate.py
+-rw-r--r--   0        0        0     5135 2023-04-27 18:51:50.354029 fastapi_sql-0.2.0/fastapi_sql/model.py
+-rw-r--r--   0        0        0      417 2023-04-28 14:17:59.800160 fastapi_sql-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 fastapi_sql-0.2.0/PKG-INFO
```

### Comparing `fastapi_sql-0.1.6/fastapi_sql/__init__.py` & `fastapi_sql-0.2.0/fastapi_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.1.6/fastapi_sql/migrate.py` & `fastapi_sql-0.2.0/fastapi_sql/migrate.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.1.6/fastapi_sql/model.py` & `fastapi_sql-0.2.0/fastapi_sql/model.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.1.6/PKG-INFO` & `fastapi_sql-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sql
-Version: 0.1.6
+Version: 0.2.0
 Summary: 
 Author: Michael Piccirillo
 Author-email: 70709374+Khrysys@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```


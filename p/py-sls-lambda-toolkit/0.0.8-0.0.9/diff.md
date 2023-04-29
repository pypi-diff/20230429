# Comparing `tmp/py-sls-lambda-toolkit-0.0.8.tar.gz` & `tmp/py-sls-lambda-toolkit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-sls-lambda-toolkit-0.0.8.tar", last modified: Fri Apr 28 15:03:43 2023, max compression
+gzip compressed data, was "py-sls-lambda-toolkit-0.0.9.tar", last modified: Sat Apr 29 04:23:14 2023, max compression
```

## Comparing `py-sls-lambda-toolkit-0.0.8.tar` & `py-sls-lambda-toolkit-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-28 15:03:43.604949 py-sls-lambda-toolkit-0.0.8/
--rw-rw-r--   0 julio     (1000) julio     (1000)     1069 2023-04-23 17:34:15.000000 py-sls-lambda-toolkit-0.0.8/LICENSE
--rw-rw-r--   0 julio     (1000) julio     (1000)       34 2023-04-23 18:05:48.000000 py-sls-lambda-toolkit-0.0.8/MANIFEST.in
--rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-04-28 15:03:43.604949 py-sls-lambda-toolkit-0.0.8/PKG-INFO
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-28 15:03:43.604949 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/
--rw-rw-r--   0 julio     (1000) julio     (1000)        0 2023-04-23 17:11:35.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/__init__.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1563 2023-04-28 03:49:17.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/crypto.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1370 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/dynamodb_shortcuts.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1651 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/http_event.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1222 2023-04-28 14:57:53.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/http_response.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      112 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/logger.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      646 2023-04-28 06:49:01.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/mappers.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      757 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/parsers.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     3086 2023-04-23 20:42:46.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/scan_filter_builder.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1255 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/status_code.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      863 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/validators.py
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-28 15:03:43.604949 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit.egg-info/
--rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-04-28 15:03:43.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 julio     (1000) julio     (1000)      669 2023-04-28 15:03:43.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-04-28 15:03:43.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       72 2023-04-28 15:03:43.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit.egg-info/requires.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       22 2023-04-28 15:03:43.000000 py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit.egg-info/top_level.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       94 2023-04-23 17:31:48.000000 py-sls-lambda-toolkit-0.0.8/pyproject.toml
--rw-rw-r--   0 julio     (1000) julio     (1000)      967 2023-04-28 15:03:43.604949 py-sls-lambda-toolkit-0.0.8/setup.cfg
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-29 04:23:14.501542 py-sls-lambda-toolkit-0.0.9/
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1069 2023-04-23 17:34:15.000000 py-sls-lambda-toolkit-0.0.9/LICENSE
+-rw-rw-r--   0 julio     (1000) julio     (1000)       34 2023-04-23 18:05:48.000000 py-sls-lambda-toolkit-0.0.9/MANIFEST.in
+-rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-04-29 04:23:14.501542 py-sls-lambda-toolkit-0.0.9/PKG-INFO
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-29 04:23:14.501542 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/
+-rw-rw-r--   0 julio     (1000) julio     (1000)        0 2023-04-23 17:11:35.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/__init__.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1563 2023-04-28 03:49:17.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/crypto.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1370 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/dynamodb_shortcuts.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1651 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/http_event.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1222 2023-04-28 14:57:53.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/http_response.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      112 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/logger.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      646 2023-04-28 06:49:01.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/mappers.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      757 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/parsers.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     3086 2023-04-23 20:42:46.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/scan_filter_builder.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1255 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/status_code.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      863 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/validators.py
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-04-29 04:23:14.501542 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit.egg-info/
+-rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-04-29 04:23:14.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 julio     (1000) julio     (1000)      669 2023-04-29 04:23:14.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-04-29 04:23:14.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       72 2023-04-29 04:23:14.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       22 2023-04-29 04:23:14.000000 py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       94 2023-04-23 17:31:48.000000 py-sls-lambda-toolkit-0.0.9/pyproject.toml
+-rw-rw-r--   0 julio     (1000) julio     (1000)      967 2023-04-29 04:23:14.501542 py-sls-lambda-toolkit-0.0.9/setup.cfg
```

### Comparing `py-sls-lambda-toolkit-0.0.8/LICENSE` & `py-sls-lambda-toolkit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.8/PKG-INFO` & `py-sls-lambda-toolkit-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sls-lambda-toolkit
-Version: 0.0.8
+Version: 0.0.9
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 Home-page: https://github.com/0riion/py-sls-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
 Keywords: aws,serverless,lambda,dynamodb,toolkit
 Classifier: Development Status :: 1 - Planning
```

### Comparing `py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/crypto.py` & `py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/crypto.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/dynamodb_shortcuts.py` & `py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/dynamodb_shortcuts.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/http_event.py` & `py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/http_event.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/http_response.py` & `py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/http_response.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/mappers.py` & `py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/mappers.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/parsers.py` & `py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/parsers.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/scan_filter_builder.py` & `py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/scan_filter_builder.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/status_code.py` & `py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/status_code.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit/validators.py` & `py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit/validators.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit.egg-info/PKG-INFO` & `py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sls-lambda-toolkit
-Version: 0.0.8
+Version: 0.0.9
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 Home-page: https://github.com/0riion/py-sls-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
 Keywords: aws,serverless,lambda,dynamodb,toolkit
 Classifier: Development Status :: 1 - Planning
```

### Comparing `py-sls-lambda-toolkit-0.0.8/py_sls_lambda_toolkit.egg-info/SOURCES.txt` & `py-sls-lambda-toolkit-0.0.9/py_sls_lambda_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.0.8/setup.cfg` & `py-sls-lambda-toolkit-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py-sls-lambda-toolkit
-version = 0.0.8
+version = 0.0.9
 author = Julio Flores
 author_email = juliocesarflores12@gmail.com
 author_url = juliofloresdev.com
 description = A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0riion/py-sls-lambda-toolkit
```


# Comparing `tmp/fil-0.1.0.tar.gz` & `tmp/fil-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fil-0.1.0.tar", max compression
+gzip compressed data, was "fil-0.2.0.tar", max compression
```

## Comparing `fil-0.1.0.tar` & `fil-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       52 2023-04-29 09:10:46.794486 fil-0.1.0/README.md
--rw-r--r--   0        0        0     2498 2023-04-29 10:47:03.088034 fil-0.1.0/fil.py
--rw-r--r--   0        0        0      487 2023-04-29 10:46:48.757906 fil-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 fil-0.1.0/setup.py
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 fil-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       52 2023-04-29 09:10:46.794486 fil-0.2.0/README.md
+-rw-r--r--   0        0        0     2780 2023-04-29 14:16:41.559561 fil-0.2.0/fil.py
+-rw-r--r--   0        0        0      504 2023-04-29 14:20:56.915796 fil-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 fil-0.2.0/setup.py
+-rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 fil-0.2.0/PKG-INFO
```

### Comparing `fil-0.1.0/setup.py` & `fil-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['fil']
+install_requires = \
+['safer>=4.5.0,<5.0.0']
+
 setup_kwargs = {
     'name': 'fil',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '🏺 Read/write JSON, TOML, ... files 🏺',
     'long_description': '# fil\n🏺 Read, write files (JSON, TOML, ...) 🏺\n',
     'author': 'Tom Ritchford',
     'author_email': 'tom@swirly.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'py_modules': modules,
+    'install_requires': install_requires,
     'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `fil-0.1.0/PKG-INFO` & `fil-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: fil
-Version: 0.1.0
+Version: 0.2.0
 Summary: 🏺 Read/write JSON, TOML, ... files 🏺
 License: MIT
 Author: Tom Ritchford
 Author-email: tom@swirly.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: safer (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # fil
 🏺 Read, write files (JSON, TOML, ...) 🏺
```


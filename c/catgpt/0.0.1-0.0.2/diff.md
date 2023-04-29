# Comparing `tmp/catgpt-0.0.1.tar.gz` & `tmp/catgpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catgpt-0.0.1.tar", max compression
+gzip compressed data, was "catgpt-0.0.2.tar", max compression
```

## Comparing `catgpt-0.0.1.tar` & `catgpt-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       45 2023-04-29 02:44:31.917850 catgpt-0.0.1/catgpt/__init__.py
--rw-r--r--   0        0        0     3362 2023-04-29 02:44:27.522118 catgpt-0.0.1/catgpt/model.py
--rw-r--r--   0        0        0      405 2023-04-29 02:48:53.793258 catgpt-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      685 2023-04-29 02:50:39.622697 catgpt-0.0.1/setup.py
--rw-r--r--   0        0        0      413 2023-04-29 02:50:39.623318 catgpt-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       45 2023-04-29 02:44:31.917850 catgpt-0.0.2/catgpt/__init__.py
+-rw-r--r--   0        0        0     3362 2023-04-29 02:44:27.522118 catgpt-0.0.2/catgpt/model.py
+-rw-r--r--   0        0        0      404 2023-04-29 02:52:36.690391 catgpt-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      684 2023-04-29 02:53:21.677480 catgpt-0.0.2/setup.py
+-rw-r--r--   0        0        0      512 2023-04-29 02:53:21.678281 catgpt-0.0.2/PKG-INFO
```

### Comparing `catgpt-0.0.1/catgpt/model.py` & `catgpt-0.0.2/catgpt/model.py`

 * *Files identical despite different names*

### Comparing `catgpt-0.0.1/setup.py` & `catgpt-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 install_requires = \
 ['codefast>=23.4.18,<24.0.0',
  'python-dotenv>=1.0.0,<2.0.0',
  'sseclient-py>=1.7.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'catgpt',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'A simple cli tool to generate text using GPT-turbo',
     'long_description': None,
     'author': 'tom',
     'author_email': 'tom@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```


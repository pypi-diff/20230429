# Comparing `tmp/api-hunter-cli-0.1.0.tar.gz` & `tmp/api-hunter-cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-hunter-cli-0.1.0.tar", last modified: Fri Apr 28 21:48:51 2023, max compression
+gzip compressed data, was "api-hunter-cli-0.1.1.tar", last modified: Fri Apr 28 22:09:36 2023, max compression
```

## Comparing `api-hunter-cli-0.1.0.tar` & `api-hunter-cli-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 21:48:51.808426 api-hunter-cli-0.1.0/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 21:48:51.808426 api-hunter-cli-0.1.0/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api-hunter-cli-0.1.0/README.md
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 21:48:51.808426 api-hunter-cli-0.1.0/api_hunter/
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api-hunter-cli-0.1.0/api_hunter/__init__.py
--rw-rw-r--   0 charly    (1000) charly    (1000)     4239 2023-04-28 04:53:55.000000 api-hunter-cli-0.1.0/api_hunter/main.py
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 21:48:51.808426 api-hunter-cli-0.1.0/api_hunter_cli.egg-info/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 21:48:51.000000 api-hunter-cli-0.1.0/api_hunter_cli.egg-info/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)      290 2023-04-28 21:48:51.000000 api-hunter-cli-0.1.0/api_hunter_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-28 21:48:51.000000 api-hunter-cli-0.1.0/api_hunter_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       49 2023-04-28 21:48:51.000000 api-hunter-cli-0.1.0/api_hunter_cli.egg-info/entry_points.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 21:48:51.000000 api-hunter-cli-0.1.0/api_hunter_cli.egg-info/requires.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       11 2023-04-28 21:48:51.000000 api-hunter-cli-0.1.0/api_hunter_cli.egg-info/top_level.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 21:48:51.808426 api-hunter-cli-0.1.0/setup.cfg
--rw-rw-r--   0 charly    (1000) charly    (1000)     1323 2023-04-28 21:48:49.000000 api-hunter-cli-0.1.0/setup.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:09:36.934436 api-hunter-cli-0.1.1/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 22:09:36.934436 api-hunter-cli-0.1.1/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api-hunter-cli-0.1.1/README.md
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:09:36.934436 api-hunter-cli-0.1.1/api_hunter/
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api-hunter-cli-0.1.1/api_hunter/__init__.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)     4239 2023-04-28 04:53:55.000000 api-hunter-cli-0.1.1/api_hunter/main.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:09:36.934436 api-hunter-cli-0.1.1/api_hunter_cli.egg-info/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 22:09:36.000000 api-hunter-cli-0.1.1/api_hunter_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)      290 2023-04-28 22:09:36.000000 api-hunter-cli-0.1.1/api_hunter_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-28 22:09:36.000000 api-hunter-cli-0.1.1/api_hunter_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       49 2023-04-28 22:09:36.000000 api-hunter-cli-0.1.1/api_hunter_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 22:09:36.000000 api-hunter-cli-0.1.1/api_hunter_cli.egg-info/requires.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       11 2023-04-28 22:09:36.000000 api-hunter-cli-0.1.1/api_hunter_cli.egg-info/top_level.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 22:09:36.934436 api-hunter-cli-0.1.1/setup.cfg
+-rw-rw-r--   0 charly    (1000) charly    (1000)     1323 2023-04-28 22:09:28.000000 api-hunter-cli-0.1.1/setup.py
```

### Comparing `api-hunter-cli-0.1.0/PKG-INFO` & `api-hunter-cli-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-hunter-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `api-hunter-cli-0.1.0/api_hunter/main.py` & `api-hunter-cli-0.1.1/api_hunter/main.py`

 * *Files identical despite different names*

### Comparing `api-hunter-cli-0.1.0/api_hunter_cli.egg-info/PKG-INFO` & `api-hunter-cli-0.1.1/api_hunter_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-hunter-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `api-hunter-cli-0.1.0/setup.py` & `api-hunter-cli-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def run(self):
         install.run(self)
         self.spawn([sys.executable, "post_install.py"])
 
 
 setup(
     name="api-hunter-cli",
-    version="0.1.0",
+    version="0.1.1",
     description="CLI tool for finding hidden apis in a certain url.",
     author="Charly Molero",
     author_email="perez.moleroc@gmail.com",
     url="https://github.com/engcarlosperezmolero/",
     packages=find_packages(),
     install_requires=[
         "playwright",
```


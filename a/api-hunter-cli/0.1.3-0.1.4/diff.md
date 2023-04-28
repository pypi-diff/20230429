# Comparing `tmp/api_hunter_cli-0.1.3.tar.gz` & `tmp/api_hunter_cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_hunter_cli-0.1.3.tar", last modified: Fri Apr 28 22:51:06 2023, max compression
+gzip compressed data, was "api_hunter_cli-0.1.4.tar", last modified: Fri Apr 28 22:56:29 2023, max compression
```

## Comparing `api_hunter_cli-0.1.3.tar` & `api_hunter_cli-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:51:06.019592 api_hunter_cli-0.1.3/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 22:51:06.019592 api_hunter_cli-0.1.3/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api_hunter_cli-0.1.3/README.md
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:51:06.019592 api_hunter_cli-0.1.3/api_hunter_cli/
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.1.3/api_hunter_cli/__init__.py
--rw-rw-r--   0 charly    (1000) charly    (1000)     4239 2023-04-28 04:53:55.000000 api_hunter_cli-0.1.3/api_hunter_cli/main.py
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:51:06.019592 api_hunter_cli-0.1.3/api_hunter_cli.egg-info/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 22:51:05.000000 api_hunter_cli-0.1.3/api_hunter_cli.egg-info/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)      298 2023-04-28 22:51:05.000000 api_hunter_cli-0.1.3/api_hunter_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-28 22:51:05.000000 api_hunter_cli-0.1.3/api_hunter_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       54 2023-04-28 22:51:05.000000 api_hunter_cli-0.1.3/api_hunter_cli.egg-info/entry_points.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 22:51:05.000000 api_hunter_cli-0.1.3/api_hunter_cli.egg-info/requires.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-28 22:51:05.000000 api_hunter_cli-0.1.3/api_hunter_cli.egg-info/top_level.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 22:51:06.019592 api_hunter_cli-0.1.3/setup.cfg
--rw-rw-r--   0 charly    (1000) charly    (1000)     1414 2023-04-28 22:50:11.000000 api_hunter_cli-0.1.3/setup.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:56:29.986945 api_hunter_cli-0.1.4/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 22:56:29.986945 api_hunter_cli-0.1.4/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api_hunter_cli-0.1.4/README.md
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:56:29.986945 api_hunter_cli-0.1.4/api_hunter_cli/
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.1.4/api_hunter_cli/__init__.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)     4239 2023-04-28 04:53:55.000000 api_hunter_cli-0.1.4/api_hunter_cli/main.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)      649 2023-04-28 22:53:47.000000 api_hunter_cli-0.1.4/api_hunter_cli/post_install.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:56:29.986945 api_hunter_cli-0.1.4/api_hunter_cli.egg-info/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 22:56:29.000000 api_hunter_cli-0.1.4/api_hunter_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)      329 2023-04-28 22:56:29.000000 api_hunter_cli-0.1.4/api_hunter_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-28 22:56:29.000000 api_hunter_cli-0.1.4/api_hunter_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)      130 2023-04-28 22:56:29.000000 api_hunter_cli-0.1.4/api_hunter_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 22:56:29.000000 api_hunter_cli-0.1.4/api_hunter_cli.egg-info/requires.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-28 22:56:29.000000 api_hunter_cli-0.1.4/api_hunter_cli.egg-info/top_level.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 22:56:29.986945 api_hunter_cli-0.1.4/setup.cfg
+-rw-rw-r--   0 charly    (1000) charly    (1000)     1412 2023-04-28 22:56:26.000000 api_hunter_cli-0.1.4/setup.py
```

### Comparing `api_hunter_cli-0.1.3/PKG-INFO` & `api_hunter_cli-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api_hunter_cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `api_hunter_cli-0.1.3/api_hunter_cli/main.py` & `api_hunter_cli-0.1.4/api_hunter_cli/main.py`

 * *Files identical despite different names*

### Comparing `api_hunter_cli-0.1.3/api_hunter_cli.egg-info/PKG-INFO` & `api_hunter_cli-0.1.4/api_hunter_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-hunter-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```


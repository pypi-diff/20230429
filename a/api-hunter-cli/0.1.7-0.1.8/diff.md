# Comparing `tmp/api_hunter_cli-0.1.7.tar.gz` & `tmp/api_hunter_cli-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_hunter_cli-0.1.7.tar", last modified: Fri Apr 28 23:29:16 2023, max compression
+gzip compressed data, was "api_hunter_cli-0.1.8.tar", last modified: Sat Apr 29 16:03:28 2023, max compression
```

## Comparing `api_hunter_cli-0.1.7.tar` & `api_hunter_cli-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:29:16.526376 api_hunter_cli-0.1.7/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 23:29:16.526376 api_hunter_cli-0.1.7/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api_hunter_cli-0.1.7/README.md
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:29:16.526376 api_hunter_cli-0.1.7/api_hunter_cli/
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.1.7/api_hunter_cli/__init__.py
--rw-rw-r--   0 charly    (1000) charly    (1000)     5495 2023-04-28 23:29:09.000000 api_hunter_cli-0.1.7/api_hunter_cli/main.py
--rw-rw-r--   0 charly    (1000) charly    (1000)      649 2023-04-28 22:53:47.000000 api_hunter_cli-0.1.7/api_hunter_cli/post_install.py
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:29:16.526376 api_hunter_cli-0.1.7/api_hunter_cli.egg-info/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 23:29:16.000000 api_hunter_cli-0.1.7/api_hunter_cli.egg-info/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)      329 2023-04-28 23:29:16.000000 api_hunter_cli-0.1.7/api_hunter_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-28 23:29:16.000000 api_hunter_cli-0.1.7/api_hunter_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)      129 2023-04-28 23:29:16.000000 api_hunter_cli-0.1.7/api_hunter_cli.egg-info/entry_points.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 23:29:16.000000 api_hunter_cli-0.1.7/api_hunter_cli.egg-info/requires.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-28 23:29:16.000000 api_hunter_cli-0.1.7/api_hunter_cli.egg-info/top_level.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 23:29:16.530376 api_hunter_cli-0.1.7/setup.cfg
--rw-rw-r--   0 charly    (1000) charly    (1000)     1411 2023-04-28 23:29:09.000000 api_hunter_cli-0.1.7/setup.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:03:28.163875 api_hunter_cli-0.1.8/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-29 16:03:28.163875 api_hunter_cli-0.1.8/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api_hunter_cli-0.1.8/README.md
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:03:28.163875 api_hunter_cli-0.1.8/api_hunter_cli/
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.1.8/api_hunter_cli/__init__.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)     3472 2023-04-29 16:02:23.000000 api_hunter_cli-0.1.8/api_hunter_cli/main.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)     3724 2023-04-29 16:02:02.000000 api_hunter_cli-0.1.8/api_hunter_cli/playwright_custom.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)      649 2023-04-28 22:53:47.000000 api_hunter_cli-0.1.8/api_hunter_cli/post_install.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:03:28.163875 api_hunter_cli-0.1.8/api_hunter_cli.egg-info/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-29 16:03:28.000000 api_hunter_cli-0.1.8/api_hunter_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)      365 2023-04-29 16:03:28.000000 api_hunter_cli-0.1.8/api_hunter_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-29 16:03:28.000000 api_hunter_cli-0.1.8/api_hunter_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)      129 2023-04-29 16:03:28.000000 api_hunter_cli-0.1.8/api_hunter_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-29 16:03:28.000000 api_hunter_cli-0.1.8/api_hunter_cli.egg-info/requires.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-29 16:03:28.000000 api_hunter_cli-0.1.8/api_hunter_cli.egg-info/top_level.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-29 16:03:28.163875 api_hunter_cli-0.1.8/setup.cfg
+-rw-rw-r--   0 charly    (1000) charly    (1000)     1411 2023-04-29 16:03:09.000000 api_hunter_cli-0.1.8/setup.py
```

### Comparing `api_hunter_cli-0.1.7/PKG-INFO` & `api_hunter_cli-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api_hunter_cli
-Version: 0.1.7
+Version: 0.1.8
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `api_hunter_cli-0.1.7/api_hunter_cli/post_install.py` & `api_hunter_cli-0.1.8/api_hunter_cli/post_install.py`

 * *Files identical despite different names*

### Comparing `api_hunter_cli-0.1.7/api_hunter_cli.egg-info/PKG-INFO` & `api_hunter_cli-0.1.8/api_hunter_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-hunter-cli
-Version: 0.1.7
+Version: 0.1.8
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `api_hunter_cli-0.1.7/setup.py` & `api_hunter_cli-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def run(self):
         install.run(self)
         self.spawn([sys.executable, "post_install.py"])
 
 
 setup(
     name="api_hunter_cli",
-    version="0.1.7",
+    version="0.1.8",
     description="CLI tool for finding hidden apis in a certain url.",
     author="Charly Molero",
     author_email="perez.moleroc@gmail.com",
     url="https://github.com/engcarlosperezmolero/",
     packages=find_packages(),
     install_requires=[
         "playwright",
```


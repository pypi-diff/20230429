# Comparing `tmp/UzbekLemmatizer-1.0.0.tar.gz` & `tmp/UzbekLemmatizer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UzbekLemmatizer-1.0.0.tar", last modified: Sat Mar 26 12:10:10 2022, max compression
+gzip compressed data, was "UzbekLemmatizer-1.0.1.tar", last modified: Sat Mar 26 12:19:16 2022, max compression
```

## Comparing `UzbekLemmatizer-1.0.0.tar` & `UzbekLemmatizer-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 maksud    (1000) maksud    (1000)        0 2022-03-26 12:10:10.158844 UzbekLemmatizer-1.0.0/
--rw-rw-r--   0 maksud    (1000) maksud    (1000)     1073 2022-03-05 06:39:40.000000 UzbekLemmatizer-1.0.0/LICENSE
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      623 2022-03-26 12:10:10.162844 UzbekLemmatizer-1.0.0/PKG-INFO
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      520 2022-03-05 06:43:33.000000 UzbekLemmatizer-1.0.0/README.md
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      103 2022-03-05 06:39:40.000000 UzbekLemmatizer-1.0.0/pyproject.toml
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      648 2022-03-26 12:10:10.162844 UzbekLemmatizer-1.0.0/setup.cfg
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      871 2022-03-26 12:09:16.000000 UzbekLemmatizer-1.0.0/setup.py
-drwxrwxr-x   0 maksud    (1000) maksud    (1000)        0 2022-03-26 12:10:10.158844 UzbekLemmatizer-1.0.0/src/
-drwxrwxr-x   0 maksud    (1000) maksud    (1000)        0 2022-03-26 12:10:10.158844 UzbekLemmatizer-1.0.0/src/UzbekLemmatizer.egg-info/
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      623 2022-03-26 12:10:09.000000 UzbekLemmatizer-1.0.0/src/UzbekLemmatizer.egg-info/PKG-INFO
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      246 2022-03-26 12:10:10.000000 UzbekLemmatizer-1.0.0/src/UzbekLemmatizer.egg-info/SOURCES.txt
--rw-rw-r--   0 maksud    (1000) maksud    (1000)        1 2022-03-26 12:10:09.000000 UzbekLemmatizer-1.0.0/src/UzbekLemmatizer.egg-info/dependency_links.txt
--rw-rw-r--   0 maksud    (1000) maksud    (1000)        1 2022-03-26 12:10:10.000000 UzbekLemmatizer-1.0.0/src/UzbekLemmatizer.egg-info/top_level.txt
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      175 2022-03-26 10:57:16.000000 UzbekLemmatizer-1.0.0/src/UzbekLemmatizer.py
+drwxrwxr-x   0 maksud    (1000) maksud    (1000)        0 2022-03-26 12:19:16.512422 UzbekLemmatizer-1.0.1/
+-rw-rw-r--   0 maksud    (1000) maksud    (1000)     1073 2022-03-05 06:39:40.000000 UzbekLemmatizer-1.0.1/LICENSE
+-rw-rw-r--   0 maksud    (1000) maksud    (1000)      623 2022-03-26 12:19:16.512422 UzbekLemmatizer-1.0.1/PKG-INFO
+-rw-rw-r--   0 maksud    (1000) maksud    (1000)      520 2022-03-05 06:43:33.000000 UzbekLemmatizer-1.0.1/README.md
+-rw-rw-r--   0 maksud    (1000) maksud    (1000)      103 2022-03-05 06:39:40.000000 UzbekLemmatizer-1.0.1/pyproject.toml
+-rw-rw-r--   0 maksud    (1000) maksud    (1000)      648 2022-03-26 12:19:16.512422 UzbekLemmatizer-1.0.1/setup.cfg
+-rw-rw-r--   0 maksud    (1000) maksud    (1000)      871 2022-03-26 12:12:06.000000 UzbekLemmatizer-1.0.1/setup.py
+drwxrwxr-x   0 maksud    (1000) maksud    (1000)        0 2022-03-26 12:19:16.508422 UzbekLemmatizer-1.0.1/src/
+drwxrwxr-x   0 maksud    (1000) maksud    (1000)        0 2022-03-26 12:19:16.512422 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/
+-rw-rw-r--   0 maksud    (1000) maksud    (1000)      623 2022-03-26 12:19:16.000000 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/PKG-INFO
+-rw-rw-r--   0 maksud    (1000) maksud    (1000)      335 2022-03-26 12:19:16.000000 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 maksud    (1000) maksud    (1000)      175 2022-03-26 10:57:16.000000 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/UzbekLemmatizer.py
+-rw-rw-r--   0 maksud    (1000) maksud    (1000)        0 2022-03-26 12:15:38.000000 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/__init__.py
+-rw-rw-r--   0 maksud    (1000) maksud    (1000)        1 2022-03-26 12:19:16.000000 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 maksud    (1000) maksud    (1000)        1 2022-03-26 12:19:16.000000 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/top_level.txt
+-rw-rw-r--   0 maksud    (1000) maksud    (1000)      175 2022-03-26 10:57:16.000000 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.py
```

### Comparing `UzbekLemmatizer-1.0.0/LICENSE` & `UzbekLemmatizer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `UzbekLemmatizer-1.0.0/PKG-INFO` & `UzbekLemmatizer-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UzbekLemmatizer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Uzbek Lemmatizer for Python
 Home-page: https://github.com/MaksudSharipov/UzbekLemmatizer
 Author: Maksud Sharipov
 Author-email: maqsbek72@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/MaksudSharipov/UzbekLemmatizer
 Platform: UNKNOWN
```

### Comparing `UzbekLemmatizer-1.0.0/README.md` & `UzbekLemmatizer-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `UzbekLemmatizer-1.0.0/setup.cfg` & `UzbekLemmatizer-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = UzbekLemmatizer
-version = 1.0.0
+version = 1.0.1
 author = Maksud Sharipov
 author_email = maqsbek72@gmail.com
 description = Uzbek Lemmatizer for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MaksudSharipov/UzbekLemmatizer
 project_urls =
```

### Comparing `UzbekLemmatizer-1.0.0/setup.py` & `UzbekLemmatizer-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="UzbekLemmatizer",
-    version="1.0.0",
+    version="1.0.1",
     author="Maksud Sharipov",
     author_email="maqsbek72@gmail.com",
     description="Uzbek Lemmatizer for Python",
     long_description="The Uzbek Lemmation algorithm was created by [Maksud Sharipov].",
     long_description_content_type="text/markdown",
     url="https://github.com/MaksudSharipov/UzbekLemmatizer",
     project_urls={
```

### Comparing `UzbekLemmatizer-1.0.0/src/UzbekLemmatizer.egg-info/PKG-INFO` & `UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UzbekLemmatizer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Uzbek Lemmatizer for Python
 Home-page: https://github.com/MaksudSharipov/UzbekLemmatizer
 Author: Maksud Sharipov
 Author-email: maqsbek72@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/MaksudSharipov/UzbekLemmatizer
 Platform: UNKNOWN
```


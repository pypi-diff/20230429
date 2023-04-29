# Comparing `tmp/UzbekLemmatizer-1.0.2.tar.gz` & `tmp/UzbekLemmatizer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UzbekLemmatizer-1.0.2.tar", last modified: Sat Apr 29 05:55:59 2023, max compression
+gzip compressed data, was "UzbekLemmatizer-1.0.3.tar", last modified: Sat Apr 29 06:04:51 2023, max compression
```

## Comparing `UzbekLemmatizer-1.0.2.tar` & `UzbekLemmatizer-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 05:55:59.902086 UzbekLemmatizer-1.0.2/
--rw-rw-rw-   0        0        0     1109 2023-04-29 04:36:11.000000 UzbekLemmatizer-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1122 2023-04-29 05:55:59.902086 UzbekLemmatizer-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-04-29 04:49:41.000000 UzbekLemmatizer-1.0.2/README.md
--rw-rw-rw-   0        0        0      528 2023-04-29 05:55:24.000000 UzbekLemmatizer-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 05:55:59.902086 UzbekLemmatizer-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1218 2023-04-29 05:54:18.000000 UzbekLemmatizer-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:55:59.902086 UzbekLemmatizer-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 05:55:59.902086 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer/
--rw-rw-rw-   0        0        0     4898 2023-04-29 04:10:27.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer/UzbekLemmatizer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 04:40:30.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer/__init__.py
--rw-rw-rw-   0        0        0     4035 2023-04-29 04:06:11.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer/fsms.xml
--rw-rw-rw-   0        0        0    53767 2023-04-08 11:23:16.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer/suffixes.xml
-drwxrwxrwx   0        0        0        0 2023-04-29 05:55:59.902086 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-04-29 05:55:59.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-04-29 05:55:59.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 05:55:59.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-29 05:55:59.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 06:04:51.551625 UzbekLemmatizer-1.0.3/
+-rw-rw-rw-   0        0        0     1109 2023-04-29 04:36:11.000000 UzbekLemmatizer-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1122 2023-04-29 06:04:51.546087 UzbekLemmatizer-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-04-29 04:49:41.000000 UzbekLemmatizer-1.0.3/README.md
+-rw-rw-rw-   0        0        0      528 2023-04-29 06:04:17.000000 UzbekLemmatizer-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 06:04:51.551625 UzbekLemmatizer-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2023-04-29 06:04:17.000000 UzbekLemmatizer-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 06:04:51.530459 UzbekLemmatizer-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 06:04:51.546087 UzbekLemmatizer-1.0.3/src/UzbekLemmatizer/
+-rw-rw-rw-   0        0        0     4898 2023-04-29 04:10:27.000000 UzbekLemmatizer-1.0.3/src/UzbekLemmatizer/UzbekLemmatizer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 04:40:30.000000 UzbekLemmatizer-1.0.3/src/UzbekLemmatizer/__init__.py
+-rw-rw-rw-   0        0        0     4035 2023-04-29 04:06:11.000000 UzbekLemmatizer-1.0.3/src/UzbekLemmatizer/fsms.xml
+-rw-rw-rw-   0        0        0    53767 2023-04-08 11:23:16.000000 UzbekLemmatizer-1.0.3/src/UzbekLemmatizer/suffixes.xml
+drwxrwxrwx   0        0        0        0 2023-04-29 06:04:51.546087 UzbekLemmatizer-1.0.3/src/UzbekLemmatizer.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-04-29 06:04:51.000000 UzbekLemmatizer-1.0.3/src/UzbekLemmatizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-04-29 06:04:51.000000 UzbekLemmatizer-1.0.3/src/UzbekLemmatizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 06:04:51.000000 UzbekLemmatizer-1.0.3/src/UzbekLemmatizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-29 06:04:51.000000 UzbekLemmatizer-1.0.3/src/UzbekLemmatizer.egg-info/top_level.txt
```

### Comparing `UzbekLemmatizer-1.0.2/LICENSE` & `UzbekLemmatizer-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `UzbekLemmatizer-1.0.2/PKG-INFO` & `UzbekLemmatizer-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UzbekLemmatizer
-Version: 1.0.2
+Version: 1.0.3
 Summary: Uzbek Lemmatizer for Python. A Python package to lemmatize Uzbek words.
 Home-page: https://github.com/MaksudSharipov/UzbekLemmatizer
 Author: Maksud Sharipov, Ollabergan Yuldashov
 Author-email: "Maksud Sharipov, Ollabergan Yuldashov" <maqsbek72@gmail.com>
 Project-URL: Homepage, https://github.com/MaksudSharipov/UzbekLemmatizer
 Keywords: python,UzbekLemmatizer,uzbek words,Lemmatizer
 Classifier: Programming Language :: Python :: 3
```

### Comparing `UzbekLemmatizer-1.0.2/pyproject.toml` & `UzbekLemmatizer-1.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "UzbekLemmatizer"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Maksud Sharipov, Ollabergan Yuldashov", email="maqsbek72@gmail.com" },
 ]
 description = "Uzbek Lemmatizer for Python. A Python package to lemmatize Uzbek words."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `UzbekLemmatizer-1.0.2/setup.py` & `UzbekLemmatizer-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="UzbekLemmatizer",
-    version="1.0.2",
+    version="1.0.3",
     author="Maksud Sharipov, Ollabergan Yuldashov",
     author_email="maqsbek72@gmail.com, ollaberganyuldashov@gmail.com",
     description="Uzbek Lemmatizer for Python. A Python package to lemmatize Uzbek words.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MaksudSharipov/UzbekLemmatizer",
     project_urls={
```

### Comparing `UzbekLemmatizer-1.0.2/src/UzbekLemmatizer/UzbekLemmatizer.py` & `UzbekLemmatizer-1.0.3/src/UzbekLemmatizer/UzbekLemmatizer.py`

 * *Files identical despite different names*

### Comparing `UzbekLemmatizer-1.0.2/src/UzbekLemmatizer/fsms.xml` & `UzbekLemmatizer-1.0.3/src/UzbekLemmatizer/fsms.xml`

 * *Files identical despite different names*

### Comparing `UzbekLemmatizer-1.0.2/src/UzbekLemmatizer/suffixes.xml` & `UzbekLemmatizer-1.0.3/src/UzbekLemmatizer/suffixes.xml`

 * *Files identical despite different names*

### Comparing `UzbekLemmatizer-1.0.2/src/UzbekLemmatizer.egg-info/PKG-INFO` & `UzbekLemmatizer-1.0.3/src/UzbekLemmatizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UzbekLemmatizer
-Version: 1.0.2
+Version: 1.0.3
 Summary: Uzbek Lemmatizer for Python. A Python package to lemmatize Uzbek words.
 Home-page: https://github.com/MaksudSharipov/UzbekLemmatizer
 Author: Maksud Sharipov, Ollabergan Yuldashov
 Author-email: "Maksud Sharipov, Ollabergan Yuldashov" <maqsbek72@gmail.com>
 Project-URL: Homepage, https://github.com/MaksudSharipov/UzbekLemmatizer
 Keywords: python,UzbekLemmatizer,uzbek words,Lemmatizer
 Classifier: Programming Language :: Python :: 3
```


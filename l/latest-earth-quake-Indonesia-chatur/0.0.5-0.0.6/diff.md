# Comparing `tmp/latest_earth_quake_Indonesia_chatur-0.0.5.tar.gz` & `tmp/latest_earth_quake_Indonesia_chatur-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latest_earth_quake_Indonesia_chatur-0.0.5.tar", last modified: Fri Apr 28 01:16:19 2023, max compression
+gzip compressed data, was "latest_earth_quake_Indonesia_chatur-0.0.6.tar", last modified: Fri Apr 28 23:46:55 2023, max compression
```

## Comparing `latest_earth_quake_Indonesia_chatur-0.0.5.tar` & `latest_earth_quake_Indonesia_chatur-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 01:16:19.678515 latest_earth_quake_Indonesia_chatur-0.0.5/
--rw-rw-rw-   0        0        0    35823 2023-04-27 00:11:05.000000 latest_earth_quake_Indonesia_chatur-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1047 2023-04-28 01:16:19.677517 latest_earth_quake_Indonesia_chatur-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-04-28 01:15:21.000000 latest_earth_quake_Indonesia_chatur-0.0.5/README.md
--rw-rw-rw-   0        0        0      636 2023-04-28 01:15:45.000000 latest_earth_quake_Indonesia_chatur-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 01:16:19.679518 latest_earth_quake_Indonesia_chatur-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 01:16:19.627515 latest_earth_quake_Indonesia_chatur-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 01:16:19.639540 latest_earth_quake_Indonesia_chatur-0.0.5/src/gempaterkini_chatur/
--rw-rw-rw-   0        0        0     2761 2023-04-28 01:12:42.000000 latest_earth_quake_Indonesia_chatur-0.0.5/src/gempaterkini_chatur/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-27 23:38:48.000000 latest_earth_quake_Indonesia_chatur-0.0.5/src/gempaterkini_chatur/example.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:16:19.674678 latest_earth_quake_Indonesia_chatur-0.0.5/src/latest_earth_quake_Indonesia_chatur.egg-info/
--rw-rw-rw-   0        0        0     1047 2023-04-28 01:16:19.000000 latest_earth_quake_Indonesia_chatur-0.0.5/src/latest_earth_quake_Indonesia_chatur.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-04-28 01:16:19.000000 latest_earth_quake_Indonesia_chatur-0.0.5/src/latest_earth_quake_Indonesia_chatur.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 01:16:19.000000 latest_earth_quake_Indonesia_chatur-0.0.5/src/latest_earth_quake_Indonesia_chatur.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-28 01:16:19.000000 latest_earth_quake_Indonesia_chatur-0.0.5/src/latest_earth_quake_Indonesia_chatur.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 23:46:55.644013 latest_earth_quake_Indonesia_chatur-0.0.6/
+-rw-rw-rw-   0        0        0    35823 2023-04-27 00:11:05.000000 latest_earth_quake_Indonesia_chatur-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1047 2023-04-28 23:46:55.642948 latest_earth_quake_Indonesia_chatur-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-04-28 01:15:21.000000 latest_earth_quake_Indonesia_chatur-0.0.6/README.md
+-rw-rw-rw-   0        0        0      636 2023-04-28 23:46:04.000000 latest_earth_quake_Indonesia_chatur-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 23:46:55.644949 latest_earth_quake_Indonesia_chatur-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 23:46:55.579949 latest_earth_quake_Indonesia_chatur-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 23:46:55.608948 latest_earth_quake_Indonesia_chatur-0.0.6/src/gempaterkini_chatur/
+-rw-rw-rw-   0        0        0     2837 2023-04-28 23:42:00.000000 latest_earth_quake_Indonesia_chatur-0.0.6/src/gempaterkini_chatur/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 23:38:48.000000 latest_earth_quake_Indonesia_chatur-0.0.6/src/gempaterkini_chatur/example.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:46:55.640080 latest_earth_quake_Indonesia_chatur-0.0.6/src/latest_earth_quake_Indonesia_chatur.egg-info/
+-rw-rw-rw-   0        0        0     1047 2023-04-28 23:46:55.000000 latest_earth_quake_Indonesia_chatur-0.0.6/src/latest_earth_quake_Indonesia_chatur.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-04-28 23:46:55.000000 latest_earth_quake_Indonesia_chatur-0.0.6/src/latest_earth_quake_Indonesia_chatur.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 23:46:55.000000 latest_earth_quake_Indonesia_chatur-0.0.6/src/latest_earth_quake_Indonesia_chatur.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-28 23:46:55.000000 latest_earth_quake_Indonesia_chatur-0.0.6/src/latest_earth_quake_Indonesia_chatur.egg-info/top_level.txt
```

### Comparing `latest_earth_quake_Indonesia_chatur-0.0.5/LICENSE` & `latest_earth_quake_Indonesia_chatur-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `latest_earth_quake_Indonesia_chatur-0.0.5/PKG-INFO` & `latest_earth_quake_Indonesia_chatur-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latest_earth_quake_Indonesia_chatur
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package will get the latest earthquake (Indonesia) from https://www.bmkg.go.id/ BMKG
 Author-email: Chatur Agus Priyono <chatur.agus.priyono@gmail.com>
 Project-URL: Homepage, https://github.com/chaturap/bmkg-latest-earthquake
 Project-URL: Bug Tracker, https://github.com/chaturap/bmkg-latest-earthquake/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `latest_earth_quake_Indonesia_chatur-0.0.5/pyproject.toml` & `latest_earth_quake_Indonesia_chatur-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "latest_earth_quake_Indonesia_chatur"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Chatur Agus Priyono", email="chatur.agus.priyono@gmail.com" },
 ]
 description = "This package will get the latest earthquake (Indonesia) from https://www.bmkg.go.id/ BMKG"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `latest_earth_quake_Indonesia_chatur-0.0.5/src/gempaterkini_chatur/__init__.py` & `latest_earth_quake_Indonesia_chatur-0.0.6/src/gempaterkini_chatur/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 from bs4 import BeautifulSoup
 
+description = 'To get the latest earathquake in Indonesia from BMKG.go.ig'
 
 def ekstrasi_data():
     """
 tanggal : 26 April 2023,
 waktu : 09:56:27 WIB
 Magnitudo :     4.7
 Kedalaman : 61 km
```

### Comparing `latest_earth_quake_Indonesia_chatur-0.0.5/src/latest_earth_quake_Indonesia_chatur.egg-info/PKG-INFO` & `latest_earth_quake_Indonesia_chatur-0.0.6/src/latest_earth_quake_Indonesia_chatur.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latest-earth-quake-Indonesia-chatur
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package will get the latest earthquake (Indonesia) from https://www.bmkg.go.id/ BMKG
 Author-email: Chatur Agus Priyono <chatur.agus.priyono@gmail.com>
 Project-URL: Homepage, https://github.com/chaturap/bmkg-latest-earthquake
 Project-URL: Bug Tracker, https://github.com/chaturap/bmkg-latest-earthquake/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


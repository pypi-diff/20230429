# Comparing `tmp/mpxl2csv-0.1.1.tar.gz` & `tmp/mpxl2csv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpxl2csv-0.1.1.tar", max compression
+gzip compressed data, was "mpxl2csv-0.2.0.tar", max compression
```

## Comparing `mpxl2csv-0.1.1.tar` & `mpxl2csv-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-27 17:18:37.783554 mpxl2csv-0.1.1/LICENSE
--rw-r--r--   0        0        0      600 2023-04-27 19:18:33.676762 mpxl2csv-0.1.1/README.md
--rw-r--r--   0        0        0       31 2023-04-27 17:44:35.339913 mpxl2csv-0.1.1/mpxl2csv/__init__.py
--rw-r--r--   0        0        0     3134 2023-04-27 18:05:06.498301 mpxl2csv-0.1.1/mpxl2csv/mpxl2csv.py
--rw-r--r--   0        0        0      809 2023-04-27 20:30:54.842524 mpxl2csv-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1672 1970-01-01 00:00:00.000000 mpxl2csv-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-27 17:18:37.783554 mpxl2csv-0.2.0/LICENSE
+-rw-r--r--   0        0        0      600 2023-04-27 19:18:33.676762 mpxl2csv-0.2.0/README.md
+-rw-r--r--   0        0        0       31 2023-04-27 17:44:35.339913 mpxl2csv-0.2.0/mpxl2csv/__init__.py
+-rw-r--r--   0        0        0     5114 2023-04-28 21:58:38.221799 mpxl2csv-0.2.0/mpxl2csv/mpxl2csv.py
+-rw-r--r--   0        0        0      872 2023-04-28 21:49:50.095461 mpxl2csv-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 mpxl2csv-0.2.0/PKG-INFO
```

### Comparing `mpxl2csv-0.1.1/LICENSE` & `mpxl2csv-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpxl2csv-0.1.1/README.md` & `mpxl2csv-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mpxl2csv-0.1.1/pyproject.toml` & `mpxl2csv-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpxl2csv"
-version = "0.1.1"
+version = "0.2.0"
 description = "Uses Python multiprocessing to convert multiple Excel files to CSV files"
 authors = ["Harish Chauhan <harish.chauhan99@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/hariya99/mpxl2csv"
 repository = "https://github.com/hariya99/mpxl2csv"
 keywords = ["Excel", "CSV", "multiprocessing"]
@@ -14,16 +14,21 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = [
     "LICENSE",
 ]
+exclude = [
+    "resources*", 
+    "tests*",
+]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 openpyxl = "^3.1.2"
+xlrd = "^2.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mpxl2csv-0.1.1/PKG-INFO` & `mpxl2csv-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpxl2csv
-Version: 0.1.1
+Version: 0.2.0
 Summary: Uses Python multiprocessing to convert multiple Excel files to CSV files
 Home-page: https://github.com/hariya99/mpxl2csv
 License: MIT
 Keywords: Excel,CSV,multiprocessing
 Author: Harish Chauhan
 Author-email: harish.chauhan99@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
+Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/hariya99/mpxl2csv
 Description-Content-Type: text/markdown
 
 # MPXL2CSV
 A Python Multiprocessing library to convert Excel(xlsx) files to csv. Python based libraries are notoriously slow to process large Excel files. This library utilizes Python multiprocessing and openpyxl to process multiple Excel files in parallel so as to reduce the total time taken to convert them. 
 # Installing
 ```
```


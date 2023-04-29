# Comparing `tmp/blankimage-0.1.1.tar.gz` & `tmp/blankimage-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blankimage-0.1.1.tar", max compression
+gzip compressed data, was "blankimage-0.1.2.tar", max compression
```

## Comparing `blankimage-0.1.1.tar` & `blankimage-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       55 2023-04-29 07:54:05.374779 blankimage-0.1.1/README.md
--rw-r--r--   0        0        0       26 2023-04-29 07:54:10.458848 blankimage-0.1.1/blankimage/__init__.py
--rw-r--r--   0        0        0     2615 2023-04-29 07:39:10.626691 blankimage-0.1.1/blankimage/format_options.py
--rw-r--r--   0        0        0     1514 2023-04-29 07:09:53.422626 blankimage-0.1.1/blankimage/parse_cli_options.py
--rw-r--r--   0        0        0     1255 2023-04-29 07:20:23.947407 blankimage-0.1.1/blankimage/process_task.py
--rw-r--r--   0        0        0     1042 2023-04-29 07:53:50.282594 blankimage-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 blankimage-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      111 2023-04-29 11:05:12.546204 blankimage-0.1.2/README.md
+-rw-r--r--   0        0        0       26 2023-04-29 11:03:42.376448 blankimage-0.1.2/blankimage/__init__.py
+-rw-r--r--   0        0        0     2615 2023-04-29 07:39:10.626691 blankimage-0.1.2/blankimage/format_options.py
+-rw-r--r--   0        0        0     1514 2023-04-29 07:09:53.422626 blankimage-0.1.2/blankimage/parse_cli_options.py
+-rw-r--r--   0        0        0     1255 2023-04-29 07:20:23.947407 blankimage-0.1.2/blankimage/process_task.py
+-rw-r--r--   0        0        0     1038 2023-04-29 11:03:35.496315 blankimage-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1114 1970-01-01 00:00:00.000000 blankimage-0.1.2/PKG-INFO
```

### Comparing `blankimage-0.1.1/blankimage/format_options.py` & `blankimage-0.1.2/blankimage/format_options.py`

 * *Files identical despite different names*

### Comparing `blankimage-0.1.1/blankimage/parse_cli_options.py` & `blankimage-0.1.2/blankimage/parse_cli_options.py`

 * *Files identical despite different names*

### Comparing `blankimage-0.1.1/blankimage/process_task.py` & `blankimage-0.1.2/blankimage/process_task.py`

 * *Files identical despite different names*

### Comparing `blankimage-0.1.1/pyproject.toml` & `blankimage-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blankimage"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python Command Line Tool to Generate Blank Images"
 authors = ["Sumanth <sumanthreddystar@gmail.com>"]
 maintainers  = ["Sumanth <sumanthreddystar@gmail.com>"]
 readme = "README.md"
 
 homepage = "https://pypi.org/project/blankimage/"
 repository = "https://github.com/insumanth/blankimage"
@@ -22,19 +22,19 @@
     "Operating System :: Microsoft",
     "Operating System :: Unix",
     "Operating System :: POSIX"
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 ril = "^0.4.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry.scripts]
-my_package_cli = 'blankimage.parse_cli_options:main'
+blankimage = 'blankimage.parse_cli_options:main'
```

### Comparing `blankimage-0.1.1/PKG-INFO` & `blankimage-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: blankimage
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Command Line Tool to Generate Blank Images
 Home-page: https://pypi.org/project/blankimage/
 Keywords: packaging,poetry
 Author: Sumanth
 Author-email: sumanthreddystar@gmail.com
 Maintainer: Sumanth
 Maintainer-email: sumanthreddystar@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ril (>=0.4.0,<0.5.0)
 Project-URL: Documentation, https://insumanth.github.io/blankimage
 Project-URL: Repository, https://github.com/insumanth/blankimage
 Description-Content-Type: text/markdown
 
 # blankimage
 Blank Image Generator CLI
-Version : 0.1.1
+version : 0.1.2
+
+
+Generate Blank Image of any size and color from CLI.
+
```


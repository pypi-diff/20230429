# Comparing `tmp/python-observer-0.3.1.tar.gz` & `tmp/python_observer-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-observer-0.3.1.tar", max compression
+gzip compressed data, was "python_observer-0.3.2.tar", max compression
```

## Comparing `python-observer-0.3.1.tar` & `python_observer-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1065 2023-04-24 10:28:29.010276 python-observer-0.3.1/LICENSE
--rw-r--r--   0        0        0      580 2023-04-28 10:51:14.439129 python-observer-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 09:24:48.929131 python-observer-0.3.1/python_observer/__init__.py
--rw-r--r--   0        0        0     4446 2023-04-28 10:31:08.927636 python-observer-0.3.1/python_observer/cli.py
--rw-r--r--   0        0        0       48 2023-04-23 10:25:03.851281 python-observer-0.3.1/python_observer/constants.py
--rw-r--r--   0        0        0      529 2023-04-24 10:10:37.131958 python-observer-0.3.1/python_observer/date.py
--rw-r--r--   0        0        0      992 2023-04-28 10:31:06.738394 python-observer-0.3.1/python_observer/display.py
--rw-r--r--   0        0        0     1019 2023-04-28 10:49:03.740134 python-observer-0.3.1/python_observer/misc.py
--rw-r--r--   0        0        0     2855 2023-04-25 13:30:23.405542 python-observer-0.3.1/python_observer/watch.py
--rw-r--r--   0        0        0      149 2023-04-24 10:36:02.903294 python-observer-0.3.1/README.md
--rw-r--r--   0        0        0      966 2023-04-28 10:51:43.005696 python-observer-0.3.1/setup.py
--rw-r--r--   0        0        0      787 2023-04-28 10:51:43.006696 python-observer-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-24 10:28:29.010276 python_observer-0.3.2/LICENSE
+-rw-r--r--   0        0        0      626 2023-04-29 10:05:23.788407 python_observer-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-04-29 10:05:23.806617 python_observer-0.3.2/python_observer/__init__.py
+-rw-r--r--   0        0        0     4446 2023-04-28 10:31:08.927636 python_observer-0.3.2/python_observer/cli.py
+-rw-r--r--   0        0        0       48 2023-04-29 09:49:29.930221 python_observer-0.3.2/python_observer/constants.py
+-rw-r--r--   0        0        0      529 2023-04-24 10:10:37.131958 python_observer-0.3.2/python_observer/date.py
+-rw-r--r--   0        0        0      992 2023-04-28 10:31:06.738394 python_observer-0.3.2/python_observer/display.py
+-rw-r--r--   0        0        0      879 2023-04-29 09:49:33.818936 python_observer-0.3.2/python_observer/misc.py
+-rw-r--r--   0        0        0     2855 2023-04-25 13:30:23.405542 python_observer-0.3.2/python_observer/watch.py
+-rw-r--r--   0        0        0      149 2023-04-24 10:36:02.903294 python_observer-0.3.2/README.md
+-rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 python_observer-0.3.2/PKG-INFO
```

### Comparing `python-observer-0.3.1/LICENSE` & `python_observer-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-observer-0.3.1/pyproject.toml` & `python_observer-0.3.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "python-observer"
-version = "0.3.1"
+version = "0.3.2"
 description = "Live reload for Python apps"
 authors = ["Skyascii <savioxavier112@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "python_observer/**/*.py" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = ">=12.5.1"
 humanfriendly = "^10.0"
 pyboxen = "^1.2.0"
-tomli = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
 
+[tool.poetry_bumpversion.file."python_observer/__init__.py"]
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 observer = "python_observer.cli:main"
```

### Comparing `python-observer-0.3.1/python_observer/cli.py` & `python_observer-0.3.2/python_observer/cli.py`

 * *Files identical despite different names*

### Comparing `python-observer-0.3.1/python_observer/date.py` & `python_observer-0.3.2/python_observer/date.py`

 * *Files identical despite different names*

### Comparing `python-observer-0.3.1/python_observer/display.py` & `python_observer-0.3.2/python_observer/display.py`

 * *Files identical despite different names*

### Comparing `python-observer-0.3.1/python_observer/watch.py` & `python_observer-0.3.2/python_observer/watch.py`

 * *Files identical despite different names*

### Comparing `python-observer-0.3.1/PKG-INFO` & `python_observer-0.3.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: python-observer
-Version: 0.3.1
+Version: 0.3.2
 Summary: Live reload for Python apps
 License: MIT
 Author: Skyascii
 Author-email: savioxavier112@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: humanfriendly (>=10.0,<11.0)
 Requires-Dist: pyboxen (>=1.2.0,<2.0.0)
 Requires-Dist: rich (>=12.5.1)
-Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # observer
 
 ![observer image](https://i.imgur.com/ZoafdEY.png)
 
 > Live reload for Python apps
```


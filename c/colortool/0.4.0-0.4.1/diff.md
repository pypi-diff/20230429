# Comparing `tmp/colortool-0.4.0.tar.gz` & `tmp/colortool-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colortool-0.4.0.tar", last modified: Sat Apr 29 10:46:44 2023, max compression
+gzip compressed data, was "colortool-0.4.1.tar", last modified: Sat Apr 29 10:50:11 2023, max compression
```

## Comparing `colortool-0.4.0.tar` & `colortool-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:46:44.240223 colortool-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-29 10:46:44.240223 colortool-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-29 10:46:29.000000 colortool-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:46:44.240223 colortool-0.4.0/colortool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-29 10:46:44.000000 colortool-0.4.0/colortool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-29 10:46:44.000000 colortool-0.4.0/colortool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:46:44.000000 colortool-0.4.0/colortool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 10:46:44.000000 colortool-0.4.0/colortool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 10:46:44.000000 colortool-0.4.0/colortool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-29 10:46:29.000000 colortool-0.4.0/colortool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-29 10:46:29.000000 colortool-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 10:46:44.240223 colortool-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:50:11.773640 colortool-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-29 10:50:11.769640 colortool-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-29 10:49:57.000000 colortool-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:50:11.769640 colortool-0.4.1/colortool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-29 10:50:11.000000 colortool-0.4.1/colortool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-29 10:50:11.000000 colortool-0.4.1/colortool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:50:11.000000 colortool-0.4.1/colortool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 10:50:11.000000 colortool-0.4.1/colortool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 10:50:11.000000 colortool-0.4.1/colortool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-29 10:49:57.000000 colortool-0.4.1/colortool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-29 10:49:57.000000 colortool-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 10:50:11.773640 colortool-0.4.1/setup.cfg
```

### Comparing `colortool-0.4.0/PKG-INFO` & `colortool-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colortool
-Version: 0.4.0
+Version: 0.4.1
 Summary: set of tools to work with different color formats
 Author-email: Alexander Rodionov <tandav@tandav.me>
 Project-URL: source, https://github.com/tandav/colortool
 Project-URL: issues, https://tandav.github.io/colortool/issues
 Project-URL: release notes, https://tandav.github.io/colortool/releases
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `colortool-0.4.0/README.md` & `colortool-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `colortool-0.4.0/colortool.egg-info/PKG-INFO` & `colortool-0.4.1/colortool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colortool
-Version: 0.4.0
+Version: 0.4.1
 Summary: set of tools to work with different color formats
 Author-email: Alexander Rodionov <tandav@tandav.me>
 Project-URL: source, https://github.com/tandav/colortool
 Project-URL: issues, https://tandav.github.io/colortool/issues
 Project-URL: release notes, https://tandav.github.io/colortool/releases
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `colortool-0.4.0/colortool.py` & `colortool-0.4.1/colortool.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import math
 import random
 import string
 import typing as tp
 
 from dsplib.scale import minmax_scaler
 
-__version__ = '0.4.0'
+__version__ = '0.4.1'
 
 Float3 = tp.Tuple[float, float, float]
 Float4 = tp.Tuple[float, float, float, float]
 Int3 = tp.Tuple[int, int, int]
 Int4 = tp.Tuple[int, int, int, int]
 Int3Float = tp.Tuple[int, int, int, float]
```

### Comparing `colortool-0.4.0/pyproject.toml` & `colortool-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "colortool"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
     {name = "Alexander Rodionov", email = "tandav@tandav.me"},
 ]
 description = "set of tools to work with different color formats"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
@@ -29,15 +29,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 # ==============================================================================
 
 [tool.bumpver]
-current_version = "v0.4.0"
+current_version = "v0.4.1"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```


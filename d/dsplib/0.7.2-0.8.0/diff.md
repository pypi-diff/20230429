# Comparing `tmp/dsplib-0.7.2.tar.gz` & `tmp/dsplib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsplib-0.7.2.tar", last modified: Sun Mar 19 20:37:54 2023, max compression
+gzip compressed data, was "dsplib-0.8.0.tar", last modified: Sat Apr 29 04:15:20 2023, max compression
```

## Comparing `dsplib-0.7.2.tar` & `dsplib-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:37:54.591262 dsplib-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-19 20:37:54.591262 dsplib-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-19 20:37:39.000000 dsplib-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:37:54.591262 dsplib-0.7.2/dsplib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-19 20:37:39.000000 dsplib-0.7.2/dsplib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-19 20:37:39.000000 dsplib-0.7.2/dsplib/circular_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-19 20:37:39.000000 dsplib-0.7.2/dsplib/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-19 20:37:39.000000 dsplib-0.7.2/dsplib/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:37:54.591262 dsplib-0.7.2/dsplib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-19 20:37:54.000000 dsplib-0.7.2/dsplib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-19 20:37:54.000000 dsplib-0.7.2/dsplib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 20:37:54.000000 dsplib-0.7.2/dsplib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-19 20:37:54.000000 dsplib-0.7.2/dsplib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-19 20:37:54.000000 dsplib-0.7.2/dsplib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-03-19 20:37:39.000000 dsplib-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 20:37:54.591262 dsplib-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:15:20.575287 dsplib-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-29 04:15:20.575287 dsplib-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-29 04:14:58.000000 dsplib-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:15:20.575287 dsplib-0.8.0/dsplib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 04:14:58.000000 dsplib-0.8.0/dsplib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-29 04:14:58.000000 dsplib-0.8.0/dsplib/circular_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-29 04:14:58.000000 dsplib-0.8.0/dsplib/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-29 04:14:58.000000 dsplib-0.8.0/dsplib/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:15:20.575287 dsplib-0.8.0/dsplib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-29 04:15:20.000000 dsplib-0.8.0/dsplib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-29 04:15:20.000000 dsplib-0.8.0/dsplib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 04:15:20.000000 dsplib-0.8.0/dsplib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 04:15:20.000000 dsplib-0.8.0/dsplib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 04:15:20.000000 dsplib-0.8.0/dsplib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-29 04:14:58.000000 dsplib-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 04:15:20.575287 dsplib-0.8.0/setup.cfg
```

### Comparing `dsplib-0.7.2/PKG-INFO` & `dsplib-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplib
-Version: 0.7.2
+Version: 0.8.0
 Summary: A set of tools for DSP projects
 Author-email: Alexander Rodionov <tandav@tandav.me>
 Project-URL: source, https://github.com/tandav/dsplib
 Project-URL: issues, https://github.com/tandav/dsplib/issues
 Project-URL: release notes, https://github.com/tandav/dsplib/releases
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `dsplib-0.7.2/dsplib/circular_buffer.py` & `dsplib-0.8.0/dsplib/circular_buffer.py`

 * *Files identical despite different names*

### Comparing `dsplib-0.7.2/dsplib/window.py` & `dsplib-0.8.0/dsplib/window.py`

 * *Files identical despite different names*

### Comparing `dsplib-0.7.2/dsplib.egg-info/PKG-INFO` & `dsplib-0.8.0/dsplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplib
-Version: 0.7.2
+Version: 0.8.0
 Summary: A set of tools for DSP projects
 Author-email: Alexander Rodionov <tandav@tandav.me>
 Project-URL: source, https://github.com/tandav/dsplib
 Project-URL: issues, https://github.com/tandav/dsplib/issues
 Project-URL: release notes, https://github.com/tandav/dsplib/releases
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `dsplib-0.7.2/pyproject.toml` & `dsplib-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dsplib"
-version = "0.7.2"
+version = "0.8.0"
 authors = [
     {name = "Alexander Rodionov", email = "tandav@tandav.me"},
 ]
 description = "A set of tools for DSP projects"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
@@ -29,15 +29,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 # ==============================================================================
 
 [tool.bumpver]
-current_version = "v0.7.2"
+current_version = "v0.8.0"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
@@ -141,7 +141,21 @@
 
 [tool.autopep8]
 ignore="E501,E701"
 recursive = true
 aggressive = 3
 
 # ==============================================================================
+
+[tool.flake8]
+ignore = [
+    'E501',
+    'E741',
+]
+
+# ==============================================================================
+
+[tool.pyright]
+venvPath = "/Users/tandav/.cache/virtualenvs"
+venv = "dsplib"
+
+# ==============================================================================
```


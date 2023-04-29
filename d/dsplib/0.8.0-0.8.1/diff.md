# Comparing `tmp/dsplib-0.8.0.tar.gz` & `tmp/dsplib-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsplib-0.8.0.tar", last modified: Sat Apr 29 04:15:20 2023, max compression
+gzip compressed data, was "dsplib-0.8.1.tar", last modified: Sat Apr 29 06:15:37 2023, max compression
```

## Comparing `dsplib-0.8.0.tar` & `dsplib-0.8.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:15:20.575287 dsplib-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-29 04:15:20.575287 dsplib-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-29 04:14:58.000000 dsplib-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:15:20.575287 dsplib-0.8.0/dsplib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 04:14:58.000000 dsplib-0.8.0/dsplib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-29 04:14:58.000000 dsplib-0.8.0/dsplib/circular_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-29 04:14:58.000000 dsplib-0.8.0/dsplib/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-29 04:14:58.000000 dsplib-0.8.0/dsplib/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:15:20.575287 dsplib-0.8.0/dsplib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-29 04:15:20.000000 dsplib-0.8.0/dsplib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-29 04:15:20.000000 dsplib-0.8.0/dsplib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 04:15:20.000000 dsplib-0.8.0/dsplib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 04:15:20.000000 dsplib-0.8.0/dsplib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 04:15:20.000000 dsplib-0.8.0/dsplib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-29 04:14:58.000000 dsplib-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 04:15:20.575287 dsplib-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:15:37.866777 dsplib-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-29 06:15:37.866777 dsplib-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-29 06:15:11.000000 dsplib-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:15:37.866777 dsplib-0.8.1/dsplib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 06:15:11.000000 dsplib-0.8.1/dsplib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-29 06:15:11.000000 dsplib-0.8.1/dsplib/circular_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:15:37.866777 dsplib-0.8.1/dsplib/scale/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-29 06:15:11.000000 dsplib-0.8.1/dsplib/scale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-29 06:15:11.000000 dsplib-0.8.1/dsplib/scale/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-29 06:15:11.000000 dsplib-0.8.1/dsplib/scale/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-29 06:15:11.000000 dsplib-0.8.1/dsplib/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:15:37.866777 dsplib-0.8.1/dsplib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-29 06:15:37.000000 dsplib-0.8.1/dsplib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-29 06:15:37.000000 dsplib-0.8.1/dsplib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:15:37.000000 dsplib-0.8.1/dsplib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-29 06:15:37.000000 dsplib-0.8.1/dsplib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 06:15:37.000000 dsplib-0.8.1/dsplib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-29 06:15:11.000000 dsplib-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 06:15:37.866777 dsplib-0.8.1/setup.cfg
```

### Comparing `dsplib-0.8.0/dsplib/circular_buffer.py` & `dsplib-0.8.1/dsplib/circular_buffer.py`

 * *Files identical despite different names*

### Comparing `dsplib-0.8.0/dsplib/scale.py` & `dsplib-0.8.1/dsplib/scale/numpy.py`

 * *Files identical despite different names*

### Comparing `dsplib-0.8.0/dsplib/window.py` & `dsplib-0.8.1/dsplib/window.py`

 * *Files identical despite different names*

### Comparing `dsplib-0.8.0/pyproject.toml` & `dsplib-0.8.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [project]
 name = "dsplib"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
     {name = "Alexander Rodionov", email = "tandav@tandav.me"},
 ]
 description = "A set of tools for DSP projects"
 readme = "README.md"
 requires-python = ">=3.8"
-dependencies = [
-    "numpy>=1.15.0",
-]
+dependencies = []
 
 [project.optional-dependencies]
 dev = [
     "bumpver",
     "pre-commit",
     "pytest",
 ]
+numpy = [
+    "numpy>=1.15.0",
+]
 
 [project.urls]
 source = "https://github.com/tandav/dsplib"
 # docs = "https://tandav.github.io/dsplib/"
 issues = "https://github.com/tandav/dsplib/issues"
 "release notes" = "https://github.com/tandav/dsplib/releases"
 
@@ -29,15 +30,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 # ==============================================================================
 
 [tool.bumpver]
-current_version = "v0.8.0"
+current_version = "v0.8.1"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
@@ -71,15 +72,15 @@
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
-[tool.mypy.overrides]
+[[tool.mypy.overrides]]
 module = ["tests.*"]
 disallow_untyped_defs = false
 
 # ==============================================================================
 
 [tool.ruff]
 extend-select = [
@@ -127,14 +128,15 @@
     "missing-class-docstring",
     "missing-module-docstring",
     "line-too-long",
     "import-outside-toplevel",
     "unused-variable",
     "too-many-arguments",
     "import-error",
+    "duplicate-code",
 ]
 
 [tool.pylint-per-file-ignores]
 "/tests/" = "redefined-outer-name"
 
 
 # ==============================================================================
```


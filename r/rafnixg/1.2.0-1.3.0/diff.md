# Comparing `tmp/rafnixg-1.2.0.tar.gz` & `tmp/rafnixg-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rafnixg-1.2.0.tar", last modified: Sat Apr 29 04:09:19 2023, max compression
+gzip compressed data, was "rafnixg-1.3.0.tar", last modified: Sat Apr 29 04:30:55 2023, max compression
```

## Comparing `rafnixg-1.2.0.tar` & `rafnixg-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rafnixg   (1000) rafnixg   (1000)        0 2023-04-29 04:09:19.547654 rafnixg-1.2.0/
--rw-r--r--   0 rafnixg   (1000) rafnixg   (1000)     1095 2023-04-29 03:45:28.000000 rafnixg-1.2.0/LICENSE
--rw-r--r--   0 rafnixg   (1000) rafnixg   (1000)     1986 2023-04-29 04:09:19.547654 rafnixg-1.2.0/PKG-INFO
--rw-r--r--   0 rafnixg   (1000) rafnixg   (1000)      242 2023-04-29 01:43:35.000000 rafnixg-1.2.0/README.md
--rw-r--r--   0 rafnixg   (1000) rafnixg   (1000)     1168 2023-04-29 04:09:04.000000 rafnixg-1.2.0/pyproject.toml
--rw-r--r--   0 rafnixg   (1000) rafnixg   (1000)       38 2023-04-29 04:09:19.547654 rafnixg-1.2.0/setup.cfg
-drwxr-xr-x   0 rafnixg   (1000) rafnixg   (1000)        0 2023-04-29 04:09:19.543655 rafnixg-1.2.0/src/
-drwxr-xr-x   0 rafnixg   (1000) rafnixg   (1000)        0 2023-04-29 04:09:19.547654 rafnixg-1.2.0/src/rafnixg/
--rw-r--r--   0 rafnixg   (1000) rafnixg   (1000)       89 2023-04-29 04:09:04.000000 rafnixg-1.2.0/src/rafnixg/__init__.py
--rw-r--r--   0 rafnixg   (1000) rafnixg   (1000)      147 2023-04-29 03:57:33.000000 rafnixg-1.2.0/src/rafnixg/__main__.py
--rw-r--r--   0 rafnixg   (1000) rafnixg   (1000)     2352 2023-04-29 03:30:40.000000 rafnixg-1.2.0/src/rafnixg/rafnixg.py
-drwxr-xr-x   0 rafnixg   (1000) rafnixg   (1000)        0 2023-04-29 04:09:19.547654 rafnixg-1.2.0/src/rafnixg.egg-info/
--rw-r--r--   0 rafnixg   (1000) rafnixg   (1000)     1986 2023-04-29 04:09:19.000000 rafnixg-1.2.0/src/rafnixg.egg-info/PKG-INFO
--rw-r--r--   0 rafnixg   (1000) rafnixg   (1000)      315 2023-04-29 04:09:19.000000 rafnixg-1.2.0/src/rafnixg.egg-info/SOURCES.txt
--rw-r--r--   0 rafnixg   (1000) rafnixg   (1000)        1 2023-04-29 04:09:19.000000 rafnixg-1.2.0/src/rafnixg.egg-info/dependency_links.txt
--rw-r--r--   0 rafnixg   (1000) rafnixg   (1000)       50 2023-04-29 04:09:19.000000 rafnixg-1.2.0/src/rafnixg.egg-info/entry_points.txt
--rw-r--r--   0 rafnixg   (1000) rafnixg   (1000)       49 2023-04-29 04:09:19.000000 rafnixg-1.2.0/src/rafnixg.egg-info/requires.txt
--rw-r--r--   0 rafnixg   (1000) rafnixg   (1000)        8 2023-04-29 04:09:19.000000 rafnixg-1.2.0/src/rafnixg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:30:55.688943 rafnixg-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-29 04:30:42.000000 rafnixg-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-29 04:30:55.688943 rafnixg-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-29 04:30:42.000000 rafnixg-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-29 04:30:42.000000 rafnixg-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 04:30:55.688943 rafnixg-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:30:55.684943 rafnixg-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:30:55.684943 rafnixg-1.3.0/src/rafnixg/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-29 04:30:42.000000 rafnixg-1.3.0/src/rafnixg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-29 04:30:42.000000 rafnixg-1.3.0/src/rafnixg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-29 04:30:42.000000 rafnixg-1.3.0/src/rafnixg/rafnixg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:30:55.688943 rafnixg-1.3.0/src/rafnixg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-29 04:30:55.000000 rafnixg-1.3.0/src/rafnixg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-29 04:30:55.000000 rafnixg-1.3.0/src/rafnixg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 04:30:55.000000 rafnixg-1.3.0/src/rafnixg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-29 04:30:55.000000 rafnixg-1.3.0/src/rafnixg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-29 04:30:55.000000 rafnixg-1.3.0/src/rafnixg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 04:30:55.000000 rafnixg-1.3.0/src/rafnixg.egg-info/top_level.txt
```

### Comparing `rafnixg-1.2.0/LICENSE` & `rafnixg-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rafnixg-1.2.0/PKG-INFO` & `rafnixg-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rafnixg
-Version: 1.2.0
+Version: 1.3.0
 Summary: Rafnix Guzman Personal Card
 Author-email: Rafnix Guzman <rafnixg@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Rafnix Gabriel Guzmán García @rafnixg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rafnixg-1.2.0/pyproject.toml` & `rafnixg-1.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rafnixg"
-version = "1.2.0"
+version = "1.3.0"
 description = "Rafnix Guzman Personal Card"
 readme = "README.md"
 authors = [{ name = "Rafnix Guzman", email = "rafnixg@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -25,15 +25,15 @@
 
 [project.urls]
 Homepage = "https://github.com/rafnixg/rafnixg-lib"
 
 [project.scripts]
 rafnixg = "rafnixg.__main__:main"
 [tool.bumpver]
-current_version = "1.2.0"
+current_version = "1.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `rafnixg-1.2.0/src/rafnixg/rafnixg.py` & `rafnixg-1.3.0/src/rafnixg/rafnixg.py`

 * *Files identical despite different names*

### Comparing `rafnixg-1.2.0/src/rafnixg.egg-info/PKG-INFO` & `rafnixg-1.3.0/src/rafnixg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rafnixg
-Version: 1.2.0
+Version: 1.3.0
 Summary: Rafnix Guzman Personal Card
 Author-email: Rafnix Guzman <rafnixg@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Rafnix Gabriel Guzmán García @rafnixg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


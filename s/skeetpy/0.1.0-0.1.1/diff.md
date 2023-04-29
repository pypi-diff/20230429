# Comparing `tmp/skeetpy-0.1.0.tar.gz` & `tmp/skeetpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skeetpy-0.1.0.tar", last modified: Sat Apr 29 20:38:10 2023, max compression
+gzip compressed data, was "skeetpy-0.1.1.tar", last modified: Sat Apr 29 21:31:01 2023, max compression
```

## Comparing `skeetpy-0.1.0.tar` & `skeetpy-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-04-29 01:52:08.346256 skeetpy-0.1.0/LICENSE
--rw-r--r--   0        0        0      190 2023-04-29 03:00:45.017490 skeetpy-0.1.0/README.md
--rw-r--r--   0        0        0      392 2023-04-29 03:10:57.364038 skeetpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      350 2023-04-29 20:37:19.318277 skeetpy-0.1.0/requirements.txt
--rw-r--r--   0        0        0    37579 2023-04-29 20:34:37.459873 skeetpy-0.1.0/skeetpy.py
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 skeetpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-29 01:52:08.346256 skeetpy-0.1.1/LICENSE
+-rw-r--r--   0        0        0      190 2023-04-29 03:00:45.017490 skeetpy-0.1.1/README.md
+-rw-r--r--   0        0        0      392 2023-04-29 03:10:57.364038 skeetpy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      350 2023-04-29 20:37:19.318277 skeetpy-0.1.1/requirements.txt
+-rw-r--r--   0        0        0    37579 2023-04-29 21:30:45.439645 skeetpy-0.1.1/skeetpy.py
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 skeetpy-0.1.1/PKG-INFO
```

### Comparing `skeetpy-0.1.0/LICENSE` & `skeetpy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skeetpy-0.1.0/skeetpy.py` & `skeetpy-0.1.1/skeetpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """Skeetpy is a Python library for interacting with the AT protocol."""
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 import requests
 import json
 import jwt
 import time
 import os
 import sys
```

### Comparing `skeetpy-0.1.0/PKG-INFO` & `skeetpy-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeetpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Skeetpy is a Python library for interacting with the AT protocol.
 Author-email: Yves Junqueira <yves.junqueira@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/nictuku/skeetpy
 
 # skeetpy
```


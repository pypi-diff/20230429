# Comparing `tmp/malla-0.1.2.tar.gz` & `tmp/malla-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malla-0.1.2.tar", max compression
+gzip compressed data, was "malla-0.1.3.tar", max compression
```

## Comparing `malla-0.1.2.tar` & `malla-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      526 2023-04-29 16:35:40.386927 malla-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.2/malla/__init__.py
--rw-r--r--   0        0        0     6383 2023-04-29 15:54:17.906880 malla-0.1.2/malla/directed_edge.py
--rw-r--r--   0        0        0      717 2023-04-29 16:00:39.890220 malla-0.1.2/malla/off.py
--rw-r--r--   0        0        0      266 2023-04-29 16:38:59.130263 malla-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 malla-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      526 2023-04-29 16:35:40.386927 malla-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.3/malla/__init__.py
+-rw-r--r--   0        0        0     6389 2023-04-29 16:49:03.813608 malla-0.1.3/malla/directed_edge.py
+-rw-r--r--   0        0        0      717 2023-04-29 16:00:39.890220 malla-0.1.3/malla/off.py
+-rw-r--r--   0        0        0      266 2023-04-29 16:49:30.586942 malla-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 malla-0.1.3/PKG-INFO
```

### Comparing `malla-0.1.2/README.md` & `malla-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `malla-0.1.2/malla/directed_edge.py` & `malla-0.1.3/malla/directed_edge.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 vertex
     a class representing a single mesh vertex
 half_edge
     a class representing a single half edge
 """
 
 from dataclasses import dataclass
-from typing import Generator
-
+from typing import Generator, Tuple
 @dataclass
 class vertex:
     """
     A class representing a mesh vertex
 
     Attributes
     ----------
```

### Comparing `malla-0.1.2/malla/off.py` & `malla-0.1.3/malla/off.py`

 * *Files identical despite different names*

### Comparing `malla-0.1.2/PKG-INFO` & `malla-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malla
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Dimas Martínez
 Author-email: dimas@ufam.edu.br
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


# Comparing `tmp/gslconsts-1.1.0.tar.gz` & `tmp/gslconsts-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gslconsts-1.1.0.tar", last modified: Wed Apr 26 15:00:04 2023, max compression
+gzip compressed data, was "gslconsts-1.1.1.tar", last modified: Fri Apr 28 22:41:51 2023, max compression
```

## Comparing `gslconsts-1.1.0.tar` & `gslconsts-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-26 15:00:04.898164 gslconsts-1.1.0/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    35147 2023-01-12 16:19:56.000000 gslconsts-1.1.0/LICENSE.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      257 2023-04-26 14:59:35.000000 gslconsts-1.1.0/MANIFEST.in
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1757 2023-04-26 15:00:04.898469 gslconsts-1.1.0/PKG-INFO
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      953 2023-01-12 21:02:04.000000 gslconsts-1.1.0/README.rst
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-26 15:00:04.890851 gslconsts-1.1.0/gslconsts/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      279 2023-04-26 14:55:49.000000 gslconsts-1.1.0/gslconsts/__about__.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      126 2023-04-26 14:55:49.000000 gslconsts-1.1.0/gslconsts/__init__.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    32503 2023-04-26 14:59:50.000000 gslconsts-1.1.0/gslconsts/consts.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1593 2023-04-26 14:59:50.000000 gslconsts-1.1.0/gslconsts/math.py
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-26 15:00:04.896968 gslconsts-1.1.0/gslconsts.egg-info/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1757 2023-04-26 15:00:04.000000 gslconsts-1.1.0/gslconsts.egg-info/PKG-INFO
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      300 2023-04-26 15:00:04.000000 gslconsts-1.1.0/gslconsts.egg-info/SOURCES.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        1 2023-04-26 15:00:04.000000 gslconsts-1.1.0/gslconsts.egg-info/dependency_links.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       39 2023-04-26 15:00:04.000000 gslconsts-1.1.0/gslconsts.egg-info/requires.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       10 2023-04-26 15:00:04.000000 gslconsts-1.1.0/gslconsts.egg-info/top_level.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      107 2023-04-26 15:00:04.899657 gslconsts-1.1.0/setup.cfg
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     6062 2023-01-12 21:02:04.000000 gslconsts-1.1.0/setup.py
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-28 22:41:51.268635 gslconsts-1.1.1/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    35147 2023-01-12 16:19:56.000000 gslconsts-1.1.1/LICENSE.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      257 2023-04-26 14:59:35.000000 gslconsts-1.1.1/MANIFEST.in
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1757 2023-04-28 22:41:51.268918 gslconsts-1.1.1/PKG-INFO
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      953 2023-01-12 21:02:04.000000 gslconsts-1.1.1/README.rst
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-28 22:41:51.260420 gslconsts-1.1.1/gslconsts/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      279 2023-04-28 22:41:26.000000 gslconsts-1.1.1/gslconsts/__about__.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      126 2023-04-26 14:55:49.000000 gslconsts-1.1.1/gslconsts/__init__.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    32503 2023-04-28 22:41:32.000000 gslconsts-1.1.1/gslconsts/consts.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1593 2023-04-28 22:41:32.000000 gslconsts-1.1.1/gslconsts/math.py
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-28 22:41:51.267336 gslconsts-1.1.1/gslconsts.egg-info/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1757 2023-04-28 22:41:51.000000 gslconsts-1.1.1/gslconsts.egg-info/PKG-INFO
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      300 2023-04-28 22:41:51.000000 gslconsts-1.1.1/gslconsts.egg-info/SOURCES.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        1 2023-04-28 22:41:51.000000 gslconsts-1.1.1/gslconsts.egg-info/dependency_links.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       39 2023-04-28 22:41:51.000000 gslconsts-1.1.1/gslconsts.egg-info/requires.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       10 2023-04-28 22:41:51.000000 gslconsts-1.1.1/gslconsts.egg-info/top_level.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      107 2023-04-28 22:41:51.270042 gslconsts-1.1.1/setup.cfg
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     6062 2023-01-12 21:02:04.000000 gslconsts-1.1.1/setup.py
```

### Comparing `gslconsts-1.1.0/LICENSE.txt` & `gslconsts-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gslconsts-1.1.0/PKG-INFO` & `gslconsts-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gslconsts
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python project GNU Scientific Library (GSL) constants
 Home-page: https://github.com/mbradle/gslconsts
 Author: Clemson University
 Author-email: mbradle@g.clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/mbradle/gslconsts/issues
 Project-URL: Source, https://github.com/mbradle/gslconsts/
```

### Comparing `gslconsts-1.1.0/README.rst` & `gslconsts-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `gslconsts-1.1.0/gslconsts/consts.py` & `gslconsts-1.1.1/gslconsts/consts.py`

 * *Files identical despite different names*

### Comparing `gslconsts-1.1.0/gslconsts/math.py` & `gslconsts-1.1.1/gslconsts/math.py`

 * *Files identical despite different names*

### Comparing `gslconsts-1.1.0/gslconsts.egg-info/PKG-INFO` & `gslconsts-1.1.1/gslconsts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gslconsts
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python project GNU Scientific Library (GSL) constants
 Home-page: https://github.com/mbradle/gslconsts
 Author: Clemson University
 Author-email: mbradle@g.clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/mbradle/gslconsts/issues
 Project-URL: Source, https://github.com/mbradle/gslconsts/
```

### Comparing `gslconsts-1.1.0/setup.py` & `gslconsts-1.1.1/setup.py`

 * *Files identical despite different names*


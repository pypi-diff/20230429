# Comparing `tmp/highdicom-0.9.1.tar.gz` & `tmp/highdicom-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highdicom-0.9.1.tar", last modified: Tue Sep 14 21:20:03 2021, max compression
+gzip compressed data, was "highdicom-0.9.2.tar", last modified: Tue Sep 21 05:54:53 2021, max compression
```

## Comparing `highdicom-0.9.1.tar` & `highdicom-0.9.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-14 21:20:03.612493 highdicom-0.9.1/
--rw-r--r--   0 mdherrmann   (501) staff       (20)     1067 2020-02-02 01:38:35.000000 highdicom-0.9.1/LICENSE
--rw-r--r--   0 mdherrmann   (501) staff       (20)      137 2020-02-19 18:31:41.000000 highdicom-0.9.1/MANIFEST.in
--rw-r--r--   0 mdherrmann   (501) staff       (20)      977 2021-09-14 21:20:03.612637 highdicom-0.9.1/PKG-INFO
--rw-r--r--   0 mdherrmann   (501) staff       (20)     2132 2021-08-06 16:28:03.000000 highdicom-0.9.1/README.md
--rw-r--r--   0 mdherrmann   (501) staff       (20)      322 2021-09-14 21:20:03.613567 highdicom-0.9.1/setup.cfg
--rw-r--r--   0 mdherrmann   (501) staff       (20)     1432 2021-08-31 21:42:09.000000 highdicom-0.9.1/setup.py
-drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-14 21:20:03.550449 highdicom-0.9.1/src/
-drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-14 21:20:03.597634 highdicom-0.9.1/src/highdicom/
--rw-r--r--   0 mdherrmann   (501) staff       (20)     1852 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/__init__.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)   363523 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/_iods.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)     6251 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/_module_utils.py
--rw-r--r--   0 mdherrmann   (501) staff       (20) 19919291 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/_modules.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)    11831 2021-08-31 21:50:04.000000 highdicom-0.9.1/src/highdicom/base.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)     3788 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/coding_schemes.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)     3117 2021-05-19 12:14:03.000000 highdicom-0.9.1/src/highdicom/color.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)    31380 2021-09-14 21:18:20.000000 highdicom-0.9.1/src/highdicom/content.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)     3470 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/enum.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)    11857 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/frame.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)    18582 2021-09-13 17:10:44.000000 highdicom-0.9.1/src/highdicom/io.py
-drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-14 21:20:03.599904 highdicom-0.9.1/src/highdicom/legacy/
--rw-r--r--   0 mdherrmann   (501) staff       (20)      612 2021-05-19 13:56:46.000000 highdicom-0.9.1/src/highdicom/legacy/__init__.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)    22017 2021-09-14 15:40:22.000000 highdicom-0.9.1/src/highdicom/legacy/sop.py
-drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-14 21:20:03.601560 highdicom-0.9.1/src/highdicom/pm/
--rw-r--r--   0 mdherrmann   (501) staff       (20)      348 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/pm/__init__.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)    14695 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/pm/content.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)    32281 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/pm/sop.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)      189 2020-04-26 00:53:37.000000 highdicom-0.9.1/src/highdicom/py.typed
-drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-14 21:20:03.603993 highdicom-0.9.1/src/highdicom/sc/
--rw-r--r--   0 mdherrmann   (501) staff       (20)      283 2021-05-19 13:56:46.000000 highdicom-0.9.1/src/highdicom/sc/__init__.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)      510 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/sc/enum.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)    23597 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/sc/sop.py
-drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-14 21:20:03.606843 highdicom-0.9.1/src/highdicom/seg/
--rw-r--r--   0 mdherrmann   (501) staff       (20)      856 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/seg/__init__.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)    21045 2021-09-14 15:39:47.000000 highdicom-0.9.1/src/highdicom/seg/content.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)     1059 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/seg/enum.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)   118583 2021-09-14 15:39:47.000000 highdicom-0.9.1/src/highdicom/seg/sop.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)     1820 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/seg/utils.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)    19605 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/spatial.py
-drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-14 21:20:03.611958 highdicom-0.9.1/src/highdicom/sr/
--rw-r--r--   0 mdherrmann   (501) staff       (20)     4627 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/sr/__init__.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)     4610 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/sr/coding.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)    52791 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/sr/content.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)     6420 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/sr/enum.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)    34077 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/sr/sop.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)   148734 2021-09-14 15:40:22.000000 highdicom-0.9.1/src/highdicom/sr/templates.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)     5593 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/sr/utils.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)    66992 2021-09-14 21:18:20.000000 highdicom-0.9.1/src/highdicom/sr/value_types.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)      495 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/uid.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)     8279 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/utils.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)     2539 2021-08-31 21:42:09.000000 highdicom-0.9.1/src/highdicom/valuerep.py
--rw-r--r--   0 mdherrmann   (501) staff       (20)       22 2021-09-14 21:18:43.000000 highdicom-0.9.1/src/highdicom/version.py
-drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-14 21:20:03.599161 highdicom-0.9.1/src/highdicom.egg-info/
--rw-r--r--   0 mdherrmann   (501) staff       (20)      977 2021-09-14 21:20:03.000000 highdicom-0.9.1/src/highdicom.egg-info/PKG-INFO
--rw-r--r--   0 mdherrmann   (501) staff       (20)     1226 2021-09-14 21:20:03.000000 highdicom-0.9.1/src/highdicom.egg-info/SOURCES.txt
--rw-r--r--   0 mdherrmann   (501) staff       (20)        1 2021-09-14 21:20:03.000000 highdicom-0.9.1/src/highdicom.egg-info/dependency_links.txt
--rw-r--r--   0 mdherrmann   (501) staff       (20)       39 2021-09-14 21:20:03.000000 highdicom-0.9.1/src/highdicom.egg-info/requires.txt
--rw-r--r--   0 mdherrmann   (501) staff       (20)       10 2021-09-14 21:20:03.000000 highdicom-0.9.1/src/highdicom.egg-info/top_level.txt
+drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-21 05:54:53.617742 highdicom-0.9.2/
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     1067 2020-02-02 01:38:35.000000 highdicom-0.9.2/LICENSE
+-rw-r--r--   0 mdherrmann   (501) staff       (20)      137 2020-02-19 18:31:41.000000 highdicom-0.9.2/MANIFEST.in
+-rw-r--r--   0 mdherrmann   (501) staff       (20)      977 2021-09-21 05:54:53.617969 highdicom-0.9.2/PKG-INFO
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     2132 2021-08-06 16:28:03.000000 highdicom-0.9.2/README.md
+-rw-r--r--   0 mdherrmann   (501) staff       (20)      322 2021-09-21 05:54:53.618941 highdicom-0.9.2/setup.cfg
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     1432 2021-08-31 21:42:09.000000 highdicom-0.9.2/setup.py
+drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-21 05:54:53.552821 highdicom-0.9.2/src/
+drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-21 05:54:53.602473 highdicom-0.9.2/src/highdicom/
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     1852 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/__init__.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)   363523 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/_iods.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     6251 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/_module_utils.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20) 19919291 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/_modules.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)    11831 2021-08-31 21:50:04.000000 highdicom-0.9.2/src/highdicom/base.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     3788 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/coding_schemes.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     3117 2021-05-19 12:14:03.000000 highdicom-0.9.2/src/highdicom/color.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)    31386 2021-09-21 05:48:56.000000 highdicom-0.9.2/src/highdicom/content.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     3470 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/enum.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)    11857 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/frame.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)    18582 2021-09-13 17:10:44.000000 highdicom-0.9.2/src/highdicom/io.py
+drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-21 05:54:53.605282 highdicom-0.9.2/src/highdicom/legacy/
+-rw-r--r--   0 mdherrmann   (501) staff       (20)      612 2021-05-19 13:56:46.000000 highdicom-0.9.2/src/highdicom/legacy/__init__.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)    22196 2021-09-21 05:48:56.000000 highdicom-0.9.2/src/highdicom/legacy/sop.py
+drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-21 05:54:53.606906 highdicom-0.9.2/src/highdicom/pm/
+-rw-r--r--   0 mdherrmann   (501) staff       (20)      348 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/pm/__init__.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)    14695 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/pm/content.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)    32281 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/pm/sop.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)      189 2020-04-26 00:53:37.000000 highdicom-0.9.2/src/highdicom/py.typed
+drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-21 05:54:53.608420 highdicom-0.9.2/src/highdicom/sc/
+-rw-r--r--   0 mdherrmann   (501) staff       (20)      283 2021-05-19 13:56:46.000000 highdicom-0.9.2/src/highdicom/sc/__init__.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)      510 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/sc/enum.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)    23597 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/sc/sop.py
+drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-21 05:54:53.611287 highdicom-0.9.2/src/highdicom/seg/
+-rw-r--r--   0 mdherrmann   (501) staff       (20)      856 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/seg/__init__.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)    21045 2021-09-14 15:39:47.000000 highdicom-0.9.2/src/highdicom/seg/content.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     1059 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/seg/enum.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)   118583 2021-09-14 15:39:47.000000 highdicom-0.9.2/src/highdicom/seg/sop.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     1820 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/seg/utils.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)    19605 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/spatial.py
+drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-21 05:54:53.617200 highdicom-0.9.2/src/highdicom/sr/
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     4627 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/sr/__init__.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     4610 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/sr/coding.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)    52791 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/sr/content.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     6420 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/sr/enum.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)    34077 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/sr/sop.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)   148734 2021-09-14 15:40:22.000000 highdicom-0.9.2/src/highdicom/sr/templates.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     5593 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/sr/utils.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)    66992 2021-09-14 21:18:20.000000 highdicom-0.9.2/src/highdicom/sr/value_types.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)      495 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/uid.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     8279 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/utils.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     2539 2021-08-31 21:42:09.000000 highdicom-0.9.2/src/highdicom/valuerep.py
+-rw-r--r--   0 mdherrmann   (501) staff       (20)       22 2021-09-21 05:49:09.000000 highdicom-0.9.2/src/highdicom/version.py
+drwxr-xr-x   0 mdherrmann   (501) staff       (20)        0 2021-09-21 05:54:53.604560 highdicom-0.9.2/src/highdicom.egg-info/
+-rw-r--r--   0 mdherrmann   (501) staff       (20)      977 2021-09-21 05:54:53.000000 highdicom-0.9.2/src/highdicom.egg-info/PKG-INFO
+-rw-r--r--   0 mdherrmann   (501) staff       (20)     1226 2021-09-21 05:54:53.000000 highdicom-0.9.2/src/highdicom.egg-info/SOURCES.txt
+-rw-r--r--   0 mdherrmann   (501) staff       (20)        1 2021-09-21 05:54:53.000000 highdicom-0.9.2/src/highdicom.egg-info/dependency_links.txt
+-rw-r--r--   0 mdherrmann   (501) staff       (20)       39 2021-09-21 05:54:53.000000 highdicom-0.9.2/src/highdicom.egg-info/requires.txt
+-rw-r--r--   0 mdherrmann   (501) staff       (20)       10 2021-09-21 05:54:53.000000 highdicom-0.9.2/src/highdicom.egg-info/top_level.txt
```

### Comparing `highdicom-0.9.1/LICENSE` & `highdicom-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/PKG-INFO` & `highdicom-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highdicom
-Version: 0.9.1
+Version: 0.9.2
 Summary: High-level DICOM abstractions.
 Home-page: https://github.com/mghcomputationalpathology/highdicom
 Author: Markus D. Herrmann
 Maintainer: Markus D. Herrmann
 License: MIT
 Platform: Linux
 Platform: MacOS
```

### Comparing `highdicom-0.9.1/README.md` & `highdicom-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/setup.py` & `highdicom-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/__init__.py` & `highdicom-0.9.2/src/highdicom/__init__.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/_iods.py` & `highdicom-0.9.2/src/highdicom/_iods.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/_module_utils.py` & `highdicom-0.9.2/src/highdicom/_module_utils.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/_modules.py` & `highdicom-0.9.2/src/highdicom/_modules.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/base.py` & `highdicom-0.9.2/src/highdicom/base.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/coding_schemes.py` & `highdicom-0.9.2/src/highdicom/coding_schemes.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/color.py` & `highdicom-0.9.2/src/highdicom/color.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/content.py` & `highdicom-0.9.2/src/highdicom/content.py`

 * *Files 1% similar despite different names*

```diff
@@ -768,15 +768,15 @@
             tissue_fixative_item = CodeContentItem(
                 name=codes.SCT.TissueFixative,
                 value=fixative
             )
             self.append(tissue_fixative_item)
         if embedding_medium is not None:
             embedding_medium_item = CodeContentItem(
-                name=codes.SCT.EmbeddingMedium,
+                name=codes.SCT.TissueEmbeddingMedium,
                 value=embedding_medium
             )
             self.append(embedding_medium_item)
 
 
 class SpecimenDescription(Dataset):
```

### Comparing `highdicom-0.9.1/src/highdicom/enum.py` & `highdicom-0.9.2/src/highdicom/enum.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/frame.py` & `highdicom-0.9.2/src/highdicom/frame.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/io.py` & `highdicom-0.9.2/src/highdicom/io.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/legacy/__init__.py` & `highdicom-0.9.2/src/highdicom/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/legacy/sop.py` & `highdicom-0.9.2/src/highdicom/legacy/sop.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,18 @@
                 frame_type.append('NONE')
             else:
                 logger.warn('unknown derived pixel contrast')
                 frame_type.append('OTHER')
         unique_image_types.add(tuple(frame_type))
         frame_type_item = Dataset()
         frame_type_item.FrameType = frame_type
-        frame_type_item.PixelRepresentation = pixel_representation
+        if pixel_representation == 0:
+          frame_type_item.PixelPresentation = 'MONOCHROME'
+        else:
+          frame_type_item.PixelPresentation = 'COLOR'
         frame_type_item.VolumetricProperties = volumetric_properties
         if frame_type[0] == 'ORIGINAL':
             frame_type_item.VolumeBasedCalculationTechnique = 'NONE'
         else:
             frame_type_item.VolumeBasedCalculationTechnique = 'MIXED'
 
         if sop_class_uid == '1.2.840.10008.5.1.4.1.1.4.4':
@@ -331,15 +334,18 @@
         else:
             for i, da in enumerate(dataelements):
                 unassigned_perframe_ca_items[i].add(da)
 
     mf_dataset.ImageType = list(list(unique_image_types)[0])
     if len(unique_image_types) > 1:
         mf_dataset.ImageType[2] = 'MIXED'
-    mf_dataset.PixelRepresentation = pixel_representation
+    if pixel_representation == 0:
+      mf_dataset.PixelPresentation = 'MONOCHROME'
+    else:
+      mf_dataset.PixelPresentation = 'COLOR'
     mf_dataset.VolumetricProperties = volumetric_properties
 
     # Shared Functional Groups
     shared_item = Dataset()
 
     # Pixel Measures (M)
     pixel_measures_item = Dataset()
```

### Comparing `highdicom-0.9.1/src/highdicom/pm/content.py` & `highdicom-0.9.2/src/highdicom/pm/content.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/pm/sop.py` & `highdicom-0.9.2/src/highdicom/pm/sop.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/sc/sop.py` & `highdicom-0.9.2/src/highdicom/sc/sop.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/seg/__init__.py` & `highdicom-0.9.2/src/highdicom/seg/__init__.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/seg/content.py` & `highdicom-0.9.2/src/highdicom/seg/content.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/seg/enum.py` & `highdicom-0.9.2/src/highdicom/seg/enum.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/seg/sop.py` & `highdicom-0.9.2/src/highdicom/seg/sop.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/seg/utils.py` & `highdicom-0.9.2/src/highdicom/seg/utils.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/spatial.py` & `highdicom-0.9.2/src/highdicom/spatial.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/sr/__init__.py` & `highdicom-0.9.2/src/highdicom/sr/__init__.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/sr/coding.py` & `highdicom-0.9.2/src/highdicom/sr/coding.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/sr/content.py` & `highdicom-0.9.2/src/highdicom/sr/content.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/sr/enum.py` & `highdicom-0.9.2/src/highdicom/sr/enum.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/sr/sop.py` & `highdicom-0.9.2/src/highdicom/sr/sop.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/sr/templates.py` & `highdicom-0.9.2/src/highdicom/sr/templates.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/sr/utils.py` & `highdicom-0.9.2/src/highdicom/sr/utils.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/sr/value_types.py` & `highdicom-0.9.2/src/highdicom/sr/value_types.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/utils.py` & `highdicom-0.9.2/src/highdicom/utils.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom/valuerep.py` & `highdicom-0.9.2/src/highdicom/valuerep.py`

 * *Files identical despite different names*

### Comparing `highdicom-0.9.1/src/highdicom.egg-info/PKG-INFO` & `highdicom-0.9.2/src/highdicom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highdicom
-Version: 0.9.1
+Version: 0.9.2
 Summary: High-level DICOM abstractions.
 Home-page: https://github.com/mghcomputationalpathology/highdicom
 Author: Markus D. Herrmann
 Maintainer: Markus D. Herrmann
 License: MIT
 Platform: Linux
 Platform: MacOS
```

### Comparing `highdicom-0.9.1/src/highdicom.egg-info/SOURCES.txt` & `highdicom-0.9.2/src/highdicom.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/cocojamboo-2.0.8.tar.gz` & `tmp/cocojamboo-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocojamboo-2.0.8.tar", last modified: Sat Apr 29 09:38:26 2023, max compression
+gzip compressed data, was "cocojamboo-2.0.9.tar", last modified: Sat Apr 29 09:42:07 2023, max compression
```

## Comparing `cocojamboo-2.0.8.tar` & `cocojamboo-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:38:26.952811 cocojamboo-2.0.8/
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)    19334 2023-01-10 14:44:25.000000 cocojamboo-2.0.8/LICENSE
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 09:38:26.952276 cocojamboo-2.0.8/PKG-INFO
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)      122 2023-03-31 12:26:52.000000 cocojamboo-2.0.8/README.md
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:38:26.948549 cocojamboo-2.0.8/cocojamboo/
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)       87 2023-04-29 09:28:42.000000 cocojamboo-2.0.8/cocojamboo/__init__.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    52494 2023-04-29 09:37:26.000000 cocojamboo-2.0.8/cocojamboo/coco_eval2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     8893 2023-02-17 12:32:17.000000 cocojamboo-2.0.8/cocojamboo/coco_utils.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    45829 2023-04-29 07:00:48.000000 cocojamboo-2.0.8/cocojamboo/cocoeval2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     4562 2023-04-29 09:03:23.000000 cocojamboo-2.0.8/cocojamboo/engine2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23337 2023-02-17 12:32:17.000000 cocojamboo-2.0.8/cocojamboo/transforms.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     8388 2023-02-17 12:32:17.000000 cocojamboo-2.0.8/cocojamboo/utils.py
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:38:26.951015 cocojamboo-2.0.8/cocojamboo.egg-info/
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 09:38:26.000000 cocojamboo-2.0.8/cocojamboo.egg-info/PKG-INFO
--rw-r--r--   0 georgianamanolache   (501) staff       (20)      332 2023-04-29 09:38:26.000000 cocojamboo-2.0.8/cocojamboo.egg-info/SOURCES.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)        1 2023-04-29 09:38:26.000000 cocojamboo-2.0.8/cocojamboo.egg-info/dependency_links.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)       11 2023-04-29 09:38:26.000000 cocojamboo-2.0.8/cocojamboo.egg-info/top_level.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)      670 2023-04-29 09:31:39.000000 cocojamboo-2.0.8/pyproject.toml
--rw-r--r--   0 georgianamanolache   (501) staff       (20)       38 2023-04-29 09:38:26.952919 cocojamboo-2.0.8/setup.cfg
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:42:07.472917 cocojamboo-2.0.9/
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)    19334 2023-01-10 14:44:25.000000 cocojamboo-2.0.9/LICENSE
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 09:42:07.472590 cocojamboo-2.0.9/PKG-INFO
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)      122 2023-03-31 12:26:52.000000 cocojamboo-2.0.9/README.md
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:42:07.469785 cocojamboo-2.0.9/cocojamboo/
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)       87 2023-04-29 09:41:32.000000 cocojamboo-2.0.9/cocojamboo/__init__.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    52494 2023-04-29 09:37:26.000000 cocojamboo-2.0.9/cocojamboo/coco_eval2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     8893 2023-02-17 12:32:17.000000 cocojamboo-2.0.9/cocojamboo/coco_utils.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    45829 2023-04-29 07:00:48.000000 cocojamboo-2.0.9/cocojamboo/cocoeval2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     4562 2023-04-29 09:03:23.000000 cocojamboo-2.0.9/cocojamboo/engine2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23337 2023-02-17 12:32:17.000000 cocojamboo-2.0.9/cocojamboo/transforms.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     8388 2023-02-17 12:32:17.000000 cocojamboo-2.0.9/cocojamboo/utils.py
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:42:07.471929 cocojamboo-2.0.9/cocojamboo.egg-info/
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 09:42:07.000000 cocojamboo-2.0.9/cocojamboo.egg-info/PKG-INFO
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)      332 2023-04-29 09:42:07.000000 cocojamboo-2.0.9/cocojamboo.egg-info/SOURCES.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)        1 2023-04-29 09:42:07.000000 cocojamboo-2.0.9/cocojamboo.egg-info/dependency_links.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)       11 2023-04-29 09:42:07.000000 cocojamboo-2.0.9/cocojamboo.egg-info/top_level.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)      670 2023-04-29 09:41:42.000000 cocojamboo-2.0.9/pyproject.toml
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)       38 2023-04-29 09:42:07.473003 cocojamboo-2.0.9/setup.cfg
```

### Comparing `cocojamboo-2.0.8/LICENSE` & `cocojamboo-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.8/PKG-INFO` & `cocojamboo-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocojamboo
-Version: 2.0.8
+Version: 2.0.9
 Summary: An extension to COCO evaluation metric to provide mAP scores with custom paramters.
 Author: Georgiana Manolache
 License: 
         Attribution-NonCommercial 4.0 International
         
         =======================================================================
```

### Comparing `cocojamboo-2.0.8/cocojamboo/coco_eval2.py` & `cocojamboo-2.0.9/cocojamboo/coco_eval2.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.8/cocojamboo/coco_utils.py` & `cocojamboo-2.0.9/cocojamboo/coco_utils.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.8/cocojamboo/cocoeval2.py` & `cocojamboo-2.0.9/cocojamboo/cocoeval2.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.8/cocojamboo/engine2.py` & `cocojamboo-2.0.9/cocojamboo/engine2.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.8/cocojamboo/transforms.py` & `cocojamboo-2.0.9/cocojamboo/transforms.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.8/cocojamboo/utils.py` & `cocojamboo-2.0.9/cocojamboo/utils.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.8/cocojamboo.egg-info/PKG-INFO` & `cocojamboo-2.0.9/cocojamboo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocojamboo
-Version: 2.0.8
+Version: 2.0.9
 Summary: An extension to COCO evaluation metric to provide mAP scores with custom paramters.
 Author: Georgiana Manolache
 License: 
         Attribution-NonCommercial 4.0 International
         
         =======================================================================
```

### Comparing `cocojamboo-2.0.8/pyproject.toml` & `cocojamboo-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "numpy", "wheel", "pycocotools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cocojamboo"
-version = "2.0.8"
+version = "2.0.9"
 description = "An extension to COCO evaluation metric to provide mAP scores with custom paramters."
 readme = "README.md"
 authors = [{ name = "Georgiana Manolache" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: Free for non-commercial use",
     "Programming Language :: Python",
```


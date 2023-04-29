# Comparing `tmp/cocojamboo-2.0.4.tar.gz` & `tmp/cocojamboo-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocojamboo-2.0.4.tar", last modified: Sat Apr 29 09:11:06 2023, max compression
+gzip compressed data, was "cocojamboo-2.0.5.tar", last modified: Sat Apr 29 09:15:29 2023, max compression
```

## Comparing `cocojamboo-2.0.4.tar` & `cocojamboo-2.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:11:06.795243 cocojamboo-2.0.4/
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)    19334 2023-01-10 14:44:25.000000 cocojamboo-2.0.4/LICENSE
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 09:11:06.794823 cocojamboo-2.0.4/PKG-INFO
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)      122 2023-03-31 12:26:52.000000 cocojamboo-2.0.4/README.md
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:11:06.791972 cocojamboo-2.0.4/cocojamboo/
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)       98 2023-04-29 09:10:25.000000 cocojamboo-2.0.4/cocojamboo/__init__.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     6638 2023-04-29 09:03:26.000000 cocojamboo-2.0.4/cocojamboo/coco_eval2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     8893 2023-02-17 12:32:17.000000 cocojamboo-2.0.4/cocojamboo/coco_utils.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    45829 2023-04-29 07:00:48.000000 cocojamboo-2.0.4/cocojamboo/cocoeval2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     4562 2023-04-29 09:03:23.000000 cocojamboo-2.0.4/cocojamboo/engine2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23337 2023-02-17 12:32:17.000000 cocojamboo-2.0.4/cocojamboo/transforms.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     8388 2023-02-17 12:32:17.000000 cocojamboo-2.0.4/cocojamboo/utils.py
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:11:06.794171 cocojamboo-2.0.4/cocojamboo.egg-info/
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 09:11:06.000000 cocojamboo-2.0.4/cocojamboo.egg-info/PKG-INFO
--rw-r--r--   0 georgianamanolache   (501) staff       (20)      332 2023-04-29 09:11:06.000000 cocojamboo-2.0.4/cocojamboo.egg-info/SOURCES.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)        1 2023-04-29 09:11:06.000000 cocojamboo-2.0.4/cocojamboo.egg-info/dependency_links.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)       11 2023-04-29 09:11:06.000000 cocojamboo-2.0.4/cocojamboo.egg-info/top_level.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)      661 2023-04-29 09:10:49.000000 cocojamboo-2.0.4/pyproject.toml
--rw-r--r--   0 georgianamanolache   (501) staff       (20)       38 2023-04-29 09:11:06.795348 cocojamboo-2.0.4/setup.cfg
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:15:29.316053 cocojamboo-2.0.5/
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)    19334 2023-01-10 14:44:25.000000 cocojamboo-2.0.5/LICENSE
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 09:15:29.315708 cocojamboo-2.0.5/PKG-INFO
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)      122 2023-03-31 12:26:52.000000 cocojamboo-2.0.5/README.md
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:15:29.313614 cocojamboo-2.0.5/cocojamboo/
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)      100 2023-04-29 09:14:12.000000 cocojamboo-2.0.5/cocojamboo/__init__.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     6638 2023-04-29 09:03:26.000000 cocojamboo-2.0.5/cocojamboo/coco_eval2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     8893 2023-02-17 12:32:17.000000 cocojamboo-2.0.5/cocojamboo/coco_utils.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    45829 2023-04-29 07:00:48.000000 cocojamboo-2.0.5/cocojamboo/cocoeval2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     4562 2023-04-29 09:03:23.000000 cocojamboo-2.0.5/cocojamboo/engine2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23337 2023-02-17 12:32:17.000000 cocojamboo-2.0.5/cocojamboo/transforms.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     8388 2023-02-17 12:32:17.000000 cocojamboo-2.0.5/cocojamboo/utils.py
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:15:29.314976 cocojamboo-2.0.5/cocojamboo.egg-info/
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 09:15:29.000000 cocojamboo-2.0.5/cocojamboo.egg-info/PKG-INFO
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)      332 2023-04-29 09:15:29.000000 cocojamboo-2.0.5/cocojamboo.egg-info/SOURCES.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)        1 2023-04-29 09:15:29.000000 cocojamboo-2.0.5/cocojamboo.egg-info/dependency_links.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)       11 2023-04-29 09:15:29.000000 cocojamboo-2.0.5/cocojamboo.egg-info/top_level.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)      661 2023-04-29 09:15:14.000000 cocojamboo-2.0.5/pyproject.toml
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)       38 2023-04-29 09:15:29.316160 cocojamboo-2.0.5/setup.cfg
```

### Comparing `cocojamboo-2.0.4/LICENSE` & `cocojamboo-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.4/PKG-INFO` & `cocojamboo-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocojamboo
-Version: 2.0.4
+Version: 2.0.5
 Summary: An extension to COCO evaluation metric to provide mAP scores with custom paramters.
 Author: Georgiana Manolache
 License: 
         Attribution-NonCommercial 4.0 International
         
         =======================================================================
```

### Comparing `cocojamboo-2.0.4/cocojamboo/coco_eval2.py` & `cocojamboo-2.0.5/cocojamboo/coco_eval2.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.4/cocojamboo/coco_utils.py` & `cocojamboo-2.0.5/cocojamboo/coco_utils.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.4/cocojamboo/cocoeval2.py` & `cocojamboo-2.0.5/cocojamboo/cocoeval2.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.4/cocojamboo/engine2.py` & `cocojamboo-2.0.5/cocojamboo/engine2.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.4/cocojamboo/transforms.py` & `cocojamboo-2.0.5/cocojamboo/transforms.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.4/cocojamboo/utils.py` & `cocojamboo-2.0.5/cocojamboo/utils.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.4/cocojamboo.egg-info/PKG-INFO` & `cocojamboo-2.0.5/cocojamboo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocojamboo
-Version: 2.0.4
+Version: 2.0.5
 Summary: An extension to COCO evaluation metric to provide mAP scores with custom paramters.
 Author: Georgiana Manolache
 License: 
         Attribution-NonCommercial 4.0 International
         
         =======================================================================
```

### Comparing `cocojamboo-2.0.4/pyproject.toml` & `cocojamboo-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "pycocotools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cocojamboo"
-version = "2.0.4"
+version = "2.0.5"
 description = "An extension to COCO evaluation metric to provide mAP scores with custom paramters."
 readme = "README.md"
 authors = [{ name = "Georgiana Manolache" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: Free for non-commercial use",
     "Programming Language :: Python",
```


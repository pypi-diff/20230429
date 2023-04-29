# Comparing `tmp/cocojamboo-2.0.6.tar.gz` & `tmp/cocojamboo-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocojamboo-2.0.6.tar", last modified: Sat Apr 29 09:19:52 2023, max compression
+gzip compressed data, was "cocojamboo-2.0.7.tar", last modified: Sat Apr 29 09:29:22 2023, max compression
```

## Comparing `cocojamboo-2.0.6.tar` & `cocojamboo-2.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:19:52.979005 cocojamboo-2.0.6/
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)    19334 2023-01-10 14:44:25.000000 cocojamboo-2.0.6/LICENSE
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 09:19:52.978426 cocojamboo-2.0.6/PKG-INFO
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)      122 2023-03-31 12:26:52.000000 cocojamboo-2.0.6/README.md
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:19:52.974876 cocojamboo-2.0.6/cocojamboo/
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)       98 2023-04-29 09:18:40.000000 cocojamboo-2.0.6/cocojamboo/__init__.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     6638 2023-04-29 09:03:26.000000 cocojamboo-2.0.6/cocojamboo/coco_eval2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     8893 2023-02-17 12:32:17.000000 cocojamboo-2.0.6/cocojamboo/coco_utils.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    45829 2023-04-29 07:00:48.000000 cocojamboo-2.0.6/cocojamboo/cocoeval2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     4562 2023-04-29 09:03:23.000000 cocojamboo-2.0.6/cocojamboo/engine2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23337 2023-02-17 12:32:17.000000 cocojamboo-2.0.6/cocojamboo/transforms.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     8388 2023-02-17 12:32:17.000000 cocojamboo-2.0.6/cocojamboo/utils.py
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:19:52.977466 cocojamboo-2.0.6/cocojamboo.egg-info/
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 09:19:52.000000 cocojamboo-2.0.6/cocojamboo.egg-info/PKG-INFO
--rw-r--r--   0 georgianamanolache   (501) staff       (20)      332 2023-04-29 09:19:52.000000 cocojamboo-2.0.6/cocojamboo.egg-info/SOURCES.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)        1 2023-04-29 09:19:52.000000 cocojamboo-2.0.6/cocojamboo.egg-info/dependency_links.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)       11 2023-04-29 09:19:52.000000 cocojamboo-2.0.6/cocojamboo.egg-info/top_level.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)      661 2023-04-29 09:18:56.000000 cocojamboo-2.0.6/pyproject.toml
--rw-r--r--   0 georgianamanolache   (501) staff       (20)       38 2023-04-29 09:19:52.979111 cocojamboo-2.0.6/setup.cfg
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:29:22.901368 cocojamboo-2.0.7/
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)    19334 2023-01-10 14:44:25.000000 cocojamboo-2.0.7/LICENSE
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 09:29:22.900651 cocojamboo-2.0.7/PKG-INFO
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)      122 2023-03-31 12:26:52.000000 cocojamboo-2.0.7/README.md
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:29:22.896309 cocojamboo-2.0.7/cocojamboo/
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)       87 2023-04-29 09:28:42.000000 cocojamboo-2.0.7/cocojamboo/__init__.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     6665 2023-04-29 09:28:35.000000 cocojamboo-2.0.7/cocojamboo/coco_eval2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     8893 2023-02-17 12:32:17.000000 cocojamboo-2.0.7/cocojamboo/coco_utils.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    45829 2023-04-29 07:00:48.000000 cocojamboo-2.0.7/cocojamboo/cocoeval2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     4562 2023-04-29 09:03:23.000000 cocojamboo-2.0.7/cocojamboo/engine2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23337 2023-02-17 12:32:17.000000 cocojamboo-2.0.7/cocojamboo/transforms.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     8388 2023-02-17 12:32:17.000000 cocojamboo-2.0.7/cocojamboo/utils.py
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:29:22.899756 cocojamboo-2.0.7/cocojamboo.egg-info/
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 09:29:22.000000 cocojamboo-2.0.7/cocojamboo.egg-info/PKG-INFO
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)      332 2023-04-29 09:29:22.000000 cocojamboo-2.0.7/cocojamboo.egg-info/SOURCES.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)        1 2023-04-29 09:29:22.000000 cocojamboo-2.0.7/cocojamboo.egg-info/dependency_links.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)       11 2023-04-29 09:29:22.000000 cocojamboo-2.0.7/cocojamboo.egg-info/top_level.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)      661 2023-04-29 09:29:04.000000 cocojamboo-2.0.7/pyproject.toml
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)       38 2023-04-29 09:29:22.901649 cocojamboo-2.0.7/setup.cfg
```

### Comparing `cocojamboo-2.0.6/LICENSE` & `cocojamboo-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.6/PKG-INFO` & `cocojamboo-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocojamboo
-Version: 2.0.6
+Version: 2.0.7
 Summary: An extension to COCO evaluation metric to provide mAP scores with custom paramters.
 Author: Georgiana Manolache
 License: 
         Attribution-NonCommercial 4.0 International
         
         =======================================================================
```

### Comparing `cocojamboo-2.0.6/cocojamboo/coco_eval2.py` & `cocojamboo-2.0.7/cocojamboo/coco_eval2.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 from contextlib import redirect_stdout
 
 import numpy as np
 import pycocotools.mask as mask_util
 import torch
 #import utils
 from pycocotools.coco import COCO
-from cocoeval2 import COCOeval2 # maybe comment out
-
+import cocoeval2
+#from cocoeval2 import COCOeval2 # maybe comment out
 
 class CocoEvaluator:
     def __init__(self, coco_gt, iou_types):
         if not isinstance(iou_types, (list, tuple)):
             raise TypeError(f"This constructor expects iou_types of type list or tuple, instead  got {type(iou_types)}")
         coco_gt = copy.deepcopy(coco_gt)
         self.coco_gt = coco_gt
 
         self.iou_types = iou_types
         self.coco_eval = {}
         for iou_type in iou_types:
-            self.coco_eval[iou_type] = COCOeval2(coco_gt, iouType=iou_type)
+            self.coco_eval[iou_type] = cocoeval2.COCOeval2(coco_gt, iouType=iou_type)
             
         self.img_ids = []
         self.eval_imgs = {k: [] for k in iou_types}
         self.stats = []
 
     def update(self, predictions):
         img_ids = list(np.unique(list(predictions.keys())))
```

### Comparing `cocojamboo-2.0.6/cocojamboo/coco_utils.py` & `cocojamboo-2.0.7/cocojamboo/coco_utils.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.6/cocojamboo/cocoeval2.py` & `cocojamboo-2.0.7/cocojamboo/cocoeval2.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.6/cocojamboo/engine2.py` & `cocojamboo-2.0.7/cocojamboo/engine2.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.6/cocojamboo/transforms.py` & `cocojamboo-2.0.7/cocojamboo/transforms.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.6/cocojamboo/utils.py` & `cocojamboo-2.0.7/cocojamboo/utils.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.0.6/cocojamboo.egg-info/PKG-INFO` & `cocojamboo-2.0.7/cocojamboo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocojamboo
-Version: 2.0.6
+Version: 2.0.7
 Summary: An extension to COCO evaluation metric to provide mAP scores with custom paramters.
 Author: Georgiana Manolache
 License: 
         Attribution-NonCommercial 4.0 International
         
         =======================================================================
```

### Comparing `cocojamboo-2.0.6/pyproject.toml` & `cocojamboo-2.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "pycocotools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cocojamboo"
-version = "2.0.6"
+version = "2.0.7"
 description = "An extension to COCO evaluation metric to provide mAP scores with custom paramters."
 readme = "README.md"
 authors = [{ name = "Georgiana Manolache" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: Free for non-commercial use",
     "Programming Language :: Python",
```


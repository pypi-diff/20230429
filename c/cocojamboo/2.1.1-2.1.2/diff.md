# Comparing `tmp/cocojamboo-2.1.1.tar.gz` & `tmp/cocojamboo-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocojamboo-2.1.1.tar", last modified: Sat Apr 29 10:25:47 2023, max compression
+gzip compressed data, was "cocojamboo-2.1.2.tar", last modified: Sat Apr 29 10:37:35 2023, max compression
```

## Comparing `cocojamboo-2.1.1.tar` & `cocojamboo-2.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 10:25:47.475360 cocojamboo-2.1.1/
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)    19334 2023-01-10 14:44:25.000000 cocojamboo-2.1.1/LICENSE
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 10:25:47.474867 cocojamboo-2.1.1/PKG-INFO
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)      122 2023-03-31 12:26:52.000000 cocojamboo-2.1.1/README.md
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 10:25:47.472729 cocojamboo-2.1.1/cocojamboo/
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)      169 2023-04-29 10:18:07.000000 cocojamboo-2.1.1/cocojamboo/__init__.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     6646 2023-04-29 10:18:09.000000 cocojamboo-2.1.1/cocojamboo/coco_eval2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     8904 2023-04-29 10:18:01.000000 cocojamboo-2.1.1/cocojamboo/coco_utils.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    45829 2023-04-29 07:00:48.000000 cocojamboo-2.1.1/cocojamboo/cocoeval2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     4547 2023-04-29 10:17:58.000000 cocojamboo-2.1.1/cocojamboo/engine2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23337 2023-02-17 12:32:17.000000 cocojamboo-2.1.1/cocojamboo/transforms.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     8388 2023-02-17 12:32:17.000000 cocojamboo-2.1.1/cocojamboo/utils.py
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 10:25:47.474133 cocojamboo-2.1.1/cocojamboo.egg-info/
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 10:25:47.000000 cocojamboo-2.1.1/cocojamboo.egg-info/PKG-INFO
--rw-r--r--   0 georgianamanolache   (501) staff       (20)      332 2023-04-29 10:25:47.000000 cocojamboo-2.1.1/cocojamboo.egg-info/SOURCES.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)        1 2023-04-29 10:25:47.000000 cocojamboo-2.1.1/cocojamboo.egg-info/dependency_links.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)       11 2023-04-29 10:25:47.000000 cocojamboo-2.1.1/cocojamboo.egg-info/top_level.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)      670 2023-04-29 10:19:56.000000 cocojamboo-2.1.1/pyproject.toml
--rw-r--r--   0 georgianamanolache   (501) staff       (20)       38 2023-04-29 10:25:47.475504 cocojamboo-2.1.1/setup.cfg
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 10:37:35.159299 cocojamboo-2.1.2/
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)    19334 2023-01-10 14:44:25.000000 cocojamboo-2.1.2/LICENSE
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 10:37:35.158648 cocojamboo-2.1.2/PKG-INFO
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)      122 2023-03-31 12:26:52.000000 cocojamboo-2.1.2/README.md
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 10:37:35.155558 cocojamboo-2.1.2/cocojamboo/
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)      169 2023-04-29 10:36:40.000000 cocojamboo-2.1.2/cocojamboo/__init__.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     6634 2023-04-29 10:36:37.000000 cocojamboo-2.1.2/cocojamboo/coco_eval2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     8904 2023-04-29 10:18:01.000000 cocojamboo-2.1.2/cocojamboo/coco_utils.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    45829 2023-04-29 07:00:48.000000 cocojamboo-2.1.2/cocojamboo/cocoeval2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     4547 2023-04-29 10:17:58.000000 cocojamboo-2.1.2/cocojamboo/engine2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23337 2023-02-17 12:32:17.000000 cocojamboo-2.1.2/cocojamboo/transforms.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     8388 2023-02-17 12:32:17.000000 cocojamboo-2.1.2/cocojamboo/utils.py
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 10:37:35.157361 cocojamboo-2.1.2/cocojamboo.egg-info/
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 10:37:35.000000 cocojamboo-2.1.2/cocojamboo.egg-info/PKG-INFO
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)      332 2023-04-29 10:37:35.000000 cocojamboo-2.1.2/cocojamboo.egg-info/SOURCES.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)        1 2023-04-29 10:37:35.000000 cocojamboo-2.1.2/cocojamboo.egg-info/dependency_links.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)       11 2023-04-29 10:37:35.000000 cocojamboo-2.1.2/cocojamboo.egg-info/top_level.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)      670 2023-04-29 10:36:48.000000 cocojamboo-2.1.2/pyproject.toml
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)       38 2023-04-29 10:37:35.159509 cocojamboo-2.1.2/setup.cfg
```

### Comparing `cocojamboo-2.1.1/LICENSE` & `cocojamboo-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.1.1/PKG-INFO` & `cocojamboo-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocojamboo
-Version: 2.1.1
+Version: 2.1.2
 Summary: An extension to COCO evaluation metric to provide mAP scores with custom paramters.
 Author: Georgiana Manolache
 License: 
         Attribution-NonCommercial 4.0 International
         
         =======================================================================
```

### Comparing `cocojamboo-2.1.1/cocojamboo/coco_eval2.py` & `cocojamboo-2.1.2/cocojamboo/coco_eval2.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,16 +152,16 @@
 
 def convert_to_xywh(boxes):
     xmin, ymin, xmax, ymax = boxes.unbind(1)
     return torch.stack((xmin, ymin, xmax - xmin, ymax - ymin), dim=1)
 
 
 def merge(img_ids, eval_imgs):
-    all_img_ids = utils.all_gather(img_ids)
-    all_eval_imgs = utils.all_gather(eval_imgs)
+    all_img_ids = all_gather(img_ids)
+    all_eval_imgs = all_gather(eval_imgs)
 
     merged_img_ids = []
     for p in all_img_ids:
         merged_img_ids.extend(p)
 
     merged_eval_imgs = []
     for p in all_eval_imgs:
```

### Comparing `cocojamboo-2.1.1/cocojamboo/coco_utils.py` & `cocojamboo-2.1.2/cocojamboo/coco_utils.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.1.1/cocojamboo/cocoeval2.py` & `cocojamboo-2.1.2/cocojamboo/cocoeval2.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.1.1/cocojamboo/engine2.py` & `cocojamboo-2.1.2/cocojamboo/engine2.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.1.1/cocojamboo/transforms.py` & `cocojamboo-2.1.2/cocojamboo/transforms.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.1.1/cocojamboo/utils.py` & `cocojamboo-2.1.2/cocojamboo/utils.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.1.1/cocojamboo.egg-info/PKG-INFO` & `cocojamboo-2.1.2/cocojamboo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocojamboo
-Version: 2.1.1
+Version: 2.1.2
 Summary: An extension to COCO evaluation metric to provide mAP scores with custom paramters.
 Author: Georgiana Manolache
 License: 
         Attribution-NonCommercial 4.0 International
         
         =======================================================================
```

### Comparing `cocojamboo-2.1.1/pyproject.toml` & `cocojamboo-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "numpy", "wheel", "pycocotools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cocojamboo"
-version = "2.1.1"
+version = "2.1.2"
 description = "An extension to COCO evaluation metric to provide mAP scores with custom paramters."
 readme = "README.md"
 authors = [{ name = "Georgiana Manolache" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: Free for non-commercial use",
     "Programming Language :: Python",
```


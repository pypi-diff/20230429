# Comparing `tmp/forensicface-0.1.8.tar.gz` & `tmp/forensicface-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forensicface-0.1.8.tar", last modified: Wed Mar 22 20:06:26 2023, max compression
+gzip compressed data, was "forensicface-0.1.9.tar", last modified: Thu Apr  6 00:04:57 2023, max compression
```

## Comparing `forensicface-0.1.8.tar` & `forensicface-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 rafael    (1000) rafael    (1000)        0 2023-03-22 20:06:26.124344 forensicface-0.1.8/
--rw-r--r--   0 rafael    (1000) rafael    (1000)     1510 2022-12-18 01:33:06.000000 forensicface-0.1.8/LICENSE
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      111 2022-09-05 16:31:43.000000 forensicface-0.1.8/MANIFEST.in
--rw-r--r--   0 rafael    (1000) rafael    (1000)     3128 2023-03-22 20:06:26.114344 forensicface-0.1.8/PKG-INFO
--rw-r--r--   0 rafael    (1000) rafael    (1000)     2323 2023-03-22 20:05:28.000000 forensicface-0.1.8/README.md
-drwxr-xr-x   0 rafael    (1000) rafael    (1000)        0 2023-03-22 20:06:26.114344 forensicface-0.1.8/forensicface/
--rw-r--r--   0 rafael    (1000) rafael    (1000)       22 2023-03-22 20:04:08.000000 forensicface-0.1.8/forensicface/__init__.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)     5124 2023-03-22 20:04:12.000000 forensicface-0.1.8/forensicface/_modidx.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)    22314 2023-03-22 20:04:08.000000 forensicface-0.1.8/forensicface/app.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)      142 2022-12-18 01:33:47.000000 forensicface-0.1.8/forensicface/core.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)     3279 2022-12-22 03:19:11.000000 forensicface-0.1.8/forensicface/forensicface.py
-drwxr-xr-x   0 rafael    (1000) rafael    (1000)        0 2023-03-22 20:06:26.114344 forensicface-0.1.8/forensicface.egg-info/
--rw-r--r--   0 rafael    (1000) rafael    (1000)     3128 2023-03-22 20:06:26.000000 forensicface-0.1.8/forensicface.egg-info/PKG-INFO
--rw-r--r--   0 rafael    (1000) rafael    (1000)      423 2023-03-22 20:06:26.000000 forensicface-0.1.8/forensicface.egg-info/SOURCES.txt
--rw-r--r--   0 rafael    (1000) rafael    (1000)        1 2023-03-22 20:06:26.000000 forensicface-0.1.8/forensicface.egg-info/dependency_links.txt
--rw-r--r--   0 rafael    (1000) rafael    (1000)       46 2023-03-22 20:06:26.000000 forensicface-0.1.8/forensicface.egg-info/entry_points.txt
--rw-r--r--   0 rafael    (1000) rafael    (1000)        1 2022-12-22 03:15:43.000000 forensicface-0.1.8/forensicface.egg-info/not-zip-safe
--rw-r--r--   0 rafael    (1000) rafael    (1000)       69 2023-03-22 20:06:26.000000 forensicface-0.1.8/forensicface.egg-info/requires.txt
--rw-r--r--   0 rafael    (1000) rafael    (1000)       13 2023-03-22 20:06:26.000000 forensicface-0.1.8/forensicface.egg-info/top_level.txt
--rw-r--r--   0 rafael    (1000) rafael    (1000)     1030 2023-03-22 20:02:47.000000 forensicface-0.1.8/settings.ini
--rw-r--r--   0 rafael    (1000) rafael    (1000)       38 2023-03-22 20:06:26.124344 forensicface-0.1.8/setup.cfg
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     2541 2022-09-05 16:31:43.000000 forensicface-0.1.8/setup.py
+drwxr-xr-x   0 rafael    (1000) rafael    (1000)        0 2023-04-06 00:04:57.460522 forensicface-0.1.9/
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     1510 2022-12-18 01:33:06.000000 forensicface-0.1.9/LICENSE
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      111 2022-09-05 16:31:43.000000 forensicface-0.1.9/MANIFEST.in
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     3128 2023-04-06 00:04:57.460522 forensicface-0.1.9/PKG-INFO
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     2323 2023-03-22 20:05:28.000000 forensicface-0.1.9/README.md
+drwxr-xr-x   0 rafael    (1000) rafael    (1000)        0 2023-04-06 00:04:57.460522 forensicface-0.1.9/forensicface/
+-rw-r--r--   0 rafael    (1000) rafael    (1000)       22 2023-04-06 00:03:37.000000 forensicface-0.1.9/forensicface/__init__.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     5124 2023-04-06 00:03:44.000000 forensicface-0.1.9/forensicface/_modidx.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)    22319 2023-04-06 00:03:37.000000 forensicface-0.1.9/forensicface/app.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)      142 2022-12-18 01:33:47.000000 forensicface-0.1.9/forensicface/core.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     3279 2022-12-22 03:19:11.000000 forensicface-0.1.9/forensicface/forensicface.py
+drwxr-xr-x   0 rafael    (1000) rafael    (1000)        0 2023-04-06 00:04:57.460522 forensicface-0.1.9/forensicface.egg-info/
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     3128 2023-04-06 00:04:57.000000 forensicface-0.1.9/forensicface.egg-info/PKG-INFO
+-rw-r--r--   0 rafael    (1000) rafael    (1000)      423 2023-04-06 00:04:57.000000 forensicface-0.1.9/forensicface.egg-info/SOURCES.txt
+-rw-r--r--   0 rafael    (1000) rafael    (1000)        1 2023-04-06 00:04:57.000000 forensicface-0.1.9/forensicface.egg-info/dependency_links.txt
+-rw-r--r--   0 rafael    (1000) rafael    (1000)       46 2023-04-06 00:04:57.000000 forensicface-0.1.9/forensicface.egg-info/entry_points.txt
+-rw-r--r--   0 rafael    (1000) rafael    (1000)        1 2022-12-22 03:15:43.000000 forensicface-0.1.9/forensicface.egg-info/not-zip-safe
+-rw-r--r--   0 rafael    (1000) rafael    (1000)       69 2023-04-06 00:04:57.000000 forensicface-0.1.9/forensicface.egg-info/requires.txt
+-rw-r--r--   0 rafael    (1000) rafael    (1000)       13 2023-04-06 00:04:57.000000 forensicface-0.1.9/forensicface.egg-info/top_level.txt
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     1030 2023-04-06 00:02:48.000000 forensicface-0.1.9/settings.ini
+-rw-r--r--   0 rafael    (1000) rafael    (1000)       38 2023-04-06 00:04:57.460522 forensicface-0.1.9/setup.cfg
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     2541 2022-09-05 16:31:43.000000 forensicface-0.1.9/setup.py
```

### Comparing `forensicface-0.1.8/LICENSE` & `forensicface-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `forensicface-0.1.8/PKG-INFO` & `forensicface-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forensicface
-Version: 0.1.8
+Version: 0.1.9
 Summary: An attempt to build a package for forensic face examination
 Home-page: https://github.com/rafribeiro/forensicface
 Author: Rafael O. Ribeiro
 Author-email: rafaeloliveiraribeiro@gmail.com
 License: BSD License
 Keywords: nbdev jupyter python face recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `forensicface-0.1.8/README.md` & `forensicface-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `forensicface-0.1.8/forensicface/_modidx.py` & `forensicface-0.1.9/forensicface/_modidx.py`

 * *Files identical despite different names*

### Comparing `forensicface-0.1.8/forensicface/app.py` & `forensicface-0.1.9/forensicface/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,17 +542,17 @@
     vs.set(cv2.CAP_PROP_POS_FRAMES, start_frame)
     current_frame = start_frame
     nfaces = 0
     while True:
 
         if (current_frame % every_n_frames) != 0:
             current_frame = current_frame + 1
-            vs.set(cv2.CAP_PROP_POS_FRAMES, current_frame)
             continue
-
+        
+        vs.set(cv2.CAP_PROP_POS_FRAMES, current_frame) 
         ret, frame = vs.read()
 
         if not ret:
             break
         current_frame = current_frame + 1
         (h, w) = frame.shape[:2]
```

### Comparing `forensicface-0.1.8/forensicface/forensicface.py` & `forensicface-0.1.9/forensicface/forensicface.py`

 * *Files identical despite different names*

### Comparing `forensicface-0.1.8/forensicface.egg-info/PKG-INFO` & `forensicface-0.1.9/forensicface.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forensicface
-Version: 0.1.8
+Version: 0.1.9
 Summary: An attempt to build a package for forensic face examination
 Home-page: https://github.com/rafribeiro/forensicface
 Author: Rafael O. Ribeiro
 Author-email: rafaeloliveiraribeiro@gmail.com
 License: BSD License
 Keywords: nbdev jupyter python face recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `forensicface-0.1.8/settings.ini` & `forensicface-0.1.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = forensicface
 lib_name = %(repo)s
-version = 0.1.8
+version = 0.1.9
 min_python = 3.7
 license = bsd3
 
 ### nbdev ###
 doc_path = _docs
 lib_path = forensicface
 nbs_path = nbs
```

### Comparing `forensicface-0.1.8/setup.py` & `forensicface-0.1.9/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/space-invaders-0.1.59.tar.gz` & `tmp/space-invaders-0.1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space-invaders-0.1.59.tar", last modified: Fri Apr 28 23:05:32 2023, max compression
+gzip compressed data, was "space-invaders-0.1.60.tar", last modified: Fri Apr 28 23:14:19 2023, max compression
```

## Comparing `space-invaders-0.1.59.tar` & `space-invaders-0.1.60.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 23:05:32.902772 space-invaders-0.1.59/
--rw-rw-rw-   0        0        0      295 2023-04-28 16:42:04.000000 space-invaders-0.1.59/MANIFEST.in
--rw-rw-rw-   0        0        0     2340 2023-04-28 23:05:32.902772 space-invaders-0.1.59/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-28 23:05:32.902772 space-invaders-0.1.59/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-04-28 23:05:29.000000 space-invaders-0.1.59/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:05:32.891235 space-invaders-0.1.59/space_invaders/
--rw-rw-rw-   0        0        0        0 2023-04-28 16:51:05.000000 space-invaders-0.1.59/space_invaders/__init__.py
--rw-rw-rw-   0        0        0     3603 2023-04-28 12:41:13.000000 space-invaders-0.1.59/space_invaders/config.py
--rw-rw-rw-   0        0        0     3450 2023-04-27 14:33:59.000000 space-invaders-0.1.59/space_invaders/entity.py
--rw-rw-rw-   0        0        0    16751 2023-04-28 10:58:34.000000 space-invaders-0.1.59/space_invaders/level.py
--rw-rw-rw-   0        0        0    15997 2023-04-28 22:47:17.000000 space-invaders-0.1.59/space_invaders/main.py
--rw-rw-rw-   0        0        0     2918 2023-04-28 10:32:18.000000 space-invaders-0.1.59/space_invaders/pickup.py
--rw-rw-rw-   0        0        0    11021 2023-04-28 10:51:03.000000 space-invaders-0.1.59/space_invaders/spaceship.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:05:32.901266 space-invaders-0.1.59/space_invaders.egg-info/
--rw-rw-rw-   0        0        0     2340 2023-04-28 23:05:32.000000 space-invaders-0.1.59/space_invaders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-04-28 23:05:32.000000 space-invaders-0.1.59/space_invaders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 23:05:32.000000 space-invaders-0.1.59/space_invaders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-28 23:05:32.000000 space-invaders-0.1.59/space_invaders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-28 23:05:32.000000 space-invaders-0.1.59/space_invaders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       57 2023-04-28 23:05:32.000000 space-invaders-0.1.59/space_invaders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 23:14:19.938530 space-invaders-0.1.60/
+-rw-rw-rw-   0        0        0      295 2023-04-28 16:42:04.000000 space-invaders-0.1.60/MANIFEST.in
+-rw-rw-rw-   0        0        0     2340 2023-04-28 23:14:19.938530 space-invaders-0.1.60/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-28 23:14:19.938530 space-invaders-0.1.60/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-04-28 23:13:57.000000 space-invaders-0.1.60/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:14:19.933025 space-invaders-0.1.60/space_invaders/
+-rw-rw-rw-   0        0        0       72 2023-04-28 23:10:31.000000 space-invaders-0.1.60/space_invaders/__init__.py
+-rw-rw-rw-   0        0        0     3603 2023-04-28 12:41:13.000000 space-invaders-0.1.60/space_invaders/config.py
+-rw-rw-rw-   0        0        0     3450 2023-04-27 14:33:59.000000 space-invaders-0.1.60/space_invaders/entity.py
+-rw-rw-rw-   0        0        0    16751 2023-04-28 10:58:34.000000 space-invaders-0.1.60/space_invaders/level.py
+-rw-rw-rw-   0        0        0    15997 2023-04-28 22:47:17.000000 space-invaders-0.1.60/space_invaders/main.py
+-rw-rw-rw-   0        0        0     2918 2023-04-28 10:32:18.000000 space-invaders-0.1.60/space_invaders/pickup.py
+-rw-rw-rw-   0        0        0    11021 2023-04-28 10:51:03.000000 space-invaders-0.1.60/space_invaders/spaceship.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:14:19.937530 space-invaders-0.1.60/space_invaders.egg-info/
+-rw-rw-rw-   0        0        0     2340 2023-04-28 23:14:19.000000 space-invaders-0.1.60/space_invaders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-04-28 23:14:19.000000 space-invaders-0.1.60/space_invaders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 23:14:19.000000 space-invaders-0.1.60/space_invaders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-28 23:14:19.000000 space-invaders-0.1.60/space_invaders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-28 23:14:19.000000 space-invaders-0.1.60/space_invaders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       57 2023-04-28 23:14:19.000000 space-invaders-0.1.60/space_invaders.egg-info/top_level.txt
```

### Comparing `space-invaders-0.1.59/PKG-INFO` & `space-invaders-0.1.60/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-invaders
-Version: 0.1.59
+Version: 0.1.60
 Summary: A cool space shooter rouge like game
 Author: Bódi Martin
 Author-email: bodimartin22@gmail.com
 Description-Content-Type: text/markdown
 
 # Space Invaders
 ## HOW TO INSTALL?
```

### Comparing `space-invaders-0.1.59/setup.py` & `space-invaders-0.1.60/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='space-invaders',
-    version='0.1.59',
+    version='0.1.60',
     py_modules=['entity', 'config', 'main', 'spaceship', 'level', 'pickup'],
     packages=find_packages(),
     install_requires=[
         'pygame',
         'shapely'
     ],
     entry_points={
```

### Comparing `space-invaders-0.1.59/space_invaders/config.py` & `space-invaders-0.1.60/space_invaders/config.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.59/space_invaders/entity.py` & `space-invaders-0.1.60/space_invaders/entity.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.59/space_invaders/level.py` & `space-invaders-0.1.60/space_invaders/level.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.59/space_invaders/main.py` & `space-invaders-0.1.60/space_invaders/main.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.59/space_invaders/pickup.py` & `space-invaders-0.1.60/space_invaders/pickup.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.59/space_invaders/spaceship.py` & `space-invaders-0.1.60/space_invaders/spaceship.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.1.59/space_invaders.egg-info/PKG-INFO` & `space-invaders-0.1.60/space_invaders.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-invaders
-Version: 0.1.59
+Version: 0.1.60
 Summary: A cool space shooter rouge like game
 Author: Bódi Martin
 Author-email: bodimartin22@gmail.com
 Description-Content-Type: text/markdown
 
 # Space Invaders
 ## HOW TO INSTALL?
```


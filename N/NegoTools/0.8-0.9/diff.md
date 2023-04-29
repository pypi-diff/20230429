# Comparing `tmp/NegoTools-0.8.tar.gz` & `tmp/NegoTools-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NegoTools-0.8.tar", last modified: Sat Apr 29 13:31:04 2023, max compression
+gzip compressed data, was "NegoTools-0.9.tar", last modified: Sat Apr 29 14:36:09 2023, max compression
```

## Comparing `NegoTools-0.8.tar` & `NegoTools-0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 13:31:04.379659 NegoTools-0.8/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 13:31:04.375659 NegoTools-0.8/NegoTools.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)      194 2023-04-29 13:31:03.000000 NegoTools-0.8/NegoTools.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      363 2023-04-29 13:31:03.000000 NegoTools-0.8/NegoTools.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-29 13:31:03.000000 NegoTools-0.8/NegoTools.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-29 13:31:03.000000 NegoTools-0.8/NegoTools.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1000) alex      (1000)       63 2023-04-29 13:31:03.000000 NegoTools-0.8/NegoTools.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       26 2023-04-29 13:31:03.000000 NegoTools-0.8/NegoTools.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      194 2023-04-29 13:31:04.379659 NegoTools-0.8/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     2162 2023-04-29 12:47:29.000000 NegoTools-0.8/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 13:31:04.375659 NegoTools-0.8/Scientific/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 13:31:04.375659 NegoTools-0.8/Scientific/Clustering/
--rw-rw-r--   0 alex      (1000) alex      (1000)       27 2023-04-29 13:23:28.000000 NegoTools-0.8/Scientific/Clustering/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1052 2023-04-29 13:25:03.000000 NegoTools-0.8/Scientific/Clustering/kmeans.py
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-29 12:10:33.000000 NegoTools-0.8/Scientific/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 13:31:04.379659 NegoTools-0.8/hyperheuristic/
--rw-rw-r--   0 alex      (1000) alex      (1000)       45 2023-04-29 12:10:33.000000 NegoTools-0.8/hyperheuristic/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2708 2023-04-29 12:32:58.000000 NegoTools-0.8/hyperheuristic/hyperheuristic.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-29 13:31:04.379659 NegoTools-0.8/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      569 2023-04-29 13:24:44.000000 NegoTools-0.8/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 14:36:09.543609 NegoTools-0.9/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 14:36:09.539609 NegoTools-0.9/NegoTools.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      194 2023-04-29 14:36:09.000000 NegoTools-0.9/NegoTools.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      363 2023-04-29 14:36:09.000000 NegoTools-0.9/NegoTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-29 14:36:09.000000 NegoTools-0.9/NegoTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-29 14:36:09.000000 NegoTools-0.9/NegoTools.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1000) alex      (1000)       63 2023-04-29 14:36:09.000000 NegoTools-0.9/NegoTools.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       26 2023-04-29 14:36:09.000000 NegoTools-0.9/NegoTools.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      194 2023-04-29 14:36:09.543609 NegoTools-0.9/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2162 2023-04-29 12:47:29.000000 NegoTools-0.9/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 14:36:09.539609 NegoTools-0.9/Scientific/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 14:36:09.543609 NegoTools-0.9/Scientific/Clustering/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       27 2023-04-29 13:23:28.000000 NegoTools-0.9/Scientific/Clustering/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1052 2023-04-29 13:25:03.000000 NegoTools-0.9/Scientific/Clustering/kmeans.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-29 12:10:33.000000 NegoTools-0.9/Scientific/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 14:36:09.543609 NegoTools-0.9/hyperheuristic/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       45 2023-04-29 12:10:33.000000 NegoTools-0.9/hyperheuristic/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2708 2023-04-29 12:32:58.000000 NegoTools-0.9/hyperheuristic/hyperheuristic.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-29 14:36:09.543609 NegoTools-0.9/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      569 2023-04-29 14:33:07.000000 NegoTools-0.9/setup.py
```

### Comparing `NegoTools-0.8/README.md` & `NegoTools-0.9/README.md`

 * *Files identical despite different names*

### Comparing `NegoTools-0.8/Scientific/Clustering/kmeans.py` & `NegoTools-0.9/Scientific/Clustering/kmeans.py`

 * *Files identical despite different names*

### Comparing `NegoTools-0.8/hyperheuristic/hyperheuristic.py` & `NegoTools-0.9/hyperheuristic/hyperheuristic.py`

 * *Files identical despite different names*

### Comparing `NegoTools-0.8/setup.py` & `NegoTools-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='NegoTools', 
-    version='0.8', 
+    version='0.9', 
     description='nego tools',
     author='Alexandro Rocha', 
     url='https://github.com/AlexandroLuis/NegoTools',
     package_dir = {
     	"hyperheuristic": "hyperheuristic",
     	"Scientific": "Scientific",
     },
```


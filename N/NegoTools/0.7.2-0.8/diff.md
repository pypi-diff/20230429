# Comparing `tmp/NegoTools-0.7.2.tar.gz` & `tmp/NegoTools-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NegoTools-0.7.2.tar", last modified: Wed Dec 28 22:52:46 2022, max compression
+gzip compressed data, was "NegoTools-0.8.tar", last modified: Sat Apr 29 13:31:04 2023, max compression
```

## Comparing `NegoTools-0.7.2.tar` & `NegoTools-0.8.tar`

### file list

```diff
@@ -1,26 +1,20 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-12-28 22:52:46.936148 NegoTools-0.7.2/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-12-28 22:52:46.936148 NegoTools-0.7.2/NegoTools.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)      196 2022-12-28 22:52:46.000000 NegoTools-0.7.2/NegoTools.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      517 2022-12-28 22:52:46.000000 NegoTools-0.7.2/NegoTools.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2022-12-28 22:52:46.000000 NegoTools-0.7.2/NegoTools.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2022-12-28 22:52:42.000000 NegoTools-0.7.2/NegoTools.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1000) alex      (1000)       50 2022-12-28 22:52:46.000000 NegoTools-0.7.2/NegoTools.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       26 2022-12-28 22:52:46.000000 NegoTools-0.7.2/NegoTools.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      196 2022-12-28 22:52:46.936148 NegoTools-0.7.2/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)       12 2022-12-27 19:19:37.000000 NegoTools-0.7.2/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-12-28 22:52:46.936148 NegoTools-0.7.2/Scientific/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-12-28 22:52:46.936148 NegoTools-0.7.2/Scientific/Classification/
--rw-rw-r--   0 alex      (1000) alex      (1000)     2181 2022-12-28 20:51:46.000000 NegoTools-0.7.2/Scientific/Classification/NaiveBayes.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       35 2022-12-28 20:35:45.000000 NegoTools-0.7.2/Scientific/Classification/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-12-28 22:52:46.936148 NegoTools-0.7.2/Scientific/Clustering/
--rw-rw-r--   0 alex      (1000) alex      (1000)     2170 2022-12-28 19:32:18.000000 NegoTools-0.7.2/Scientific/Clustering/Kmeans.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       27 2022-12-28 22:50:38.000000 NegoTools-0.7.2/Scientific/Clustering/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-12-28 22:52:46.936148 NegoTools-0.7.2/Scientific/Regression/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1809 2022-12-28 19:32:15.000000 NegoTools-0.7.2/Scientific/Regression/LinearRegression.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       47 2022-12-28 20:28:09.000000 NegoTools-0.7.2/Scientific/Regression/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-28 19:47:14.000000 NegoTools-0.7.2/Scientific/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-12-28 22:52:46.936148 NegoTools-0.7.2/hyperheuristic/
--rw-rw-r--   0 alex      (1000) alex      (1000)       45 2022-12-28 20:22:34.000000 NegoTools-0.7.2/hyperheuristic/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1342 2022-12-27 19:19:37.000000 NegoTools-0.7.2/hyperheuristic/hyperheuristic.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2022-12-28 22:52:46.936148 NegoTools-0.7.2/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      612 2022-12-28 22:52:31.000000 NegoTools-0.7.2/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 13:31:04.379659 NegoTools-0.8/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 13:31:04.375659 NegoTools-0.8/NegoTools.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      194 2023-04-29 13:31:03.000000 NegoTools-0.8/NegoTools.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      363 2023-04-29 13:31:03.000000 NegoTools-0.8/NegoTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-29 13:31:03.000000 NegoTools-0.8/NegoTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-29 13:31:03.000000 NegoTools-0.8/NegoTools.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1000) alex      (1000)       63 2023-04-29 13:31:03.000000 NegoTools-0.8/NegoTools.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       26 2023-04-29 13:31:03.000000 NegoTools-0.8/NegoTools.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      194 2023-04-29 13:31:04.379659 NegoTools-0.8/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2162 2023-04-29 12:47:29.000000 NegoTools-0.8/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 13:31:04.375659 NegoTools-0.8/Scientific/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 13:31:04.375659 NegoTools-0.8/Scientific/Clustering/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       27 2023-04-29 13:23:28.000000 NegoTools-0.8/Scientific/Clustering/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1052 2023-04-29 13:25:03.000000 NegoTools-0.8/Scientific/Clustering/kmeans.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-29 12:10:33.000000 NegoTools-0.8/Scientific/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-29 13:31:04.379659 NegoTools-0.8/hyperheuristic/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       45 2023-04-29 12:10:33.000000 NegoTools-0.8/hyperheuristic/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2708 2023-04-29 12:32:58.000000 NegoTools-0.8/hyperheuristic/hyperheuristic.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-29 13:31:04.379659 NegoTools-0.8/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      569 2023-04-29 13:24:44.000000 NegoTools-0.8/setup.py
```

### Comparing `NegoTools-0.7.2/setup.py` & `NegoTools-0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from setuptools import setup
 
 setup(
     name='NegoTools', 
-    version='0.7.2', 
+    version='0.8', 
     description='nego tools',
     author='Alexandro Rocha', 
     url='https://github.com/AlexandroLuis/NegoTools',
     package_dir = {
     	"hyperheuristic": "hyperheuristic",
     	"Scientific": "Scientific",
     },
     packages=[
     	'hyperheuristic',
     	'Scientific',
-    	'Scientific.Regression',
     	'Scientific.Clustering',
-    	'Scientific.Classification',
     ],
     install_requires=[
         'thompson-sampling',
         'pandas',
         'random2',
         'numpy',
         'matplotlib',
+        'scikit-learn'
     ],
     zip_safe=False
 )
```


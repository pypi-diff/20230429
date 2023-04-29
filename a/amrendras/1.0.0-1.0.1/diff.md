# Comparing `tmp/amrendras-1.0.0.tar.gz` & `tmp/amrendras-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amrendras-1.0.0.tar", last modified: Fri Apr 28 16:58:56 2023, max compression
+gzip compressed data, was "amrendras-1.0.1.tar", last modified: Sat Apr 29 10:02:22 2023, max compression
```

## Comparing `amrendras-1.0.0.tar` & `amrendras-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 sony       (501) staff       (20)        0 2023-04-28 16:58:56.204688 amrendras-1.0.0/
--rw-r--r--   0 sony       (501) staff       (20)      473 2023-04-28 16:58:56.204512 amrendras-1.0.0/PKG-INFO
-drwxr-xr-x   0 sony       (501) staff       (20)        0 2023-04-28 16:58:56.203436 amrendras-1.0.0/amrendras/
--rw-r--r--   0 sony       (501) staff       (20)       39 2023-04-28 16:57:04.000000 amrendras-1.0.0/amrendras/__init__.py
--rw-r--r--   0 sony       (501) staff       (20)     3703 2023-04-28 16:56:52.000000 amrendras-1.0.0/amrendras/amrendras.py
-drwxr-xr-x   0 sony       (501) staff       (20)        0 2023-04-28 16:58:56.204248 amrendras-1.0.0/amrendras.egg-info/
--rw-r--r--   0 sony       (501) staff       (20)      473 2023-04-28 16:58:56.000000 amrendras-1.0.0/amrendras.egg-info/PKG-INFO
--rw-r--r--   0 sony       (501) staff       (20)      185 2023-04-28 16:58:56.000000 amrendras-1.0.0/amrendras.egg-info/SOURCES.txt
--rw-r--r--   0 sony       (501) staff       (20)        1 2023-04-28 16:58:56.000000 amrendras-1.0.0/amrendras.egg-info/dependency_links.txt
--rw-r--r--   0 sony       (501) staff       (20)       10 2023-04-28 16:58:56.000000 amrendras-1.0.0/amrendras.egg-info/top_level.txt
--rw-r--r--   0 sony       (501) staff       (20)       38 2023-04-28 16:58:56.204746 amrendras-1.0.0/setup.cfg
--rw-r--r--   0 sony       (501) staff       (20)      743 2023-04-28 16:57:30.000000 amrendras-1.0.0/setup.py
+drwxr-xr-x   0 sony       (501) staff       (20)        0 2023-04-29 10:02:22.346895 amrendras-1.0.1/
+-rw-r--r--   0 sony       (501) staff       (20)      478 2023-04-29 10:02:22.346722 amrendras-1.0.1/PKG-INFO
+drwxr-xr-x   0 sony       (501) staff       (20)        0 2023-04-29 10:02:22.345705 amrendras-1.0.1/amrendras/
+-rw-r--r--   0 sony       (501) staff       (20)       39 2023-04-28 16:57:04.000000 amrendras-1.0.1/amrendras/__init__.py
+-rw-r--r--   0 sony       (501) staff       (20)      277 2023-04-29 10:00:09.000000 amrendras-1.0.1/amrendras/amrendras.py
+drwxr-xr-x   0 sony       (501) staff       (20)        0 2023-04-29 10:02:22.346477 amrendras-1.0.1/amrendras.egg-info/
+-rw-r--r--   0 sony       (501) staff       (20)      478 2023-04-29 10:02:22.000000 amrendras-1.0.1/amrendras.egg-info/PKG-INFO
+-rw-r--r--   0 sony       (501) staff       (20)      185 2023-04-29 10:02:22.000000 amrendras-1.0.1/amrendras.egg-info/SOURCES.txt
+-rw-r--r--   0 sony       (501) staff       (20)        1 2023-04-29 10:02:22.000000 amrendras-1.0.1/amrendras.egg-info/dependency_links.txt
+-rw-r--r--   0 sony       (501) staff       (20)       10 2023-04-29 10:02:22.000000 amrendras-1.0.1/amrendras.egg-info/top_level.txt
+-rw-r--r--   0 sony       (501) staff       (20)       38 2023-04-29 10:02:22.346947 amrendras-1.0.1/setup.cfg
+-rw-r--r--   0 sony       (501) staff       (20)      748 2023-04-29 10:02:15.000000 amrendras-1.0.1/setup.py
```

### Comparing `amrendras-1.0.0/setup.py` & `amrendras-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.0'
-DESCRIPTION = 'maja lo'
+VERSION = '1.0.1'
+DESCRIPTION = 'maja le liya'
 
 # Setting up
 setup(
     name="amrendras",
     version=VERSION,
     author="Prajwal",
     author_email="<prajwalupadhyay13@gmail.com>",
```


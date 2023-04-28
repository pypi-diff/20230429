# Comparing `tmp/efpy-0.1.1.tar.gz` & `tmp/efpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efpy-0.1.1.tar", last modified: Fri Apr 28 23:26:32 2023, max compression
+gzip compressed data, was "efpy-0.1.2.tar", last modified: Fri Apr 28 23:41:39 2023, max compression
```

## Comparing `efpy-0.1.1.tar` & `efpy-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 23:26:32.776074 efpy-0.1.1/
--rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 efpy-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      278 2023-04-28 23:26:32.775076 efpy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       65 2022-07-09 03:01:52.000000 efpy-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 23:26:32.772084 efpy-0.1.1/efpy.egg-info/
--rw-rw-rw-   0        0        0      278 2023-04-28 23:26:32.000000 efpy-0.1.1/efpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2023-04-28 23:26:32.000000 efpy-0.1.1/efpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 23:26:32.000000 efpy-0.1.1/efpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 23:26:32.000000 efpy-0.1.1/efpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 23:26:32.776074 efpy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      741 2023-04-28 23:25:49.000000 efpy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:41:39.549472 efpy-0.1.2/
+-rw-rw-rw-   0        0        0      255 2023-04-28 23:41:39.548473 efpy-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-28 23:41:39.538386 efpy-0.1.2/efpy/
+-rw-rw-rw-   0        0        0      836 2023-04-28 23:40:39.000000 efpy-0.1.2/efpy/__init__.py
+-rw-rw-rw-   0        0        0     1447 2021-06-24 08:59:48.000000 efpy-0.1.2/efpy/env.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:41:39.547446 efpy-0.1.2/efpy.egg-info/
+-rw-rw-rw-   0        0        0      255 2023-04-28 23:41:39.000000 efpy-0.1.2/efpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-04-28 23:41:39.000000 efpy-0.1.2/efpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 23:41:39.000000 efpy-0.1.2/efpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-28 23:41:39.000000 efpy-0.1.2/efpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 23:41:39.549472 efpy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      741 2023-04-28 23:41:30.000000 efpy-0.1.2/setup.py
```

### Comparing `efpy-0.1.1/setup.py` & `efpy-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
     name = "efpy",
-    version = "0.1.1",
+    version = "0.1.2",
     keywords = ("experience","environment"),
     description = "experience",
     long_description = "experience",
     license = "MIT Licence",
 
     url = "https://github.com/imcjp/efpy",
     author = "Cai Jianping",
```


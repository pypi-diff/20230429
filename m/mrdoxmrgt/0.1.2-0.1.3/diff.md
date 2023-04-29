# Comparing `tmp/mrdoxmrgt-0.1.2.tar.gz` & `tmp/mrdoxmrgt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrdoxmrgt-0.1.2.tar", last modified: Sat Apr 29 08:46:18 2023, max compression
+gzip compressed data, was "mrdoxmrgt-0.1.3.tar", last modified: Sat Apr 29 09:39:10 2023, max compression
```

## Comparing `mrdoxmrgt-0.1.2.tar` & `mrdoxmrgt-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 08:46:14.000000 mrdoxmrgt-0.1.2/
--rw-rw-rw-   0        0        0     1091 2023-04-14 09:24:50.000000 mrdoxmrgt-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      800 2023-04-29 08:46:20.000000 mrdoxmrgt-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-04-14 09:24:50.000000 mrdoxmrgt-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 08:46:16.000000 mrdoxmrgt-0.1.2/mrdoxmrgt/
--rw-rw-rw-   0        0        0        0 2023-04-28 10:15:20.000000 mrdoxmrgt-0.1.2/mrdoxmrgt/__init__.py
--rw-rw-rw-   0        0        0     3792 2023-04-28 10:21:08.000000 mrdoxmrgt-0.1.2/mrdoxmrgt/main.py
--rw-rw-rw-   0        0        0    15122 2023-04-28 10:15:42.000000 mrdoxmrgt-0.1.2/mrdoxmrgt/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-29 08:46:16.000000 mrdoxmrgt-0.1.2/mrdoxmrgt.egg-info/
--rw-rw-rw-   0        0        0      800 2023-04-29 08:46:14.000000 mrdoxmrgt-0.1.2/mrdoxmrgt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-29 08:46:14.000000 mrdoxmrgt-0.1.2/mrdoxmrgt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 08:46:14.000000 mrdoxmrgt-0.1.2/mrdoxmrgt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-29 08:46:14.000000 mrdoxmrgt-0.1.2/mrdoxmrgt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 08:46:14.000000 mrdoxmrgt-0.1.2/mrdoxmrgt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-29 08:46:14.000000 mrdoxmrgt-0.1.2/mrdoxmrgt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 08:46:20.000000 mrdoxmrgt-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1253 2023-04-29 08:45:16.000000 mrdoxmrgt-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 09:39:10.000000 mrdoxmrgt-0.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-04-14 09:24:50.000000 mrdoxmrgt-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      800 2023-04-29 09:39:12.000000 mrdoxmrgt-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-14 09:24:50.000000 mrdoxmrgt-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 09:39:10.000000 mrdoxmrgt-0.1.3/mrdoxmrgt/
+-rw-rw-rw-   0        0        0        0 2023-04-28 10:15:20.000000 mrdoxmrgt-0.1.3/mrdoxmrgt/__init__.py
+-rw-rw-rw-   0        0        0     3792 2023-04-28 10:21:08.000000 mrdoxmrgt-0.1.3/mrdoxmrgt/main.py
+-rw-rw-rw-   0        0        0    15122 2023-04-28 10:15:42.000000 mrdoxmrgt-0.1.3/mrdoxmrgt/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 09:39:10.000000 mrdoxmrgt-0.1.3/mrdoxmrgt.egg-info/
+-rw-rw-rw-   0        0        0      800 2023-04-29 09:39:10.000000 mrdoxmrgt-0.1.3/mrdoxmrgt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-29 09:39:10.000000 mrdoxmrgt-0.1.3/mrdoxmrgt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 09:39:10.000000 mrdoxmrgt-0.1.3/mrdoxmrgt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-29 09:39:10.000000 mrdoxmrgt-0.1.3/mrdoxmrgt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 09:39:10.000000 mrdoxmrgt-0.1.3/mrdoxmrgt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-29 09:39:10.000000 mrdoxmrgt-0.1.3/mrdoxmrgt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 09:39:12.000000 mrdoxmrgt-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1253 2023-04-29 09:38:16.000000 mrdoxmrgt-0.1.3/setup.py
```

### Comparing `mrdoxmrgt-0.1.2/LICENSE` & `mrdoxmrgt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.1.2/PKG-INFO` & `mrdoxmrgt-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.1.2
+Version: 0.1.3
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/gtf
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.1.2/mrdoxmrgt/main.py` & `mrdoxmrgt-0.1.3/mrdoxmrgt/main.py`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.1.2/mrdoxmrgt/utils.py` & `mrdoxmrgt-0.1.3/mrdoxmrgt/utils.py`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.1.2/mrdoxmrgt.egg-info/PKG-INFO` & `mrdoxmrgt-0.1.3/mrdoxmrgt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.1.2
+Version: 0.1.3
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/gtf
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.1.2/setup.py` & `mrdoxmrgt-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mrdoxmrgt',
     packages=find_packages(),
     include_package_data=True,
-    version="0.1.2",
+    version="0.1.3",
     description='A small example package',
     long_description="A small example package HI",
     long_description_content_type="text/markdown",
     author='MR_GT',
     author_email='friendyt89@gmail.com',
     url='https://github.com/GreyTechno/gtf',
     download_url="https://github.com/GreyTechno/gtf/archive/pypi.zip",
```


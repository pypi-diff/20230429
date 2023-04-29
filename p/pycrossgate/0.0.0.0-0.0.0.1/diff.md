# Comparing `tmp/pycrossgate-0.0.0.0.tar.gz` & `tmp/pycrossgate-0.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pycrossgate-0.0.0.0.tar", last modified: Sat Apr 29 12:33:34 2023, max compression
+gzip compressed data, was "dist\pycrossgate-0.0.0.1.tar", last modified: Sat Apr 29 13:34:35 2023, max compression
```

## Comparing `pycrossgate-0.0.0.0.tar` & `pycrossgate-0.0.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 12:33:34.693299 pycrossgate-0.0.0.0/
-drwxrwxrwx   0        0        0        0 2023-04-29 12:33:34.519775 pycrossgate-0.0.0.0/Core/
--rw-rw-rw-   0        0        0        0 2023-04-29 12:26:53.000000 pycrossgate-0.0.0.0/Core/__init__.py
--rw-rw-rw-   0        0        0     1333 2023-04-29 12:33:34.687315 pycrossgate-0.0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 12:33:34.523753 pycrossgate-0.0.0.0/gui/
--rw-rw-rw-   0        0        0        0 2023-04-29 12:26:53.000000 pycrossgate-0.0.0.0/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:33:34.528739 pycrossgate-0.0.0.0/hybrides/
--rw-rw-rw-   0        0        0        0 2023-04-29 12:26:53.000000 pycrossgate-0.0.0.0/hybrides/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:33:34.678339 pycrossgate-0.0.0.0/pycrossgate.egg-info/
--rw-rw-rw-   0        0        0     1333 2023-04-29 12:33:33.000000 pycrossgate-0.0.0.0/pycrossgate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-04-29 12:33:34.000000 pycrossgate-0.0.0.0/pycrossgate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 12:33:33.000000 pycrossgate-0.0.0.0/pycrossgate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-29 12:33:33.000000 pycrossgate-0.0.0.0/pycrossgate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2023-04-29 12:33:33.000000 pycrossgate-0.0.0.0/pycrossgate.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-29 12:33:34.682330 pycrossgate-0.0.0.0/serve/
--rw-rw-rw-   0        0        0        0 2023-04-29 12:26:53.000000 pycrossgate-0.0.0.0/serve/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-29 12:33:34.693299 pycrossgate-0.0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2088 2023-04-29 12:32:57.000000 pycrossgate-0.0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:34:35.002751 pycrossgate-0.0.0.1/
+drwxrwxrwx   0        0        0        0 2023-04-29 13:34:34.968037 pycrossgate-0.0.0.1/Core/
+-rw-rw-rw-   0        0        0        0 2023-04-29 12:26:53.000000 pycrossgate-0.0.0.1/Core/__init__.py
+-rw-rw-rw-   0        0        0     1333 2023-04-29 13:34:35.001781 pycrossgate-0.0.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 13:34:34.969051 pycrossgate-0.0.0.1/gui/
+-rw-rw-rw-   0        0        0        0 2023-04-29 12:26:53.000000 pycrossgate-0.0.0.1/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:34:34.970031 pycrossgate-0.0.0.1/hybrides/
+-rw-rw-rw-   0        0        0        0 2023-04-29 12:26:53.000000 pycrossgate-0.0.0.1/hybrides/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:34:34.998866 pycrossgate-0.0.0.1/pycrossgate.egg-info/
+-rw-rw-rw-   0        0        0     1333 2023-04-29 13:34:34.000000 pycrossgate-0.0.0.1/pycrossgate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-04-29 13:34:34.000000 pycrossgate-0.0.0.1/pycrossgate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 13:34:34.000000 pycrossgate-0.0.0.1/pycrossgate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-29 13:34:34.000000 pycrossgate-0.0.0.1/pycrossgate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-04-29 13:34:34.000000 pycrossgate-0.0.0.1/pycrossgate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 13:34:35.000746 pycrossgate-0.0.0.1/serve/
+-rw-rw-rw-   0        0        0        0 2023-04-29 12:26:53.000000 pycrossgate-0.0.0.1/serve/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-29 13:34:35.002751 pycrossgate-0.0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2088 2023-04-29 13:34:31.000000 pycrossgate-0.0.0.1/setup.py
```

### Comparing `pycrossgate-0.0.0.0/PKG-INFO` & `pycrossgate-0.0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrossgate
-Version: 0.0.0.0
+Version: 0.0.0.1
 Summary:  👨‍💻"pycrossgate" is a Python package that automatically imports missing modules on-the-fly, saving time and effort during coding 🛠️⌛
 Home-page: https://github.com/yourusername/pycrossgate
 Author: Juste Elysée MALNADILA
 Author-email: malandilajusteelysee@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycrossgate-0.0.0.0/pycrossgate.egg-info/PKG-INFO` & `pycrossgate-0.0.0.1/pycrossgate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrossgate
-Version: 0.0.0.0
+Version: 0.0.0.1
 Summary:  👨‍💻"pycrossgate" is a Python package that automatically imports missing modules on-the-fly, saving time and effort during coding 🛠️⌛
 Home-page: https://github.com/yourusername/pycrossgate
 Author: Juste Elysée MALNADILA
 Author-email: malandilajusteelysee@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycrossgate-0.0.0.0/setup.py` & `pycrossgate-0.0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import atexit
 
 setup(
     # name=['pycrossgate', 'pycrossgate'],#name='pycrossgate',
     name='pycrossgate',
-    version='0.0.0.0',
+    version='0.0.0.1',
     packages=find_packages(),
     install_requires=[],
     entry_points={
         'console_scripts': [
             'pycrossgate = pycrossgate.__main__:main'
         ]
     },
```


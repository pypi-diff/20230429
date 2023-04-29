# Comparing `tmp/saheffects-0.1.0.tar.gz` & `tmp/saheffects-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saheffects-0.1.0.tar", last modified: Sat Apr 29 19:01:45 2023, max compression
+gzip compressed data, was "saheffects-0.1.1.tar", last modified: Sat Apr 29 19:24:18 2023, max compression
```

## Comparing `saheffects-0.1.0.tar` & `saheffects-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 19:01:45.710434 saheffects-0.1.0/
--rw-rw-rw-   0        0        0      167 2023-04-29 18:57:57.000000 saheffects-0.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3672 2023-04-29 18:57:57.000000 saheffects-0.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-29 18:57:57.000000 saheffects-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1089 2023-04-29 18:57:57.000000 saheffects-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-29 18:57:57.000000 saheffects-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1809 2023-04-29 19:01:45.711433 saheffects-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      949 2023-04-29 19:01:01.000000 saheffects-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-29 19:01:45.649471 saheffects-0.1.0/docs/
--rw-rw-rw-   0        0        0      631 2023-04-29 18:57:57.000000 saheffects-0.1.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-04-29 18:57:57.000000 saheffects-0.1.0/docs/authors.rst
--rw-rw-rw-   0        0        0     4967 2023-04-29 18:57:57.000000 saheffects-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-29 18:57:57.000000 saheffects-0.1.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-29 18:57:57.000000 saheffects-0.1.0/docs/history.rst
--rw-rw-rw-   0        0        0      327 2023-04-29 18:57:57.000000 saheffects-0.1.0/docs/index.rst
--rw-rw-rw-   0        0        0     1189 2023-04-29 18:57:57.000000 saheffects-0.1.0/docs/installation.rst
--rwxrwxrwx   0        0        0      808 2023-04-29 18:57:57.000000 saheffects-0.1.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-29 18:57:57.000000 saheffects-0.1.0/docs/readme.rst
--rw-rw-rw-   0        0        0       82 2023-04-29 18:57:57.000000 saheffects-0.1.0/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-04-29 19:01:45.660465 saheffects-0.1.0/saheffects/
--rw-rw-rw-   0        0        0      131 2023-04-29 18:57:57.000000 saheffects-0.1.0/saheffects/__init__.py
--rw-rw-rw-   0        0        0       20 2023-04-29 18:57:57.000000 saheffects-0.1.0/saheffects/saheffects.py
-drwxrwxrwx   0        0        0        0 2023-04-29 19:01:45.690445 saheffects-0.1.0/saheffects.egg-info/
--rw-rw-rw-   0        0        0     1809 2023-04-29 19:01:44.000000 saheffects-0.1.0/saheffects.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-04-29 19:01:45.000000 saheffects-0.1.0/saheffects.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 19:01:44.000000 saheffects-0.1.0/saheffects.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-29 19:01:44.000000 saheffects-0.1.0/saheffects.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-04-29 19:01:44.000000 saheffects-0.1.0/saheffects.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      453 2023-04-29 19:01:45.713431 saheffects-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1352 2023-04-29 18:57:57.000000 saheffects-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 19:01:45.708434 saheffects-0.1.0/tests/
--rw-rw-rw-   0        0        0       41 2023-04-29 18:57:57.000000 saheffects-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      586 2023-04-29 18:57:57.000000 saheffects-0.1.0/tests/test_saheffects.py
+drwxrwxrwx   0        0        0        0 2023-04-29 19:24:18.300375 saheffects-0.1.1/
+-rw-rw-rw-   0        0        0      167 2023-04-29 18:57:57.000000 saheffects-0.1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3672 2023-04-29 18:57:57.000000 saheffects-0.1.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-29 18:57:57.000000 saheffects-0.1.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1089 2023-04-29 18:57:57.000000 saheffects-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-29 18:57:57.000000 saheffects-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1809 2023-04-29 19:24:18.301375 saheffects-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      949 2023-04-29 19:02:48.000000 saheffects-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-29 19:24:18.268394 saheffects-0.1.1/docs/
+-rw-rw-rw-   0        0        0      631 2023-04-29 18:57:57.000000 saheffects-0.1.1/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-29 18:57:57.000000 saheffects-0.1.1/docs/authors.rst
+-rw-rw-rw-   0        0        0     4967 2023-04-29 18:57:57.000000 saheffects-0.1.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-29 18:57:57.000000 saheffects-0.1.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-29 18:57:57.000000 saheffects-0.1.1/docs/history.rst
+-rw-rw-rw-   0        0        0      327 2023-04-29 18:57:57.000000 saheffects-0.1.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1189 2023-04-29 18:57:57.000000 saheffects-0.1.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      808 2023-04-29 18:57:57.000000 saheffects-0.1.1/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-29 18:57:57.000000 saheffects-0.1.1/docs/readme.rst
+-rw-rw-rw-   0        0        0       82 2023-04-29 18:57:57.000000 saheffects-0.1.1/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-29 19:24:18.272392 saheffects-0.1.1/saheffects/
+-rw-rw-rw-   0        0        0      131 2023-04-29 18:57:57.000000 saheffects-0.1.1/saheffects/__init__.py
+-rw-rw-rw-   0        0        0       20 2023-04-29 18:57:57.000000 saheffects-0.1.1/saheffects/saheffects.py
+drwxrwxrwx   0        0        0        0 2023-04-29 19:24:18.295378 saheffects-0.1.1/saheffects.egg-info/
+-rw-rw-rw-   0        0        0     1809 2023-04-29 19:24:17.000000 saheffects-0.1.1/saheffects.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-04-29 19:24:18.000000 saheffects-0.1.1/saheffects.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 19:24:17.000000 saheffects-0.1.1/saheffects.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-29 19:01:44.000000 saheffects-0.1.1/saheffects.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-04-29 19:24:17.000000 saheffects-0.1.1/saheffects.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      453 2023-04-29 19:24:18.303373 saheffects-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1352 2023-04-29 19:24:03.000000 saheffects-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 19:24:18.299377 saheffects-0.1.1/tests/
+-rw-rw-rw-   0        0        0       41 2023-04-29 18:57:57.000000 saheffects-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      586 2023-04-29 18:57:57.000000 saheffects-0.1.1/tests/test_saheffects.py
```

### Comparing `saheffects-0.1.0/CONTRIBUTING.rst` & `saheffects-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `saheffects-0.1.0/LICENSE` & `saheffects-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `saheffects-0.1.0/PKG-INFO` & `saheffects-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saheffects
-Version: 0.1.0
+Version: 0.1.1
 Summary: saheffects  is a Python package for applying various image filters to images.
 Home-page: https://github.com/SahSofts/saheffects
 Author: SahSofts
 Author-email: sahsofts97@gmail.com
 License: MIT license
 Keywords: saheffects
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `saheffects-0.1.0/README.rst` & `saheffects-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `saheffects-0.1.0/docs/Makefile` & `saheffects-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `saheffects-0.1.0/docs/conf.py` & `saheffects-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `saheffects-0.1.0/docs/installation.rst` & `saheffects-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `saheffects-0.1.0/docs/make.bat` & `saheffects-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `saheffects-0.1.0/saheffects.egg-info/PKG-INFO` & `saheffects-0.1.1/saheffects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saheffects
-Version: 0.1.0
+Version: 0.1.1
 Summary: saheffects  is a Python package for applying various image filters to images.
 Home-page: https://github.com/SahSofts/saheffects
 Author: SahSofts
 Author-email: sahsofts97@gmail.com
 License: MIT license
 Keywords: saheffects
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `saheffects-0.1.0/saheffects.egg-info/SOURCES.txt` & `saheffects-0.1.1/saheffects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saheffects-0.1.0/setup.py` & `saheffects-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='saheffects',
     name='saheffects',
     packages=find_packages(include=['saheffects', 'saheffects.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/SahSofts/saheffects',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `saheffects-0.1.0/tests/test_saheffects.py` & `saheffects-0.1.1/tests/test_saheffects.py`

 * *Files identical despite different names*


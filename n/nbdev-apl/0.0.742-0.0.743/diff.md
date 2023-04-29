# Comparing `tmp/nbdev-apl-0.0.742.tar.gz` & `tmp/nbdev-apl-0.0.743.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbdev-apl-0.0.742.tar", last modified: Sat Apr 29 01:42:14 2023, max compression
+gzip compressed data, was "nbdev-apl-0.0.743.tar", last modified: Sat Apr 29 13:15:44 2023, max compression
```

## Comparing `nbdev-apl-0.0.742.tar` & `nbdev-apl-0.0.743.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:42:14.342007 nbdev-apl-0.0.742/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 01:31:29.000000 nbdev-apl-0.0.742/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-29 01:31:29.000000 nbdev-apl-0.0.742/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-29 01:42:14.342007 nbdev-apl-0.0.742/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-29 01:31:29.000000 nbdev-apl-0.0.742/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:42:14.342007 nbdev-apl-0.0.742/nbdev_apl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 01:42:14.000000 nbdev-apl-0.0.742/nbdev_apl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-29 01:31:29.000000 nbdev-apl-0.0.742/nbdev_apl/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-29 01:42:14.000000 nbdev-apl-0.0.742/nbdev_apl/_nbdev.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:42:14.342007 nbdev-apl-0.0.742/nbdev_apl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-29 01:42:14.000000 nbdev-apl-0.0.742/nbdev_apl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-29 01:42:14.000000 nbdev-apl-0.0.742/nbdev_apl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 01:42:14.000000 nbdev-apl-0.0.742/nbdev_apl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-29 01:42:14.000000 nbdev-apl-0.0.742/nbdev_apl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 01:42:14.000000 nbdev-apl-0.0.742/nbdev_apl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 01:42:14.000000 nbdev-apl-0.0.742/nbdev_apl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 01:42:14.000000 nbdev-apl-0.0.742/nbdev_apl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-29 01:42:14.000000 nbdev-apl-0.0.742/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 01:42:14.342007 nbdev-apl-0.0.742/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-29 01:31:29.000000 nbdev-apl-0.0.742/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:15:44.898072 nbdev-apl-0.0.743/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 13:04:51.000000 nbdev-apl-0.0.743/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-29 13:04:51.000000 nbdev-apl-0.0.743/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-29 13:15:44.898072 nbdev-apl-0.0.743/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-29 13:04:51.000000 nbdev-apl-0.0.743/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:15:44.898072 nbdev-apl-0.0.743/nbdev_apl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 13:15:44.000000 nbdev-apl-0.0.743/nbdev_apl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-29 13:04:51.000000 nbdev-apl-0.0.743/nbdev_apl/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-29 13:15:44.000000 nbdev-apl-0.0.743/nbdev_apl/_nbdev.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:15:44.898072 nbdev-apl-0.0.743/nbdev_apl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-29 13:15:44.000000 nbdev-apl-0.0.743/nbdev_apl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-29 13:15:44.000000 nbdev-apl-0.0.743/nbdev_apl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:15:44.000000 nbdev-apl-0.0.743/nbdev_apl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-29 13:15:44.000000 nbdev-apl-0.0.743/nbdev_apl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:15:44.000000 nbdev-apl-0.0.743/nbdev_apl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 13:15:44.000000 nbdev-apl-0.0.743/nbdev_apl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 13:15:44.000000 nbdev-apl-0.0.743/nbdev_apl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-29 13:15:44.000000 nbdev-apl-0.0.743/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 13:15:44.898072 nbdev-apl-0.0.743/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-29 13:04:51.000000 nbdev-apl-0.0.743/setup.py
```

### Comparing `nbdev-apl-0.0.742/LICENSE` & `nbdev-apl-0.0.743/LICENSE`

 * *Files identical despite different names*

### Comparing `nbdev-apl-0.0.742/PKG-INFO` & `nbdev-apl-0.0.743/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdev-apl
-Version: 0.0.742
+Version: 0.0.743
 Summary: nbdev docs lookup for numpy
 Home-page: https://github.com/fastai/nbdev-index/tree/master/
 Author: Jeremy Howard
 Author-email: info@fast.ai
 License: Apache Software License 2.0
 Keywords: nbdev fastai python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nbdev-apl-0.0.742/nbdev_apl/_modidx.py` & `nbdev-apl-0.0.743/nbdev_apl/_modidx.py`

 * *Files identical despite different names*

### Comparing `nbdev-apl-0.0.742/nbdev_apl.egg-info/PKG-INFO` & `nbdev-apl-0.0.743/nbdev_apl.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdev-apl
-Version: 0.0.742
+Version: 0.0.743
 Summary: nbdev docs lookup for numpy
 Home-page: https://github.com/fastai/nbdev-index/tree/master/
 Author: Jeremy Howard
 Author-email: info@fast.ai
 License: Apache Software License 2.0
 Keywords: nbdev fastai python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nbdev-apl-0.0.742/setup.py` & `nbdev-apl-0.0.743/setup.py`

 * *Files identical despite different names*


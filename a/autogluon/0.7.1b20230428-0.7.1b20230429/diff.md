# Comparing `tmp/autogluon-0.7.1b20230428.tar.gz` & `tmp/autogluon-0.7.1b20230429.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.7.1b20230428.tar", last modified: Fri Apr 28 09:04:38 2023, max compression
+gzip compressed data, was "autogluon-0.7.1b20230429.tar", last modified: Sat Apr 29 09:04:23 2023, max compression
```

## Comparing `autogluon-0.7.1b20230428.tar` & `autogluon-0.7.1b20230429.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:04:38.428729 autogluon-0.7.1b20230428/
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-04-28 09:04:38.428729 autogluon-0.7.1b20230428/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:04:38.428729 autogluon-0.7.1b20230428/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-28 09:03:36.000000 autogluon-0.7.1b20230428/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:04:38.424729 autogluon-0.7.1b20230428/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:04:38.424729 autogluon-0.7.1b20230428/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 09:03:36.000000 autogluon-0.7.1b20230428/src/autogluon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 09:04:38.000000 autogluon-0.7.1b20230428/src/autogluon/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:04:38.428729 autogluon-0.7.1b20230428/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-04-28 09:04:38.000000 autogluon-0.7.1b20230428/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-28 09:04:38.000000 autogluon-0.7.1b20230428/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:04:38.000000 autogluon-0.7.1b20230428/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 09:04:38.000000 autogluon-0.7.1b20230428/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-28 09:04:38.000000 autogluon-0.7.1b20230428/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 09:04:38.000000 autogluon-0.7.1b20230428/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:04:38.000000 autogluon-0.7.1b20230428/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:04:23.244120 autogluon-0.7.1b20230429/
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-04-29 09:04:23.244120 autogluon-0.7.1b20230429/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 09:04:23.244120 autogluon-0.7.1b20230429/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-29 09:03:32.000000 autogluon-0.7.1b20230429/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:04:23.240120 autogluon-0.7.1b20230429/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:04:23.240120 autogluon-0.7.1b20230429/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-29 09:03:32.000000 autogluon-0.7.1b20230429/src/autogluon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 09:04:23.000000 autogluon-0.7.1b20230429/src/autogluon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:04:23.240120 autogluon-0.7.1b20230429/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-04-29 09:04:23.000000 autogluon-0.7.1b20230429/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-29 09:04:23.000000 autogluon-0.7.1b20230429/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 09:04:23.000000 autogluon-0.7.1b20230429/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 09:04:23.000000 autogluon-0.7.1b20230429/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-29 09:04:23.000000 autogluon-0.7.1b20230429/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 09:04:23.000000 autogluon-0.7.1b20230429/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 09:04:23.000000 autogluon-0.7.1b20230429/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.7.1b20230428/PKG-INFO` & `autogluon-0.7.1b20230429/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.7.1b20230428
+Version: 0.7.1b20230429
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-0.7.1b20230428/setup.py` & `autogluon-0.7.1b20230429/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.7.1b20230428/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.7.1b20230429/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.7.1b20230428
+Version: 0.7.1b20230429
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```


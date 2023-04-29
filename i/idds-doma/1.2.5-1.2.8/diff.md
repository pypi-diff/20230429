# Comparing `tmp/idds-doma-1.2.5.tar.gz` & `tmp/idds-doma-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-doma-1.2.5.tar", last modified: Tue Apr 25 19:18:01 2023, max compression
+gzip compressed data, was "idds-doma-1.2.8.tar", last modified: Sat Apr 29 14:38:42 2023, max compression
```

## Comparing `idds-doma-1.2.5.tar` & `idds-doma-1.2.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:01.352344 idds-doma-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 19:17:47.000000 idds-doma-1.2.5/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-25 19:18:01.352344 idds-doma-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-25 19:17:47.000000 idds-doma-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:01.352344 idds-doma-1.2.5/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      747 2023-04-25 19:17:47.000000 idds-doma-1.2.5/bin/setup_panda_token
--rwxr-xr-x   0 runner    (1001) docker     (123)    10028 2023-04-25 19:17:47.000000 idds-doma-1.2.5/bin/setup_panda_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:01.352344 idds-doma-1.2.5/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:01.352344 idds-doma-1.2.5/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 19:17:47.000000 idds-doma-1.2.5/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:01.352344 idds-doma-1.2.5/lib/idds/doma/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 19:17:47.000000 idds-doma-1.2.5/lib/idds/doma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 19:17:56.000000 idds-doma-1.2.5/lib/idds/doma/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:01.352344 idds-doma-1.2.5/lib/idds/doma/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 19:17:47.000000 idds-doma-1.2.5/lib/idds/doma/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56124 2023-04-25 19:17:47.000000 idds-doma-1.2.5/lib/idds/doma/workflow/domapandawork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:01.352344 idds-doma-1.2.5/lib/idds/doma/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 19:17:47.000000 idds-doma-1.2.5/lib/idds/doma/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68326 2023-04-25 19:17:47.000000 idds-doma-1.2.5/lib/idds/doma/workflowv2/domapandawork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:01.352344 idds-doma-1.2.5/lib/idds_doma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-25 19:18:01.000000 idds-doma-1.2.5/lib/idds_doma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-25 19:18:01.000000 idds-doma-1.2.5/lib/idds_doma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 19:18:01.000000 idds-doma-1.2.5/lib/idds_doma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-25 19:18:01.000000 idds-doma-1.2.5/lib/idds_doma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 19:18:01.000000 idds-doma-1.2.5/lib/idds_doma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 19:18:01.352344 idds-doma-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-25 19:17:47.000000 idds-doma-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:01.352344 idds-doma-1.2.5/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:01.352344 idds-doma-1.2.5/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-25 19:17:56.000000 idds-doma-1.2.5/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-29 14:38:28.000000 idds-doma-1.2.8/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-29 14:38:42.384074 idds-doma-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-29 14:38:28.000000 idds-doma-1.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      747 2023-04-29 14:38:28.000000 idds-doma-1.2.8/bin/setup_panda_token
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10028 2023-04-29 14:38:28.000000 idds-doma-1.2.8/bin/setup_panda_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 14:38:28.000000 idds-doma-1.2.8/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/lib/idds/doma/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 14:38:28.000000 idds-doma-1.2.8/lib/idds/doma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 14:38:37.000000 idds-doma-1.2.8/lib/idds/doma/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/lib/idds/doma/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 14:38:28.000000 idds-doma-1.2.8/lib/idds/doma/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56124 2023-04-29 14:38:28.000000 idds-doma-1.2.8/lib/idds/doma/workflow/domapandawork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/lib/idds/doma/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 14:38:28.000000 idds-doma-1.2.8/lib/idds/doma/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68326 2023-04-29 14:38:28.000000 idds-doma-1.2.8/lib/idds/doma/workflowv2/domapandawork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/lib/idds_doma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-29 14:38:42.000000 idds-doma-1.2.8/lib/idds_doma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-29 14:38:42.000000 idds-doma-1.2.8/lib/idds_doma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 14:38:42.000000 idds-doma-1.2.8/lib/idds_doma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-29 14:38:42.000000 idds-doma-1.2.8/lib/idds_doma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 14:38:42.000000 idds-doma-1.2.8/lib/idds_doma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-29 14:38:42.384074 idds-doma-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-29 14:38:28.000000 idds-doma-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-29 14:38:37.000000 idds-doma-1.2.8/tools/env/environment.yml
```

### Comparing `idds-doma-1.2.5/LICENSE.rst` & `idds-doma-1.2.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.5/PKG-INFO` & `idds-doma-1.2.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
-Version: 1.2.5
+Version: 1.2.8
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-doma-1.2.5/bin/setup_panda_token` & `idds-doma-1.2.8/bin/setup_panda_token`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.5/bin/setup_panda_token.py` & `idds-doma-1.2.8/bin/setup_panda_token.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.5/lib/idds/doma/workflow/domapandawork.py` & `idds-doma-1.2.8/lib/idds/doma/workflow/domapandawork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.5/lib/idds/doma/workflowv2/domapandawork.py` & `idds-doma-1.2.8/lib/idds/doma/workflowv2/domapandawork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.5/lib/idds_doma.egg-info/PKG-INFO` & `idds-doma-1.2.8/lib/idds_doma.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
-Version: 1.2.5
+Version: 1.2.8
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-doma-1.2.5/lib/idds_doma.egg-info/SOURCES.txt` & `idds-doma-1.2.8/lib/idds_doma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.5/setup.py` & `idds-doma-1.2.8/setup.py`

 * *Files identical despite different names*


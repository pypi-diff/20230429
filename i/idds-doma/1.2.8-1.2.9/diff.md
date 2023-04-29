# Comparing `tmp/idds-doma-1.2.8.tar.gz` & `tmp/idds-doma-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-doma-1.2.8.tar", last modified: Sat Apr 29 14:38:42 2023, max compression
+gzip compressed data, was "idds-doma-1.2.9.tar", last modified: Sat Apr 29 19:24:59 2023, max compression
```

## Comparing `idds-doma-1.2.8.tar` & `idds-doma-1.2.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-29 14:38:28.000000 idds-doma-1.2.8/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-29 14:38:42.384074 idds-doma-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-29 14:38:28.000000 idds-doma-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      747 2023-04-29 14:38:28.000000 idds-doma-1.2.8/bin/setup_panda_token
--rwxr-xr-x   0 runner    (1001) docker     (123)    10028 2023-04-29 14:38:28.000000 idds-doma-1.2.8/bin/setup_panda_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 14:38:28.000000 idds-doma-1.2.8/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/lib/idds/doma/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 14:38:28.000000 idds-doma-1.2.8/lib/idds/doma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 14:38:37.000000 idds-doma-1.2.8/lib/idds/doma/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/lib/idds/doma/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 14:38:28.000000 idds-doma-1.2.8/lib/idds/doma/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56124 2023-04-29 14:38:28.000000 idds-doma-1.2.8/lib/idds/doma/workflow/domapandawork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/lib/idds/doma/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 14:38:28.000000 idds-doma-1.2.8/lib/idds/doma/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68326 2023-04-29 14:38:28.000000 idds-doma-1.2.8/lib/idds/doma/workflowv2/domapandawork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/lib/idds_doma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-29 14:38:42.000000 idds-doma-1.2.8/lib/idds_doma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-29 14:38:42.000000 idds-doma-1.2.8/lib/idds_doma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 14:38:42.000000 idds-doma-1.2.8/lib/idds_doma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-29 14:38:42.000000 idds-doma-1.2.8/lib/idds_doma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 14:38:42.000000 idds-doma-1.2.8/lib/idds_doma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-29 14:38:42.384074 idds-doma-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-29 14:38:28.000000 idds-doma-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:42.384074 idds-doma-1.2.8/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-29 14:38:37.000000 idds-doma-1.2.8/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-29 19:24:44.000000 idds-doma-1.2.9/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-29 19:24:59.595692 idds-doma-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-29 19:24:44.000000 idds-doma-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      747 2023-04-29 19:24:44.000000 idds-doma-1.2.9/bin/setup_panda_token
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10028 2023-04-29 19:24:44.000000 idds-doma-1.2.9/bin/setup_panda_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-doma-1.2.9/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/lib/idds/doma/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-doma-1.2.9/lib/idds/doma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 19:24:53.000000 idds-doma-1.2.9/lib/idds/doma/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/lib/idds/doma/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-doma-1.2.9/lib/idds/doma/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56124 2023-04-29 19:24:44.000000 idds-doma-1.2.9/lib/idds/doma/workflow/domapandawork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/lib/idds/doma/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-doma-1.2.9/lib/idds/doma/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68326 2023-04-29 19:24:44.000000 idds-doma-1.2.9/lib/idds/doma/workflowv2/domapandawork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/lib/idds_doma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-29 19:24:59.000000 idds-doma-1.2.9/lib/idds_doma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-29 19:24:59.000000 idds-doma-1.2.9/lib/idds_doma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 19:24:59.000000 idds-doma-1.2.9/lib/idds_doma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-29 19:24:59.000000 idds-doma-1.2.9/lib/idds_doma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 19:24:59.000000 idds-doma-1.2.9/lib/idds_doma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-29 19:24:59.595692 idds-doma-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-29 19:24:44.000000 idds-doma-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-29 19:24:53.000000 idds-doma-1.2.9/tools/env/environment.yml
```

### Comparing `idds-doma-1.2.8/LICENSE.rst` & `idds-doma-1.2.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.8/PKG-INFO` & `idds-doma-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
-Version: 1.2.8
+Version: 1.2.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-doma-1.2.8/bin/setup_panda_token` & `idds-doma-1.2.9/bin/setup_panda_token`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.8/bin/setup_panda_token.py` & `idds-doma-1.2.9/bin/setup_panda_token.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.8/lib/idds/doma/workflow/domapandawork.py` & `idds-doma-1.2.9/lib/idds/doma/workflow/domapandawork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.8/lib/idds/doma/workflowv2/domapandawork.py` & `idds-doma-1.2.9/lib/idds/doma/workflowv2/domapandawork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.8/lib/idds_doma.egg-info/PKG-INFO` & `idds-doma-1.2.9/lib/idds_doma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
-Version: 1.2.8
+Version: 1.2.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-doma-1.2.8/lib/idds_doma.egg-info/SOURCES.txt` & `idds-doma-1.2.9/lib/idds_doma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.8/setup.py` & `idds-doma-1.2.9/setup.py`

 * *Files identical despite different names*


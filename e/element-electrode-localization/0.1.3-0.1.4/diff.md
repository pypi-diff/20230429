# Comparing `tmp/element-electrode-localization-0.1.3.tar.gz` & `tmp/element-electrode-localization-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-electrode-localization-0.1.3.tar", last modified: Fri Apr 21 18:30:19 2023, max compression
+gzip compressed data, was "element-electrode-localization-0.1.4.tar", last modified: Fri Apr 28 22:42:15 2023, max compression
```

## Comparing `element-electrode-localization-0.1.3.tar` & `element-electrode-localization-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:30:19.286504 element-electrode-localization-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-21 18:30:15.000000 element-electrode-localization-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-21 18:30:19.286504 element-electrode-localization-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-21 18:30:15.000000 element-electrode-localization-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:30:19.286504 element-electrode-localization-0.1.3/element_electrode_localization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:30:15.000000 element-electrode-localization-0.1.3/element_electrode_localization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-21 18:30:15.000000 element-electrode-localization-0.1.3/element_electrode_localization/coordinate_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-04-21 18:30:15.000000 element-electrode-localization-0.1.3/element_electrode_localization/electrode_localization.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-21 18:30:15.000000 element-electrode-localization-0.1.3/element_electrode_localization/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:30:19.286504 element-electrode-localization-0.1.3/element_electrode_localization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-21 18:30:19.000000 element-electrode-localization-0.1.3/element_electrode_localization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-21 18:30:19.000000 element-electrode-localization-0.1.3/element_electrode_localization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:30:19.000000 element-electrode-localization-0.1.3/element_electrode_localization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 18:30:19.000000 element-electrode-localization-0.1.3/element_electrode_localization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 18:30:19.000000 element-electrode-localization-0.1.3/element_electrode_localization.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 18:30:19.286504 element-electrode-localization-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-21 18:30:15.000000 element-electrode-localization-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:42:15.336622 element-electrode-localization-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-28 22:42:12.000000 element-electrode-localization-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-28 22:42:15.336622 element-electrode-localization-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-28 22:42:12.000000 element-electrode-localization-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:42:15.336622 element-electrode-localization-0.1.4/element_electrode_localization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:42:12.000000 element-electrode-localization-0.1.4/element_electrode_localization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-28 22:42:12.000000 element-electrode-localization-0.1.4/element_electrode_localization/coordinate_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-04-28 22:42:12.000000 element-electrode-localization-0.1.4/element_electrode_localization/electrode_localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 22:42:12.000000 element-electrode-localization-0.1.4/element_electrode_localization/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:42:15.336622 element-electrode-localization-0.1.4/element_electrode_localization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-28 22:42:15.000000 element-electrode-localization-0.1.4/element_electrode_localization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-28 22:42:15.000000 element-electrode-localization-0.1.4/element_electrode_localization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:42:15.000000 element-electrode-localization-0.1.4/element_electrode_localization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 22:42:15.000000 element-electrode-localization-0.1.4/element_electrode_localization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-28 22:42:15.000000 element-electrode-localization-0.1.4/element_electrode_localization.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:42:15.336622 element-electrode-localization-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-28 22:42:12.000000 element-electrode-localization-0.1.4/setup.py
```

### Comparing `element-electrode-localization-0.1.3/LICENSE` & `element-electrode-localization-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `element-electrode-localization-0.1.3/PKG-INFO` & `element-electrode-localization-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-electrode-localization
-Version: 0.1.3
+Version: 0.1.4
 Summary: Electrode localization DataJoint element
 Home-page: https://github.com/datajoint/element-electrode-localization
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience electrode science datajoint
 Platform: UNKNOWN
```

### Comparing `element-electrode-localization-0.1.3/README.md` & `element-electrode-localization-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `element-electrode-localization-0.1.3/element_electrode_localization/coordinate_framework.py` & `element-electrode-localization-0.1.4/element_electrode_localization/coordinate_framework.py`

 * *Files identical despite different names*

### Comparing `element-electrode-localization-0.1.3/element_electrode_localization/electrode_localization.py` & `element-electrode-localization-0.1.4/element_electrode_localization/electrode_localization.py`

 * *Files identical despite different names*

### Comparing `element-electrode-localization-0.1.3/element_electrode_localization.egg-info/PKG-INFO` & `element-electrode-localization-0.1.4/element_electrode_localization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-electrode-localization
-Version: 0.1.3
+Version: 0.1.4
 Summary: Electrode localization DataJoint element
 Home-page: https://github.com/datajoint/element-electrode-localization
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience electrode science datajoint
 Platform: UNKNOWN
```

### Comparing `element-electrode-localization-0.1.3/setup.py` & `element-electrode-localization-0.1.4/setup.py`

 * *Files identical despite different names*


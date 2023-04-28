# Comparing `tmp/element-array-ephys-0.2.7.tar.gz` & `tmp/element-array-ephys-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-array-ephys-0.2.7.tar", last modified: Thu Apr 20 14:14:54 2023, max compression
+gzip compressed data, was "element-array-ephys-0.2.8.tar", last modified: Fri Apr 28 22:38:16 2023, max compression
```

## Comparing `element-array-ephys-0.2.7.tar` & `element-array-ephys-0.2.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:14:54.467100 element-array-ephys-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-20 14:14:54.463100 element-array-ephys-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:14:54.463100 element-array-ephys-0.2.7/element_array_ephys/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63954 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/ephys_acute.py
--rw-r--r--   0 runner    (1001) docker     (123)    61073 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/ephys_chronic.py
--rw-r--r--   0 runner    (1001) docker     (123)    61593 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/ephys_no_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)    57140 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/ephys_precluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/ephys_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:14:54.463100 element-array-ephys-0.2.7/element_array_ephys/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:14:54.463100 element-array-ephys-0.2.7/element_array_ephys/export/nwb/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/export/nwb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24154 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/export/nwb/nwb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:14:54.463100 element-array-ephys-0.2.7/element_array_ephys/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/plotting/corr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/plotting/probe_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    15284 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/plotting/qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/plotting/unit_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/plotting/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/probe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:14:54.463100 element-array-ephys-0.2.7/element_array_ephys/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/readers/kilosort.py
--rw-r--r--   0 runner    (1001) docker     (123)    30278 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/readers/kilosort_triggering.py
--rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/readers/openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/readers/spikeglx.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/readers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/element_array_ephys/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:14:54.463100 element-array-ephys-0.2.7/element_array_ephys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-20 14:14:54.000000 element-array-ephys-0.2.7/element_array_ephys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-20 14:14:54.000000 element-array-ephys-0.2.7/element_array_ephys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:14:54.000000 element-array-ephys-0.2.7/element_array_ephys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-20 14:14:54.000000 element-array-ephys-0.2.7/element_array_ephys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 14:14:54.000000 element-array-ephys-0.2.7/element_array_ephys.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:14:54.467100 element-array-ephys-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-20 14:14:49.000000 element-array-ephys-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:38:16.426767 element-array-ephys-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-28 22:38:16.426767 element-array-ephys-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:38:16.422767 element-array-ephys-0.2.8/element_array_ephys/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63954 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/ephys_acute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61073 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/ephys_chronic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61593 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/ephys_no_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57140 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/ephys_precluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/ephys_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:38:16.426767 element-array-ephys-0.2.8/element_array_ephys/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:38:16.426767 element-array-ephys-0.2.8/element_array_ephys/export/nwb/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/export/nwb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24154 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/export/nwb/nwb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:38:16.426767 element-array-ephys-0.2.8/element_array_ephys/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/plotting/corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/plotting/probe_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15284 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/plotting/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/plotting/unit_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/plotting/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/probe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:38:16.426767 element-array-ephys-0.2.8/element_array_ephys/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/readers/kilosort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30278 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/readers/kilosort_triggering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/readers/openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/readers/spikeglx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/readers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/element_array_ephys/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:38:16.426767 element-array-ephys-0.2.8/element_array_ephys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-28 22:38:16.000000 element-array-ephys-0.2.8/element_array_ephys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-28 22:38:16.000000 element-array-ephys-0.2.8/element_array_ephys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:38:16.000000 element-array-ephys-0.2.8/element_array_ephys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-28 22:38:16.000000 element-array-ephys-0.2.8/element_array_ephys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 22:38:16.000000 element-array-ephys-0.2.8/element_array_ephys.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:38:16.426767 element-array-ephys-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-28 22:38:13.000000 element-array-ephys-0.2.8/setup.py
```

### Comparing `element-array-ephys-0.2.7/LICENSE` & `element-array-ephys-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/PKG-INFO` & `element-array-ephys-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-array-ephys
-Version: 0.2.7
+Version: 0.2.8
 Summary: DataJoint Element for Extracellular Array Electrophysiology
 Home-page: https://github.com/datajoint/element-array-ephys
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience electrophysiology science datajoint
 Platform: UNKNOWN
```

### Comparing `element-array-ephys-0.2.7/README.md` & `element-array-ephys-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/ephys_acute.py` & `element-array-ephys-0.2.8/element_array_ephys/ephys_acute.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/ephys_chronic.py` & `element-array-ephys-0.2.8/element_array_ephys/ephys_chronic.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/ephys_no_curation.py` & `element-array-ephys-0.2.8/element_array_ephys/ephys_no_curation.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/ephys_precluster.py` & `element-array-ephys-0.2.8/element_array_ephys/ephys_precluster.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/ephys_report.py` & `element-array-ephys-0.2.8/element_array_ephys/ephys_report.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/export/nwb/nwb.py` & `element-array-ephys-0.2.8/element_array_ephys/export/nwb/nwb.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/plotting/corr.py` & `element-array-ephys-0.2.8/element_array_ephys/plotting/corr.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/plotting/probe_level.py` & `element-array-ephys-0.2.8/element_array_ephys/plotting/probe_level.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/plotting/qc.py` & `element-array-ephys-0.2.8/element_array_ephys/plotting/qc.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/plotting/unit_level.py` & `element-array-ephys-0.2.8/element_array_ephys/plotting/unit_level.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/plotting/widget.py` & `element-array-ephys-0.2.8/element_array_ephys/plotting/widget.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/probe.py` & `element-array-ephys-0.2.8/element_array_ephys/probe.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/readers/kilosort.py` & `element-array-ephys-0.2.8/element_array_ephys/readers/kilosort.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/readers/kilosort_triggering.py` & `element-array-ephys-0.2.8/element_array_ephys/readers/kilosort_triggering.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/readers/openephys.py` & `element-array-ephys-0.2.8/element_array_ephys/readers/openephys.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys/readers/spikeglx.py` & `element-array-ephys-0.2.8/element_array_ephys/readers/spikeglx.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/element_array_ephys.egg-info/PKG-INFO` & `element-array-ephys-0.2.8/element_array_ephys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-array-ephys
-Version: 0.2.7
+Version: 0.2.8
 Summary: DataJoint Element for Extracellular Array Electrophysiology
 Home-page: https://github.com/datajoint/element-array-ephys
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience electrophysiology science datajoint
 Platform: UNKNOWN
```

### Comparing `element-array-ephys-0.2.7/element_array_ephys.egg-info/SOURCES.txt` & `element-array-ephys-0.2.8/element_array_ephys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.7/setup.py` & `element-array-ephys-0.2.8/setup.py`

 * *Files identical despite different names*


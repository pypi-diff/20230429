# Comparing `tmp/audioviz-0.1.3.tar.gz` & `tmp/audioviz-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioviz-0.1.3.tar", last modified: Thu Apr 27 03:19:27 2023, max compression
+gzip compressed data, was "audioviz-0.1.4.tar", last modified: Sat Apr 29 03:34:31 2023, max compression
```

## Comparing `audioviz-0.1.3.tar` & `audioviz-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-27 03:19:27.951593 audioviz-0.1.3/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      684 2023-04-27 03:19:27.951593 audioviz-0.1.3/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1258 2023-04-25 05:51:15.000000 audioviz-0.1.3/README.md
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-27 03:19:27.951593 audioviz-0.1.3/audioviz/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.1.3/audioviz/BeatAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9467 2023-04-23 03:57:05.000000 audioviz-0.1.3/audioviz/ChordAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     3211 2023-04-23 03:57:05.000000 audioviz-0.1.3/audioviz/GeneralAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.3/audioviz/PitchAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.1.3/audioviz/StructureAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.3/audioviz/TimbreAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      238 2023-04-23 03:57:05.000000 audioviz-0.1.3/audioviz/__init__.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.1.3/audioviz/colabInterface.py
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-27 03:19:27.951593 audioviz-0.1.3/audioviz.egg-info/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      684 2023-04-27 03:19:27.000000 audioviz-0.1.3/audioviz.egg-info/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      428 2023-04-27 03:19:27.000000 audioviz-0.1.3/audioviz.egg-info/SOURCES.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.3/audioviz.egg-info/dependency_links.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.3/audioviz.egg-info/not-zip-safe
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       51 2023-04-27 03:19:27.000000 audioviz-0.1.3/audioviz.egg-info/requires.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-04-27 03:19:27.000000 audioviz-0.1.3/audioviz.egg-info/top_level.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-04-27 03:19:27.951593 audioviz-0.1.3/setup.cfg
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1122 2023-04-27 03:18:14.000000 audioviz-0.1.3/setup.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-29 03:34:31.307517 audioviz-0.1.4/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      684 2023-04-29 03:34:31.307517 audioviz-0.1.4/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1258 2023-04-25 05:51:15.000000 audioviz-0.1.4/README.md
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-29 03:34:31.307517 audioviz-0.1.4/audioviz/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.1.4/audioviz/BeatAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9467 2023-04-23 03:57:05.000000 audioviz-0.1.4/audioviz/ChordAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     3211 2023-04-23 03:57:05.000000 audioviz-0.1.4/audioviz/GeneralAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.4/audioviz/PitchAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.1.4/audioviz/StructureAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.4/audioviz/TimbreAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      264 2023-04-29 03:28:24.000000 audioviz-0.1.4/audioviz/__init__.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.1.4/audioviz/colabInterface.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      708 2023-04-29 03:30:14.000000 audioviz-0.1.4/audioviz/utils.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-29 03:34:31.307517 audioviz-0.1.4/audioviz.egg-info/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      684 2023-04-29 03:34:31.000000 audioviz-0.1.4/audioviz.egg-info/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      446 2023-04-29 03:34:31.000000 audioviz-0.1.4/audioviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-29 03:34:31.000000 audioviz-0.1.4/audioviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.4/audioviz.egg-info/not-zip-safe
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       51 2023-04-29 03:34:31.000000 audioviz-0.1.4/audioviz.egg-info/requires.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-04-29 03:34:31.000000 audioviz-0.1.4/audioviz.egg-info/top_level.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-04-29 03:34:31.307517 audioviz-0.1.4/setup.cfg
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1122 2023-04-29 03:33:20.000000 audioviz-0.1.4/setup.py
```

### Comparing `audioviz-0.1.3/PKG-INFO` & `audioviz-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.1.3
+Version: 0.1.4
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `audioviz-0.1.3/README.md` & `audioviz-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.3/audioviz/BeatAnalysis.py` & `audioviz-0.1.4/audioviz/BeatAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.3/audioviz/ChordAnalysis.py` & `audioviz-0.1.4/audioviz/ChordAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.3/audioviz/GeneralAnalysis.py` & `audioviz-0.1.4/audioviz/GeneralAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.3/audioviz/PitchAnalysis.py` & `audioviz-0.1.4/audioviz/PitchAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.3/audioviz/StructureAnalysis.py` & `audioviz-0.1.4/audioviz/StructureAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.3/audioviz/TimbreAnalysis.py` & `audioviz-0.1.4/audioviz/TimbreAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.3/audioviz/colabInterface.py` & `audioviz-0.1.4/audioviz/colabInterface.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.3/audioviz.egg-info/PKG-INFO` & `audioviz-0.1.4/audioviz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.1.3
+Version: 0.1.4
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `audioviz-0.1.3/setup.py` & `audioviz-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='audioviz',
     packages=['audioviz'],
-    version='0.1.3',
+    version='0.1.4',
     description='An user-friendly music information retrieval tools interfacing with Google Colab',
 
     url='https://github.com/TrangDuLam/audioviz',
     author='ayTrang',
     author_email='andrew.chuang@gapp.nthu.edu.tw',
     license='MIT',
     zip_safe=False,
```


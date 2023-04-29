# Comparing `tmp/ukmon_meteortools-2023.4.21.tar.gz` & `tmp/ukmon_meteortools-2023.4.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukmon_meteortools-2023.4.21.tar", last modified: Sat Apr 29 13:57:33 2023, max compression
+gzip compressed data, was "ukmon_meteortools-2023.4.22.tar", last modified: Sat Apr 29 16:54:41 2023, max compression
```

## Comparing `ukmon_meteortools-2023.4.21.tar` & `ukmon_meteortools-2023.4.22.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 13:57:33.086823 ukmon_meteortools-2023.4.21/
--rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.4.21/LICENSE
--rw-rw-rw-   0        0        0    42683 2023-04-29 13:57:33.086823 ukmon_meteortools-2023.4.21/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.4.21/README.md
--rw-rw-rw-   0        0        0     2202 2023-04-29 13:57:09.000000 ukmon_meteortools-2023.4.21/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 13:57:33.086823 ukmon_meteortools-2023.4.21/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 13:57:33.000823 ukmon_meteortools-2023.4.21/ukmon_meteortools/
--rw-rw-rw-   0        0        0      779 2023-04-29 13:57:14.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 13:57:33.038824 ukmon_meteortools-2023.4.21/ukmon_meteortools/fileformats/
--rw-rw-rw-   0        0        0    12830 2023-04-18 13:55:16.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py
--rw-rw-rw-   0        0        0     6608 2023-04-27 21:05:51.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/fileformats/ReadUFOCapXML.py
--rw-rw-rw-   0        0        0      358 2023-04-27 21:06:46.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/fileformats/__init__.py
--rw-rw-rw-   0        0        0    19234 2023-04-27 21:07:04.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/fileformats/ftpDetectInfo.py
--rw-rw-rw-   0        0        0     7513 2023-04-18 22:30:53.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/fileformats/imoWorkingShowerList.py
--rw-rw-rw-   0        0        0     2330 2023-03-08 12:49:15.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/fileformats/platepar.py
-drwxrwxrwx   0        0        0        0 2023-04-29 13:57:33.048821 ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/
--rw-rw-rw-   0        0        0      580 2023-04-17 20:41:56.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/__init__.py
--rw-rw-rw-   0        0        0     1783 2023-04-17 20:39:11.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
--rw-rw-rw-   0        0        0     4617 2023-03-08 12:53:11.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/multiDayRadiant.py
--rw-rw-rw-   0        0        0     2990 2023-04-16 21:51:50.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/multiEventGroundMap.py
--rw-rw-rw-   0        0        0     3980 2023-04-16 21:46:43.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/multiTrackStack.py
--rw-rw-rw-   0        0        0     1732 2023-04-16 21:42:36.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
--rw-rw-rw-   0        0        0     1431 2023-04-16 21:42:13.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/plotRMSOrbits.py
-drwxrwxrwx   0        0        0        0 2023-04-29 13:57:33.052822 ukmon_meteortools-2023.4.21/ukmon_meteortools/share/
--rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
--rw-rw-rw-   0        0        0       41 2023-04-18 21:54:45.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/share/__init__.py
--rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/share/streamfulldata.npy
-drwxrwxrwx   0        0        0        0 2023-04-29 13:57:33.070821 ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/
--rw-rw-rw-   0        0        0      524 2023-04-16 21:29:05.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-04-13 21:43:11.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/apiExampleCode.py
--rw-rw-rw-   0        0        0     2317 2023-04-18 22:57:34.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/drawFTPfile.py
--rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/findNearDuplicates.py
--rw-rw-rw-   0        0        0     6386 2023-04-18 22:55:02.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/getLiveImages.py
--rw-rw-rw-   0        0        0     2984 2023-04-18 22:49:26.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/getOverlappingFovs.py
--rw-rw-rw-   0        0        0     3253 2023-04-18 22:44:54.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/plotTrack.py
--rw-rw-rw-   0        0        0     2369 2023-04-18 22:43:12.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/retrieveECSV.py
-drwxrwxrwx   0        0        0        0 2023-04-29 13:57:33.084823 ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/
--rw-rw-rw-   0        0        0    13528 2023-04-12 22:11:48.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/Math.py
--rw-rw-rw-   0        0        0      512 2023-04-16 21:06:04.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/VectorMaths.py
--rw-rw-rw-   0        0        0     1660 2023-04-18 14:09:57.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/__init__.py
--rw-rw-rw-   0        0        0     2494 2023-04-18 20:38:58.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/annotateImage.py
--rw-rw-rw-   0        0        0     1298 2023-04-18 21:00:49.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/convertSolLon.py
--rw-rw-rw-   0        0        0     2088 2023-04-18 20:58:02.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/getActiveShowers.py
--rw-rw-rw-   0        0        0     3525 2023-04-18 13:55:45.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/getShowerDates.py
--rw-rw-rw-   0        0        0     3366 2023-04-16 21:22:26.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/kmlHandlers.py
--rw-rw-rw-   0        0        0     3272 2023-04-29 13:56:36.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/sendAnEmail.py
-drwxrwxrwx   0        0        0        0 2023-04-29 13:57:33.030822 ukmon_meteortools-2023.4.21/ukmon_meteortools.egg-info/
--rw-rw-rw-   0        0        0    42683 2023-04-29 13:57:32.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1716 2023-04-29 13:57:32.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 13:57:32.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      265 2023-04-29 13:57:32.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-29 13:57:32.000000 ukmon_meteortools-2023.4.21/ukmon_meteortools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.821559 ukmon_meteortools-2023.4.22/
+-rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.4.22/LICENSE
+-rw-rw-rw-   0        0        0    42683 2023-04-29 16:54:41.820567 ukmon_meteortools-2023.4.22/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.4.22/README.md
+-rw-rw-rw-   0        0        0     2202 2023-04-29 16:54:17.000000 ukmon_meteortools-2023.4.22/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 16:54:41.821559 ukmon_meteortools-2023.4.22/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.739558 ukmon_meteortools-2023.4.22/ukmon_meteortools/
+-rw-rw-rw-   0        0        0      779 2023-04-29 16:54:21.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.774558 ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/
+-rw-rw-rw-   0        0        0    12830 2023-04-18 13:55:16.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py
+-rw-rw-rw-   0        0        0     6608 2023-04-27 21:05:51.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/ReadUFOCapXML.py
+-rw-rw-rw-   0        0        0      358 2023-04-27 21:06:46.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/__init__.py
+-rw-rw-rw-   0        0        0    19234 2023-04-27 21:07:04.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/ftpDetectInfo.py
+-rw-rw-rw-   0        0        0     7513 2023-04-18 22:30:53.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/imoWorkingShowerList.py
+-rw-rw-rw-   0        0        0     2330 2023-03-08 12:49:15.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/platepar.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.785559 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/
+-rw-rw-rw-   0        0        0      580 2023-04-17 20:41:56.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/__init__.py
+-rw-rw-rw-   0        0        0     1783 2023-04-17 20:39:11.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
+-rw-rw-rw-   0        0        0     4617 2023-03-08 12:53:11.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/multiDayRadiant.py
+-rw-rw-rw-   0        0        0     2990 2023-04-16 21:51:50.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/multiEventGroundMap.py
+-rw-rw-rw-   0        0        0     3980 2023-04-16 21:46:43.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/multiTrackStack.py
+-rw-rw-rw-   0        0        0     1732 2023-04-16 21:42:36.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
+-rw-rw-rw-   0        0        0     1431 2023-04-16 21:42:13.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/plotRMSOrbits.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.788563 ukmon_meteortools-2023.4.22/ukmon_meteortools/share/
+-rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
+-rw-rw-rw-   0        0        0       41 2023-04-18 21:54:45.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/share/__init__.py
+-rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/share/streamfulldata.npy
+drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.806558 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/
+-rw-rw-rw-   0        0        0      524 2023-04-16 21:29:05.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-04-13 21:43:11.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/apiExampleCode.py
+-rw-rw-rw-   0        0        0     2317 2023-04-18 22:57:34.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/drawFTPfile.py
+-rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/findNearDuplicates.py
+-rw-rw-rw-   0        0        0     6386 2023-04-18 22:55:02.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/getLiveImages.py
+-rw-rw-rw-   0        0        0     2984 2023-04-18 22:49:26.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/getOverlappingFovs.py
+-rw-rw-rw-   0        0        0     3253 2023-04-18 22:44:54.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/plotTrack.py
+-rw-rw-rw-   0        0        0     2369 2023-04-18 22:43:12.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/retrieveECSV.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.818558 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/
+-rw-rw-rw-   0        0        0    13528 2023-04-12 22:11:48.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/Math.py
+-rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/VectorMaths.py
+-rw-rw-rw-   0        0        0     1536 2023-04-29 16:46:55.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/__init__.py
+-rw-rw-rw-   0        0        0     2494 2023-04-18 20:38:58.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/annotateImage.py
+-rw-rw-rw-   0        0        0     1298 2023-04-18 21:00:49.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/convertSolLon.py
+-rw-rw-rw-   0        0        0     2088 2023-04-18 20:58:02.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/getActiveShowers.py
+-rw-rw-rw-   0        0        0     3525 2023-04-18 13:55:45.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/getShowerDates.py
+-rw-rw-rw-   0        0        0     3988 2023-04-29 16:41:40.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/kmlHandlers.py
+-rw-rw-rw-   0        0        0     3291 2023-04-29 14:01:37.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/sendAnEmail.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.767558 ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/
+-rw-rw-rw-   0        0        0    42683 2023-04-29 16:54:41.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1716 2023-04-29 16:54:41.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 16:54:41.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      265 2023-04-29 16:54:41.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-29 16:54:41.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/top_level.txt
```

### Comparing `ukmon_meteortools-2023.4.21/LICENSE` & `ukmon_meteortools-2023.4.22/LICENSE`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/PKG-INFO` & `ukmon_meteortools-2023.4.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon_meteortools
-Version: 2023.4.21
+Version: 2023.4.22
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -687,15 +687,15 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # ukmon_meteortools
-## Version 2023.04.21
+## Version 2023.04.22
 
 Python tools and utilities to work with meteor data from the UK Meteor Network
 
 To get more information about the submodules and functions use Python's built-in help capability
 
 ``` python
 from ukmon_meteortools import utils
```

### Comparing `ukmon_meteortools-2023.4.21/README.md` & `ukmon_meteortools-2023.4.22/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/pyproject.toml` & `ukmon_meteortools-2023.4.22/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ukmon_meteortools"
-version = "2023.04.21"
+version = "2023.04.22"
 description = "Python Tools for Meteor Data Analysis"
 readme = "ukmon_meteortools/README.md"
 authors = [{ name = "Mark McIntyre", email = "ukmon@markmcintyreastro.co.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -63,15 +63,15 @@
 #[tool.setuptools.packages.find]
 #where = ["ukmon_meteortools"]
 
 [tool.setuptools.package-data]
 "*" = ["*.npy", "*.xml"]
 
 [tool.bumpver]
-current_version = "2023.04.21"
+current_version = "2023.04.22"
 version_pattern = "YYYY.0M.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/README.md` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ukmon_meteortools
-## Version 2023.04.21
+## Version 2023.04.22
 
 Python tools and utilities to work with meteor data from the UK Meteor Network
 
 To get more information about the submodules and functions use Python's built-in help capability
 
 ``` python
 from ukmon_meteortools import utils
```

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/fileformats/ReadUFOCapXML.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/ReadUFOCapXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/fileformats/ftpDetectInfo.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/ftpDetectInfo.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/fileformats/imoWorkingShowerList.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/imoWorkingShowerList.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/fileformats/platepar.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/platepar.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/__init__.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/multiDayRadiant.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/multiDayRadiant.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/multiEventGroundMap.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/multiEventGroundMap.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/multiTrackStack.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/multiTrackStack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/plotCAMSOrbits.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/plotCAMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/rmsutils/plotRMSOrbits.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/plotRMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/share/streamfulldata.npy` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/share/streamfulldata.npy`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/__init__.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/apiExampleCode.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/apiExampleCode.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/drawFTPfile.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/drawFTPfile.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/findNearDuplicates.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/findNearDuplicates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/getLiveImages.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/getLiveImages.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/getOverlappingFovs.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/getOverlappingFovs.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/plotTrack.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/plotTrack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/usertools/retrieveECSV.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/retrieveECSV.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/Math.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/Math.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/VectorMaths.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/VectorMaths.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/__init__.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 # flake8: noqa
 """
 Utility functions used across the UKMON toolset
 
 List of Functions:
-jd2Date, date2JD, datetime2DJ, jd2DynamicalTimeJD, jd2LST, sollon2jd
+jd2Date, date2JD, datetime2JD, jd2DynamicalTimeJD, jd2LST, sollon2jd
 greatCircleDistance, angleBetweenSphericalCoords, calcApparentSiderealEarthRotation
 calcNutationComponents, equatorialCoordPrecession,  raDec2AltAz, altAz2RADec
 altAz2RADec_vect, raDec2AltAz_vect, equatorialCoordPrecession_vect
 annotateImage, annotateImageArbitrary
 getActiveShowers, getActiveShowersStr, getShowerDets, getShowerPeak
-refreshShowerData, loadJenniskensShowers, loadDataFile, loadFullData, loadLookupTable
 trackCsvtoKML, getTrackDetails, getTrajPickle, munchKML
 sendAnEmail
-shortestDistance
+shortestDistance2Lines
 """
 
 from .Math import jd2Date, date2JD,datetime2JD, jd2DynamicalTimeJD, JULIAN_EPOCH, J2000_JD, jd2LST
 from .Math import greatCircleDistance, angleBetweenSphericalCoords, calcApparentSiderealEarthRotation
 from .Math import calcNutationComponents, equatorialCoordPrecession,  raDec2AltAz, altAz2RADec
 from .Math import altAz2RADec_vect, raDec2AltAz_vect, equatorialCoordPrecession_vect
 
 from .annotateImage import annotateImage, annotateImageArbitrary
 
 from .convertSolLon import sollon2jd
 
 from .getActiveShowers import getActiveShowers, getActiveShowersStr
 
-from .getShowerDates import getShowerDets, refreshShowerData, getShowerPeak
-from .getShowerDates import loadJenniskensShowers, loadDataFile, loadFullData
-from .getShowerDates import loadLookupTable
+from .getShowerDates import getShowerDets, getShowerPeak
+#from .getShowerDates import loadJenniskensShowers, loadDataFile, loadFullData, refreshShowerData
+#from .getShowerDates import loadLookupTable
 
 from .kmlHandlers import trackCsvtoKML, getTrackDetails, getTrajPickle, munchKML
 
 from .sendAnEmail import sendAnEmail
-
-from .VectorMaths import shortestDistance
```

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/annotateImage.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/annotateImage.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/convertSolLon.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/convertSolLon.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/getActiveShowers.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/getActiveShowers.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/getShowerDates.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/getShowerDates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/kmlHandlers.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/kmlHandlers.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,27 +34,41 @@
             for lin in coords:
                 s = lin.split(',')
                 ptsarr.append((float(s[0]), float(s[1])))
             polyg = Polygon(ptsarr)
             return cname, polyg 
 
 
-def trackCsvtoKML(trackcsvfile, trackdata=None):
+def trackCsvtoKML(trackcsvfile, trackdata=None, saveOutput=True):
+    """ 
+    Either reads a CSV file containing lat, long, height, time of an event and 
+    creates a 3d KML file from it or, if trackdata is populated, converts a Pandas dataframe containing
+    the same data. Output is written to disk unless saveOutput is false. 
+    
+    Arguments:
+        trackcsvfile:   [string] full path to the file to read from
+        trackdata:      [array] pandas dataframe containing the data. Default None
+        saveOutput:     [bool] write the KML file to disk. Default true
+
+    Returns:
+        the KML file as a tuple
+        """
     kml=simplekml.Kml()
     kml.document.name = trackcsvfile
     if trackdata is None:
         inputfile = csv.reader(open(trackcsvfile))
         for row in inputfile:
             #columns are lat, long, height, times
             kml.newpoint(name='', coords=[(row[1], row[0], row[2])])
     else:
         for i,r in trackdata.iterrows():
             kml.newpoint(name='', coords=[(r[1], r[0], r[2])], extrude=1, altitudemode='absolute')
     outname = trackcsvfile.replace('.csv','.kml')
-    kml.save(outname)
+    if saveOutput:
+        kml.save(outname)
     return kml
 
 
 def getTrackDetails(traj):
     lats = []
     lons = []
     alts = []
```

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools/utils/sendAnEmail.py` & `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/sendAnEmail.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,11 +83,11 @@
         retval = (service.users().messages().send(userId='me', body=mailmsg).execute())
         print('Message Id: %s' % retval['id'])
     except:
         print('An error occurred sending the message')
 
 
 if __name__ == '__main__':
-    if len(sys.argv) < 3:
-        print('usage: sendAnEmail.py recipient "message in quotes" Alert|Warning|Error ')
+    if len(sys.argv) < 4:
+        print('usage: sendAnEmail.py recipient "message in quotes" Alert|Warning|Error sender ')
     else:
-        sendAnEmail(sys.argv[1], sys.argv[2], sys.argv[3])
+        sendAnEmail(sys.argv[1], sys.argv[2], sys.argv[3],sys.argv[4])
```

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools.egg-info/PKG-INFO` & `ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon-meteortools
-Version: 2023.4.21
+Version: 2023.4.22
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -687,15 +687,15 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # ukmon_meteortools
-## Version 2023.04.21
+## Version 2023.04.22
 
 Python tools and utilities to work with meteor data from the UK Meteor Network
 
 To get more information about the submodules and functions use Python's built-in help capability
 
 ``` python
 from ukmon_meteortools import utils
```

### Comparing `ukmon_meteortools-2023.4.21/ukmon_meteortools.egg-info/SOURCES.txt` & `ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/ukmon_meteortools-2023.4.22.tar.gz` & `tmp/ukmon_meteortools-2023.4.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukmon_meteortools-2023.4.22.tar", last modified: Sat Apr 29 16:54:41 2023, max compression
+gzip compressed data, was "ukmon_meteortools-2023.4.23.tar", last modified: Sat Apr 29 17:29:19 2023, max compression
```

## Comparing `ukmon_meteortools-2023.4.22.tar` & `ukmon_meteortools-2023.4.23.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.821559 ukmon_meteortools-2023.4.22/
--rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.4.22/LICENSE
--rw-rw-rw-   0        0        0    42683 2023-04-29 16:54:41.820567 ukmon_meteortools-2023.4.22/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.4.22/README.md
--rw-rw-rw-   0        0        0     2202 2023-04-29 16:54:17.000000 ukmon_meteortools-2023.4.22/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 16:54:41.821559 ukmon_meteortools-2023.4.22/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.739558 ukmon_meteortools-2023.4.22/ukmon_meteortools/
--rw-rw-rw-   0        0        0      779 2023-04-29 16:54:21.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.774558 ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/
--rw-rw-rw-   0        0        0    12830 2023-04-18 13:55:16.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py
--rw-rw-rw-   0        0        0     6608 2023-04-27 21:05:51.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/ReadUFOCapXML.py
--rw-rw-rw-   0        0        0      358 2023-04-27 21:06:46.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/__init__.py
--rw-rw-rw-   0        0        0    19234 2023-04-27 21:07:04.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/ftpDetectInfo.py
--rw-rw-rw-   0        0        0     7513 2023-04-18 22:30:53.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/imoWorkingShowerList.py
--rw-rw-rw-   0        0        0     2330 2023-03-08 12:49:15.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/platepar.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.785559 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/
--rw-rw-rw-   0        0        0      580 2023-04-17 20:41:56.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/__init__.py
--rw-rw-rw-   0        0        0     1783 2023-04-17 20:39:11.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
--rw-rw-rw-   0        0        0     4617 2023-03-08 12:53:11.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/multiDayRadiant.py
--rw-rw-rw-   0        0        0     2990 2023-04-16 21:51:50.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/multiEventGroundMap.py
--rw-rw-rw-   0        0        0     3980 2023-04-16 21:46:43.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/multiTrackStack.py
--rw-rw-rw-   0        0        0     1732 2023-04-16 21:42:36.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
--rw-rw-rw-   0        0        0     1431 2023-04-16 21:42:13.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/plotRMSOrbits.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.788563 ukmon_meteortools-2023.4.22/ukmon_meteortools/share/
--rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
--rw-rw-rw-   0        0        0       41 2023-04-18 21:54:45.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/share/__init__.py
--rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/share/streamfulldata.npy
-drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.806558 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/
--rw-rw-rw-   0        0        0      524 2023-04-16 21:29:05.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-04-13 21:43:11.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/apiExampleCode.py
--rw-rw-rw-   0        0        0     2317 2023-04-18 22:57:34.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/drawFTPfile.py
--rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/findNearDuplicates.py
--rw-rw-rw-   0        0        0     6386 2023-04-18 22:55:02.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/getLiveImages.py
--rw-rw-rw-   0        0        0     2984 2023-04-18 22:49:26.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/getOverlappingFovs.py
--rw-rw-rw-   0        0        0     3253 2023-04-18 22:44:54.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/plotTrack.py
--rw-rw-rw-   0        0        0     2369 2023-04-18 22:43:12.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/retrieveECSV.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.818558 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/
--rw-rw-rw-   0        0        0    13528 2023-04-12 22:11:48.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/Math.py
--rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/VectorMaths.py
--rw-rw-rw-   0        0        0     1536 2023-04-29 16:46:55.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/__init__.py
--rw-rw-rw-   0        0        0     2494 2023-04-18 20:38:58.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/annotateImage.py
--rw-rw-rw-   0        0        0     1298 2023-04-18 21:00:49.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/convertSolLon.py
--rw-rw-rw-   0        0        0     2088 2023-04-18 20:58:02.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/getActiveShowers.py
--rw-rw-rw-   0        0        0     3525 2023-04-18 13:55:45.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/getShowerDates.py
--rw-rw-rw-   0        0        0     3988 2023-04-29 16:41:40.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/kmlHandlers.py
--rw-rw-rw-   0        0        0     3291 2023-04-29 14:01:37.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/sendAnEmail.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:54:41.767558 ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/
--rw-rw-rw-   0        0        0    42683 2023-04-29 16:54:41.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1716 2023-04-29 16:54:41.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 16:54:41.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      265 2023-04-29 16:54:41.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-29 16:54:41.000000 ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 17:29:19.815071 ukmon_meteortools-2023.4.23/
+-rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.4.23/LICENSE
+-rw-rw-rw-   0        0        0    42683 2023-04-29 17:29:19.814071 ukmon_meteortools-2023.4.23/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.4.23/README.md
+-rw-rw-rw-   0        0        0     2202 2023-04-29 17:28:55.000000 ukmon_meteortools-2023.4.23/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 17:29:19.816073 ukmon_meteortools-2023.4.23/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 17:29:19.726071 ukmon_meteortools-2023.4.23/ukmon_meteortools/
+-rw-rw-rw-   0        0        0      779 2023-04-29 17:28:59.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 17:29:19.762071 ukmon_meteortools-2023.4.23/ukmon_meteortools/fileformats/
+-rw-rw-rw-   0        0        0    12830 2023-04-18 13:55:16.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py
+-rw-rw-rw-   0        0        0     6608 2023-04-27 21:05:51.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/fileformats/ReadUFOCapXML.py
+-rw-rw-rw-   0        0        0      358 2023-04-27 21:06:46.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/fileformats/__init__.py
+-rw-rw-rw-   0        0        0    19234 2023-04-27 21:07:04.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/fileformats/ftpDetectInfo.py
+-rw-rw-rw-   0        0        0     7513 2023-04-18 22:30:53.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/fileformats/imoWorkingShowerList.py
+-rw-rw-rw-   0        0        0     2330 2023-03-08 12:49:15.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/fileformats/platepar.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:29:19.775073 ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/
+-rw-rw-rw-   0        0        0      580 2023-04-17 20:41:56.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/__init__.py
+-rw-rw-rw-   0        0        0     1783 2023-04-17 20:39:11.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
+-rw-rw-rw-   0        0        0     4617 2023-03-08 12:53:11.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/multiDayRadiant.py
+-rw-rw-rw-   0        0        0     2990 2023-04-16 21:51:50.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/multiEventGroundMap.py
+-rw-rw-rw-   0        0        0     3980 2023-04-16 21:46:43.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/multiTrackStack.py
+-rw-rw-rw-   0        0        0     1732 2023-04-16 21:42:36.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
+-rw-rw-rw-   0        0        0     1431 2023-04-16 21:42:13.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/plotRMSOrbits.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:29:19.779073 ukmon_meteortools-2023.4.23/ukmon_meteortools/share/
+-rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
+-rw-rw-rw-   0        0        0       41 2023-04-18 21:54:45.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/share/__init__.py
+-rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/share/streamfulldata.npy
+drwxrwxrwx   0        0        0        0 2023-04-29 17:29:19.798070 ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/
+-rw-rw-rw-   0        0        0      524 2023-04-16 21:29:05.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-04-13 21:43:11.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/apiExampleCode.py
+-rw-rw-rw-   0        0        0     2317 2023-04-18 22:57:34.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/drawFTPfile.py
+-rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/findNearDuplicates.py
+-rw-rw-rw-   0        0        0     6386 2023-04-18 22:55:02.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/getLiveImages.py
+-rw-rw-rw-   0        0        0     2984 2023-04-18 22:49:26.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/getOverlappingFovs.py
+-rw-rw-rw-   0        0        0     3253 2023-04-18 22:44:54.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/plotTrack.py
+-rw-rw-rw-   0        0        0     2369 2023-04-18 22:43:12.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/retrieveECSV.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:29:19.812071 ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/
+-rw-rw-rw-   0        0        0    13528 2023-04-12 22:11:48.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/Math.py
+-rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/VectorMaths.py
+-rw-rw-rw-   0        0        0     1536 2023-04-29 16:46:55.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/__init__.py
+-rw-rw-rw-   0        0        0     2494 2023-04-18 20:38:58.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/annotateImage.py
+-rw-rw-rw-   0        0        0     1298 2023-04-18 21:00:49.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/convertSolLon.py
+-rw-rw-rw-   0        0        0     2088 2023-04-18 20:58:02.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/getActiveShowers.py
+-rw-rw-rw-   0        0        0     3525 2023-04-18 13:55:45.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/getShowerDates.py
+-rw-rw-rw-   0        0        0     3988 2023-04-29 16:41:40.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/kmlHandlers.py
+-rw-rw-rw-   0        0        0     3668 2023-04-29 17:26:52.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/sendAnEmail.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:29:19.750071 ukmon_meteortools-2023.4.23/ukmon_meteortools.egg-info/
+-rw-rw-rw-   0        0        0    42683 2023-04-29 17:29:19.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1716 2023-04-29 17:29:19.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 17:29:19.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      265 2023-04-29 17:29:19.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-29 17:29:19.000000 ukmon_meteortools-2023.4.23/ukmon_meteortools.egg-info/top_level.txt
```

### Comparing `ukmon_meteortools-2023.4.22/LICENSE` & `ukmon_meteortools-2023.4.23/LICENSE`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/PKG-INFO` & `ukmon_meteortools-2023.4.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon_meteortools
-Version: 2023.4.22
+Version: 2023.4.23
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
-## Version 2023.04.22
+## Version 2023.04.23
 
 Python tools and utilities to work with meteor data from the UK Meteor Network
 
 To get more information about the submodules and functions use Python's built-in help capability
 
 ``` python
 from ukmon_meteortools import utils
```

### Comparing `ukmon_meteortools-2023.4.22/README.md` & `ukmon_meteortools-2023.4.23/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/pyproject.toml` & `ukmon_meteortools-2023.4.23/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ukmon_meteortools"
-version = "2023.04.22"
+version = "2023.04.23"
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
-current_version = "2023.04.22"
+current_version = "2023.04.23"
 version_pattern = "YYYY.0M.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/README.md` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ukmon_meteortools
-## Version 2023.04.22
+## Version 2023.04.23
 
 Python tools and utilities to work with meteor data from the UK Meteor Network
 
 To get more information about the submodules and functions use Python's built-in help capability
 
 ``` python
 from ukmon_meteortools import utils
```

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/ReadUFOCapXML.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/fileformats/ReadUFOCapXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/ftpDetectInfo.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/fileformats/ftpDetectInfo.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/imoWorkingShowerList.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/fileformats/imoWorkingShowerList.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/fileformats/platepar.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/fileformats/platepar.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/__init__.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/multiDayRadiant.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/multiDayRadiant.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/multiEventGroundMap.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/multiEventGroundMap.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/multiTrackStack.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/multiTrackStack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/plotCAMSOrbits.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/plotCAMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/rmsutils/plotRMSOrbits.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/rmsutils/plotRMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/share/streamfulldata.npy` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/share/streamfulldata.npy`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/__init__.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/apiExampleCode.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/apiExampleCode.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/drawFTPfile.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/drawFTPfile.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/findNearDuplicates.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/findNearDuplicates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/getLiveImages.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/getLiveImages.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/getOverlappingFovs.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/getOverlappingFovs.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/plotTrack.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/plotTrack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/usertools/retrieveECSV.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/usertools/retrieveECSV.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/Math.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/Math.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/VectorMaths.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/VectorMaths.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/__init__.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/annotateImage.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/annotateImage.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/convertSolLon.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/convertSolLon.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/getActiveShowers.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/getActiveShowers.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/getShowerDates.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/getShowerDates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/kmlHandlers.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/kmlHandlers.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools/utils/sendAnEmail.py` & `ukmon_meteortools-2023.4.23/ukmon_meteortools/utils/sendAnEmail.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     if os.path.exists(tokfile):
         creds = Credentials.from_authorized_user_file(tokfile, SCOPES)
     # If there are no (valid) credentials available, let the user log in.
     if not creds or not creds.valid:
         if creds and creds.expired and creds.refresh_token:
             creds.refresh(Request())
         else:
+            if not os.path.isfile(crdfile):
+                print('to use this function you must have stored your Google OAUTH2 secret json file in ~/.ssh/gmailcreds.json.')
+                print('To set up OAUTH2 go to your google cloud console, select APIs then Credentials, and add an OAUTH2 desktop client ID.')
+                return None
             flow = InstalledAppFlow.from_client_secrets_file(crdfile, SCOPES)
             creds = flow.run_local_server(port=0)
         # Save the credentials for the next run
         with open(tokfile, 'w') as token:
             token.write(creds.to_json())
     return creds
 
@@ -60,22 +64,23 @@
 
         Notes:
             You must have gmail OAUTH2 set up. The gmail credentials must be stored as follows:
                 token: $HOME/.ssh/gmailtoken.json
                 creds: $HOME/.ssh/gmailcreds.json
 
             On Windows, $HOME corresponds to c:/users/yourid. If there is no .ssh folder, create it. 
-
         """
     
     if msgtype is None:
         msgtype = platform.uname()[1]
 
     # email a summary to the mailrecip
     creds = getGmailCreds()
+    if not creds:
+        return 
     service = build('gmail', 'v1', credentials=creds)
 
     subj ='{:s}: {:s}'.format(msgtype, message[:30])
     message = '{:s}: {:s}'.format(msgtype, message)
 
     mailmsg = create_message(mailfrom, mailrecip, subj, message)
```

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/PKG-INFO` & `ukmon_meteortools-2023.4.23/ukmon_meteortools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon-meteortools
-Version: 2023.4.22
+Version: 2023.4.23
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
-## Version 2023.04.22
+## Version 2023.04.23
 
 Python tools and utilities to work with meteor data from the UK Meteor Network
 
 To get more information about the submodules and functions use Python's built-in help capability
 
 ``` python
 from ukmon_meteortools import utils
```

### Comparing `ukmon_meteortools-2023.4.22/ukmon_meteortools.egg-info/SOURCES.txt` & `ukmon_meteortools-2023.4.23/ukmon_meteortools.egg-info/SOURCES.txt`

 * *Files identical despite different names*


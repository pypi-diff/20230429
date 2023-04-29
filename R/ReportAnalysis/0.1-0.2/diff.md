# Comparing `tmp/ReportAnalysis-0.1.tar.gz` & `tmp/ReportAnalysis-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReportAnalysis-0.1.tar", last modified: Sat Apr 29 12:13:29 2023, max compression
+gzip compressed data, was "ReportAnalysis-0.2.tar", last modified: Sat Apr 29 12:58:40 2023, max compression
```

## Comparing `ReportAnalysis-0.1.tar` & `ReportAnalysis-0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2023-04-29 12:13:29.945110 ReportAnalysis-0.1/
--rw-rw-r--   0 al        (1000) al        (1000)     1068 2023-04-29 11:12:29.000000 ReportAnalysis-0.1/LICENSE
--rw-rw-r--   0 al        (1000) al        (1000)      280 2023-04-29 12:13:29.945110 ReportAnalysis-0.1/PKG-INFO
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2023-04-29 12:13:29.945110 ReportAnalysis-0.1/ReportAnalysis.egg-info/
--rw-rw-r--   0 al        (1000) al        (1000)      280 2023-04-29 12:13:29.000000 ReportAnalysis-0.1/ReportAnalysis.egg-info/PKG-INFO
--rw-rw-r--   0 al        (1000) al        (1000)      302 2023-04-29 12:13:29.000000 ReportAnalysis-0.1/ReportAnalysis.egg-info/SOURCES.txt
--rw-rw-r--   0 al        (1000) al        (1000)        1 2023-04-29 12:13:29.000000 ReportAnalysis-0.1/ReportAnalysis.egg-info/dependency_links.txt
--rw-rw-r--   0 al        (1000) al        (1000)       76 2023-04-29 12:13:29.000000 ReportAnalysis-0.1/ReportAnalysis.egg-info/entry_points.txt
--rw-rw-r--   0 al        (1000) al        (1000)        5 2023-04-29 12:13:29.000000 ReportAnalysis-0.1/ReportAnalysis.egg-info/requires.txt
--rw-rw-r--   0 al        (1000) al        (1000)       16 2023-04-29 12:13:29.000000 ReportAnalysis-0.1/ReportAnalysis.egg-info/top_level.txt
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2023-04-29 12:13:29.945110 ReportAnalysis-0.1/report_analysis/
--rw-rw-r--   0 al        (1000) al        (1000)        0 2023-04-29 10:58:02.000000 ReportAnalysis-0.1/report_analysis/__init__.py
--rw-rw-r--   0 al        (1000) al        (1000)      915 2023-04-29 10:59:56.000000 ReportAnalysis-0.1/report_analysis/analyzer.py
--rw-rw-r--   0 al        (1000) al        (1000)       38 2023-04-29 12:13:29.949110 ReportAnalysis-0.1/setup.cfg
--rw-rw-r--   0 al        (1000) al        (1000)      542 2023-04-29 12:09:34.000000 ReportAnalysis-0.1/setup.py
+drwxrwxr-x   0 al        (1000) al        (1000)        0 2023-04-29 12:58:40.607319 ReportAnalysis-0.2/
+-rw-rw-r--   0 al        (1000) al        (1000)     1068 2023-04-29 11:12:29.000000 ReportAnalysis-0.2/LICENSE
+-rw-rw-r--   0 al        (1000) al        (1000)      280 2023-04-29 12:58:40.607319 ReportAnalysis-0.2/PKG-INFO
+-rw-rw-r--   0 al        (1000) al        (1000)     1081 2023-04-29 12:54:06.000000 ReportAnalysis-0.2/README.md
+drwxrwxr-x   0 al        (1000) al        (1000)        0 2023-04-29 12:58:40.591318 ReportAnalysis-0.2/ReportAnalysis.egg-info/
+-rw-rw-r--   0 al        (1000) al        (1000)      280 2023-04-29 12:58:40.000000 ReportAnalysis-0.2/ReportAnalysis.egg-info/PKG-INFO
+-rw-rw-r--   0 al        (1000) al        (1000)      312 2023-04-29 12:58:40.000000 ReportAnalysis-0.2/ReportAnalysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 al        (1000) al        (1000)        1 2023-04-29 12:58:40.000000 ReportAnalysis-0.2/ReportAnalysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 al        (1000) al        (1000)       76 2023-04-29 12:58:40.000000 ReportAnalysis-0.2/ReportAnalysis.egg-info/entry_points.txt
+-rw-rw-r--   0 al        (1000) al        (1000)        5 2023-04-29 12:58:40.000000 ReportAnalysis-0.2/ReportAnalysis.egg-info/requires.txt
+-rw-rw-r--   0 al        (1000) al        (1000)       16 2023-04-29 12:58:40.000000 ReportAnalysis-0.2/ReportAnalysis.egg-info/top_level.txt
+drwxrwxr-x   0 al        (1000) al        (1000)        0 2023-04-29 12:58:40.595318 ReportAnalysis-0.2/report_analysis/
+-rw-rw-r--   0 al        (1000) al        (1000)        0 2023-04-29 10:58:02.000000 ReportAnalysis-0.2/report_analysis/__init__.py
+-rw-rw-r--   0 al        (1000) al        (1000)      915 2023-04-29 10:59:56.000000 ReportAnalysis-0.2/report_analysis/analyzer.py
+-rw-rw-r--   0 al        (1000) al        (1000)       38 2023-04-29 12:58:40.607319 ReportAnalysis-0.2/setup.cfg
+-rw-rw-r--   0 al        (1000) al        (1000)      542 2023-04-29 12:58:19.000000 ReportAnalysis-0.2/setup.py
```

### Comparing `ReportAnalysis-0.1/LICENSE` & `ReportAnalysis-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ReportAnalysis-0.1/report_analysis/analyzer.py` & `ReportAnalysis-0.2/report_analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `ReportAnalysis-0.1/setup.py` & `ReportAnalysis-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ReportAnalysis',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
         'nltk',
     ],
     entry_points={
         'console_scripts': [
             'report_analysis = report_analysis.analyzer:analyze_report'
```


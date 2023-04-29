# Comparing `tmp/AlgoSolver-0.1.2.tar.gz` & `tmp/AlgoSolver-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgoSolver-0.1.2.tar", last modified: Wed Apr  5 01:01:22 2023, max compression
+gzip compressed data, was "AlgoSolver-0.1.4.tar", last modified: Sat Apr 29 19:12:25 2023, max compression
```

## Comparing `AlgoSolver-0.1.2.tar` & `AlgoSolver-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,79 @@
-drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-05 01:01:22.065764 AlgoSolver-0.1.2/
-drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-05 01:01:22.040440 AlgoSolver-0.1.2/AlgoSolver.egg-info/
--rw-r--r--   0 nickbohm   (501) staff       (20)    15854 2023-04-05 01:01:21.000000 AlgoSolver-0.1.2/AlgoSolver.egg-info/PKG-INFO
--rw-r--r--   0 nickbohm   (501) staff       (20)      408 2023-04-05 01:01:21.000000 AlgoSolver-0.1.2/AlgoSolver.egg-info/SOURCES.txt
--rw-r--r--   0 nickbohm   (501) staff       (20)        1 2023-04-05 01:01:21.000000 AlgoSolver-0.1.2/AlgoSolver.egg-info/dependency_links.txt
--rw-r--r--   0 nickbohm   (501) staff       (20)      156 2023-04-05 01:01:21.000000 AlgoSolver-0.1.2/AlgoSolver.egg-info/requires.txt
--rw-r--r--   0 nickbohm   (501) staff       (20)        1 2023-04-05 01:01:21.000000 AlgoSolver-0.1.2/AlgoSolver.egg-info/top_level.txt
-drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-05 01:01:22.055306 AlgoSolver-0.1.2/Algo_Solver/
--rw-r--r--   0 nickbohm   (501) staff       (20)        0 2023-04-05 00:44:42.000000 AlgoSolver-0.1.2/Algo_Solver/__init__.py
--rw-r--r--   0 nickbohm   (501) staff       (20)      625 2023-03-29 17:56:12.000000 AlgoSolver-0.1.2/Algo_Solver/graphs.py
--rw-r--r--   0 nickbohm   (501) staff       (20)      223 2023-04-05 00:55:45.000000 AlgoSolver-0.1.2/Algo_Solver/main.py
--rw-r--r--   0 nickbohm   (501) staff       (20)      821 2023-03-29 17:56:12.000000 AlgoSolver-0.1.2/Algo_Solver/searching.py
--rw-r--r--   0 nickbohm   (501) staff       (20)     3832 2023-03-29 17:56:12.000000 AlgoSolver-0.1.2/Algo_Solver/sorting.py
-drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-05 01:01:22.063231 AlgoSolver-0.1.2/Algo_Solver/tests/
--rw-r--r--   0 nickbohm   (501) staff       (20)     2735 2023-03-29 17:56:12.000000 AlgoSolver-0.1.2/Algo_Solver/tests/test_all.py
--rw-r--r--   0 nickbohm   (501) staff       (20)     1122 2023-03-29 18:07:07.000000 AlgoSolver-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 nickbohm   (501) staff       (20)    11357 2023-03-22 00:14:09.000000 AlgoSolver-0.1.2/LICENSE
--rw-r--r--   0 nickbohm   (501) staff       (20)      385 2023-03-29 17:56:12.000000 AlgoSolver-0.1.2/MANIFEST.in
--rw-r--r--   0 nickbohm   (501) staff       (20)     2181 2023-03-29 17:56:12.000000 AlgoSolver-0.1.2/Makefile
--rw-r--r--   0 nickbohm   (501) staff       (20)    15854 2023-04-05 01:01:22.065277 AlgoSolver-0.1.2/PKG-INFO
--rw-r--r--   0 nickbohm   (501) staff       (20)     2010 2023-04-05 00:44:42.000000 AlgoSolver-0.1.2/README.md
--rw-r--r--   0 nickbohm   (501) staff       (20)     2262 2023-04-05 00:55:45.000000 AlgoSolver-0.1.2/pyproject.toml
--rw-r--r--   0 nickbohm   (501) staff       (20)     2760 2023-03-22 00:16:05.000000 AlgoSolver-0.1.2/requirements.txt
--rw-r--r--   0 nickbohm   (501) staff       (20)       38 2023-04-05 01:01:22.067535 AlgoSolver-0.1.2/setup.cfg
--rw-r--r--   0 nickbohm   (501) staff       (20)       39 2023-03-29 17:56:12.000000 AlgoSolver-0.1.2/setup.py
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.690968 AlgoSolver-0.1.4/
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.453919 AlgoSolver-0.1.4/AlgoSolver.egg-info/
+-rw-r--r--   0 nickbohm   (501) staff       (20)    15960 2023-04-29 19:12:24.000000 AlgoSolver-0.1.4/AlgoSolver.egg-info/PKG-INFO
+-rw-r--r--   0 nickbohm   (501) staff       (20)     1866 2023-04-29 19:12:25.000000 AlgoSolver-0.1.4/AlgoSolver.egg-info/SOURCES.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)        1 2023-04-29 19:12:24.000000 AlgoSolver-0.1.4/AlgoSolver.egg-info/dependency_links.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)      156 2023-04-29 19:12:24.000000 AlgoSolver-0.1.4/AlgoSolver.egg-info/requires.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)        1 2023-04-29 19:12:24.000000 AlgoSolver-0.1.4/AlgoSolver.egg-info/top_level.txt
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.466549 AlgoSolver-0.1.4/Algo_Solver/
+-rw-r--r--   0 nickbohm   (501) staff       (20)        0 2023-04-05 00:44:42.000000 AlgoSolver-0.1.4/Algo_Solver/__init__.py
+-rw-r--r--   0 nickbohm   (501) staff       (20)     5461 2023-04-29 17:55:29.000000 AlgoSolver-0.1.4/Algo_Solver/graphs.py
+-rw-r--r--   0 nickbohm   (501) staff       (20)      189 2023-04-29 19:05:52.000000 AlgoSolver-0.1.4/Algo_Solver/main.py
+-rw-r--r--   0 nickbohm   (501) staff       (20)     3154 2023-04-28 19:53:14.000000 AlgoSolver-0.1.4/Algo_Solver/searching.py
+-rw-r--r--   0 nickbohm   (501) staff       (20)     6065 2023-04-28 19:53:15.000000 AlgoSolver-0.1.4/Algo_Solver/sorting.py
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.467625 AlgoSolver-0.1.4/Algo_Solver/tests/
+-rw-r--r--   0 nickbohm   (501) staff       (20)     5880 2023-04-29 17:55:29.000000 AlgoSolver-0.1.4/Algo_Solver/tests/test_all.py
+-rw-r--r--   0 nickbohm   (501) staff       (20)     1122 2023-03-29 18:07:07.000000 AlgoSolver-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 nickbohm   (501) staff       (20)    11357 2023-03-22 00:14:09.000000 AlgoSolver-0.1.4/LICENSE
+-rw-r--r--   0 nickbohm   (501) staff       (20)      591 2023-04-28 19:50:15.000000 AlgoSolver-0.1.4/MANIFEST.in
+-rw-r--r--   0 nickbohm   (501) staff       (20)     2181 2023-03-29 17:56:12.000000 AlgoSolver-0.1.4/Makefile
+-rw-r--r--   0 nickbohm   (501) staff       (20)    15960 2023-04-29 19:12:25.690289 AlgoSolver-0.1.4/PKG-INFO
+-rw-r--r--   0 nickbohm   (501) staff       (20)     2116 2023-04-29 19:05:52.000000 AlgoSolver-0.1.4/README.md
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.497787 AlgoSolver-0.1.4/docs/
+-rw-r--r--   0 nickbohm   (501) staff       (20)      633 2023-04-28 18:12:18.000000 AlgoSolver-0.1.4/docs/Makefile
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.420012 AlgoSolver-0.1.4/docs/build/
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.499049 AlgoSolver-0.1.4/docs/build/doctest/
+-rw-r--r--   0 nickbohm   (501) staff       (20)      374 2023-04-12 00:52:53.000000 AlgoSolver-0.1.4/docs/build/doctest/output.txt
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.424905 AlgoSolver-0.1.4/docs/build/html/
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.554684 AlgoSolver-0.1.4/docs/build/html/_sources/
+-rw-r--r--   0 nickbohm   (501) staff       (20)       60 2023-04-12 00:59:48.000000 AlgoSolver-0.1.4/docs/build/html/_sources/api.rst.txt
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.422751 AlgoSolver-0.1.4/docs/build/html/_sources/build/
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.556627 AlgoSolver-0.1.4/docs/build/html/_sources/build/doctest/
+-rw-r--r--   0 nickbohm   (501) staff       (20)      374 2023-04-12 00:52:53.000000 AlgoSolver-0.1.4/docs/build/html/_sources/build/doctest/output.txt
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.423089 AlgoSolver-0.1.4/docs/build/html/_sources/build/html/
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.423346 AlgoSolver-0.1.4/docs/build/html/_sources/build/html/_static/
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.558737 AlgoSolver-0.1.4/docs/build/html/_sources/build/html/_static/scripts/
+-rw-r--r--   0 nickbohm   (501) staff       (20)      187 2023-04-12 00:11:53.000000 AlgoSolver-0.1.4/docs/build/html/_sources/build/html/_static/scripts/furo.js.LICENSE.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)     1134 2023-04-27 18:52:54.000000 AlgoSolver-0.1.4/docs/build/html/_sources/contributing.md.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)      932 2023-04-20 12:11:48.000000 AlgoSolver-0.1.4/docs/build/html/_sources/contributing.rst.txt
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.670799 AlgoSolver-0.1.4/docs/build/html/_sources/generated/
+-rw-r--r--   0 nickbohm   (501) staff       (20)      260 2023-04-12 01:09:15.000000 AlgoSolver-0.1.4/docs/build/html/_sources/generated/lumache.rst.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)      162 2023-04-20 12:05:52.000000 AlgoSolver-0.1.4/docs/build/html/_sources/graphs.rst.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)     1533 2023-04-28 17:08:32.000000 AlgoSolver-0.1.4/docs/build/html/_sources/index.md.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)     1206 2023-04-20 12:16:10.000000 AlgoSolver-0.1.4/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)     2332 2023-04-27 17:58:13.000000 AlgoSolver-0.1.4/docs/build/html/_sources/quickguide.md.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)     2421 2023-04-27 17:51:49.000000 AlgoSolver-0.1.4/docs/build/html/_sources/quickguide.rst.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)      354 2023-04-28 16:59:19.000000 AlgoSolver-0.1.4/docs/build/html/_sources/requirements.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)      136 2023-04-27 18:22:17.000000 AlgoSolver-0.1.4/docs/build/html/_sources/searching.md.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)      168 2023-04-20 12:06:56.000000 AlgoSolver-0.1.4/docs/build/html/_sources/searching.rst.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)      135 2023-04-27 19:11:52.000000 AlgoSolver-0.1.4/docs/build/html/_sources/sorting.md.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)      164 2023-04-20 12:03:13.000000 AlgoSolver-0.1.4/docs/build/html/_sources/sorting.rst.txt
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.683749 AlgoSolver-0.1.4/docs/build/html/_sources/source/
+-rw-r--r--   0 nickbohm   (501) staff       (20)       60 2023-04-12 00:59:48.000000 AlgoSolver-0.1.4/docs/build/html/_sources/source/api.rst.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)      932 2023-04-16 21:54:24.000000 AlgoSolver-0.1.4/docs/build/html/_sources/source/contributing.rst.txt
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.685802 AlgoSolver-0.1.4/docs/build/html/_sources/source/generated/
+-rw-r--r--   0 nickbohm   (501) staff       (20)      260 2023-04-12 01:09:15.000000 AlgoSolver-0.1.4/docs/build/html/_sources/source/generated/lumache.rst.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)     1711 2023-04-13 20:24:32.000000 AlgoSolver-0.1.4/docs/build/html/_sources/source/graphs.rst.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)        0 2023-04-20 12:09:46.000000 AlgoSolver-0.1.4/docs/build/html/_sources/source/modules.rst.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)     1789 2023-04-16 21:30:21.000000 AlgoSolver-0.1.4/docs/build/html/_sources/source/quickguide.rst.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)      821 2023-04-13 20:22:17.000000 AlgoSolver-0.1.4/docs/build/html/_sources/source/searching.rst.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)      178 2023-04-19 01:27:44.000000 AlgoSolver-0.1.4/docs/build/html/_sources/source/sorting.rst.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)     2696 2023-04-28 17:58:38.000000 AlgoSolver-0.1.4/docs/build/html/_sources/tutorial.md.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)      936 2023-04-12 01:10:51.000000 AlgoSolver-0.1.4/docs/build/html/_sources/usage.rst.txt
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.425181 AlgoSolver-0.1.4/docs/build/html/_static/
+drwxr-xr-x   0 nickbohm   (501) staff       (20)        0 2023-04-29 19:12:25.687857 AlgoSolver-0.1.4/docs/build/html/_static/scripts/
+-rw-r--r--   0 nickbohm   (501) staff       (20)      187 2023-04-12 00:11:53.000000 AlgoSolver-0.1.4/docs/build/html/_static/scripts/furo.js.LICENSE.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)     2463 2023-04-28 18:12:18.000000 AlgoSolver-0.1.4/docs/conf.py
+-rw-r--r--   0 nickbohm   (501) staff       (20)     1134 2023-04-28 18:12:18.000000 AlgoSolver-0.1.4/docs/contributing.md
+-rw-r--r--   0 nickbohm   (501) staff       (20)      162 2023-04-28 18:12:18.000000 AlgoSolver-0.1.4/docs/graphs.rst
+-rw-r--r--   0 nickbohm   (501) staff       (20)     1527 2023-04-29 19:05:52.000000 AlgoSolver-0.1.4/docs/index.md
+-rw-r--r--   0 nickbohm   (501) staff       (20)      804 2023-04-28 18:12:18.000000 AlgoSolver-0.1.4/docs/make.bat
+-rw-r--r--   0 nickbohm   (501) staff       (20)     2326 2023-04-29 19:05:52.000000 AlgoSolver-0.1.4/docs/quickguide.md
+-rw-r--r--   0 nickbohm   (501) staff       (20)      413 2023-04-29 19:05:52.000000 AlgoSolver-0.1.4/docs/requirements.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)      136 2023-04-28 18:12:18.000000 AlgoSolver-0.1.4/docs/searching.md
+-rw-r--r--   0 nickbohm   (501) staff       (20)      135 2023-04-28 18:12:18.000000 AlgoSolver-0.1.4/docs/sorting.md
+-rw-r--r--   0 nickbohm   (501) staff       (20)     2696 2023-04-28 18:33:55.000000 AlgoSolver-0.1.4/docs/tutorial.md
+-rw-r--r--   0 nickbohm   (501) staff       (20)     2310 2023-04-29 19:05:52.000000 AlgoSolver-0.1.4/pyproject.toml
+-rw-r--r--   0 nickbohm   (501) staff       (20)     2760 2023-04-13 21:08:32.000000 AlgoSolver-0.1.4/requirements.txt
+-rw-r--r--   0 nickbohm   (501) staff       (20)       38 2023-04-29 19:12:25.691126 AlgoSolver-0.1.4/setup.cfg
+-rw-r--r--   0 nickbohm   (501) staff       (20)       39 2023-03-29 17:56:12.000000 AlgoSolver-0.1.4/setup.py
```

### Comparing `AlgoSolver-0.1.2/AlgoSolver.egg-info/PKG-INFO` & `AlgoSolver-0.1.4/AlgoSolver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgoSolver
-Version: 0.1.2
+Version: 0.1.4
 Summary: A library to help developers use complex algorithms without having to code it themselves
 Author-email: Nicholas Bohm <ntb2135@Columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -223,16 +223,16 @@
 # AlgoSolver
 
 
 [![](https://img.shields.io/badge/license-Apache-green)](https://www.apache.org/licenses/LICENSE-2.0)
 [![](https://img.shields.io/github/issues/nickbohm555/AlgoSolver)](https://github.com/Nickbohm555/AlgoSolver/issues)
 [![Build Status](https://github.com/Nickbohm555/AlgoSolver/actions/workflows/build.yml/badge.svg)](https://github.com/Nickbohm555/AlgoSolver/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/nickbohm555/AlgoSolver/branch/main/graph/badge.svg)](https://app.codecov.io/gh/Nickbohm555/AlgoSolver/tree/main)
-[![PyPI](https://img.shields.io/pypi/v/AlgoSolver)](https://pypi.org/project/AlgoSolver/0.1.1/)
-
+[![PyPI](https://img.shields.io/pypi/v/AlgoSolver)](https://pypi.org/project/AlgoSolver/)
+[![readthedocs](https://img.shields.io/badge/docs-passing-green)](https://algosolver.readthedocs.io/en/latest/) 
 
 
 ## Overview
 My goal is to develop a library in python to help programmers solve a variety of algorithms style questions. For example, with Dynamic Programming problems the main things we need to know are if we are using a 1D of 2D array, what the base case is, and what the recurrence relation is. With this in mind, we can create multiple templates for different types of questions to take out the implementation process. I wanted to have a special focus on graph algorithms for the library. This will allow programmers to spend more of their time thinking about high level design questions.
 
 
 ## Installation
```

### Comparing `AlgoSolver-0.1.2/CONTRIBUTING.md` & `AlgoSolver-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `AlgoSolver-0.1.2/LICENSE` & `AlgoSolver-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AlgoSolver-0.1.2/Makefile` & `AlgoSolver-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `AlgoSolver-0.1.2/PKG-INFO` & `AlgoSolver-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgoSolver
-Version: 0.1.2
+Version: 0.1.4
 Summary: A library to help developers use complex algorithms without having to code it themselves
 Author-email: Nicholas Bohm <ntb2135@Columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -223,16 +223,16 @@
 # AlgoSolver
 
 
 [![](https://img.shields.io/badge/license-Apache-green)](https://www.apache.org/licenses/LICENSE-2.0)
 [![](https://img.shields.io/github/issues/nickbohm555/AlgoSolver)](https://github.com/Nickbohm555/AlgoSolver/issues)
 [![Build Status](https://github.com/Nickbohm555/AlgoSolver/actions/workflows/build.yml/badge.svg)](https://github.com/Nickbohm555/AlgoSolver/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/nickbohm555/AlgoSolver/branch/main/graph/badge.svg)](https://app.codecov.io/gh/Nickbohm555/AlgoSolver/tree/main)
-[![PyPI](https://img.shields.io/pypi/v/AlgoSolver)](https://pypi.org/project/AlgoSolver/0.1.1/)
-
+[![PyPI](https://img.shields.io/pypi/v/AlgoSolver)](https://pypi.org/project/AlgoSolver/)
+[![readthedocs](https://img.shields.io/badge/docs-passing-green)](https://algosolver.readthedocs.io/en/latest/) 
 
 
 ## Overview
 My goal is to develop a library in python to help programmers solve a variety of algorithms style questions. For example, with Dynamic Programming problems the main things we need to know are if we are using a 1D of 2D array, what the base case is, and what the recurrence relation is. With this in mind, we can create multiple templates for different types of questions to take out the implementation process. I wanted to have a special focus on graph algorithms for the library. This will allow programmers to spend more of their time thinking about high level design questions.
 
 
 ## Installation
```

### Comparing `AlgoSolver-0.1.2/README.md` & `AlgoSolver-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # AlgoSolver
 
 
 [![](https://img.shields.io/badge/license-Apache-green)](https://www.apache.org/licenses/LICENSE-2.0)
 [![](https://img.shields.io/github/issues/nickbohm555/AlgoSolver)](https://github.com/Nickbohm555/AlgoSolver/issues)
 [![Build Status](https://github.com/Nickbohm555/AlgoSolver/actions/workflows/build.yml/badge.svg)](https://github.com/Nickbohm555/AlgoSolver/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/nickbohm555/AlgoSolver/branch/main/graph/badge.svg)](https://app.codecov.io/gh/Nickbohm555/AlgoSolver/tree/main)
-[![PyPI](https://img.shields.io/pypi/v/AlgoSolver)](https://pypi.org/project/AlgoSolver/0.1.1/)
-
+[![PyPI](https://img.shields.io/pypi/v/AlgoSolver)](https://pypi.org/project/AlgoSolver/)
+[![readthedocs](https://img.shields.io/badge/docs-passing-green)](https://algosolver.readthedocs.io/en/latest/) 
 
 
 ## Overview
 My goal is to develop a library in python to help programmers solve a variety of algorithms style questions. For example, with Dynamic Programming problems the main things we need to know are if we are using a 1D of 2D array, what the base case is, and what the recurrence relation is. With this in mind, we can create multiple templates for different types of questions to take out the implementation process. I wanted to have a special focus on graph algorithms for the library. This will allow programmers to spend more of their time thinking about high level design questions.
 
 
 ## Installation
```

### Comparing `AlgoSolver-0.1.2/pyproject.toml` & `AlgoSolver-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "AlgoSolver"
 authors = [{name = "Nicholas Bohm", email = "ntb2135@Columbia.edu"}]
 description="A library to help developers use complex algorithms without having to code it themselves"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.4"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -57,15 +57,15 @@
 skip-string-normalization = true
 
 [tool.check-manifest]
 ignore = [
 ]
 
 [tool.flake8]
-ignore = ['E203', 'W503']
+ignore = ['E203', 'W503', 'F403', 'E402', 'F405', 'E501', 'W293', 'F811']
 max-line-length=120
 exclude=[
     'Algo_Solver/tests/*'
 ]
 per-file-ignores= [
     'Algo_Solver/__init__.py:F401, F403'
 ]
```

### Comparing `AlgoSolver-0.1.2/requirements.txt` & `AlgoSolver-0.1.4/requirements.txt`

 * *Files identical despite different names*


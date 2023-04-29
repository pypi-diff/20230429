# Comparing `tmp/qgate_graph-1.2rc4.tar.gz` & `tmp/qgate_graph-1.2rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgate_graph-1.2rc4.tar", last modified: Sat Apr 29 10:09:11 2023, max compression
+gzip compressed data, was "qgate_graph-1.2rc5.tar", last modified: Sat Apr 29 10:14:07 2023, max compression
```

## Comparing `qgate_graph-1.2rc4.tar` & `qgate_graph-1.2rc5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:09:11.395226 qgate_graph-1.2rc4/
--rw-rw-rw-   0        0        0      392 2023-04-29 10:09:11.395226 qgate_graph-1.2rc4/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-04-27 20:17:36.000000 qgate_graph-1.2rc4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 10:09:11.346701 qgate_graph-1.2rc4/qgate_graph/
--rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_graph-1.2rc4/qgate_graph/__init__.py
--rw-rw-rw-   0        0        0      913 2023-04-27 20:17:36.000000 qgate_graph-1.2rc4/qgate_graph/constant.py
--rw-rw-rw-   0        0        0     8695 2023-04-29 09:32:27.000000 qgate_graph-1.2rc4/qgate_graph/graph.py
--rw-rw-rw-   0        0        0      217 2023-04-29 10:08:43.000000 qgate_graph-1.2rc4/qgate_graph/version.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:09:11.378921 qgate_graph-1.2rc4/qgate_graph.egg-info/
--rw-rw-rw-   0        0        0      392 2023-04-29 10:09:11.000000 qgate_graph-1.2rc4/qgate_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-29 10:09:11.000000 qgate_graph-1.2rc4/qgate_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:09:11.000000 qgate_graph-1.2rc4/qgate_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-29 10:09:11.000000 qgate_graph-1.2rc4/qgate_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 10:09:11.000000 qgate_graph-1.2rc4/qgate_graph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 10:09:11.395226 qgate_graph-1.2rc4/setup.cfg
--rw-rw-rw-   0        0        0     1071 2023-04-29 09:54:54.000000 qgate_graph-1.2rc4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:14:07.401485 qgate_graph-1.2rc5/
+-rw-rw-rw-   0        0        0      392 2023-04-29 10:14:07.401485 qgate_graph-1.2rc5/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-04-27 20:17:36.000000 qgate_graph-1.2rc5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 10:14:07.355409 qgate_graph-1.2rc5/qgate_graph/
+-rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_graph-1.2rc5/qgate_graph/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-04-27 20:17:36.000000 qgate_graph-1.2rc5/qgate_graph/constant.py
+-rw-rw-rw-   0        0        0     8695 2023-04-29 09:32:27.000000 qgate_graph-1.2rc5/qgate_graph/graph.py
+-rw-rw-rw-   0        0        0      217 2023-04-29 10:13:51.000000 qgate_graph-1.2rc5/qgate_graph/version.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:14:07.395167 qgate_graph-1.2rc5/qgate_graph.egg-info/
+-rw-rw-rw-   0        0        0      392 2023-04-29 10:14:07.000000 qgate_graph-1.2rc5/qgate_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-29 10:14:07.000000 qgate_graph-1.2rc5/qgate_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 10:14:07.000000 qgate_graph-1.2rc5/qgate_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-29 10:14:07.000000 qgate_graph-1.2rc5/qgate_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 10:14:07.000000 qgate_graph-1.2rc5/qgate_graph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 10:14:07.401485 qgate_graph-1.2rc5/setup.cfg
+-rw-rw-rw-   0        0        0     1137 2023-04-29 10:13:42.000000 qgate_graph-1.2rc5/setup.py
```

### Comparing `qgate_graph-1.2rc4/qgate_graph/constant.py` & `qgate_graph-1.2rc5/qgate_graph/constant.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.2rc4/qgate_graph/graph.py` & `qgate_graph-1.2rc5/qgate_graph/graph.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.2rc4/setup.py` & `qgate_graph-1.2rc5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 try:
     from setuptools import setup, find_packages
 except ImportError:
     from distutils.core import setup
 
 import json
 import logging
-
+from qgate_graph.version import __version__
 #import dependencies
 #import packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
-exec(open('qgate_graph/version.py').read())
+# define __version__
+#exec(open('qgate_graph/version.py').read())
 
 #with open('HISTORY.md') as history_file:
 #    HISTORY = history_file.read()
 setup_args = dict(
     name='qgate_graph',
     version=__version__,
     description='Generate graphs based on outputs from Quality Gate',
```


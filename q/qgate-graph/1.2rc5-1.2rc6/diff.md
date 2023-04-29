# Comparing `tmp/qgate_graph-1.2rc5.tar.gz` & `tmp/qgate_graph-1.2rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgate_graph-1.2rc5.tar", last modified: Sat Apr 29 10:14:07 2023, max compression
+gzip compressed data, was "qgate_graph-1.2rc6.tar", last modified: Sat Apr 29 10:39:11 2023, max compression
```

## Comparing `qgate_graph-1.2rc5.tar` & `qgate_graph-1.2rc6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:14:07.401485 qgate_graph-1.2rc5/
--rw-rw-rw-   0        0        0      392 2023-04-29 10:14:07.401485 qgate_graph-1.2rc5/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-04-27 20:17:36.000000 qgate_graph-1.2rc5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 10:14:07.355409 qgate_graph-1.2rc5/qgate_graph/
--rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_graph-1.2rc5/qgate_graph/__init__.py
--rw-rw-rw-   0        0        0      913 2023-04-27 20:17:36.000000 qgate_graph-1.2rc5/qgate_graph/constant.py
--rw-rw-rw-   0        0        0     8695 2023-04-29 09:32:27.000000 qgate_graph-1.2rc5/qgate_graph/graph.py
--rw-rw-rw-   0        0        0      217 2023-04-29 10:13:51.000000 qgate_graph-1.2rc5/qgate_graph/version.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:14:07.395167 qgate_graph-1.2rc5/qgate_graph.egg-info/
--rw-rw-rw-   0        0        0      392 2023-04-29 10:14:07.000000 qgate_graph-1.2rc5/qgate_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-29 10:14:07.000000 qgate_graph-1.2rc5/qgate_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:14:07.000000 qgate_graph-1.2rc5/qgate_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-29 10:14:07.000000 qgate_graph-1.2rc5/qgate_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 10:14:07.000000 qgate_graph-1.2rc5/qgate_graph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 10:14:07.401485 qgate_graph-1.2rc5/setup.cfg
--rw-rw-rw-   0        0        0     1137 2023-04-29 10:13:42.000000 qgate_graph-1.2rc5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:39:11.921126 qgate_graph-1.2rc6/
+-rw-rw-rw-   0        0        0      926 2023-04-29 10:39:11.921126 qgate_graph-1.2rc6/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2023-04-29 10:37:41.000000 qgate_graph-1.2rc6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 10:39:11.873556 qgate_graph-1.2rc6/qgate_graph/
+-rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_graph-1.2rc6/qgate_graph/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-04-27 20:17:36.000000 qgate_graph-1.2rc6/qgate_graph/constant.py
+-rw-rw-rw-   0        0        0     8655 2023-04-29 10:16:42.000000 qgate_graph-1.2rc6/qgate_graph/graph.py
+-rw-rw-rw-   0        0        0      217 2023-04-29 10:38:57.000000 qgate_graph-1.2rc6/qgate_graph/version.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:39:11.921126 qgate_graph-1.2rc6/qgate_graph.egg-info/
+-rw-rw-rw-   0        0        0      926 2023-04-29 10:39:11.000000 qgate_graph-1.2rc6/qgate_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-29 10:39:11.000000 qgate_graph-1.2rc6/qgate_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 10:39:11.000000 qgate_graph-1.2rc6/qgate_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-29 10:39:11.000000 qgate_graph-1.2rc6/qgate_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 10:39:11.000000 qgate_graph-1.2rc6/qgate_graph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 10:39:11.921126 qgate_graph-1.2rc6/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-04-29 10:17:53.000000 qgate_graph-1.2rc6/setup.py
```

### Comparing `qgate_graph-1.2rc5/qgate_graph/constant.py` & `qgate_graph-1.2rc6/qgate_graph/constant.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.2rc5/qgate_graph/graph.py` & `qgate_graph-1.2rc6/qgate_graph/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os.path, os
 import matplotlib.pyplot as plt
 import qgate_graph.constant as cns
+import qgate_graph
 import json, datetime
 import logging
 class Graph:
     """
     Generate graph based on input data
 
         example::
@@ -66,17 +67,15 @@
     def _reset_marker(self):
         self._marker_point=0
 
     def _reset_color(self):
         self._color_point=0
 
     def _watermark(self, plt, ax):
-        #print(cns.__version__)
-        #print(qgate_graph.constant.__version__)
-        watermark='qgate_graph (v1.1)'
+        watermark=f'qgate_graph (v{qgate_graph.__version__})'
         plt.text(1.0, 0, watermark,
                  horizontalalignment='right',
                  verticalalignment='bottom',
                  transform = ax.transAxes,
                  alpha=0.4, fontsize=8)
 
     def _show_graph(self, executors, total_performance, avrg_time, std_deviation, title, file_name,output_dir):
```

### Comparing `qgate_graph-1.2rc5/setup.py` & `qgate_graph-1.2rc6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 from qgate_graph.version import __version__
 #import dependencies
 #import packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
-# define __version__
-#exec(open('qgate_graph/version.py').read())
-
 #with open('HISTORY.md') as history_file:
 #    HISTORY = history_file.read()
 setup_args = dict(
     name='qgate_graph',
     version=__version__,
     description='Generate graphs based on outputs from Quality Gate',
     long_description_content_type="text/markdown",
```


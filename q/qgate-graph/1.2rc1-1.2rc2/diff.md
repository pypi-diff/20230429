# Comparing `tmp/qgate_graph-1.2rc1.tar.gz` & `tmp/qgate_graph-1.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgate_graph-1.2rc1.tar", last modified: Fri Apr 28 10:23:24 2023, max compression
+gzip compressed data, was "qgate_graph-1.2rc2.tar", last modified: Sat Apr 29 08:54:15 2023, max compression
```

## Comparing `qgate_graph-1.2rc1.tar` & `qgate_graph-1.2rc2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 10:23:24.778486 qgate_graph-1.2rc1/
--rw-rw-rw-   0        0        0      392 2023-04-28 10:23:24.762730 qgate_graph-1.2rc1/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-04-27 20:17:36.000000 qgate_graph-1.2rc1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 10:23:24.731442 qgate_graph-1.2rc1/qgate_graph/
--rw-rw-rw-   0        0        0        6 2023-04-27 20:17:36.000000 qgate_graph-1.2rc1/qgate_graph/__init__.py
--rw-rw-rw-   0        0        0      913 2023-04-27 20:17:36.000000 qgate_graph-1.2rc1/qgate_graph/constant.py
--rw-rw-rw-   0        0        0     8131 2023-04-28 10:12:15.000000 qgate_graph-1.2rc1/qgate_graph/graph.py
-drwxrwxrwx   0        0        0        0 2023-04-28 10:23:24.762730 qgate_graph-1.2rc1/qgate_graph.egg-info/
--rw-rw-rw-   0        0        0      392 2023-04-28 10:23:24.000000 qgate_graph-1.2rc1/qgate_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-28 10:23:24.000000 qgate_graph-1.2rc1/qgate_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 10:23:24.000000 qgate_graph-1.2rc1/qgate_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-28 10:23:24.000000 qgate_graph-1.2rc1/qgate_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-28 10:23:24.000000 qgate_graph-1.2rc1/qgate_graph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 10:23:24.779129 qgate_graph-1.2rc1/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-04-28 10:23:10.000000 qgate_graph-1.2rc1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 08:54:15.136290 qgate_graph-1.2rc2/
+-rw-rw-rw-   0        0        0      392 2023-04-29 08:54:15.120648 qgate_graph-1.2rc2/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-04-27 20:17:36.000000 qgate_graph-1.2rc2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 08:54:15.062902 qgate_graph-1.2rc2/qgate_graph/
+-rw-rw-rw-   0        0        0        6 2023-04-27 20:17:36.000000 qgate_graph-1.2rc2/qgate_graph/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-04-27 20:17:36.000000 qgate_graph-1.2rc2/qgate_graph/constant.py
+-rw-rw-rw-   0        0        0     8612 2023-04-29 08:40:14.000000 qgate_graph-1.2rc2/qgate_graph/graph.py
+drwxrwxrwx   0        0        0        0 2023-04-29 08:54:15.120648 qgate_graph-1.2rc2/qgate_graph.egg-info/
+-rw-rw-rw-   0        0        0      392 2023-04-29 08:54:14.000000 qgate_graph-1.2rc2/qgate_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-29 08:54:14.000000 qgate_graph-1.2rc2/qgate_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 08:54:14.000000 qgate_graph-1.2rc2/qgate_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-29 08:54:14.000000 qgate_graph-1.2rc2/qgate_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 08:54:14.000000 qgate_graph-1.2rc2/qgate_graph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 08:54:15.136290 qgate_graph-1.2rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-04-29 08:52:02.000000 qgate_graph-1.2rc2/setup.py
```

### Comparing `qgate_graph-1.2rc1/qgate_graph/constant.py` & `qgate_graph-1.2rc2/qgate_graph/constant.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.2rc1/qgate_graph/graph.py` & `qgate_graph-1.2rc2/qgate_graph/graph.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 import matplotlib.pyplot as plt
 import qgate_graph.constant as cns
 import json, datetime
 import logging
 class Graph:
     """
     Generate graph based on input data
+
+        example::
+
+            import qgate_graph.graph as grp
+            import logging
+
+            logging.basicConfig()
+            logging.getLogger().setLevel(logging.INFO)
+
+            graph=grp.Graph()
+            graph.generate_from_dir("input_adr", "output_adr")
     """
     def __init__(self):
         self._markers = ['o','x', '*', '^','X', 'D', 'p', 'H']
         self._marker_point=0
         self._colors=['c', 'm', 'r', 'b', 'g', 'y', 'k', 'w']
         self._color_point=0
 
@@ -131,19 +142,27 @@
         file_name=file_name.replace("__","_")
         return file_name
 
     def generate_from_dir(self, input_dir: str="input", output_dir: str="output"):
         """
         Generate graphs based on input directory
 
+        example::
+
+            import qgate_graph.graph as grp
+
+            graph=grp.Graph()
+            graph.generate_from_dir("input_adr", "output_adr")
+
         :param input_dir:       Input directory (default "input")
         :param output_dir:      Output directory (default "output")
         """
         for file in os.listdir(input_dir):
             self.generate_from_file(os.path.join(input_dir, file), output_dir)
+        logging.info("Done")
 
     def generate_from_file(self, input_file: str, output_dir: str="output"):
         """
         Generate graphs based on input input file
 
         :param input_file:      Input file
         :param output_dir:      Output directory (default "output")
```

### Comparing `qgate_graph-1.2rc1/setup.py` & `qgate_graph-1.2rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 #with open('HISTORY.md') as history_file:
 #    HISTORY = history_file.read()
 setup_args = dict(
     name='qgate_graph',
-    version='v1.2-rc1',
+    version='v1.2-rc2',
     description='Generate graphs based on outputs from Quality Gate',
     long_description_content_type="text/markdown",
     long_description=README, # + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Jiri Steuer',
     author_email='steuer.jiri@gmail.com',
```


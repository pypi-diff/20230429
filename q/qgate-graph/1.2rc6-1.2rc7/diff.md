# Comparing `tmp/qgate_graph-1.2rc6.tar.gz` & `tmp/qgate_graph-1.2rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgate_graph-1.2rc6.tar", last modified: Sat Apr 29 10:39:11 2023, max compression
+gzip compressed data, was "qgate_graph-1.2rc7.tar", last modified: Sat Apr 29 13:44:06 2023, max compression
```

## Comparing `qgate_graph-1.2rc6.tar` & `qgate_graph-1.2rc7.tar`

### file list

```diff
@@ -1,16 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:39:11.921126 qgate_graph-1.2rc6/
--rw-rw-rw-   0        0        0      926 2023-04-29 10:39:11.921126 qgate_graph-1.2rc6/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-04-29 10:37:41.000000 qgate_graph-1.2rc6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 10:39:11.873556 qgate_graph-1.2rc6/qgate_graph/
--rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_graph-1.2rc6/qgate_graph/__init__.py
--rw-rw-rw-   0        0        0      913 2023-04-27 20:17:36.000000 qgate_graph-1.2rc6/qgate_graph/constant.py
--rw-rw-rw-   0        0        0     8655 2023-04-29 10:16:42.000000 qgate_graph-1.2rc6/qgate_graph/graph.py
--rw-rw-rw-   0        0        0      217 2023-04-29 10:38:57.000000 qgate_graph-1.2rc6/qgate_graph/version.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:39:11.921126 qgate_graph-1.2rc6/qgate_graph.egg-info/
--rw-rw-rw-   0        0        0      926 2023-04-29 10:39:11.000000 qgate_graph-1.2rc6/qgate_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-29 10:39:11.000000 qgate_graph-1.2rc6/qgate_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:39:11.000000 qgate_graph-1.2rc6/qgate_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-29 10:39:11.000000 qgate_graph-1.2rc6/qgate_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 10:39:11.000000 qgate_graph-1.2rc6/qgate_graph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 10:39:11.921126 qgate_graph-1.2rc6/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-04-29 10:17:53.000000 qgate_graph-1.2rc6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:44:06.004644 qgate_graph-1.2rc7/
+-rw-rw-rw-   0        0        0      135 2023-04-27 20:50:17.000000 qgate_graph-1.2rc7/.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-29 13:44:05.900173 qgate_graph-1.2rc7/.idea/
+-rw-rw-rw-   0        0        0       50 2023-04-27 15:39:54.000000 qgate_graph-1.2rc7/.idea/.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-29 13:44:05.920960 qgate_graph-1.2rc7/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0    12870 2023-04-27 16:54:16.000000 qgate_graph-1.2rc7/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-rw-   0        0        0      174 2023-04-27 16:54:16.000000 qgate_graph-1.2rc7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      321 2023-04-27 16:54:16.000000 qgate_graph-1.2rc7/.idea/misc.xml
+-rw-rw-rw-   0        0        0      281 2023-04-27 16:54:16.000000 qgate_graph-1.2rc7/.idea/modules.xml
+-rw-rw-rw-   0        0        0      361 2023-04-27 16:54:16.000000 qgate_graph-1.2rc7/.idea/qgate-graph.iml
+-rw-rw-rw-   0        0        0      185 2023-04-27 20:07:09.000000 qgate_graph-1.2rc7/.idea/vcs.xml
+-rw-rw-rw-   0        0        0      953 2023-04-29 13:44:06.002400 qgate_graph-1.2rc7/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2023-04-29 10:53:59.000000 qgate_graph-1.2rc7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 13:44:05.920960 qgate_graph-1.2rc7/assets/
+-rw-rw-rw-   0        0        0   117721 2023-04-29 10:46:59.000000 qgate_graph-1.2rc7/assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png
+-rw-rw-rw-   0        0        0      560 2023-04-29 11:03:52.000000 qgate_graph-1.2rc7/main.py
+-rwxrwxrwx   0        0        0      169 2023-04-29 10:06:41.000000 qgate_graph-1.2rc7/publish.bat
+drwxrwxrwx   0        0        0        0 2023-04-29 13:44:05.952868 qgate_graph-1.2rc7/qgate_graph/
+-rw-rw-rw-   0        0        0       15 2023-04-27 20:40:11.000000 qgate_graph-1.2rc7/qgate_graph/.gitignore
+-rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_graph-1.2rc7/qgate_graph/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-04-27 20:17:36.000000 qgate_graph-1.2rc7/qgate_graph/constant.py
+-rw-rw-rw-   0        0        0     8691 2023-04-29 10:46:50.000000 qgate_graph-1.2rc7/qgate_graph/graph.py
+-rw-rw-rw-   0        0        0      217 2023-04-29 13:43:48.000000 qgate_graph-1.2rc7/qgate_graph/version.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:44:05.984148 qgate_graph-1.2rc7/qgate_graph.egg-info/
+-rw-rw-rw-   0        0        0      953 2023-04-29 13:44:04.000000 qgate_graph-1.2rc7/qgate_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      596 2023-04-29 13:44:05.000000 qgate_graph-1.2rc7/qgate_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 13:44:04.000000 qgate_graph-1.2rc7/qgate_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-29 13:44:04.000000 qgate_graph-1.2rc7/qgate_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 13:44:04.000000 qgate_graph-1.2rc7/qgate_graph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       19 2023-04-29 13:39:54.000000 qgate_graph-1.2rc7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 13:44:06.005195 qgate_graph-1.2rc7/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2023-04-29 10:57:22.000000 qgate_graph-1.2rc7/setup.py
```

### Comparing `qgate_graph-1.2rc6/PKG-INFO` & `qgate_graph-1.2rc7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: qgate_graph
-Version: 1.2rc6
+Version: 1.2rc7
 Summary: Generate graphs based on outputs from Quality Gate
 Home-page: https://github.com/george0st/qgate-graph/
 Download-URL: https://pypi.org/project/qgate_graph/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
-Keywords: Quality,QualityGate
+Keywords: Quality,QualityGate,Graph
 Description-Content-Type: text/markdown
 
 [![PyPI version fury.io](https://badge.fury.io/py/qgate-graph.svg)](https://pypi.python.org/pypi/qgate-graph/)
 # QGate-Graph
 
 Generate graphs based on performance outputs from Quality Gate solution.
 
 ## Usage
 
+```lang-python
     import qgate_graph.graph as grp
     import logging
 
     # setup login level
     logging.basicConfig()
     logging.getLogger().setLevel(logging.INFO)
 
     # generate output graphs
     graph=grp.Graph()
     graph.generate_from_dir()
+```
 
 # Outputs
 ![graph](./assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png)
```

### Comparing `qgate_graph-1.2rc6/README.md` & `qgate_graph-1.2rc7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [![PyPI version fury.io](https://badge.fury.io/py/qgate-graph.svg)](https://pypi.python.org/pypi/qgate-graph/)
 # QGate-Graph
 
 Generate graphs based on performance outputs from Quality Gate solution.
 
 ## Usage
 
+```lang-python
     import qgate_graph.graph as grp
     import logging
 
     # setup login level
     logging.basicConfig()
     logging.getLogger().setLevel(logging.INFO)
 
     # generate output graphs
     graph=grp.Graph()
     graph.generate_from_dir()
+```
 
 # Outputs
 ![graph](./assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png)
```

### Comparing `qgate_graph-1.2rc6/qgate_graph/constant.py` & `qgate_graph-1.2rc7/qgate_graph/constant.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.2rc6/qgate_graph/graph.py` & `qgate_graph-1.2rc7/qgate_graph/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 
             logging.basicConfig()
             logging.getLogger().setLevel(logging.INFO)
 
             graph=grp.Graph()
             graph.generate_from_dir("input_adr", "output_adr")
     """
-    def __init__(self):
+    def __init__(self, dpi=100):
         self._markers = ['o','x', '*', '^','X', 'D', 'p', 'H']
         self._marker_point=0
         self._colors=['c', 'm', 'r', 'b', 'g', 'y', 'k', 'w']
         self._color_point=0
+        self.dpi=dpi
 
     def _find_key(self, performance_line: str, keys):
         for key in keys:
             start=performance_line.index(key)
             if start>0:
                 start+=len(key)
                 end = performance_line.index(",",start)
@@ -128,15 +129,15 @@
             self._next_color()
             plt.xlabel('Executors')
             if key_count+1==key_view:
                 plt.ylabel('Response [sec]')
             plt.xticks(self._get_executor_list(collection=executors[key]))
 
         output_file=os.path.join(output_dir,file_name+".png")
-        plt.savefig(output_file, dpi=200)
+        plt.savefig(output_file, dpi=self.dpi)
         logging.info(f"  ... {output_file}")
         plt.close()
 
     def _unife_file_name(self, file_name):
         remove_item=" ,&?"
         for itm in remove_item:
             file_name=file_name.replace(itm,"_")
```

### Comparing `qgate_graph-1.2rc6/qgate_graph.egg-info/PKG-INFO` & `qgate_graph-1.2rc7/qgate_graph.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: qgate-graph
-Version: 1.2rc6
+Version: 1.2rc7
 Summary: Generate graphs based on outputs from Quality Gate
 Home-page: https://github.com/george0st/qgate-graph/
 Download-URL: https://pypi.org/project/qgate_graph/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
-Keywords: Quality,QualityGate
+Keywords: Quality,QualityGate,Graph
 Description-Content-Type: text/markdown
 
 [![PyPI version fury.io](https://badge.fury.io/py/qgate-graph.svg)](https://pypi.python.org/pypi/qgate-graph/)
 # QGate-Graph
 
 Generate graphs based on performance outputs from Quality Gate solution.
 
 ## Usage
 
+```lang-python
     import qgate_graph.graph as grp
     import logging
 
     # setup login level
     logging.basicConfig()
     logging.getLogger().setLevel(logging.INFO)
 
     # generate output graphs
     graph=grp.Graph()
     graph.generate_from_dir()
+```
 
 # Outputs
 ![graph](./assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png)
```

### Comparing `qgate_graph-1.2rc6/setup.py` & `qgate_graph-1.2rc7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     description='Generate graphs based on outputs from Quality Gate',
     long_description_content_type="text/markdown",
     long_description=README, # + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Jiri Steuer',
     author_email='steuer.jiri@gmail.com',
-    keywords=['Quality', 'QualityGate'],
+    keywords=['Quality', 'QualityGate', 'Graph'],
     url='https://github.com/george0st/qgate-graph/',
     download_url='https://pypi.org/project/qgate_graph/'
 )
 
 install_requires = [
     'matplotlib~=3.7',
     'click~=8.1'
```


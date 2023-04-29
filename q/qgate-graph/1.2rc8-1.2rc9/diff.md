# Comparing `tmp/qgate_graph-1.2rc8.tar.gz` & `tmp/qgate_graph-1.2rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgate_graph-1.2rc8.tar", last modified: Sat Apr 29 14:07:23 2023, max compression
+gzip compressed data, was "qgate_graph-1.2rc9.tar", last modified: Sat Apr 29 14:28:51 2023, max compression
```

## Comparing `qgate_graph-1.2rc8.tar` & `qgate_graph-1.2rc9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 14:07:23.384153 qgate_graph-1.2rc8/
--rw-rw-rw-   0        0        0      135 2023-04-27 20:50:17.000000 qgate_graph-1.2rc8/.gitignore
-drwxrwxrwx   0        0        0        0 2023-04-29 14:07:23.293799 qgate_graph-1.2rc8/.idea/
--rw-rw-rw-   0        0        0       50 2023-04-27 15:39:54.000000 qgate_graph-1.2rc8/.idea/.gitignore
-drwxrwxrwx   0        0        0        0 2023-04-29 14:07:23.311490 qgate_graph-1.2rc8/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0    12870 2023-04-27 16:54:16.000000 qgate_graph-1.2rc8/.idea/inspectionProfiles/Project_Default.xml
--rw-rw-rw-   0        0        0      174 2023-04-27 16:54:16.000000 qgate_graph-1.2rc8/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      321 2023-04-27 16:54:16.000000 qgate_graph-1.2rc8/.idea/misc.xml
--rw-rw-rw-   0        0        0      281 2023-04-27 16:54:16.000000 qgate_graph-1.2rc8/.idea/modules.xml
--rw-rw-rw-   0        0        0      361 2023-04-27 16:54:16.000000 qgate_graph-1.2rc8/.idea/qgate-graph.iml
--rw-rw-rw-   0        0        0      185 2023-04-27 20:07:09.000000 qgate_graph-1.2rc8/.idea/vcs.xml
--rw-rw-rw-   0        0        0      953 2023-04-29 14:07:23.384153 qgate_graph-1.2rc8/PKG-INFO
--rw-rw-rw-   0        0        0      574 2023-04-29 10:53:59.000000 qgate_graph-1.2rc8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 14:07:23.311490 qgate_graph-1.2rc8/assets/
--rw-rw-rw-   0        0        0   117721 2023-04-29 10:46:59.000000 qgate_graph-1.2rc8/assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png
--rw-rw-rw-   0        0        0      560 2023-04-29 11:03:52.000000 qgate_graph-1.2rc8/main.py
--rwxrwxrwx   0        0        0      169 2023-04-29 10:06:41.000000 qgate_graph-1.2rc8/publish.bat
-drwxrwxrwx   0        0        0        0 2023-04-29 14:07:23.336517 qgate_graph-1.2rc8/qgate_graph/
--rw-rw-rw-   0        0        0       15 2023-04-27 20:40:11.000000 qgate_graph-1.2rc8/qgate_graph/.gitignore
--rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_graph-1.2rc8/qgate_graph/__init__.py
--rw-rw-rw-   0        0        0      913 2023-04-27 20:17:36.000000 qgate_graph-1.2rc8/qgate_graph/constant.py
--rw-rw-rw-   0        0        0     8691 2023-04-29 10:46:50.000000 qgate_graph-1.2rc8/qgate_graph/graph.py
--rw-rw-rw-   0        0        0      217 2023-04-29 14:06:48.000000 qgate_graph-1.2rc8/qgate_graph/version.py
-drwxrwxrwx   0        0        0        0 2023-04-29 14:07:23.367803 qgate_graph-1.2rc8/qgate_graph.egg-info/
--rw-rw-rw-   0        0        0      953 2023-04-29 14:07:22.000000 qgate_graph-1.2rc8/qgate_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      596 2023-04-29 14:07:23.000000 qgate_graph-1.2rc8/qgate_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 14:07:22.000000 qgate_graph-1.2rc8/qgate_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-29 14:07:22.000000 qgate_graph-1.2rc8/qgate_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 14:07:22.000000 qgate_graph-1.2rc8/qgate_graph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       19 2023-04-29 13:39:54.000000 qgate_graph-1.2rc8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 14:07:23.384153 qgate_graph-1.2rc8/setup.cfg
--rw-rw-rw-   0        0        0     1057 2023-04-29 14:01:21.000000 qgate_graph-1.2rc8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 14:28:51.687706 qgate_graph-1.2rc9/
+-rw-rw-rw-   0        0        0      135 2023-04-27 20:50:17.000000 qgate_graph-1.2rc9/.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-29 14:28:51.589502 qgate_graph-1.2rc9/.idea/
+-rw-rw-rw-   0        0        0       50 2023-04-27 15:39:54.000000 qgate_graph-1.2rc9/.idea/.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-29 14:28:51.606045 qgate_graph-1.2rc9/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0    12870 2023-04-27 16:54:16.000000 qgate_graph-1.2rc9/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-rw-   0        0        0      174 2023-04-27 16:54:16.000000 qgate_graph-1.2rc9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      321 2023-04-27 16:54:16.000000 qgate_graph-1.2rc9/.idea/misc.xml
+-rw-rw-rw-   0        0        0      281 2023-04-27 16:54:16.000000 qgate_graph-1.2rc9/.idea/modules.xml
+-rw-rw-rw-   0        0        0      361 2023-04-27 16:54:16.000000 qgate_graph-1.2rc9/.idea/qgate-graph.iml
+-rw-rw-rw-   0        0        0      185 2023-04-27 20:07:09.000000 qgate_graph-1.2rc9/.idea/vcs.xml
+-rw-rw-rw-   0        0        0      953 2023-04-29 14:28:51.672729 qgate_graph-1.2rc9/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2023-04-29 10:53:59.000000 qgate_graph-1.2rc9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 14:28:51.606045 qgate_graph-1.2rc9/assets/
+-rw-rw-rw-   0        0        0   117721 2023-04-29 10:46:59.000000 qgate_graph-1.2rc9/assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png
+-rw-rw-rw-   0        0        0       29 2023-04-29 13:39:22.000000 qgate_graph-1.2rc9/dev-requirements.txt
+-rw-rw-rw-   0        0        0      560 2023-04-29 11:03:52.000000 qgate_graph-1.2rc9/main.py
+-rwxrwxrwx   0        0        0      169 2023-04-29 10:06:41.000000 qgate_graph-1.2rc9/publish.bat
+drwxrwxrwx   0        0        0        0 2023-04-29 14:28:51.639800 qgate_graph-1.2rc9/qgate_graph/
+-rw-rw-rw-   0        0        0       15 2023-04-27 20:40:11.000000 qgate_graph-1.2rc9/qgate_graph/.gitignore
+-rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_graph-1.2rc9/qgate_graph/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-04-27 20:17:36.000000 qgate_graph-1.2rc9/qgate_graph/constant.py
+-rw-rw-rw-   0        0        0     8691 2023-04-29 10:46:50.000000 qgate_graph-1.2rc9/qgate_graph/graph.py
+-rw-rw-rw-   0        0        0      217 2023-04-29 14:28:40.000000 qgate_graph-1.2rc9/qgate_graph/version.py
+drwxrwxrwx   0        0        0        0 2023-04-29 14:28:51.672729 qgate_graph-1.2rc9/qgate_graph.egg-info/
+-rw-rw-rw-   0        0        0      953 2023-04-29 14:28:50.000000 qgate_graph-1.2rc9/qgate_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-04-29 14:28:51.000000 qgate_graph-1.2rc9/qgate_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 14:28:50.000000 qgate_graph-1.2rc9/qgate_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-29 14:28:50.000000 qgate_graph-1.2rc9/qgate_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 14:28:50.000000 qgate_graph-1.2rc9/qgate_graph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       19 2023-04-29 13:39:54.000000 qgate_graph-1.2rc9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 14:28:51.688711 qgate_graph-1.2rc9/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2023-04-29 14:27:49.000000 qgate_graph-1.2rc9/setup.py
```

### Comparing `qgate_graph-1.2rc8/.idea/inspectionProfiles/Project_Default.xml` & `qgate_graph-1.2rc9/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.2rc8/PKG-INFO` & `qgate_graph-1.2rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate_graph
-Version: 1.2rc8
+Version: 1.2rc9
 Summary: Generate graphs based on outputs from Quality Gate
 Home-page: https://github.com/george0st/qgate-graph/
 Download-URL: https://pypi.org/project/qgate_graph/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: Quality,QualityGate,Graph
```

### Comparing `qgate_graph-1.2rc8/README.md` & `qgate_graph-1.2rc9/README.md`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.2rc8/assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png` & `qgate_graph-1.2rc9/assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.2rc8/main.py` & `qgate_graph-1.2rc9/main.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.2rc8/qgate_graph/constant.py` & `qgate_graph-1.2rc9/qgate_graph/constant.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.2rc8/qgate_graph/graph.py` & `qgate_graph-1.2rc9/qgate_graph/graph.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.2rc8/qgate_graph.egg-info/PKG-INFO` & `qgate_graph-1.2rc9/qgate_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-graph
-Version: 1.2rc8
+Version: 1.2rc9
 Summary: Generate graphs based on outputs from Quality Gate
 Home-page: https://github.com/george0st/qgate-graph/
 Download-URL: https://pypi.org/project/qgate_graph/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: Quality,QualityGate,Graph
```

### Comparing `qgate_graph-1.2rc8/qgate_graph.egg-info/SOURCES.txt` & `qgate_graph-1.2rc9/qgate_graph.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 README.md
+dev-requirements.txt
 main.py
 publish.bat
 requirements.txt
 setup.py
 .idea/.gitignore
 .idea/misc.xml
 .idea/modules.xml
```

### Comparing `qgate_graph-1.2rc8/setup.py` & `qgate_graph-1.2rc9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     from setuptools import setup, find_packages
 except ImportError:
     from distutils.core import setup
 
 import json
 import logging
 from qgate_graph.version import __version__
-#import dependencies
+import dependencies
 #import packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 #with open('HISTORY.md') as history_file:
 #    HISTORY = history_file.read()
@@ -25,13 +25,13 @@
     author='Jiri Steuer',
     author_email='steuer.jiri@gmail.com',
     keywords=['Quality', 'QualityGate', 'Graph'],
     url='https://github.com/george0st/qgate-graph/',
     download_url='https://pypi.org/project/qgate_graph/'
 )
 
-install_requires = [
-    'matplotlib>=3.5'
-]
+install_requires = dependencies.base_requirements(),
+tests_require = dependencies.dev_requirements(),
+extras_require = dependencies.extra_requirements(),
 
 if __name__ == '__main__':
     setup(**setup_args, install_requires=install_requires)
```


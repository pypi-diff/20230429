# Comparing `tmp/filter_stations-0.1.7.tar.gz` & `tmp/filter_stations-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter_stations-0.1.7.tar", last modified: Sun Mar 12 12:07:43 2023, max compression
+gzip compressed data, was "filter_stations-0.3.0.tar", last modified: Sat Apr 29 12:06:19 2023, max compression
```

## Comparing `filter_stations-0.1.7.tar` & `filter_stations-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 12:07:43.043549 filter_stations-0.1.7/
--rw-rw-rw-   0        0        0     3488 2023-03-12 12:07:43.042491 filter_stations-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3182 2023-03-12 12:07:13.000000 filter_stations-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-12 12:07:42.980574 filter_stations-0.1.7/filter_stations/
--rw-rw-rw-   0        0        0    15092 2023-03-12 09:12:00.000000 filter_stations-0.1.7/filter_stations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-12 12:07:43.039431 filter_stations-0.1.7/filter_stations.egg-info/
--rw-rw-rw-   0        0        0     3488 2023-03-12 12:07:42.000000 filter_stations-0.1.7/filter_stations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-03-12 12:07:42.000000 filter_stations-0.1.7/filter_stations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-12 12:07:42.000000 filter_stations-0.1.7/filter_stations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-03-12 12:07:42.000000 filter_stations-0.1.7/filter_stations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       83 2023-03-12 12:07:42.000000 filter_stations-0.1.7/filter_stations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-12 12:07:42.000000 filter_stations-0.1.7/filter_stations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-12 12:07:43.044609 filter_stations-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      912 2023-03-12 09:50:03.000000 filter_stations-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:06:19.743750 filter_stations-0.3.0/
+-rw-rw-rw-   0        0        0     3488 2023-04-29 12:06:19.741482 filter_stations-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3182 2023-03-12 12:07:13.000000 filter_stations-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 12:06:19.697460 filter_stations-0.3.0/filter_stations/
+-rw-rw-rw-   0        0        0    25062 2023-04-29 11:36:52.000000 filter_stations-0.3.0/filter_stations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:06:19.734594 filter_stations-0.3.0/filter_stations.egg-info/
+-rw-rw-rw-   0        0        0     3488 2023-04-29 12:06:19.000000 filter_stations-0.3.0/filter_stations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-04-29 12:06:19.000000 filter_stations-0.3.0/filter_stations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 12:06:19.000000 filter_stations-0.3.0/filter_stations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-29 12:06:19.000000 filter_stations-0.3.0/filter_stations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-04-29 12:06:19.000000 filter_stations-0.3.0/filter_stations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-29 12:06:19.000000 filter_stations-0.3.0/filter_stations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 12:06:19.744752 filter_stations-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-04-29 12:02:47.000000 filter_stations-0.3.0/setup.py
```

### Comparing `filter_stations-0.1.7/PKG-INFO` & `filter_stations-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filter_stations
-Version: 0.1.7
+Version: 0.3.0
 Summary: Making it easier to navigate and clean station data
 Home-page: https://github.com/kaburia/Packaging/tree/main/filter_stations
 Author: Austin Kaburia
 Author-email: kaburiaaustin1@gmail.com
 Description-Content-Type: text/markdown
 
 ## filter_stations
```

### Comparing `filter_stations-0.1.7/README.md` & `filter_stations-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `filter_stations-0.1.7/filter_stations.egg-info/PKG-INFO` & `filter_stations-0.3.0/filter_stations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filter-stations
-Version: 0.1.7
+Version: 0.3.0
 Summary: Making it easier to navigate and clean station data
 Home-page: https://github.com/kaburia/Packaging/tree/main/filter_stations
 Author: Austin Kaburia
 Author-email: kaburiaaustin1@gmail.com
 Description-Content-Type: text/markdown
 
 ## filter_stations
```

### Comparing `filter_stations-0.1.7/setup.py` & `filter_stations-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='filter_stations',
-    version='0.1.7',
+    version='0.3.0',
     packages=find_packages(),
     include_package_data=True,
     description='Making it easier to navigate and clean station data',
     author='Austin Kaburia',
     author_email='kaburiaaustin1@gmail.com',
     url='https://github.com/kaburia/Packaging/tree/main/filter_stations',
     install_requires=[
@@ -17,15 +17,16 @@
         'requests',
         'python-dateutil',
         'argparse',
         'haversine',
         'matplotlib',
         'numpy',
         'IPython',
-        'folium'
+        'folium',
+        'datetime'
     ],
     entry_points={
         'console_scripts': [
             'my-script=filter_stations.filter_stations:main'
         ]
     },
     long_description=long_description,
```


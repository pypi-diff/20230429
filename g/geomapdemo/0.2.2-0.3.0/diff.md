# Comparing `tmp/geomapdemo-0.2.2.tar.gz` & `tmp/geomapdemo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapdemo-0.2.2.tar", last modified: Thu Apr 27 03:40:39 2023, max compression
+gzip compressed data, was "geomapdemo-0.3.0.tar", last modified: Fri Apr 28 23:50:35 2023, max compression
```

## Comparing `geomapdemo-0.2.2.tar` & `geomapdemo-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:40:39.000934 geomapdemo-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-27 03:40:39.000934 geomapdemo-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:40:38.996934 geomapdemo-0.2.2/geomapdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/geomapdemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/geomapdemo/foliumap.py
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/geomapdemo/geomapdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:40:39.000934 geomapdemo-0.2.2/geomapdemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-27 03:40:38.000000 geomapdemo-0.2.2/geomapdemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-27 03:40:38.000000 geomapdemo-0.2.2/geomapdemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 03:40:38.000000 geomapdemo-0.2.2/geomapdemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 03:40:38.000000 geomapdemo-0.2.2/geomapdemo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 03:40:38.000000 geomapdemo-0.2.2/geomapdemo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 03:40:38.000000 geomapdemo-0.2.2/geomapdemo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-27 03:40:39.000934 geomapdemo-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:50:35.397118 geomapdemo-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-28 23:50:35.397118 geomapdemo-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:50:35.393118 geomapdemo-0.3.0/geomapdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/geomapdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/geomapdemo/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/geomapdemo/foliumap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/geomapdemo/geomapdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:50:35.397118 geomapdemo-0.3.0/geomapdemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-28 23:50:35.000000 geomapdemo-0.3.0/geomapdemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 23:50:35.000000 geomapdemo-0.3.0/geomapdemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 23:50:35.000000 geomapdemo-0.3.0/geomapdemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:50:35.000000 geomapdemo-0.3.0/geomapdemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 23:50:35.000000 geomapdemo-0.3.0/geomapdemo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 23:50:35.000000 geomapdemo-0.3.0/geomapdemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 23:50:35.397118 geomapdemo-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-28 23:50:25.000000 geomapdemo-0.3.0/setup.py
```

### Comparing `geomapdemo-0.2.2/LICENSE` & `geomapdemo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.2.2/PKG-INFO` & `geomapdemo-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.2.2
-Summary: A python package for interactive mapping, testing.
+Version: 0.3.0
+Summary: A python package for interactive mapping.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # geomapdemo
 
 [![Software License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
@@ -43,10 +43,17 @@
 
 -   Create random numbers and random text
 -   Basic Mapping and drawing
 -   Vector and raster layer function available
 -   Ipyleaflet based interactive map function
 -   Folium based interactive map function
 
-## Credits
 
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
+## Supported Python Version
+- Python 3.7
+- Python 3.9
+- Python 3.10
+- Python 3.11
+
+
+
+
```

### Comparing `geomapdemo-0.2.2/README.md` & `geomapdemo-0.3.0/geomapdemo.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: geomapdemo
+Version: 0.3.0
+Summary: A python package for interactive mapping.
+Home-page: https://github.com/zyang91/geomapdemo
+Author: Zhanchao Yang
+Author-email: zyang91@binghamton.edu
+License: MIT license
+Keywords: geomapdemo
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # geomapdemo
 
 [![Software License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
 [![Downloads](https://static.pepy.tech/badge/geomapdemo)](https://pepy.tech/project/geomapdemo)
 [![image](https://img.shields.io/pypi/v/geomapdemo.svg)](https://pypi.python.org/pypi/geomapdemo)
 [![image](https://img.shields.io/conda/vn/conda-forge/geomapdemo.svg)](https://anaconda.org/conda-forge/geomapdemo)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zyang91/geomapdemo/HEAD)
@@ -21,10 +43,17 @@
 
 -   Create random numbers and random text
 -   Basic Mapping and drawing
 -   Vector and raster layer function available
 -   Ipyleaflet based interactive map function
 -   Folium based interactive map function
 
-## Credits
 
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
+## Supported Python Version
+- Python 3.7
+- Python 3.9
+- Python 3.10
+- Python 3.11
+
+
+
+
```

### Comparing `geomapdemo-0.2.2/geomapdemo/foliumap.py` & `geomapdemo-0.3.0/geomapdemo/foliumap.py`

 * *Files 5% similar despite different names*

```diff
@@ -224,8 +224,16 @@
         )
         self.add_child(choropleth)
         self.add_child(folium.LayerControl())
     
     def add_layer_control(self):
         """Adds a layer control to the map
         """        
-        self.add_child(folium.LayerControl())
+        self.add_child(folium.LayerControl())
+    
+    def add_layer(self, layer):
+        """Adds a layer to the map
+        Args:
+            layer (TileLayer): A TileLayer instance.
+        """       
+        layer.add_to(self)
+
```

### Comparing `geomapdemo-0.2.2/geomapdemo/geomapdemo.py` & `geomapdemo-0.3.0/geomapdemo/geomapdemo.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import random
 import string
 import ipyleaflet
 
 
 
+
 class Map(ipyleaflet.Map):
 
     def __init__(self, center = [40, -100], zoom = 4, **kwargs) -> None:
         """Initializes the map
         Args:
             center (tuple): The center of the map. e.g [lat, lon]. Defaults to [40, -100].
             zoom (int): The zoom level of the map. Defaults to 4.
@@ -323,8 +324,8 @@
     Args:
         length (int, optional): the length of the number. Defaults to 1.
 
     Returns:
         int: The generated number.
     """    
     result_str = ''.join(random.choice(string.digits) for i in range(length))
-    return int(result_str)
+    return int(result_str)
```

### Comparing `geomapdemo-0.2.2/setup.py` & `geomapdemo-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,28 +31,28 @@
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
-    description="A python package for interactive mapping, testing.",
+    description="A python package for interactive mapping.",
     install_requires=install_requires,
     dependency_links=dependency_links,
     license="MIT license",
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='geomapdemo',
     name='geomapdemo',
     packages=find_packages(include=['geomapdemo', 'geomapdemo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zyang91/geomapdemo',
-    version='0.2.2',
+    version='0.3.0',
     zip_safe=False,
 )
```


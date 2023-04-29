# Comparing `tmp/bassmap-0.0.8.tar.gz` & `tmp/bassmap-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bassmap-0.0.8.tar", last modified: Wed Apr 26 04:49:49 2023, max compression
+gzip compressed data, was "bassmap-0.0.9.tar", last modified: Wed Apr 26 05:09:05 2023, max compression
```

## Comparing `bassmap-0.0.8.tar` & `bassmap-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:49:49.433621 bassmap-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-26 04:49:38.000000 bassmap-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 04:49:38.000000 bassmap-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-26 04:49:49.433621 bassmap-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-26 04:49:38.000000 bassmap-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:49:49.433621 bassmap-0.0.8/bassmap/
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-26 04:49:38.000000 bassmap-0.0.8/bassmap/Foliumatic.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-26 04:49:38.000000 bassmap-0.0.8/bassmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-04-26 04:49:38.000000 bassmap-0.0.8/bassmap/bassmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:49:49.433621 bassmap-0.0.8/bassmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-26 04:49:49.000000 bassmap-0.0.8/bassmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 04:49:49.000000 bassmap-0.0.8/bassmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-26 04:49:49.000000 bassmap-0.0.8/bassmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:49:49.000000 bassmap-0.0.8/bassmap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-26 04:49:49.000000 bassmap-0.0.8/bassmap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 04:49:49.000000 bassmap-0.0.8/bassmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-26 04:49:38.000000 bassmap-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 04:49:49.437620 bassmap-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-26 04:49:38.000000 bassmap-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:05.322196 bassmap-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-26 05:08:52.000000 bassmap-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 05:08:52.000000 bassmap-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-26 05:09:05.322196 bassmap-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-26 05:08:52.000000 bassmap-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:05.322196 bassmap-0.0.9/bassmap/
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-26 05:08:52.000000 bassmap-0.0.9/bassmap/Foliumatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-26 05:08:52.000000 bassmap-0.0.9/bassmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-04-26 05:08:52.000000 bassmap-0.0.9/bassmap/bassmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:05.322196 bassmap-0.0.9/bassmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-26 05:09:05.000000 bassmap-0.0.9/bassmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 05:09:05.000000 bassmap-0.0.9/bassmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-26 05:09:05.000000 bassmap-0.0.9/bassmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:09:05.000000 bassmap-0.0.9/bassmap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-26 05:09:05.000000 bassmap-0.0.9/bassmap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 05:09:05.000000 bassmap-0.0.9/bassmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-26 05:08:52.000000 bassmap-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 05:09:05.322196 bassmap-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-26 05:08:52.000000 bassmap-0.0.9/setup.py
```

### Comparing `bassmap-0.0.8/LICENSE` & `bassmap-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bassmap-0.0.8/PKG-INFO` & `bassmap-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bassmap
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/bassneel/bassmap
 Author: Bass Neel
 Author-email: maps.bassneel@gmail.com
 License: MIT license
 Keywords: bassmap
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bassmap-0.0.8/README.md` & `bassmap-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bassmap-0.0.8/bassmap/Foliumatic.py` & `bassmap-0.0.9/bassmap/Foliumatic.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,23 +10,29 @@
     
     def __init__(self):
         self.map = folium.Map()
         
     def __init__(self, lat=0, lon=0, zoom_start=2):
         self.map = folium.Map(location=[lat, lon], zoom_start=zoom_start)
 
-    def add_tile_layer(self, tile_url='OpenStreetMap', tile_name=None):
-        if tile_name:
-            folium.TileLayer(tiles=tile_url, name=tile_name).add_to(self.map)
-        else:
-            folium.TileLayer(tiles=tile_url).add_to(self.map)
-
-        folium.LayerControl().add_to(self.map)
-
-        return self.map
+    def add_tile_layer(self, url, name, attribution = "", **kwargs):
+        """Adds a tile layer to the map.
+        
+        Args:
+            url (str): The URL of the tile layer.
+            name (str): The name of the tile layer
+            attribution (str, optional): The attribution of the tile layer. Defaults to **
+            """
+        tile_layer = folium.TileLayer(
+            tiles= url,
+            name = name,
+            attr = attribution,
+            **kwargs
+        )
+        self.add_child(tile_layer)
 
     def add_basemap(self, basemap_name, url_template):
         """
         Adds a basemap to the map using a URL template.
         
         Parameters:
         basemap_name (str): The name of the basemap to add.
```

### Comparing `bassmap-0.0.8/bassmap/bassmap.py` & `bassmap-0.0.9/bassmap/bassmap.py`

 * *Files identical despite different names*

### Comparing `bassmap-0.0.8/bassmap.egg-info/PKG-INFO` & `bassmap-0.0.9/bassmap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bassmap
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/bassneel/bassmap
 Author: Bass Neel
 Author-email: maps.bassneel@gmail.com
 License: MIT license
 Keywords: bassmap
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bassmap-0.0.8/setup.py` & `bassmap-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='bassmap',
     name='bassmap',
     packages=find_packages(include=['bassmap', 'bassmap.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/bassneel/bassmap',
-    version='0.0.8',
+    version='0.0.9',
     zip_safe=False,
 )
```


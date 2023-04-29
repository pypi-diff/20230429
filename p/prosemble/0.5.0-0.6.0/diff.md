# Comparing `tmp/prosemble-0.5.0.tar.gz` & `tmp/prosemble-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosemble-0.5.0.tar", last modified: Sun Apr 23 19:58:20 2023, max compression
+gzip compressed data, was "prosemble-0.6.0.tar", last modified: Sat Apr 29 21:43:45 2023, max compression
```

## Comparing `prosemble-0.5.0.tar` & `prosemble-0.6.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 19:58:20.940987 prosemble-0.5.0/
--rw-rw-rw-   0        0        0     1095 2022-05-22 15:35:18.000000 prosemble-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     1896 2023-04-23 19:58:20.940987 prosemble-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      924 2023-03-05 13:07:08.000000 prosemble-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 19:58:20.888859 prosemble-0.5.0/prosemble/
--rw-rw-rw-   0        0        0      128 2023-04-23 19:39:20.000000 prosemble-0.5.0/prosemble/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 19:58:20.905826 prosemble-0.5.0/prosemble/core/
--rw-rw-rw-   0        0        0      138 2023-04-02 22:26:45.000000 prosemble-0.5.0/prosemble/core/__init__.py
--rw-rw-rw-   0        0        0      420 2023-03-05 12:42:58.000000 prosemble-0.5.0/prosemble/core/distance.py
--rw-rw-rw-   0        0        0     6312 2023-04-03 20:22:45.000000 prosemble-0.5.0/prosemble/core/graphdata.py
--rw-rw-rw-   0        0        0        2 2023-03-03 22:57:08.000000 prosemble-0.5.0/prosemble/core/initializers.py
--rw-rw-rw-   0        0        0    38834 2022-09-17 20:19:36.000000 prosemble-0.5.0/prosemble/core/labelsecurity.py
-drwxrwxrwx   0        0        0        0 2023-04-23 19:58:20.938824 prosemble-0.5.0/prosemble/models/
--rw-rw-rw-   0        0        0      446 2023-04-23 19:39:20.000000 prosemble-0.5.0/prosemble/models/__init__.py
--rw-rw-rw-   0        0        0    14031 2023-04-23 16:47:52.000000 prosemble-0.5.0/prosemble/models/afcm.py
--rw-rw-rw-   0        0        0    11784 2023-04-23 19:14:00.000000 prosemble-0.5.0/prosemble/models/bgpc.py
--rw-rw-rw-   0        0        0    11062 2023-04-23 19:14:00.000000 prosemble-0.5.0/prosemble/models/fcm.py
--rw-rw-rw-   0        0        0    11838 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/fpcm.py
--rw-rw-rw-   0        0        0     8952 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/hcm.py
--rw-rw-rw-   0        0        0    18646 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/ipcm.py
--rw-rw-rw-   0        0        0    18455 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/ipcm_2.py
--rw-rw-rw-   0        0        0    15410 2023-04-23 16:47:52.000000 prosemble-0.5.0/prosemble/models/kafcm.py
--rw-rw-rw-   0        0        0    11772 2023-04-23 16:47:52.000000 prosemble-0.5.0/prosemble/models/kfcm.py
--rw-rw-rw-   0        0        0    13516 2023-04-23 16:51:46.000000 prosemble-0.5.0/prosemble/models/kfpcm.py
--rw-rw-rw-   0        0        0     5682 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/kmeans.py
--rw-rw-rw-   0        0        0     2070 2023-04-02 22:26:45.000000 prosemble-0.5.0/prosemble/models/knn.py
--rw-rw-rw-   0        0        0    15313 2023-04-23 16:27:34.000000 prosemble-0.5.0/prosemble/models/kpcm.py
--rw-rw-rw-   0        0        0    16045 2023-04-23 16:27:34.000000 prosemble-0.5.0/prosemble/models/kpfcm.py
--rw-rw-rw-   0        0        0     2687 2023-04-02 22:26:45.000000 prosemble-0.5.0/prosemble/models/npc.py
--rw-rw-rw-   0        0        0    14305 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/pcm.py
--rw-rw-rw-   0        0        0    13648 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/pfcm.py
--rw-rw-rw-   0        0        0     3801 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/som.py
--rw-rw-rw-   0        0        0     8223 2023-04-03 14:20:26.000000 prosemble-0.5.0/prosemble/models/spectralclustering.py
-drwxrwxrwx   0        0        0        0 2023-04-23 19:58:20.897825 prosemble-0.5.0/prosemble.egg-info/
--rw-rw-rw-   0        0        0     1896 2023-04-23 19:58:20.000000 prosemble-0.5.0/prosemble.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      876 2023-04-23 19:58:20.000000 prosemble-0.5.0/prosemble.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 19:58:20.000000 prosemble-0.5.0/prosemble.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-23 19:58:20.000000 prosemble-0.5.0/prosemble.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-23 19:58:20.000000 prosemble-0.5.0/prosemble.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 19:58:20.941986 prosemble-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1327 2023-04-23 19:39:20.000000 prosemble-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:43:45.618919 prosemble-0.6.0/
+-rw-rw-rw-   0        0        0     1095 2022-05-22 15:35:18.000000 prosemble-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     1896 2023-04-29 21:43:45.616915 prosemble-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0      924 2023-03-05 13:07:08.000000 prosemble-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 21:43:45.540743 prosemble-0.6.0/prosemble/
+-rw-rw-rw-   0        0        0      128 2023-04-29 21:37:44.000000 prosemble-0.6.0/prosemble/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:43:45.562915 prosemble-0.6.0/prosemble/core/
+-rw-rw-rw-   0        0        0      138 2023-04-02 22:26:45.000000 prosemble-0.6.0/prosemble/core/__init__.py
+-rw-rw-rw-   0        0        0      420 2023-03-05 12:42:58.000000 prosemble-0.6.0/prosemble/core/distance.py
+-rw-rw-rw-   0        0        0     6312 2023-04-03 20:22:45.000000 prosemble-0.6.0/prosemble/core/graphdata.py
+-rw-rw-rw-   0        0        0        2 2023-03-03 22:57:08.000000 prosemble-0.6.0/prosemble/core/initializers.py
+-rw-rw-rw-   0        0        0    38834 2022-09-17 20:19:36.000000 prosemble-0.6.0/prosemble/core/labelsecurity.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:43:45.614915 prosemble-0.6.0/prosemble/models/
+-rw-rw-rw-   0        0        0      491 2023-04-29 21:37:44.000000 prosemble-0.6.0/prosemble/models/__init__.py
+-rw-rw-rw-   0        0        0    14031 2023-04-23 16:47:52.000000 prosemble-0.6.0/prosemble/models/afcm.py
+-rw-rw-rw-   0        0        0    11784 2023-04-23 19:14:00.000000 prosemble-0.6.0/prosemble/models/bgpc.py
+-rw-rw-rw-   0        0        0    11062 2023-04-23 19:14:00.000000 prosemble-0.6.0/prosemble/models/fcm.py
+-rw-rw-rw-   0        0        0    11838 2023-04-23 19:14:01.000000 prosemble-0.6.0/prosemble/models/fpcm.py
+-rw-rw-rw-   0        0        0     8952 2023-04-23 19:14:01.000000 prosemble-0.6.0/prosemble/models/hcm.py
+-rw-rw-rw-   0        0        0    18595 2023-04-29 11:48:47.000000 prosemble-0.6.0/prosemble/models/ipcm.py
+-rw-rw-rw-   0        0        0    18455 2023-04-23 19:14:01.000000 prosemble-0.6.0/prosemble/models/ipcm_2.py
+-rw-rw-rw-   0        0        0    15410 2023-04-23 16:47:52.000000 prosemble-0.6.0/prosemble/models/kafcm.py
+-rw-rw-rw-   0        0        0    11772 2023-04-23 16:47:52.000000 prosemble-0.6.0/prosemble/models/kfcm.py
+-rw-rw-rw-   0        0        0    13516 2023-04-23 16:51:46.000000 prosemble-0.6.0/prosemble/models/kfpcm.py
+-rw-rw-rw-   0        0        0    17825 2023-04-29 16:00:48.000000 prosemble-0.6.0/prosemble/models/kipcm.py
+-rw-rw-rw-   0        0        0    17861 2023-04-28 21:28:16.000000 prosemble-0.6.0/prosemble/models/kipcm2.py
+-rw-rw-rw-   0        0        0     5682 2023-04-23 19:14:01.000000 prosemble-0.6.0/prosemble/models/kmeans.py
+-rw-rw-rw-   0        0        0     2070 2023-04-02 22:26:45.000000 prosemble-0.6.0/prosemble/models/knn.py
+-rw-rw-rw-   0        0        0    15313 2023-04-23 16:27:34.000000 prosemble-0.6.0/prosemble/models/kpcm.py
+-rw-rw-rw-   0        0        0    16045 2023-04-23 16:27:34.000000 prosemble-0.6.0/prosemble/models/kpfcm.py
+-rw-rw-rw-   0        0        0     2687 2023-04-02 22:26:45.000000 prosemble-0.6.0/prosemble/models/npc.py
+-rw-rw-rw-   0        0        0    14305 2023-04-23 19:14:01.000000 prosemble-0.6.0/prosemble/models/pcm.py
+-rw-rw-rw-   0        0        0    13648 2023-04-23 19:14:01.000000 prosemble-0.6.0/prosemble/models/pfcm.py
+-rw-rw-rw-   0        0        0     3801 2023-04-23 19:14:01.000000 prosemble-0.6.0/prosemble/models/som.py
+-rw-rw-rw-   0        0        0     8223 2023-04-03 14:20:26.000000 prosemble-0.6.0/prosemble/models/spectralclustering.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:43:45.552916 prosemble-0.6.0/prosemble.egg-info/
+-rw-rw-rw-   0        0        0     1896 2023-04-29 21:43:45.000000 prosemble-0.6.0/prosemble.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      929 2023-04-29 21:43:45.000000 prosemble-0.6.0/prosemble.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 21:43:45.000000 prosemble-0.6.0/prosemble.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-29 21:43:45.000000 prosemble-0.6.0/prosemble.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-29 21:43:45.000000 prosemble-0.6.0/prosemble.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 21:43:45.618919 prosemble-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1327 2023-04-29 21:30:28.000000 prosemble-0.6.0/setup.py
```

### Comparing `prosemble-0.5.0/LICENSE` & `prosemble-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/PKG-INFO` & `prosemble-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosemble
-Version: 0.5.0
+Version: 0.6.0
 Summary: Prototype and non prototype-based machine learning package
 Home-page: https://github.com/naotoo1/prosemble
 Author: Nana Abeka Otoo
 Author-email: abekaotoo@gmail.com
 License: UNKNOWN
 Keywords: ensemble,Prototype models
 Platform: UNKNOWN
```

### Comparing `prosemble-0.5.0/README.md` & `prosemble-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/core/graphdata.py` & `prosemble-0.6.0/prosemble/core/graphdata.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/core/labelsecurity.py` & `prosemble-0.6.0/prosemble/core/labelsecurity.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/afcm.py` & `prosemble-0.6.0/prosemble/models/afcm.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/bgpc.py` & `prosemble-0.6.0/prosemble/models/bgpc.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/fcm.py` & `prosemble-0.6.0/prosemble/models/fcm.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/fpcm.py` & `prosemble-0.6.0/prosemble/models/fpcm.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/hcm.py` & `prosemble-0.6.0/prosemble/models/hcm.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/ipcm.py` & `prosemble-0.6.0/prosemble/models/ipcm.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 # Author: Nana Abeka Otoo <abekaotoo@gmail.com>
 # License: MIT
 
 
 from collections import Counter
 
-import matplotlib
 import numpy as np
 from matplotlib import pyplot as plt
 # matplotlib.use('QtAgg')
 from .fcm import FCM
 from prosemble.core.distance import (
     euclidean_distance,
     squared_euclidean_distance
@@ -204,22 +203,22 @@
 
     def update_fuzzy_matrix(self, centroids, u_matrix, t_matrix):  # equation 8
         initial_u_matrix = u_matrix
         for i in range(len(self.data)):
             denomenator = 0
             for j in range(self.num_clusters):
                 denomenator += np.power(
-                    (1 / euclidean_distance(centroids[j], self.data[i])) *
+                    (1 / squared_euclidean_distance(centroids[j], self.data[i])) *
                     np.power(t_matrix[i][j], (self.tipifier - 1)),
-                    2 / (self.fuzzifier - 1)
+                    1 / (self.fuzzifier - 1)
                 )
             for j in range(self.num_clusters):
-                uik_new = np.power((1 / euclidean_distance(centroids[j], self.data[i])) *
+                uik_new = np.power((1 / squared_euclidean_distance(centroids[j], self.data[i])) *
                                    (np.power(t_matrix[i][j], (self.tipifier - 1))),
-                                   2 / (self.fuzzifier - 1)) / denomenator
+                                   1 / (self.fuzzifier - 1)) / denomenator
                 initial_u_matrix[i][j] = uik_new
         return initial_u_matrix
 
     def _select_fuzzy_U_matrix(self):
         if self.set_U_matrix is None:
             return self.randomly_initialised_fuzzy_matrix()
         return self.set_U_matrix
@@ -292,25 +291,24 @@
     def get_centroids_0(self):
         u_matrix = self._select_fuzzy_U_matrix()
         centroids = self.set_centroids
         t_matrix = np.zeros((len(self.data), self.num_clusters))
         gamma = self.compute_gamma_0(u_matrix, centroids)
         for num in range(self.num_iter):
             centroids_old = centroids
-            obj = self.compute_objective_function(centroids, t_matrix, gamma, u_matrix)
+            obj = self.compute_objective_function(centroids, gamma, t_matrix, u_matrix)
             self.objective_function.append(obj)
             clusters = self.initialise_cluster(centroids_old)
             self.get_plot(clusters, centroids_old)
             t_matrix = self.update_tipicality_matrix(centroids_old, gamma, t_matrix)
             u_matrix = self.update_fuzzy_matrix(centroids, u_matrix, t_matrix)
             centroids = self.compute_centroids(u_matrix, t_matrix)
             self.get_plot(clusters, centroids)
             if self._centroid_stability(centroids_old, centroids) or num == self.num_iter - 1:
                 return u_matrix, t_matrix, centroids
-        return None
 
     def get_centroids_1(self):
         u_matrix, t_matrix, centroids = self.get_centroids_0()
         gamma = self.compute_gamma_1(u_matrix, t_matrix, centroids)
         for num in range(self.num_iter):
             centroids_old = centroids
             clusters = self.initialise_cluster(centroids_old)
@@ -362,15 +360,14 @@
             self.objective_function.append(obj)
             self.get_plot(clusters, centroids)
             if self._centroid_stability(centroid_num, centroids):
                 self.fit_clus.append(clusters)
                 self.fit_cent.append(centroids)
                 self.eta.append(gamma)
                 optimize = False
-        return u_matrix, t_matrix, centroids
 
     def get_plot(self, cluster, centroids):
         if self.plot_steps:
             for _, v in enumerate(cluster):
                 plt.scatter(self.data[v][:, 0], self.data[v][:, 1])
             for cent in centroids:
                 plt.scatter(cent[0], cent[1], marker='v', color='black')
@@ -436,22 +433,22 @@
         """
         initial_u_matrix = np.zeros((len(x), self.num_clusters))
         t_matrix = self.predict_tipicality_(x)
         for i in range(len(x)):
             denomenator = 0
             for j in range(self.num_clusters):
                 denomenator += np.power(
-                    (1 / euclidean_distance(self.fit_cent[0][j], x[i])) *
+                    (1 / squared_euclidean_distance(self.fit_cent[0][j], x[i])) *
                     np.power(t_matrix[i][j], (self.tipifier - 1)),
-                    2 / (self.fuzzifier - 1)
+                    1 / (self.fuzzifier - 1)
                 )
             for j in range(self.num_clusters):
-                uik_new = np.power((1 / euclidean_distance(self.fit_cent[0][j], x[i])) *
+                uik_new = np.power((1 / squared_euclidean_distance(self.fit_cent[0][j], x[i])) *
                                    (np.power(t_matrix[i][j], (self.tipifier - 1))),
-                                   2 / (self.fuzzifier - 1)) / denomenator
+                                   1 / (self.fuzzifier - 1)) / denomenator
                 initial_u_matrix[i][j] = uik_new
         return initial_u_matrix
 
     def predict_tipicality_(self, x):
         """
 
         :param x: array-like: input vector
```

### Comparing `prosemble-0.5.0/prosemble/models/ipcm_2.py` & `prosemble-0.6.0/prosemble/models/ipcm_2.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/kafcm.py` & `prosemble-0.6.0/prosemble/models/kafcm.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/kfcm.py` & `prosemble-0.6.0/prosemble/models/kfcm.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/kfpcm.py` & `prosemble-0.6.0/prosemble/models/kfpcm.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/kmeans.py` & `prosemble-0.6.0/prosemble/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/knn.py` & `prosemble-0.6.0/prosemble/models/knn.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/kpcm.py` & `prosemble-0.6.0/prosemble/models/kpcm.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/kpfcm.py` & `prosemble-0.6.0/prosemble/models/kpfcm.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/npc.py` & `prosemble-0.6.0/prosemble/models/npc.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/pcm.py` & `prosemble-0.6.0/prosemble/models/pcm.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/pfcm.py` & `prosemble-0.6.0/prosemble/models/pfcm.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/som.py` & `prosemble-0.6.0/prosemble/models/som.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble/models/spectralclustering.py` & `prosemble-0.6.0/prosemble/models/spectralclustering.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.5.0/prosemble.egg-info/PKG-INFO` & `prosemble-0.6.0/prosemble.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosemble
-Version: 0.5.0
+Version: 0.6.0
 Summary: Prototype and non prototype-based machine learning package
 Home-page: https://github.com/naotoo1/prosemble
 Author: Nana Abeka Otoo
 Author-email: abekaotoo@gmail.com
 License: UNKNOWN
 Keywords: ensemble,Prototype models
 Platform: UNKNOWN
```

### Comparing `prosemble-0.5.0/prosemble.egg-info/SOURCES.txt` & `prosemble-0.6.0/prosemble.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 prosemble/models/fpcm.py
 prosemble/models/hcm.py
 prosemble/models/ipcm.py
 prosemble/models/ipcm_2.py
 prosemble/models/kafcm.py
 prosemble/models/kfcm.py
 prosemble/models/kfpcm.py
+prosemble/models/kipcm.py
+prosemble/models/kipcm2.py
 prosemble/models/kmeans.py
 prosemble/models/knn.py
 prosemble/models/kpcm.py
 prosemble/models/kpfcm.py
 prosemble/models/npc.py
 prosemble/models/pcm.py
 prosemble/models/pfcm.py
```

### Comparing `prosemble-0.5.0/setup.py` & `prosemble-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="prosemble",
-    version="0.5.0",
+    version="0.6.0",
     author="Nana Abeka Otoo",
     author_email="abekaotoo@gmail.com",
     description="Prototype and non prototype-based machine learning package",
     url="https://github.com/naotoo1/prosemble",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```


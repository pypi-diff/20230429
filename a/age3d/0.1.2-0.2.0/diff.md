# Comparing `tmp/age3d-0.1.2.tar.gz` & `tmp/age3d-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "age3d-0.1.2.tar", last modified: Wed Apr  5 00:02:56 2023, max compression
+gzip compressed data, was "age3d-0.2.0.tar", last modified: Sat Apr 29 06:18:45 2023, max compression
```

## Comparing `age3d-0.1.2.tar` & `age3d-0.2.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 00:02:56.116531 age3d-0.1.2/
--rw-rw-rw-   0        0        0      294 2023-04-05 00:02:26.000000 age3d-0.1.2/.bumpversion.cfg
--rw-rw-rw-   0        0        0      493 2023-04-04 09:58:38.000000 age3d-0.1.2/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1114 2023-03-26 00:42:17.000000 age3d-0.1.2/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11357 2023-03-24 19:50:45.000000 age3d-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      644 2023-04-04 23:55:51.000000 age3d-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2570 2023-04-04 09:58:38.000000 age3d-0.1.2/Makefile
--rw-rw-rw-   0        0        0    17220 2023-04-05 00:02:56.115305 age3d-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3132 2023-04-04 09:58:38.000000 age3d-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 00:02:56.037260 age3d-0.1.2/age3d/
--rw-rw-rw-   0        0        0      339 2023-03-25 23:20:12.000000 age3d-0.1.2/age3d/__init__.py
--rw-rw-rw-   0        0        0     1215 2023-03-25 23:20:12.000000 age3d-0.1.2/age3d/__main__.py
--rw-rw-rw-   0        0        0       22 2023-04-05 00:02:26.000000 age3d-0.1.2/age3d/_version.py
--rw-rw-rw-   0        0        0    12572 2023-04-03 09:21:22.000000 age3d-0.1.2/age3d/age3d.py
--rw-rw-rw-   0        0        0    17586 2023-04-04 11:40:52.000000 age3d-0.1.2/age3d/examples.ipynb
-drwxrwxrwx   0        0        0        0 2023-04-05 00:02:56.064241 age3d-0.1.2/age3d/models/
--rw-rw-rw-   0        0        0    48484 2023-03-24 19:50:45.000000 age3d-0.1.2/age3d/models/monkey.stl
--rw-rw-rw-   0        0        0    48484 2023-03-24 19:50:45.000000 age3d-0.1.2/age3d/models/monkey_cleaned.stl
-drwxrwxrwx   0        0        0        0 2023-04-05 00:02:56.070241 age3d-0.1.2/age3d/tests/
--rw-rw-rw-   0        0        0    11744 2023-03-25 23:20:12.000000 age3d-0.1.2/age3d/tests/monkey_triangles.npy
--rw-rw-rw-   0        0        0    68912 2023-03-25 23:20:12.000000 age3d-0.1.2/age3d/tests/monkey_vertices.npy
--rw-rw-rw-   0        0        0     7056 2023-03-25 23:20:12.000000 age3d-0.1.2/age3d/tests/test_all.py
-drwxrwxrwx   0        0        0        0 2023-04-05 00:02:56.059242 age3d-0.1.2/age3d.egg-info/
--rw-rw-rw-   0        0        0    17220 2023-04-05 00:02:55.000000 age3d-0.1.2/age3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      912 2023-04-05 00:02:55.000000 age3d-0.1.2/age3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 00:02:55.000000 age3d-0.1.2/age3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      210 2023-04-05 00:02:55.000000 age3d-0.1.2/age3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-05 00:02:55.000000 age3d-0.1.2/age3d.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 00:02:56.085883 age3d-0.1.2/docs/
--rw-rw-rw-   0        0        0      683 2023-04-04 06:54:19.000000 age3d-0.1.2/docs/Makefile
--rw-rw-rw-   0        0        0     1209 2023-04-04 06:54:19.000000 age3d-0.1.2/docs/conf.py
--rw-rw-rw-   0        0        0       96 2023-04-04 06:54:19.000000 age3d-0.1.2/docs/documentation.rst
--rw-rw-rw-   0        0        0    14680 2023-04-04 11:40:52.000000 age3d-0.1.2/docs/examples.rst
--rw-rw-rw-   0        0        0     1340 2023-04-04 06:54:19.000000 age3d-0.1.2/docs/getting_started.rst
-drwxrwxrwx   0        0        0        0 2023-04-05 00:02:56.112343 age3d-0.1.2/docs/img/
--rw-rw-rw-   0        0        0    63875 2023-04-04 11:40:52.000000 age3d-0.1.2/docs/img/monkey.png
--rw-rw-rw-   0        0        0    69385 2023-04-04 11:40:52.000000 age3d-0.1.2/docs/img/monkey_below_above_between.png
--rw-rw-rw-   0        0        0   100655 2023-04-04 11:40:52.000000 age3d-0.1.2/docs/img/monkey_bound_height.png
--rw-rw-rw-   0        0        0    81498 2023-04-04 11:40:52.000000 age3d-0.1.2/docs/img/monkey_erode.png
--rw-rw-rw-   0        0        0   127495 2023-04-04 11:40:52.000000 age3d-0.1.2/docs/img/monkey_erode_wireframe.png
--rw-rw-rw-   0        0        0    64955 2023-04-04 11:40:52.000000 age3d-0.1.2/docs/img/monkey_min_max.png
--rw-rw-rw-   0        0        0    58693 2023-04-04 11:40:52.000000 age3d-0.1.2/docs/img/monkey_neighbors.png
--rw-rw-rw-   0        0        0    67341 2023-04-04 11:40:52.000000 age3d-0.1.2/docs/img/monkey_pc.png
--rw-rw-rw-   0        0        0   125751 2023-04-04 11:40:52.000000 age3d-0.1.2/docs/img/monkey_subdivision.png
--rw-rw-rw-   0        0        0    73476 2023-04-04 11:40:52.000000 age3d-0.1.2/docs/img/monkey_wireframe.png
--rw-rw-rw-   0        0        0      454 2023-04-04 11:40:52.000000 age3d-0.1.2/docs/index.rst
--rwxrwxrwx   0        0        0      765 2023-04-04 06:54:19.000000 age3d-0.1.2/docs/make.bat
--rw-rw-rw-   0        0        0     2214 2023-04-05 00:02:26.000000 age3d-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 00:02:56.117444 age3d-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-24 19:50:45.000000 age3d-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 06:18:45.991797 age3d-0.2.0/
+-rw-rw-rw-   0        0        0      294 2023-04-29 06:09:41.000000 age3d-0.2.0/.bumpversion.cfg
+-rw-rw-rw-   0        0        0      493 2023-04-04 09:58:38.000000 age3d-0.2.0/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1114 2023-03-26 00:42:17.000000 age3d-0.2.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11357 2023-03-24 19:50:45.000000 age3d-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      644 2023-04-05 00:11:10.000000 age3d-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2570 2023-04-04 09:58:38.000000 age3d-0.2.0/Makefile
+-rw-rw-rw-   0        0        0    17220 2023-04-29 06:18:45.990802 age3d-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3132 2023-04-04 09:58:38.000000 age3d-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 06:18:45.917794 age3d-0.2.0/age3d/
+-rw-rw-rw-   0        0        0      339 2023-03-25 23:20:12.000000 age3d-0.2.0/age3d/__init__.py
+-rw-rw-rw-   0        0        0     1215 2023-03-25 23:20:12.000000 age3d-0.2.0/age3d/__main__.py
+-rw-rw-rw-   0        0        0       22 2023-04-29 06:09:41.000000 age3d-0.2.0/age3d/_version.py
+-rw-rw-rw-   0        0        0    14077 2023-04-29 06:09:41.000000 age3d-0.2.0/age3d/age3d.py
+-rw-rw-rw-   0        0        0    17586 2023-04-04 11:40:52.000000 age3d-0.2.0/age3d/examples.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-29 06:18:45.949794 age3d-0.2.0/age3d/models/
+-rw-rw-rw-   0        0        0    48484 2023-03-24 19:50:45.000000 age3d-0.2.0/age3d/models/monkey.stl
+-rw-rw-rw-   0        0        0    48484 2023-03-24 19:50:45.000000 age3d-0.2.0/age3d/models/monkey_cleaned.stl
+drwxrwxrwx   0        0        0        0 2023-04-29 06:18:45.954800 age3d-0.2.0/age3d/tests/
+-rw-rw-rw-   0        0        0    11744 2023-03-25 23:20:12.000000 age3d-0.2.0/age3d/tests/monkey_triangles.npy
+-rw-rw-rw-   0        0        0    68912 2023-03-25 23:20:12.000000 age3d-0.2.0/age3d/tests/monkey_vertices.npy
+-rw-rw-rw-   0        0        0     7056 2023-03-25 23:20:12.000000 age3d-0.2.0/age3d/tests/test_all.py
+drwxrwxrwx   0        0        0        0 2023-04-29 06:18:45.946796 age3d-0.2.0/age3d.egg-info/
+-rw-rw-rw-   0        0        0    17220 2023-04-29 06:18:45.000000 age3d-0.2.0/age3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      912 2023-04-29 06:18:45.000000 age3d-0.2.0/age3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 06:18:45.000000 age3d-0.2.0/age3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-04-29 06:18:45.000000 age3d-0.2.0/age3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-29 06:18:45.000000 age3d-0.2.0/age3d.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 06:18:45.966795 age3d-0.2.0/docs/
+-rw-rw-rw-   0        0        0      683 2023-04-04 06:54:19.000000 age3d-0.2.0/docs/Makefile
+-rw-rw-rw-   0        0        0     1209 2023-04-04 06:54:19.000000 age3d-0.2.0/docs/conf.py
+-rw-rw-rw-   0        0        0       96 2023-04-04 06:54:19.000000 age3d-0.2.0/docs/documentation.rst
+-rw-rw-rw-   0        0        0    14680 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/examples.rst
+-rw-rw-rw-   0        0        0     1340 2023-04-04 06:54:19.000000 age3d-0.2.0/docs/getting_started.rst
+drwxrwxrwx   0        0        0        0 2023-04-29 06:18:45.986797 age3d-0.2.0/docs/img/
+-rw-rw-rw-   0        0        0    63875 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey.png
+-rw-rw-rw-   0        0        0    69385 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_below_above_between.png
+-rw-rw-rw-   0        0        0   100655 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_bound_height.png
+-rw-rw-rw-   0        0        0    81498 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_erode.png
+-rw-rw-rw-   0        0        0   127495 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_erode_wireframe.png
+-rw-rw-rw-   0        0        0    64955 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_min_max.png
+-rw-rw-rw-   0        0        0    58693 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_neighbors.png
+-rw-rw-rw-   0        0        0    67341 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_pc.png
+-rw-rw-rw-   0        0        0   125751 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_subdivision.png
+-rw-rw-rw-   0        0        0    73476 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_wireframe.png
+-rw-rw-rw-   0        0        0      454 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/index.rst
+-rwxrwxrwx   0        0        0      765 2023-04-04 06:54:19.000000 age3d-0.2.0/docs/make.bat
+-rw-rw-rw-   0        0        0     2214 2023-04-29 06:09:41.000000 age3d-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 06:18:45.991797 age3d-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-24 19:50:45.000000 age3d-0.2.0/setup.py
```

### Comparing `age3d-0.1.2/CONTRIBUTING.md` & `age3d-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/LICENSE` & `age3d-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/MANIFEST.in` & `age3d-0.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/Makefile` & `age3d-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/PKG-INFO` & `age3d-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: age3d
-Version: 0.1.2
+Version: 0.2.0
 Summary: Aging 3D models
 Author-email: Abhishek Chaudhary <ac5003@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `age3d-0.1.2/README.md` & `age3d-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/age3d/__main__.py` & `age3d-0.2.0/age3d/__main__.py`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/age3d/age3d.py` & `age3d-0.2.0/age3d/age3d.py`

 * *Files 7% similar despite different names*

```diff
@@ -332,46 +332,81 @@
     vertices_idx, vertices = find_all_above(mesh, calculate_bounds_height(mesh), True)
 
     set_vertices_idx = set()
     for idx in vertices_idx:
         set_vertices_idx.add(idx)
     # print('set', set_vertices_idx)
 
+    # Create New Mesh
     new_mesh = o3d.geometry.TriangleMesh()
     new_vertices = np.asarray(mesh.vertices)
     new_triangles = np.asarray(mesh.triangles)
     updated_vertices = []
 
     new_mesh.vertices = o3d.utility.Vector3dVector(new_vertices)
     new_mesh.triangles = o3d.utility.Vector3iVector(new_triangles)
 
     mesh_max_height = find_maximum(mesh)[1][0, 2]
     rng = np.random.default_rng(10)
 
     for iter_no in range(iterations):
-        v_idx_curr = vertices_idx[int(rng.random() * vertices.shape[0])]
+        v_idx_curr = int(vertices_idx[int(rng.random() * vertices.shape[0])])
         print('Iter: ', iter_no, ', V_idx: ', v_idx_curr)
 
-        lifetime = erosion_lifetime
+        lifetime = 0
         strength = 0.5
-        while lifetime > 0:
-            new_mesh.vertices = o3d.utility.Vector3dVector(new_vertices)
+        v_idx_prev = None
+
+        while lifetime < erosion_lifetime:
             neighbors_idx, _ = find_neighbors(new_mesh, v_idx_curr)
             v_idx_next = int(find_minimum(new_mesh, 1, neighbors_idx)[0])
 
             if v_idx_next not in vertices_idx:
                 break
 
             # if #TODO Angle Calculations
+            if v_idx_prev:
+                print(
+                    v_idx_prev,
+                    v_idx_curr,
+                    v_idx_next,
+                    type(new_vertices[v_idx_prev]),
+                    new_vertices[v_idx_prev],
+                    new_vertices[v_idx_curr],
+                    new_vertices[v_idx_next],
+                )
+                vector_1 = new_vertices[v_idx_curr] - new_vertices[v_idx_prev]
+                vector_2 = new_vertices[v_idx_next] - new_vertices[v_idx_curr]
+                direction_1 = np.sign(vector_1)
+                direction_2 = np.sign(vector_2)
+                # print(vector_1, vector_2, direction_1, direction_2, np.dot(direction_1 , direction_2))
+
+                if vector_2[2] > 0:
+                    break
+
+                vector_1[2] = 0
+                vector_2[2] = 0
+                norm_vector_1 = np.linalg.norm(vector_1)
+                norm_vector_2 = np.linalg.norm(vector_2)
+                angle = np.arccos(np.clip(np.dot(vector_1, vector_2) / (norm_vector_1 * norm_vector_2), -1.0, 1.0))
+                print(vector_1, vector_2, direction_1, direction_2, np.dot(direction_1, direction_2), angle)
+                # if angle < 0:
+                #     print('negative angle', angle)
+                if angle > np.pi / 2:
+                    # print('pi angle', angle)
+                    break
+                # if angle > np.pi / 2
 
             new_vertices[v_idx_curr, 2] -= (
                 strength * abs(new_vertices[v_idx_next, 2] - new_vertices[v_idx_curr, 2]) / mesh_max_height
             )
+            new_mesh.vertices = o3d.utility.Vector3dVector(new_vertices)
             updated_vertices.append(v_idx_curr)
 
-            lifetime -= 1
+            lifetime += 1
             strength *= 0.69
+            v_idx_prev = v_idx_curr
             v_idx_curr = v_idx_next
 
     new_mesh.vertices = o3d.utility.Vector3dVector(new_vertices)
     new_mesh.triangles = o3d.utility.Vector3iVector(new_triangles)
     return np.array(updated_vertices), new_mesh
```

### Comparing `age3d-0.1.2/age3d/examples.ipynb` & `age3d-0.2.0/age3d/examples.ipynb`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/age3d/models/monkey.stl` & `age3d-0.2.0/age3d/models/monkey.stl`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/age3d/models/monkey_cleaned.stl` & `age3d-0.2.0/age3d/models/monkey_cleaned.stl`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/age3d/tests/monkey_triangles.npy` & `age3d-0.2.0/age3d/tests/monkey_triangles.npy`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/age3d/tests/monkey_vertices.npy` & `age3d-0.2.0/age3d/tests/monkey_vertices.npy`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/age3d/tests/test_all.py` & `age3d-0.2.0/age3d/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/age3d.egg-info/PKG-INFO` & `age3d-0.2.0/age3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: age3d
-Version: 0.1.2
+Version: 0.2.0
 Summary: Aging 3D models
 Author-email: Abhishek Chaudhary <ac5003@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `age3d-0.1.2/age3d.egg-info/SOURCES.txt` & `age3d-0.2.0/age3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/Makefile` & `age3d-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/conf.py` & `age3d-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/examples.rst` & `age3d-0.2.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/getting_started.rst` & `age3d-0.2.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/img/monkey.png` & `age3d-0.2.0/docs/img/monkey.png`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/img/monkey_below_above_between.png` & `age3d-0.2.0/docs/img/monkey_below_above_between.png`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/img/monkey_bound_height.png` & `age3d-0.2.0/docs/img/monkey_bound_height.png`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/img/monkey_erode.png` & `age3d-0.2.0/docs/img/monkey_erode.png`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/img/monkey_erode_wireframe.png` & `age3d-0.2.0/docs/img/monkey_erode_wireframe.png`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/img/monkey_min_max.png` & `age3d-0.2.0/docs/img/monkey_min_max.png`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/img/monkey_neighbors.png` & `age3d-0.2.0/docs/img/monkey_neighbors.png`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/img/monkey_pc.png` & `age3d-0.2.0/docs/img/monkey_pc.png`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/img/monkey_subdivision.png` & `age3d-0.2.0/docs/img/monkey_subdivision.png`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/img/monkey_wireframe.png` & `age3d-0.2.0/docs/img/monkey_wireframe.png`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/docs/make.bat` & `age3d-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `age3d-0.1.2/pyproject.toml` & `age3d-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "age3d"
 authors = [{name = "Abhishek Chaudhary", email = "ac5003@columbia.edu"}]
 description="Aging 3D models"
 readme = "README.md"
-version = "0.1.2"
+version = "0.2.0"
 requires-python = ">=3.7"
 
 dependencies = [
     "open3d==0.16.0"
 ]
 
 classifiers = [
```


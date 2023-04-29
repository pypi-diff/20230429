# Comparing `tmp/malla-0.1.3.tar.gz` & `tmp/malla-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malla-0.1.3.tar", max compression
+gzip compressed data, was "malla-0.1.4.tar", max compression
```

## Comparing `malla-0.1.3.tar` & `malla-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      526 2023-04-29 16:35:40.386927 malla-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.3/malla/__init__.py
--rw-r--r--   0        0        0     6389 2023-04-29 16:49:03.813608 malla-0.1.3/malla/directed_edge.py
--rw-r--r--   0        0        0      717 2023-04-29 16:00:39.890220 malla-0.1.3/malla/off.py
--rw-r--r--   0        0        0      266 2023-04-29 16:49:30.586942 malla-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 malla-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      526 2023-04-29 16:35:40.386927 malla-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.4/malla/__init__.py
+-rw-r--r--   0        0        0     6398 2023-04-29 17:02:44.313624 malla-0.1.4/malla/directed_edge.py
+-rw-r--r--   0        0        0      717 2023-04-29 16:59:32.283620 malla-0.1.4/malla/off.py
+-rw-r--r--   0        0        0      266 2023-04-29 17:05:27.680293 malla-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 malla-0.1.4/PKG-INFO
```

### Comparing `malla-0.1.3/README.md` & `malla-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `malla-0.1.3/malla/directed_edge.py` & `malla-0.1.4/malla/directed_edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,20 +76,20 @@
     vertex_neighboring_faces(self, v: int):
         generator yielding the indices of faces incident to vertex v
     face_neighbors(self, f: int):
         generator yielding the indices of faces neighbors to face f
     """
 
     def __init__(self, vertices, faces):
-        self.vertices = [ vertex(v) for v in vertices ]
+        self._vertices = [ vertex(v) for v in vertices ]
         self.half_edges = []
         self._half_edges_map = {}
         for f in faces:
             self.__add_face(f)
-        for i in range(len(self.vertices)):
+        for i in range(len(self._vertices)):
             self.__assert_vertex_half_edge(i)
         self._half_edges_map = None
 
     @staticmethod
     def next(he: int) -> int:
         if he % 3 == 2:
             return he - 2
@@ -104,21 +104,21 @@
             return he - 1;
 
     @staticmethod
     def face(he: int) -> int:
         return int(he/3)
 
     def vertex(self, v: int) -> vertex:
-        return self.vertices[v]
+        return self._vertices[v]
 
     def half_edge(self, he: int) -> half_edge:
         return self.half_edges[he]
 
     def number_of_vertices(self) -> int:
-        return len(self.vertices)
+        return len(self._vertices)
 
     def number_of_faces(self) -> int:
         return int(len(self.half_edges)/3)
 
     def vertex_neighbors(self, v: int) -> Generator[int, None, None]:
         he = self.vertex(v).half_edge
         if he != -1:
@@ -165,15 +165,15 @@
         for f in range(self.number_of_faces()):
             i = self.half_edge(3*f).dst
             j = self.half_edge(3*f+1).dst
             k = self.half_edge(3*f+2).dst
             yield (i, j, k)
 
     def vertices(self) -> Generator[any, None, None]:
-        for v in self.vertices:
+        for v in self._vertices:
             yield v.data
 
     def __add_face(self, f: any) -> None:
         self.__put_half_edge(f[0], f[1])
         self.__put_half_edge(f[1], f[2])
         self.__put_half_edge(f[2], f[0])
 
@@ -181,36 +181,36 @@
         pair = (vi, vj)
         if pair in self._half_edges_map:
             print("Error  : wrong orientation on mesh. Quitting ...")
             exit()
         h = len(self.half_edges)
         he = half_edge(vj)
         self.half_edges.append(he)
-        if self.vertices[vi].half_edge == -1:
-            self.vertices[vi].half_edge = h
+        if self._vertices[vi].half_edge == -1:
+            self._vertices[vi].half_edge = h
         self._half_edges_map[pair] = h
         other_pair = (vj, vi)
         if other_pair in self._half_edges_map:
             self.__link(h, self._half_edges_map[other_pair]);
 
     def __link(self, he1: int, he2: int) -> None:
         if he1 != -1:
             self.half_edges[he1].mate = he2
         if he2 != -1:
             self.half_edges[he2].mate = he1
 
     def __assert_vertex_half_edge(self, v: int) -> None:
-        first = self.vertices[v].half_edge
+        first = self._vertices[v].half_edge
         if first != -1:
             mate  = self.half_edges[first].mate
             if mate != -1:
                 current = self.next(mate)
                 while current != first:
                     mate = self.half_edges[current].mate
                     if mate != -1:
                         current = self.next(mate)
                     else:
-                        self.vertices[v].half_edge = current
+                        self._vertices[v].half_edge = current
                         current = first
         else:
             print("Warning : vetex %d is isolated." % v)
```

### Comparing `malla-0.1.3/malla/off.py` & `malla-0.1.4/malla/off.py`

 * *Files identical despite different names*

### Comparing `malla-0.1.3/PKG-INFO` & `malla-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malla
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Dimas Martínez
 Author-email: dimas@ufam.edu.br
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


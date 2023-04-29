# Comparing `tmp/malla-0.1.1.tar.gz` & `tmp/malla-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malla-0.1.1.tar", max compression
+gzip compressed data, was "malla-0.1.2.tar", max compression
```

## Comparing `malla-0.1.1.tar` & `malla-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.1/malla/__init__.py
--rw-r--r--   0        0        0     6382 2023-04-27 15:52:38.670048 malla-0.1.1/malla/directed_edge.py
--rw-r--r--   0        0        0      618 2023-04-27 15:46:05.623373 malla-0.1.1/malla/off.py
--rw-r--r--   0        0        0      266 2023-04-27 17:09:35.293468 malla-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 malla-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      526 2023-04-29 16:35:40.386927 malla-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.2/malla/__init__.py
+-rw-r--r--   0        0        0     6383 2023-04-29 15:54:17.906880 malla-0.1.2/malla/directed_edge.py
+-rw-r--r--   0        0        0      717 2023-04-29 16:00:39.890220 malla-0.1.2/malla/off.py
+-rw-r--r--   0        0        0      266 2023-04-29 16:38:59.130263 malla-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 malla-0.1.2/PKG-INFO
```

### Comparing `malla-0.1.1/malla/directed_edge.py` & `malla-0.1.2/malla/directed_edge.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,24 +158,24 @@
         hf = 3*f
         for i in range(3):
             h = hf+i
             mate = self.half_edge(h).mate
             if mate > -1:
                 yield self.face(mate)
 
-    def face_strings(self) -> Generator[str, None, None]:
+    def faces(self) -> Generator[Tuple[int, int, int], None, None]:
         for f in range(self.number_of_faces()):
-            i = m.half_edge(3*f).dst
-            j = m.half_edge(3*f+1).dst
-            k = m.half_edge(3*f+2).dst
-            yield f'3 {i} {j} {k}'
+            i = self.half_edge(3*f).dst
+            j = self.half_edge(3*f+1).dst
+            k = self.half_edge(3*f+2).dst
+            yield (i, j, k)
 
-    def vertex_strings(self) -> Generator[str, None, None]:
+    def vertices(self) -> Generator[any, None, None]:
         for v in self.vertices:
-            yield str(v.data)
+            yield v.data
 
     def __add_face(self, f: any) -> None:
         self.__put_half_edge(f[0], f[1])
         self.__put_half_edge(f[1], f[2])
         self.__put_half_edge(f[2], f[0])
 
     def __put_half_edge(self, vi: int, vj: int) -> None:
```


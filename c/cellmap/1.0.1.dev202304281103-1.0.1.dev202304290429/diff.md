# Comparing `tmp/cellmap-1.0.1.dev202304281103-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304290429-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,7 @@
-Zip file size: 1395164 bytes, number of entries: 6
--rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
+Zip file size: 17762 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
 -rw-r--r--  2.0 unx    91233 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304281103.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304281103.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304281103.dist-info/RECORD
-6 files, 4540629 bytes uncompressed, 1394278 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304290429.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304290429.dist-info/WHEEL
+?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304290429.dist-info/RECORD
+5 files, 93646 bytes uncompressed, 17008 bytes compressed:  81.8%
```

## zipnote {}

```diff
@@ -1,19 +1,16 @@
-Filename: cellmap/CellMap_view_3D.html
-Comment: 
-
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304281103.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304290429.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304281103.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304290429.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304281103.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304290429.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cellmap-1.0.1.dev202304281103.dist-info/METADATA` & `cellmap-1.0.1.dev202304290429.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304281103
+Version: 1.0.1.dev202304290429
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: anndata (>=0.8.0,<0.9.0)
+Requires-Dist: adjustText (>=0.8)
+Requires-Dist: anndata (>=0.8.0)
 Requires-Dist: matplotlib (>=3.7.1)
 Requires-Dist: numpy (>=1.20)
 Requires-Dist: plotly (>=5.14.1)
 Requires-Dist: scanpy (>=1.9.3)
 Requires-Dist: scikit-learn (>=0.24)
-Requires-Dist: scipy (>=1.8.1,<2.0.0)
+Requires-Dist: scipy (>=1.8.1)
+Requires-Dist: scvelo (>=0.2.5)
 Project-URL: Documentation, https://github.com/yusuke-imoto-lab/CellMap/
 Project-URL: Repository, https://github.com/yusuke-imoto-lab/CellMap
 Description-Content-Type: text/markdown
 
 # CellMap - RNA landscape inference method
 
 <div style="text-align:left"><img style="width:100%; height: auto" src="https://github.com/yusuke-imoto-lab/CellMap/blob/main/figures/CellMap_Overview.jpg"/></div>
```


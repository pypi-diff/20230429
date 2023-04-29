# Comparing `tmp/pc_zap_scrapper-1.0.2.dev1.tar.gz` & `tmp/pc_zap_scrapper-1.0.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pc_zap_scrapper-1.0.2.dev1.tar", last modified: Sat Apr 29 03:05:12 2023, max compression
+gzip compressed data, was "pc_zap_scrapper-1.0.2rc0.tar", last modified: Sat Apr 29 03:06:08 2023, max compression
```

## Comparing `pc_zap_scrapper-1.0.2.dev1.tar` & `pc_zap_scrapper-1.0.2rc0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-29 03:05:12.498317 pc_zap_scrapper-1.0.2.dev1/
--rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)     1286 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2.dev1/LICENSE
--rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)      132 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2.dev1/MANIFEST.in
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5449 2023-04-29 03:05:12.498317 pc_zap_scrapper-1.0.2.dev1/PKG-INFO
--rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)     3480 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2.dev1/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-29 03:05:12.498317 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      756 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3184 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/__main__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       26 2023-04-29 03:05:00.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/_version.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-29 03:05:12.498317 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/datasets/
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-29 03:05:12.498317 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/datasets/external/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7696 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/datasets/external/neighbor_latlong.parquet
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1575 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/imoveis_db.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1231 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/load.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3478 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/maps.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1307 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/scrap.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6092 2023-04-29 03:02:38.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/transform.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2237 2023-04-29 03:02:49.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/utils.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-29 03:05:12.498317 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper.egg-info/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5449 2023-04-29 03:05:12.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      580 2023-04-29 03:05:12.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-29 03:05:12.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       58 2023-04-29 03:05:12.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper.egg-info/entry_points.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      278 2023-04-29 03:05:12.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       16 2023-04-29 03:05:12.000000 pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper.egg-info/top_level.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1895 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2.dev1/pyproject.toml
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-29 03:05:12.498317 pc_zap_scrapper-1.0.2.dev1/setup.cfg
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-29 03:06:08.272096 pc_zap_scrapper-1.0.2rc0/
+-rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)     1286 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2rc0/LICENSE
+-rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)      132 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2rc0/MANIFEST.in
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5447 2023-04-29 03:06:08.272096 pc_zap_scrapper-1.0.2rc0/PKG-INFO
+-rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)     3480 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2rc0/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-29 03:06:08.272096 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      756 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3184 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/__main__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       25 2023-04-29 03:06:03.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/_version.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-29 03:06:08.272096 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/datasets/
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-29 03:06:08.272096 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/datasets/external/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7696 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/datasets/external/neighbor_latlong.parquet
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1575 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/imoveis_db.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1231 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/load.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3478 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/maps.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1307 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/scrap.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6092 2023-04-29 03:02:38.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/transform.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2237 2023-04-29 03:02:49.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/utils.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-29 03:06:08.272096 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper.egg-info/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5447 2023-04-29 03:06:08.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      580 2023-04-29 03:06:08.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-29 03:06:08.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       58 2023-04-29 03:06:08.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper.egg-info/entry_points.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      278 2023-04-29 03:06:08.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       16 2023-04-29 03:06:08.000000 pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper.egg-info/top_level.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1895 2023-04-29 02:34:41.000000 pc_zap_scrapper-1.0.2rc0/pyproject.toml
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-29 03:06:08.272096 pc_zap_scrapper-1.0.2rc0/setup.cfg
```

### Comparing `pc_zap_scrapper-1.0.2.dev1/LICENSE` & `pc_zap_scrapper-1.0.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `pc_zap_scrapper-1.0.2.dev1/PKG-INFO` & `pc_zap_scrapper-1.0.2rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pc_zap_scrapper
-Version: 1.0.2.dev1
+Version: 1.0.2rc0
 Summary: Um template para começar o desenvolvimento de apps
 Author-email: Eduardo <emdemor415@gmail.com.br>
 License: Copyright (c) 2023, Eduardo Morais
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `pc_zap_scrapper-1.0.2.dev1/README.md` & `pc_zap_scrapper-1.0.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/__init__.py` & `pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/__main__.py` & `pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/datasets/external/neighbor_latlong.parquet` & `pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/datasets/external/neighbor_latlong.parquet`

 * *Files identical despite different names*

### Comparing `pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/imoveis_db.py` & `pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/imoveis_db.py`

 * *Files identical despite different names*

### Comparing `pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/load.py` & `pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/load.py`

 * *Files identical despite different names*

### Comparing `pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/maps.py` & `pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/maps.py`

 * *Files identical despite different names*

### Comparing `pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/scrap.py` & `pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/scrap.py`

 * *Files identical despite different names*

### Comparing `pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/transform.py` & `pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/transform.py`

 * *Files identical despite different names*

### Comparing `pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper/utils.py` & `pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper/utils.py`

 * *Files identical despite different names*

### Comparing `pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper.egg-info/PKG-INFO` & `pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pc-zap-scrapper
-Version: 1.0.2.dev1
+Version: 1.0.2rc0
 Summary: Um template para começar o desenvolvimento de apps
 Author-email: Eduardo <emdemor415@gmail.com.br>
 License: Copyright (c) 2023, Eduardo Morais
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `pc_zap_scrapper-1.0.2.dev1/pc_zap_scrapper.egg-info/SOURCES.txt` & `pc_zap_scrapper-1.0.2rc0/pc_zap_scrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pc_zap_scrapper-1.0.2.dev1/pyproject.toml` & `pc_zap_scrapper-1.0.2rc0/pyproject.toml`

 * *Files identical despite different names*


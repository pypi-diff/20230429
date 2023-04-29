# Comparing `tmp/MakePdfEasily-0.0.8.tar.gz` & `tmp/MakePdfEasily-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MakePdfEasily-0.0.8.tar", last modified: Wed Aug 10 15:06:52 2022, max compression
+gzip compressed data, was "MakePdfEasily-0.0.9.tar", last modified: Wed Aug 10 21:08:46 2022, max compression
```

## Comparing `MakePdfEasily-0.0.8.tar` & `MakePdfEasily-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-08-10 15:06:52.394272 MakePdfEasily-0.0.8/
--rw-rw-rw-   0        0        0     1091 2022-07-24 15:00:02.000000 MakePdfEasily-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2531 2022-08-10 15:06:52.393198 MakePdfEasily-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      761 2022-08-10 14:52:19.000000 MakePdfEasily-0.0.8/README.md
--rw-rw-rw-   0        0        0      644 2022-08-10 14:50:38.000000 MakePdfEasily-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-10 15:06:52.395206 MakePdfEasily-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-10 15:06:52.385219 MakePdfEasily-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-08-10 15:06:52.391192 MakePdfEasily-0.0.8/src/MakePdfEasily.egg-info/
--rw-rw-rw-   0        0        0     2531 2022-08-10 15:06:52.000000 MakePdfEasily-0.0.8/src/MakePdfEasily.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2022-08-10 15:06:52.000000 MakePdfEasily-0.0.8/src/MakePdfEasily.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-10 15:06:52.000000 MakePdfEasily-0.0.8/src/MakePdfEasily.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2022-08-10 15:06:52.000000 MakePdfEasily-0.0.8/src/MakePdfEasily.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1197 2022-08-10 14:48:20.000000 MakePdfEasily-0.0.8/src/MakePdfEasily.py
+drwxrwxrwx   0        0        0        0 2022-08-10 21:08:46.534237 MakePdfEasily-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2022-07-24 15:00:02.000000 MakePdfEasily-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2531 2022-08-10 21:08:46.533239 MakePdfEasily-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      761 2022-08-10 14:52:19.000000 MakePdfEasily-0.0.9/README.md
+-rw-rw-rw-   0        0        0      644 2022-08-10 20:56:29.000000 MakePdfEasily-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-08-10 21:08:46.534237 MakePdfEasily-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       96 2022-08-10 20:56:18.000000 MakePdfEasily-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-10 21:08:46.524275 MakePdfEasily-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-08-10 21:08:46.532239 MakePdfEasily-0.0.9/src/MakePdfEasily.egg-info/
+-rw-rw-rw-   0        0        0     2531 2022-08-10 21:08:46.000000 MakePdfEasily-0.0.9/src/MakePdfEasily.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2022-08-10 21:08:46.000000 MakePdfEasily-0.0.9/src/MakePdfEasily.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-10 21:08:46.000000 MakePdfEasily-0.0.9/src/MakePdfEasily.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2022-08-10 21:08:46.000000 MakePdfEasily-0.0.9/src/MakePdfEasily.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1197 2022-08-10 14:48:20.000000 MakePdfEasily-0.0.9/src/MakePdfEasily.py
```

### Comparing `MakePdfEasily-0.0.8/LICENSE` & `MakePdfEasily-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `MakePdfEasily-0.0.8/PKG-INFO` & `MakePdfEasily-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MakePdfEasily
-Version: 0.0.8
+Version: 0.0.9
 Summary: MakePdfEasily
 Author-email: MakePdfEasily <ali0088552211@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `MakePdfEasily-0.0.8/README.md` & `MakePdfEasily-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `MakePdfEasily-0.0.8/pyproject.toml` & `MakePdfEasily-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pyproject.toml
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel","pillow","PyPDF2"]
 
 [project]
 name = "MakePdfEasily"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="MakePdfEasily", email="ali0088552211@gmail.com" },
 ]
 description ="MakePdfEasily"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `MakePdfEasily-0.0.8/src/MakePdfEasily.egg-info/PKG-INFO` & `MakePdfEasily-0.0.9/src/MakePdfEasily.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MakePdfEasily
-Version: 0.0.8
+Version: 0.0.9
 Summary: MakePdfEasily
 Author-email: MakePdfEasily <ali0088552211@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `MakePdfEasily-0.0.8/src/MakePdfEasily.py` & `MakePdfEasily-0.0.9/src/MakePdfEasily.py`

 * *Files identical despite different names*


# Comparing `tmp/RubAmin-0.0.6.tar.gz` & `tmp/RubAmin-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RubAmin-0.0.6.tar", last modified: Sat Mar  4 22:37:36 2023, max compression
+gzip compressed data, was "RubAmin-0.1.0.tar", last modified: Sun Mar  5 20:36:08 2023, max compression
```

## Comparing `RubAmin-0.0.6.tar` & `RubAmin-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-04 22:37:36.425711 RubAmin-0.0.6/
--rw-rw-rw-   0        0        0     1089 2023-01-30 20:21:09.000000 RubAmin-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      518 2023-03-04 22:37:36.425711 RubAmin-0.0.6/PKG-INFO
--r--r--r--   0        0        0       28 2023-01-29 22:19:47.000000 RubAmin-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-03-04 22:37:36.410087 RubAmin-0.0.6/RubAmin/
--rw-rw-rw-   0        0        0      886 2023-03-04 22:12:51.000000 RubAmin-0.0.6/RubAmin/Socket.py
--rw-rw-rw-   0        0        0      117 2023-03-04 21:45:50.000000 RubAmin-0.0.6/RubAmin/__init__.py
--rw-rw-rw-   0        0        0      536 2023-03-04 21:53:09.000000 RubAmin-0.0.6/RubAmin/connections.py
--rw-rw-rw-   0        0        0     1434 2023-03-04 22:12:37.000000 RubAmin-0.0.6/RubAmin/createMethod.py
--rw-rw-rw-   0        0        0     1184 2022-08-26 10:37:26.000000 RubAmin-0.0.6/RubAmin/encryption.py
--rw-rw-rw-   0        0        0       54 2022-08-26 10:37:26.000000 RubAmin-0.0.6/RubAmin/login.py
--rw-rw-rw-   0        0        0      828 2022-08-26 10:37:26.000000 RubAmin-0.0.6/RubAmin/media.py
--rw-rw-rw-   0        0        0    25469 2023-03-04 22:02:37.000000 RubAmin-0.0.6/RubAmin/rubika.py
--rw-rw-rw-   0        0        0     1207 2023-03-04 22:23:01.000000 RubAmin-0.0.6/RubAmin/rubino.py
--rw-rw-rw-   0        0        0     1126 2023-03-04 22:16:41.000000 RubAmin-0.0.6/RubAmin/socket__init__.py
--rw-rw-rw-   0        0        0     1905 2022-08-26 10:37:26.000000 RubAmin-0.0.6/RubAmin/tools.py
-drwxrwxrwx   0        0        0        0 2023-03-04 22:37:36.425711 RubAmin-0.0.6/RubAmin.egg-info/
--rw-rw-rw-   0        0        0      518 2023-03-04 22:37:36.000000 RubAmin-0.0.6/RubAmin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-03-04 22:37:36.000000 RubAmin-0.0.6/RubAmin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-04 22:37:36.000000 RubAmin-0.0.6/RubAmin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-03-04 22:37:36.000000 RubAmin-0.0.6/RubAmin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-04 22:37:36.000000 RubAmin-0.0.6/RubAmin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-04 22:37:36.425711 RubAmin-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      780 2023-03-04 22:31:03.000000 RubAmin-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-05 20:36:08.426002 RubAmin-0.1.0/
+-rw-rw-rw-   0        0        0     1089 2023-01-30 20:21:09.000000 RubAmin-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      209 2023-03-05 20:36:08.426002 RubAmin-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-03-05 20:34:42.000000 RubAmin-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-03-05 20:36:08.414008 RubAmin-0.1.0/RubAmin/
+-rw-rw-rw-   0        0        0      886 2023-03-04 22:12:51.000000 RubAmin-0.1.0/RubAmin/Socket.py
+-rw-rw-rw-   0        0        0      117 2023-03-05 20:31:43.000000 RubAmin-0.1.0/RubAmin/__init__.py
+-rw-rw-rw-   0        0        0      536 2023-03-04 21:53:09.000000 RubAmin-0.1.0/RubAmin/connections.py
+-rw-rw-rw-   0        0        0     1434 2023-03-04 22:12:37.000000 RubAmin-0.1.0/RubAmin/createMethod.py
+-rw-rw-rw-   0        0        0     1184 2022-08-26 10:37:26.000000 RubAmin-0.1.0/RubAmin/encryption.py
+-rw-rw-rw-   0        0        0       54 2022-08-26 10:37:26.000000 RubAmin-0.1.0/RubAmin/login.py
+-rw-rw-rw-   0        0        0      828 2022-08-26 10:37:26.000000 RubAmin-0.1.0/RubAmin/media.py
+-rw-rw-rw-   0        0        0    25453 2023-03-05 20:32:35.000000 RubAmin-0.1.0/RubAmin/rubika.py
+-rw-rw-rw-   0        0        0     1200 2023-03-05 01:51:38.000000 RubAmin-0.1.0/RubAmin/rubino.py
+-rw-rw-rw-   0        0        0     1126 2023-03-04 22:16:41.000000 RubAmin-0.1.0/RubAmin/socket__init__.py
+-rw-rw-rw-   0        0        0     1905 2022-08-26 10:37:26.000000 RubAmin-0.1.0/RubAmin/tools.py
+drwxrwxrwx   0        0        0        0 2023-03-05 20:36:08.424001 RubAmin-0.1.0/RubAmin.egg-info/
+-rw-rw-rw-   0        0        0      209 2023-03-05 20:36:08.000000 RubAmin-0.1.0/RubAmin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-03-05 20:36:08.000000 RubAmin-0.1.0/RubAmin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-05 20:36:08.000000 RubAmin-0.1.0/RubAmin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-03-05 20:36:08.000000 RubAmin-0.1.0/RubAmin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-03-05 20:36:08.000000 RubAmin-0.1.0/RubAmin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-05 20:36:08.426002 RubAmin-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      438 2023-03-05 20:31:12.000000 RubAmin-0.1.0/setup.py
```

### Comparing `RubAmin-0.0.6/LICENSE` & `RubAmin-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RubAmin-0.0.6/RubAmin/Socket.py` & `RubAmin-0.1.0/RubAmin/Socket.py`

 * *Files identical despite different names*

### Comparing `RubAmin-0.0.6/RubAmin/connections.py` & `RubAmin-0.1.0/RubAmin/connections.py`

 * *Files identical despite different names*

### Comparing `RubAmin-0.0.6/RubAmin/createMethod.py` & `RubAmin-0.1.0/RubAmin/createMethod.py`

 * *Files identical despite different names*

### Comparing `RubAmin-0.0.6/RubAmin/encryption.py` & `RubAmin-0.1.0/RubAmin/encryption.py`

 * *Files identical despite different names*

### Comparing `RubAmin-0.0.6/RubAmin/media.py` & `RubAmin-0.1.0/RubAmin/media.py`

 * *Files identical despite different names*

### Comparing `RubAmin-0.0.6/RubAmin/rubika.py` & `RubAmin-0.1.0/RubAmin/rubika.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from time import sleep , time
 from .encryption import Encryption
-import connections
+from .import connections
 from json import dumps , loads
-from time import time
 from random import randint , choice
 from .createMethod import createMethod
 from .tools import Tools
 
-__version__ : str = '0.0.6'
+__version__ : str = '0.1.0'
 __author__ : str = 'Amin Tatality'
 
 class Rubika(object):
 	def __init__(self , auth : str , displayWelcome : bool = True) -> int:
 		if displayWelcome: 
 			text : str = f'This library was created by {__author__}, with versions {__version__} ...\n\n'
 			for char in text:
```

### Comparing `RubAmin-0.0.6/RubAmin/rubino.py` & `RubAmin-0.1.0/RubAmin/rubino.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from RubAmin import connections
+from .import connections
 from json import loads , dumps
 from .encryption import Encryption
 from random import choice
 from .createMethod import createMethod
 
 class Rubino(object):
 	def __init__(self , auth : str) -> int:
```

### Comparing `RubAmin-0.0.6/RubAmin/socket__init__.py` & `RubAmin-0.1.0/RubAmin/socket__init__.py`

 * *Files identical despite different names*

### Comparing `RubAmin-0.0.6/RubAmin/tools.py` & `RubAmin-0.1.0/RubAmin/tools.py`

 * *Files identical despite different names*


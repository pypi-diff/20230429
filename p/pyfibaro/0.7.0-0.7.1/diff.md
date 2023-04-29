# Comparing `tmp/pyfibaro-0.7.0.tar.gz` & `tmp/pyfibaro-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfibaro-0.7.0.tar", last modified: Sun Apr 16 17:16:07 2023, max compression
+gzip compressed data, was "pyfibaro-0.7.1.tar", last modified: Sat Apr 29 15:53:31 2023, max compression
```

## Comparing `pyfibaro-0.7.0.tar` & `pyfibaro-0.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:16:07.571606 pyfibaro-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-16 17:16:07.571606 pyfibaro-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:16:07.567606 pyfibaro-0.7.0/pyfibaro/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:16:07.567606 pyfibaro-0.7.0/pyfibaro/common/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/common/rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/fibaro_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/fibaro_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/fibaro_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/fibaro_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/fibaro_room.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/fibaro_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/fibaro_state_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:16:07.571606 pyfibaro-0.7.0/pyfibaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-16 17:16:06.000000 pyfibaro-0.7.0/pyfibaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-16 17:16:07.000000 pyfibaro-0.7.0/pyfibaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:16:06.000000 pyfibaro-0.7.0/pyfibaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-16 17:16:07.000000 pyfibaro-0.7.0/pyfibaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 17:16:07.000000 pyfibaro-0.7.0/pyfibaro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-16 17:16:07.571606 pyfibaro-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:53:31.286889 pyfibaro-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-29 15:53:08.000000 pyfibaro-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-29 15:53:31.286889 pyfibaro-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-29 15:53:08.000000 pyfibaro-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:53:31.282889 pyfibaro-0.7.1/pyfibaro/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-29 15:53:08.000000 pyfibaro-0.7.1/pyfibaro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:53:31.286889 pyfibaro-0.7.1/pyfibaro/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-29 15:53:08.000000 pyfibaro-0.7.1/pyfibaro/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-29 15:53:08.000000 pyfibaro-0.7.1/pyfibaro/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-29 15:53:08.000000 pyfibaro-0.7.1/pyfibaro/common/rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-29 15:53:08.000000 pyfibaro-0.7.1/pyfibaro/fibaro_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-04-29 15:53:08.000000 pyfibaro-0.7.1/pyfibaro/fibaro_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-29 15:53:08.000000 pyfibaro-0.7.1/pyfibaro/fibaro_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-29 15:53:08.000000 pyfibaro-0.7.1/pyfibaro/fibaro_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-29 15:53:08.000000 pyfibaro-0.7.1/pyfibaro/fibaro_room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-29 15:53:08.000000 pyfibaro-0.7.1/pyfibaro/fibaro_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-29 15:53:08.000000 pyfibaro-0.7.1/pyfibaro/fibaro_state_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:53:31.286889 pyfibaro-0.7.1/pyfibaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-29 15:53:30.000000 pyfibaro-0.7.1/pyfibaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-29 15:53:31.000000 pyfibaro-0.7.1/pyfibaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:53:30.000000 pyfibaro-0.7.1/pyfibaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 15:53:31.000000 pyfibaro-0.7.1/pyfibaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 15:53:31.000000 pyfibaro-0.7.1/pyfibaro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-29 15:53:08.000000 pyfibaro-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-29 15:53:31.286889 pyfibaro-0.7.1/setup.cfg
```

### Comparing `pyfibaro-0.7.0/LICENSE` & `pyfibaro-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.0/PKG-INFO` & `pyfibaro-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfibaro
-Version: 0.7.0
+Version: 0.7.1
 Summary: Simple API to access fibaro home center from any Python 3 script. Designed for Home Assistant (but not only)
 Home-page: https://github.com/rappenze/pyfibaro
 Author: Roman Appenzeller
 Author-email: 
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfibaro-0.7.0/README.md` & `pyfibaro-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.0/pyfibaro/common/const.py` & `pyfibaro-0.7.1/pyfibaro/common/const.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.0/pyfibaro/common/rest_client.py` & `pyfibaro-0.7.1/pyfibaro/common/rest_client.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.0/pyfibaro/fibaro_client.py` & `pyfibaro-0.7.1/pyfibaro/fibaro_client.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.0/pyfibaro/fibaro_device.py` & `pyfibaro-0.7.1/pyfibaro/fibaro_device.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.0/pyfibaro/fibaro_info.py` & `pyfibaro-0.7.1/pyfibaro/fibaro_info.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.0/pyfibaro/fibaro_room.py` & `pyfibaro-0.7.1/pyfibaro/fibaro_room.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.0/pyfibaro/fibaro_scene.py` & `pyfibaro-0.7.1/pyfibaro/fibaro_scene.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.0/pyfibaro/fibaro_state_handler.py` & `pyfibaro-0.7.1/pyfibaro/fibaro_state_handler.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.0/pyfibaro.egg-info/PKG-INFO` & `pyfibaro-0.7.1/pyfibaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfibaro
-Version: 0.7.0
+Version: 0.7.1
 Summary: Simple API to access fibaro home center from any Python 3 script. Designed for Home Assistant (but not only)
 Home-page: https://github.com/rappenze/pyfibaro
 Author: Roman Appenzeller
 Author-email: 
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfibaro-0.7.0/setup.cfg` & `pyfibaro-0.7.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyfibaro
-version = 0.7.0
+version = 0.7.1
 description = Simple API to access fibaro home center from any Python 3 script. Designed for Home Assistant (but not only)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rappenze/pyfibaro
 author = Roman Appenzeller
 author_email = 
 license = MIT
@@ -21,15 +21,15 @@
 	Topic :: Home Automation
 
 [options]
 packages = 
 	pyfibaro
 	pyfibaro.common
 install_requires = 
-	requests~=2.28.1
+	requests~=2.28
 python_requires = >=3.9
 include_package_data = True
 package_dir = 
 	=.
 
 [tool:pytest]
 testpaths =
```


# Comparing `tmp/microgue-1.0.8.tar.gz` & `tmp/microgue-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/microgue-1.0.8.tar", last modified: Fri Dec 30 17:37:20 2022, max compression
+gzip compressed data, was "dist/microgue-1.0.9.tar", last modified: Sat Apr 29 02:01:29 2023, max compression
```

## Comparing `microgue-1.0.8.tar` & `microgue-1.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2022-12-30 17:37:20.000000 microgue-1.0.8/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3017 2022-12-30 17:37:20.000000 microgue-1.0.8/PKG-INFO
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2022-12-30 17:37:20.000000 microgue-1.0.8/microgue/
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2022-12-30 17:37:20.000000 microgue-1.0.8/microgue/storages/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.8/microgue/storages/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     3371 2022-09-23 01:04:52.000000 microgue-1.0.8/microgue/storages/abstract_storage.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2022-12-30 17:37:20.000000 microgue-1.0.8/microgue/loggers/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.8/microgue/loggers/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1244 2022-09-23 01:14:53.000000 microgue-1.0.8/microgue/loggers/logger.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2022-12-30 17:37:20.000000 microgue-1.0.8/microgue/security/
--rw-r--r--   0 mhudelso   (501) staff       (20)      343 2022-09-21 19:42:33.000000 microgue-1.0.8/microgue/security/generic.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.8/microgue/security/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2022-12-30 17:37:20.000000 microgue-1.0.8/microgue/secrets/
--rw-r--r--   0 mhudelso   (501) staff       (20)      175 2022-09-21 19:42:32.000000 microgue-1.0.8/microgue/secrets/secrets_without_logging.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.8/microgue/secrets/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1213 2022-09-21 19:42:32.000000 microgue-1.0.8/microgue/secrets/secrets.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2022-12-30 17:37:20.000000 microgue-1.0.8/microgue/constants/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.8/microgue/constants/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)      378 2022-09-21 19:29:50.000000 microgue-1.0.8/microgue/constants/error_constants.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.8/microgue/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2022-12-30 17:37:20.000000 microgue-1.0.8/microgue/objects/
--rw-r--r--   0 mhudelso   (501) staff       (20)     8636 2022-09-23 01:14:06.000000 microgue-1.0.8/microgue/objects/abstract_model_object.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     2374 2022-09-23 00:54:22.000000 microgue-1.0.8/microgue/objects/object.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.8/microgue/objects/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1458 2022-09-23 00:49:49.000000 microgue-1.0.8/microgue/objects/abstract_expiring_model_object.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2022-12-30 17:37:20.000000 microgue-1.0.8/microgue/models/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.8/microgue/models/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)    10587 2022-09-23 00:48:36.000000 microgue-1.0.8/microgue/models/abstract_model.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     2682 2022-12-09 19:59:12.000000 microgue-1.0.8/microgue/utils.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2022-12-30 17:37:20.000000 microgue-1.0.8/microgue/queues/
--rw-r--r--   0 mhudelso   (501) staff       (20)     2908 2022-09-23 01:15:31.000000 microgue-1.0.8/microgue/queues/abstract_queue.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.8/microgue/queues/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2022-12-30 17:37:20.000000 microgue-1.0.8/microgue/events/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-03-09 20:40:18.000000 microgue-1.0.8/microgue/events/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1442 2022-09-22 23:03:47.000000 microgue-1.0.8/microgue/events/abstract_event_bus.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     5526 2022-12-30 17:34:34.000000 microgue-1.0.8/microgue/abstract_app.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2022-12-30 17:37:20.000000 microgue-1.0.8/microgue/services/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3317 2022-12-19 21:35:09.000000 microgue-1.0.8/microgue/services/service.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.8/microgue/services/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2022-12-30 17:37:20.000000 microgue-1.0.8/microgue/caches/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3043 2022-09-21 19:29:03.000000 microgue-1.0.8/microgue/caches/abstract_cache.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.8/microgue/caches/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1907 2022-09-27 19:27:36.000000 microgue-1.0.8/README.md
--rw-r--r--   0 mhudelso   (501) staff       (20)      597 2022-12-30 17:35:33.000000 microgue-1.0.8/setup.py
--rw-r--r--   0 mhudelso   (501) staff       (20)       38 2022-12-30 17:37:20.000000 microgue-1.0.8/setup.cfg
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2022-12-30 17:37:20.000000 microgue-1.0.8/microgue.egg-info/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3017 2022-12-30 17:37:19.000000 microgue-1.0.8/microgue.egg-info/PKG-INFO
--rw-r--r--   0 mhudelso   (501) staff       (20)     1054 2022-12-30 17:37:19.000000 microgue-1.0.8/microgue.egg-info/SOURCES.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)       42 2022-12-30 17:37:19.000000 microgue-1.0.8/microgue.egg-info/requires.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)        9 2022-12-30 17:37:19.000000 microgue-1.0.8/microgue.egg-info/top_level.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)        1 2022-12-30 17:37:19.000000 microgue-1.0.8/microgue.egg-info/dependency_links.txt
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3017 2023-04-29 02:01:29.000000 microgue-1.0.9/PKG-INFO
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/storages/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/storages/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3371 2022-09-23 01:04:52.000000 microgue-1.0.9/microgue/storages/abstract_storage.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/loggers/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/loggers/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1713 2023-04-29 01:51:16.000000 microgue-1.0.9/microgue/loggers/logger.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/security/
+-rw-r--r--   0 mhudelso   (501) staff       (20)      343 2022-09-21 19:42:33.000000 microgue-1.0.9/microgue/security/generic.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/security/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/secrets/
+-rw-r--r--   0 mhudelso   (501) staff       (20)      175 2022-09-21 19:42:32.000000 microgue-1.0.9/microgue/secrets/secrets_without_logging.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/secrets/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1213 2022-09-21 19:42:32.000000 microgue-1.0.9/microgue/secrets/secrets.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/constants/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/constants/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)      378 2022-09-21 19:29:50.000000 microgue-1.0.9/microgue/constants/error_constants.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/objects/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     8636 2022-09-23 01:14:06.000000 microgue-1.0.9/microgue/objects/abstract_model_object.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     2374 2022-09-23 00:54:22.000000 microgue-1.0.9/microgue/objects/object.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/objects/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1458 2022-09-23 00:49:49.000000 microgue-1.0.9/microgue/objects/abstract_expiring_model_object.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/models/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/models/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)    10587 2022-09-23 00:48:36.000000 microgue-1.0.9/microgue/models/abstract_model.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     2682 2022-12-09 19:59:12.000000 microgue-1.0.9/microgue/utils.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/queues/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     2908 2022-09-23 01:15:31.000000 microgue-1.0.9/microgue/queues/abstract_queue.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/queues/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/events/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-03-09 20:40:18.000000 microgue-1.0.9/microgue/events/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1442 2022-09-22 23:03:47.000000 microgue-1.0.9/microgue/events/abstract_event_bus.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     5526 2022-12-30 17:34:34.000000 microgue-1.0.9/microgue/abstract_app.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/services/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3317 2022-12-19 21:35:09.000000 microgue-1.0.9/microgue/services/service.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/services/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/caches/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3043 2022-09-21 19:29:03.000000 microgue-1.0.9/microgue/caches/abstract_cache.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/caches/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1907 2022-09-27 19:27:36.000000 microgue-1.0.9/README.md
+-rw-r--r--   0 mhudelso   (501) staff       (20)      597 2023-04-29 01:59:45.000000 microgue-1.0.9/setup.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)       38 2023-04-29 02:01:29.000000 microgue-1.0.9/setup.cfg
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue.egg-info/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3017 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue.egg-info/PKG-INFO
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1054 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue.egg-info/SOURCES.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)       42 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue.egg-info/requires.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)        9 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue.egg-info/top_level.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)        1 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue.egg-info/dependency_links.txt
```

### Comparing `microgue-1.0.8/PKG-INFO` & `microgue-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microgue
-Version: 1.0.8
+Version: 1.0.9
 Summary: Quickly spin up microservices in AWS using flask
 Home-page: UNKNOWN
 Author: Michael Hudelson
 Author-email: michaelhudelson@gmail.com
 License: MIT
 Description: # AWS Microservice Bootstrap Code
```

### Comparing `microgue-1.0.8/microgue/storages/abstract_storage.py` & `microgue-1.0.9/microgue/storages/abstract_storage.py`

 * *Files identical despite different names*

### Comparing `microgue-1.0.8/microgue/secrets/secrets.py` & `microgue-1.0.9/microgue/secrets/secrets.py`

 * *Files identical despite different names*

### Comparing `microgue-1.0.8/microgue/objects/abstract_model_object.py` & `microgue-1.0.9/microgue/objects/abstract_model_object.py`

 * *Files identical despite different names*

### Comparing `microgue-1.0.8/microgue/objects/object.py` & `microgue-1.0.9/microgue/objects/object.py`

 * *Files identical despite different names*

### Comparing `microgue-1.0.8/microgue/objects/abstract_expiring_model_object.py` & `microgue-1.0.9/microgue/objects/abstract_expiring_model_object.py`

 * *Files identical despite different names*

### Comparing `microgue-1.0.8/microgue/models/abstract_model.py` & `microgue-1.0.9/microgue/models/abstract_model.py`

 * *Files identical despite different names*

### Comparing `microgue-1.0.8/microgue/utils.py` & `microgue-1.0.9/microgue/utils.py`

 * *Files identical despite different names*

### Comparing `microgue-1.0.8/microgue/queues/abstract_queue.py` & `microgue-1.0.9/microgue/queues/abstract_queue.py`

 * *Files identical despite different names*

### Comparing `microgue-1.0.8/microgue/events/abstract_event_bus.py` & `microgue-1.0.9/microgue/events/abstract_event_bus.py`

 * *Files identical despite different names*

### Comparing `microgue-1.0.8/microgue/abstract_app.py` & `microgue-1.0.9/microgue/abstract_app.py`

 * *Files identical despite different names*

### Comparing `microgue-1.0.8/microgue/services/service.py` & `microgue-1.0.9/microgue/services/service.py`

 * *Files identical despite different names*

### Comparing `microgue-1.0.8/microgue/caches/abstract_cache.py` & `microgue-1.0.9/microgue/caches/abstract_cache.py`

 * *Files identical despite different names*

### Comparing `microgue-1.0.8/README.md` & `microgue-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `microgue-1.0.8/setup.py` & `microgue-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="microgue",
-    version="1.0.8",
+    version="1.0.9",
     author="Michael Hudelson",
     author_email="michaelhudelson@gmail.com",
     description="Quickly spin up microservices in AWS using flask",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     packages=find_packages(),
```

### Comparing `microgue-1.0.8/microgue.egg-info/PKG-INFO` & `microgue-1.0.9/microgue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microgue
-Version: 1.0.8
+Version: 1.0.9
 Summary: Quickly spin up microservices in AWS using flask
 Home-page: UNKNOWN
 Author: Michael Hudelson
 Author-email: michaelhudelson@gmail.com
 License: MIT
 Description: # AWS Microservice Bootstrap Code
```

### Comparing `microgue-1.0.8/microgue.egg-info/SOURCES.txt` & `microgue-1.0.9/microgue.egg-info/SOURCES.txt`

 * *Files identical despite different names*


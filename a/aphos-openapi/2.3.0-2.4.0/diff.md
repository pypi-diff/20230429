# Comparing `tmp/aphos_openapi-2.3.0.tar.gz` & `tmp/aphos_openapi-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aphos_openapi-2.3.0.tar", last modified: Wed Apr 26 21:49:45 2023, max compression
+gzip compressed data, was "aphos_openapi-2.4.0.tar", last modified: Fri Apr 28 23:12:07 2023, max compression
```

## Comparing `aphos_openapi-2.3.0.tar` & `aphos_openapi-2.4.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:49:45.614952 aphos_openapi-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15581 2023-04-26 21:49:45.614952 aphos_openapi-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15207 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:49:45.606952 aphos_openapi-2.3.0/aphos_openapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/aphos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:49:45.610952 aphos_openapi-2.3.0/aphos_openapi/api/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/api/catalog_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/api/flux_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25236 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/api/space_object_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39091 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:49:45.610952 aphos_openapi-2.3.0/aphos_openapi/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:49:45.614952 aphos_openapi-2.3.0/aphos_openapi/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/model/comparison_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/model/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/model/flux.py
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/model/flux_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/model/night.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/model/photo_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/model/space_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/model/space_object_with_fluxes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    82630 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:49:45.614952 aphos_openapi-2.3.0/aphos_openapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/models/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    14718 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/models/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/aphos_openapi/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:49:45.606952 aphos_openapi-2.3.0/aphos_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15581 2023-04-26 21:49:45.000000 aphos_openapi-2.3.0/aphos_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-26 21:49:45.000000 aphos_openapi-2.3.0/aphos_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:49:45.000000 aphos_openapi-2.3.0/aphos_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 21:49:45.000000 aphos_openapi-2.3.0/aphos_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 21:49:45.000000 aphos_openapi-2.3.0/aphos_openapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:49:45.614952 aphos_openapi-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-26 21:49:19.000000 aphos_openapi-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:12:07.576025 aphos_openapi-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15593 2023-04-28 23:12:07.576025 aphos_openapi-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:12:07.572024 aphos_openapi-2.4.0/aphos_openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/aphos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:12:07.572024 aphos_openapi-2.4.0/aphos_openapi/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/api/catalog_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/api/flux_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25235 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/api/space_object_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39091 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:12:07.576025 aphos_openapi-2.4.0/aphos_openapi/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:12:07.576025 aphos_openapi-2.4.0/aphos_openapi/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/comparison_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/flux_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/night.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/photo_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/space_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/space_object_with_fluxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82630 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:12:07.576025 aphos_openapi-2.4.0/aphos_openapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/models/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14718 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/models/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:12:07.572024 aphos_openapi-2.4.0/aphos_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15593 2023-04-28 23:12:07.000000 aphos_openapi-2.4.0/aphos_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-28 23:12:07.000000 aphos_openapi-2.4.0/aphos_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:12:07.000000 aphos_openapi-2.4.0/aphos_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 23:12:07.000000 aphos_openapi-2.4.0/aphos_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 23:12:07.000000 aphos_openapi-2.4.0/aphos_openapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:12:07.576025 aphos_openapi-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/setup.py
```

### Comparing `aphos_openapi-2.3.0/LICENSE` & `aphos_openapi-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/PKG-INFO` & `aphos_openapi-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: aphos_openapi
-Version: 2.3.0
+Version: 2.4.0
 Summary: APhoS Python library for data representation
 Author: Pavel Kinc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # APhoS client for retrieving data in Python
 
-This is Amateur Photometric Survey (APhoS) Application Programming Interface.  
-Contains models and functions for work with data in APhoS database.  
+This is Amateur Photometric Survey (APhoS) client for web application.  
+Contains documentation about modules, models and functions for working with astronomical data from APhoS database.  
 Server is accessible from: https://ip-147-251-21-104.flt.cloud.muni.cz/  
 Swagger UI (Interface for api of the server): https://ip-147-251-21-104.flt.cloud.muni.cz/swagger-ui/index.html  
 Openapi json or yaml file (documentation of api): https://ip-147-251-21-104.flt.cloud.muni.cz/api-docs
 
 ## Installation
 ### Package: `aphos_openapi`
 
@@ -30,16 +30,16 @@
 * [Basic info](README.md#aphos-client-for-retrieving-data-in-python)
 * [Installation](README.md#installation)
 * [Requirements](README.md#requirements)
 * [Basic usage](README.md#usage-api-models)
 * [Coordinates usage](README.md#usage-coordinates)
 * [GraphData usage](README.md#usage-graphdata)
 * [Support](README.md#support)
-* [Functions documentation](README.md#documentation-for-functions)
-* [Api models documentation](README.md#documentation-for-models)
+* [Functions](README.md#documentation-for-functions)
+* [Api models](README.md#documentation-for-models)
 
 
 ## Requirements
 
 * Python >=3.8,
 * 'urllib3'>=1.25.3,
 * 'python-dateutil',
```

### Comparing `aphos_openapi-2.3.0/README.md` & `aphos_openapi-2.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # APhoS client for retrieving data in Python
 
-This is Amateur Photometric Survey (APhoS) Application Programming Interface.  
-Contains models and functions for work with data in APhoS database.  
+This is Amateur Photometric Survey (APhoS) client for web application.  
+Contains documentation about modules, models and functions for working with astronomical data from APhoS database.  
 Server is accessible from: https://ip-147-251-21-104.flt.cloud.muni.cz/  
 Swagger UI (Interface for api of the server): https://ip-147-251-21-104.flt.cloud.muni.cz/swagger-ui/index.html  
 Openapi json or yaml file (documentation of api): https://ip-147-251-21-104.flt.cloud.muni.cz/api-docs
 
 ## Installation
 ### Package: `aphos_openapi`
 
@@ -18,16 +18,16 @@
 * [Basic info](README.md#aphos-client-for-retrieving-data-in-python)
 * [Installation](README.md#installation)
 * [Requirements](README.md#requirements)
 * [Basic usage](README.md#usage-api-models)
 * [Coordinates usage](README.md#usage-coordinates)
 * [GraphData usage](README.md#usage-graphdata)
 * [Support](README.md#support)
-* [Functions documentation](README.md#documentation-for-functions)
-* [Api models documentation](README.md#documentation-for-models)
+* [Functions](README.md#documentation-for-functions)
+* [Api models](README.md#documentation-for-models)
 
 
 ## Requirements
 
 * Python >=3.8,
 * 'urllib3'>=1.25.3,
 * 'python-dateutil',
```

### Comparing `aphos_openapi-2.3.0/aphos_openapi/__init__.py` & `aphos_openapi-2.4.0/aphos_openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/aphos.py` & `aphos_openapi-2.4.0/aphos_openapi/aphos.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/api/catalog_api.py` & `aphos_openapi-2.4.0/aphos_openapi/api/catalog_api.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/api/flux_api.py` & `aphos_openapi-2.4.0/aphos_openapi/api/flux_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             },
             api_client=api_client
         )
         self.get_space_object_by_id_endpoint = _Endpoint(
             settings={
                 'response_type': (SpaceObjectWithFluxes,),
                 'auth': [],
-                'endpoint_path': '/api/space-objects/find',
+                'endpoint_path': '/api/space-objects/search',
                 'operation_id': 'get_space_object_by_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'space_object_id',
@@ -180,15 +180,15 @@
             },
             api_client=api_client
         )
         self.upload_csv_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [],
-                'endpoint_path': '/api/space-objects/upload-file',
+                'endpoint_path': '/api/space-objects/upload',
                 'operation_id': 'upload_csv',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'file',
```

### Comparing `aphos_openapi-2.3.0/aphos_openapi/api/space_object_api.py` & `aphos_openapi-2.4.0/aphos_openapi/api/space_object_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
         self.find_space_objects_by_params_endpoint = _Endpoint(
             settings={
                 'response_type': ([SpaceObject],),
                 'auth': [],
-                'endpoint_path': '/api/space-objects/find-by-params',
+                'endpoint_path': '/api/space-objects/search-by-params',
                 'operation_id': 'find_space_objects_by_params',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'object_id',
@@ -207,15 +207,15 @@
             },
             api_client=api_client
         )
         self.get_space_object_by_id_endpoint = _Endpoint(
             settings={
                 'response_type': (SpaceObjectWithFluxes,),
                 'auth': [],
-                'endpoint_path': '/api/space-objects/find',
+                'endpoint_path': '/api/space-objects/search',
                 'operation_id': 'get_space_object_by_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'space_object_id',
@@ -268,15 +268,15 @@
             },
             api_client=api_client
         )
         self.upload_csv_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [],
-                'endpoint_path': '/api/space-objects/upload-file',
+                'endpoint_path': '/api/space-objects/upload',
                 'operation_id': 'upload_csv',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'file',
```

### Comparing `aphos_openapi-2.3.0/aphos_openapi/api/user_api.py` & `aphos_openapi-2.4.0/aphos_openapi/api/user_api.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/api_client.py` & `aphos_openapi-2.4.0/aphos_openapi/api_client.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/apis/__init__.py` & `aphos_openapi-2.4.0/aphos_openapi/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/configuration.py` & `aphos_openapi-2.4.0/aphos_openapi/configuration.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/exceptions.py` & `aphos_openapi-2.4.0/aphos_openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/model/comparison_object.py` & `aphos_openapi-2.4.0/aphos_openapi/model/comparison_object.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/model/error_message.py` & `aphos_openapi-2.4.0/aphos_openapi/model/error_message.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/model/flux.py` & `aphos_openapi-2.4.0/aphos_openapi/model/flux.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/model/flux_data.py` & `aphos_openapi-2.4.0/aphos_openapi/model/flux_data.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/model/night.py` & `aphos_openapi-2.4.0/aphos_openapi/model/night.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/model/photo_properties.py` & `aphos_openapi-2.4.0/aphos_openapi/model/photo_properties.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/model/space_object.py` & `aphos_openapi-2.4.0/aphos_openapi/model/space_object.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/model/space_object_with_fluxes.py` & `aphos_openapi-2.4.0/aphos_openapi/model/space_object_with_fluxes.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/model/user.py` & `aphos_openapi-2.4.0/aphos_openapi/model/user.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/model_utils.py` & `aphos_openapi-2.4.0/aphos_openapi/model_utils.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/models/__init__.py` & `aphos_openapi-2.4.0/aphos_openapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/models/coordinates.py` & `aphos_openapi-2.4.0/aphos_openapi/models/coordinates.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/models/graph_data.py` & `aphos_openapi-2.4.0/aphos_openapi/models/graph_data.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi/rest.py` & `aphos_openapi-2.4.0/aphos_openapi/rest.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/aphos_openapi.egg-info/PKG-INFO` & `aphos_openapi-2.4.0/aphos_openapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: aphos-openapi
-Version: 2.3.0
+Version: 2.4.0
 Summary: APhoS Python library for data representation
 Author: Pavel Kinc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # APhoS client for retrieving data in Python
 
-This is Amateur Photometric Survey (APhoS) Application Programming Interface.  
-Contains models and functions for work with data in APhoS database.  
+This is Amateur Photometric Survey (APhoS) client for web application.  
+Contains documentation about modules, models and functions for working with astronomical data from APhoS database.  
 Server is accessible from: https://ip-147-251-21-104.flt.cloud.muni.cz/  
 Swagger UI (Interface for api of the server): https://ip-147-251-21-104.flt.cloud.muni.cz/swagger-ui/index.html  
 Openapi json or yaml file (documentation of api): https://ip-147-251-21-104.flt.cloud.muni.cz/api-docs
 
 ## Installation
 ### Package: `aphos_openapi`
 
@@ -30,16 +30,16 @@
 * [Basic info](README.md#aphos-client-for-retrieving-data-in-python)
 * [Installation](README.md#installation)
 * [Requirements](README.md#requirements)
 * [Basic usage](README.md#usage-api-models)
 * [Coordinates usage](README.md#usage-coordinates)
 * [GraphData usage](README.md#usage-graphdata)
 * [Support](README.md#support)
-* [Functions documentation](README.md#documentation-for-functions)
-* [Api models documentation](README.md#documentation-for-models)
+* [Functions](README.md#documentation-for-functions)
+* [Api models](README.md#documentation-for-models)
 
 
 ## Requirements
 
 * Python >=3.8,
 * 'urllib3'>=1.25.3,
 * 'python-dateutil',
```

### Comparing `aphos_openapi-2.3.0/aphos_openapi.egg-info/SOURCES.txt` & `aphos_openapi-2.4.0/aphos_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.3.0/setup.py` & `aphos_openapi-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aphos_openapi",
-    version="2.3.0",
+    version="2.4.0",
     author="Pavel Kinc",
     description="APhoS Python library for data representation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
     license_files=('LICENSE',),
     classifiers=[
```


# Comparing `tmp/caveclient-5.3.2.tar.gz` & `tmp/caveclient-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caveclient-5.3.2.tar", last modified: Wed Apr 26 19:29:51 2023, max compression
+gzip compressed data, was "caveclient-5.4.0.tar", last modified: Sat Apr 29 14:23:38 2023, max compression
```

## Comparing `caveclient-5.3.2.tar` & `caveclient-5.4.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-26 19:29:51.863571 caveclient-5.3.2/
--rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.3.2/MANIFEST.in
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-26 19:29:51.863273 caveclient-5.3.2/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.3.2/README.rst
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-26 19:29:51.855492 caveclient-5.3.2/caveclient/
--rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-04-26 19:29:48.000000 caveclient-5.3.2/caveclient/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.3.2/caveclient/annotationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.3.2/caveclient/auth.py
--rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.3.2/caveclient/base.py
--rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-04-23 20:02:55.000000 caveclient-5.3.2/caveclient/chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.3.2/caveclient/datastack_lookup.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.3.2/caveclient/emannotationschemas.py
--rw-r--r--   0 forrestc   (503) staff       (20)    10725 2023-04-26 13:55:48.000000 caveclient-5.3.2/caveclient/endpoints.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1810 2023-04-23 20:02:55.000000 caveclient-5.3.2/caveclient/format_utils.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.3.2/caveclient/frameworkclient.py
--rw-r--r--   0 forrestc   (503) staff       (20)    16395 2023-02-09 16:57:03.000000 caveclient-5.3.2/caveclient/infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.3.2/caveclient/jsonservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-04-23 20:02:55.000000 caveclient-5.3.2/caveclient/l2cache.py
--rw-r--r--   0 forrestc   (503) staff       (20)    85648 2023-04-26 19:29:25.000000 caveclient-5.3.2/caveclient/materializationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.3.2/caveclient/session_config.py
--rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.3.2/caveclient/timeit.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-26 19:29:51.857914 caveclient-5.3.2/caveclient/tools/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.3.2/caveclient/tools/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.3.2/caveclient/tools/caching.py
--rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.3.2/caveclient/tools/stage.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-26 19:29:51.857101 caveclient-5.3.2/caveclient.egg-info/
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-26 19:29:51.000000 caveclient-5.3.2/caveclient.egg-info/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-04-26 19:29:51.000000 caveclient-5.3.2/caveclient.egg-info/SOURCES.txt
--rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-04-26 19:29:51.000000 caveclient-5.3.2/caveclient.egg-info/dependency_links.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      115 2023-04-26 19:29:51.000000 caveclient-5.3.2/caveclient.egg-info/requires.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-04-26 19:29:51.000000 caveclient-5.3.2/caveclient.egg-info/top_level.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      114 2022-12-21 20:12:16.000000 caveclient-5.3.2/requirements.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-04-26 19:29:51.863638 caveclient-5.3.2/setup.cfg
--rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.3.2/setup.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-26 19:29:51.860978 caveclient-5.3.2/tests/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.3.2/tests/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.3.2/tests/conftest.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.3.2/tests/test_annotation.py
--rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.3.2/tests/test_chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.3.2/tests/test_infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.3.2/tests/test_materialization.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-29 14:23:38.256892 caveclient-5.4.0/
+-rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.4.0/MANIFEST.in
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-29 14:23:38.256600 caveclient-5.4.0/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.4.0/README.rst
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-29 14:23:38.241451 caveclient-5.4.0/caveclient/
+-rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-04-29 14:23:34.000000 caveclient-5.4.0/caveclient/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.4.0/caveclient/annotationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.4.0/caveclient/auth.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.4.0/caveclient/base.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-04-23 20:02:55.000000 caveclient-5.4.0/caveclient/chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.4.0/caveclient/datastack_lookup.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.4.0/caveclient/emannotationschemas.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11066 2023-04-29 14:05:03.000000 caveclient-5.4.0/caveclient/endpoints.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1810 2023-04-23 20:02:55.000000 caveclient-5.4.0/caveclient/format_utils.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.4.0/caveclient/frameworkclient.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    16395 2023-02-09 16:57:03.000000 caveclient-5.4.0/caveclient/infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.4.0/caveclient/jsonservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-04-23 20:02:55.000000 caveclient-5.4.0/caveclient/l2cache.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    90340 2023-04-29 14:05:03.000000 caveclient-5.4.0/caveclient/materializationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.4.0/caveclient/session_config.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.4.0/caveclient/timeit.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-29 14:23:38.248552 caveclient-5.4.0/caveclient/tools/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.4.0/caveclient/tools/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.4.0/caveclient/tools/caching.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.4.0/caveclient/tools/stage.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-29 14:23:38.247560 caveclient-5.4.0/caveclient.egg-info/
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-29 14:23:38.000000 caveclient-5.4.0/caveclient.egg-info/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-04-29 14:23:38.000000 caveclient-5.4.0/caveclient.egg-info/SOURCES.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-04-29 14:23:38.000000 caveclient-5.4.0/caveclient.egg-info/dependency_links.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      115 2023-04-29 14:23:38.000000 caveclient-5.4.0/caveclient.egg-info/requires.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-04-29 14:23:38.000000 caveclient-5.4.0/caveclient.egg-info/top_level.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      114 2022-12-21 20:12:16.000000 caveclient-5.4.0/requirements.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-04-29 14:23:38.256960 caveclient-5.4.0/setup.cfg
+-rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.4.0/setup.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-29 14:23:38.255190 caveclient-5.4.0/tests/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.4.0/tests/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.4.0/tests/conftest.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.4.0/tests/test_annotation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.4.0/tests/test_chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.4.0/tests/test_infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.4.0/tests/test_materialization.py
```

### Comparing `caveclient-5.3.2/README.rst` & `caveclient-5.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/annotationengine.py` & `caveclient-5.4.0/caveclient/annotationengine.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/auth.py` & `caveclient-5.4.0/caveclient/auth.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/base.py` & `caveclient-5.4.0/caveclient/base.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/chunkedgraph.py` & `caveclient-5.4.0/caveclient/chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/datastack_lookup.py` & `caveclient-5.4.0/caveclient/datastack_lookup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/emannotationschemas.py` & `caveclient-5.4.0/caveclient/emannotationschemas.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/endpoints.py` & `caveclient-5.4.0/caveclient/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,28 +60,35 @@
     + "/datastack/{datastack_name}/version/{version}/table/{table_name}/query",
     "join_query": mat_v3_api + "/datastack/{datastack_name}/version/{version}/query",
     "table_count": mat_v2_api
     + "/datastack/{datastack_name}/version/{version}/table/{table_name}/count",
     "versions": mat_v2_api + "/datastack/{datastack_name}/versions",
     "version_metadata": mat_v2_api + "/datastack/{datastack_name}/version/{version}",
     "tables": mat_v2_api + "/datastack/{datastack_name}/version/{version}/tables",
-    "metadata": mat_v2_api
+    "metadata": mat_v3_api
     + "/datastack/{datastack_name}/version/{version}/table/{table_name}/metadata",
+    "all_tables_metadata": mat_v3_api
+    + "/datastack/{datastack_name}/version/{version}/tables/metadata",
     "versions_metadata": mat_v2_api + "/datastack/{datastack_name}/metadata",
     "ingest_annotation_table": mat_v2_api
     + "/materialize/run/ingest_annotations/datastack/{datastack_name}/{table_name}",
     "segmentation_metadata": mat_v3_api
     + "/datastack/{datastack_name}/table/{table_name}/segmentation_metadata",
     "live_live_query": mat_v3_api + "/datastack/{datastack_name}/query",
     "lookup_supervoxel_ids": mat_v2_api
     + "/materialize/run/lookup_svid/datastack/{datastack_name}/{table_name}",
     "get_views": mat_v3_api + "/datastack/{datastack_name}/version/{version}/views",
-    "get_view_metadata": mat_v3_api + "/datastack/{datastack_name}/views/{view_name}/metadata",
+    "get_view_metadata": mat_v3_api
+    + "/datastack/{datastack_name}/version/{version}/views/{view_name}/metadata",
     "view_query": mat_v3_api
     + "/datastack/{datastack_name}/version/{version}/views/{view_name}/query",
+    "view_schema": mat_v3_api
+    + "/datastack/{datastack_name}/version/{version}/views/{view_name}/schema",
+    "view_schemas": mat_v3_api
+    + "/datastack/{datastack_name}/version/{version}/views/schemas",
 }
 
 materialization_api_versions = {
     2: materialization_endpoints_v2,
     3: materialization_endpoints_v3,
 }
```

### Comparing `caveclient-5.3.2/caveclient/format_utils.py` & `caveclient-5.4.0/caveclient/format_utils.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/frameworkclient.py` & `caveclient-5.4.0/caveclient/frameworkclient.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/infoservice.py` & `caveclient-5.4.0/caveclient/infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/jsonservice.py` & `caveclient-5.4.0/caveclient/jsonservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/l2cache.py` & `caveclient-5.4.0/caveclient/l2cache.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/materializationengine.py` & `caveclient-5.4.0/caveclient/materializationengine.py`

 * *Files 2% similar despite different names*

```diff
@@ -401,14 +401,15 @@
         response = self.session.get(url)
         d = handle_response(response)
         for md in d:
             md["time_stamp"] = convert_timestamp(md["time_stamp"])
             md["expires_on"] = convert_timestamp(md["expires_on"])
         return d
 
+    
     @cached(cache=TTLCache(maxsize=100, ttl=60 * 60 * 12))
     def get_table_metadata(
         self,
         table_name: str,
         datastack_name=None,
         version: int = None,
         log_warning: bool = True,
@@ -1668,14 +1669,55 @@
         return attrs
 
 
 class MaterializatonClientV3(MaterializatonClientV2):
     def __init__(self, *args, **kwargs):
         super(MaterializatonClientV3, self).__init__(*args, **kwargs)
 
+    @cached(cache=TTLCache(maxsize=100, ttl=60 * 60 * 12))
+    def get_tables_metadata(
+        self,
+        datastack_name=None,
+        version: int = None,
+        log_warning: bool = True,
+    ):
+        """Get metadata about a table
+
+        Args:
+            datastack_name: str or None, optional,
+                Name of the datastack_name.
+                If None, uses the one specified in the client.
+            version (int, optional):
+                version to get. If None, uses the one specified in the client.
+            log_warning (bool, optional):
+                whether to print out warnings to the logger.
+                Defaults to True.
+
+        Returns:
+            dict: metadata dictionary for table
+        """
+        if datastack_name is None:
+            datastack_name = self.datastack_name
+        if version is None:
+            version = self.version
+        endpoint_mapping = self.default_url_mapping
+        endpoint_mapping["datastack_name"] = datastack_name
+        endpoint_mapping["version"] = version
+
+        url = self._endpoints["all_tables_metadata"].format_map(endpoint_mapping)
+
+        response = self.session.get(url)
+        all_metadata = handle_response(response, log_warning=log_warning)
+        for metadata_d in all_metadata:
+            vx = metadata_d.pop("voxel_resolution_x", None)
+            vy = metadata_d.pop("voxel_resolution_y", None)
+            vz = metadata_d.pop("voxel_resolution_z", None)
+            metadata_d["voxel_resolution"] = [vx, vy, vz]
+        return all_metadata
+    
     def live_live_query(
         self,
         table: str,
         timestamp: datetime,
         joins=None,
         filter_in_dict=None,
         filter_out_dict=None,
@@ -1876,23 +1918,108 @@
         endpoint_mapping["datastack_name"] = datastack_name
         endpoint_mapping["version"] = version
         url = self._endpoints["get_views"].format_map(endpoint_mapping)
         response = self.session.get(url, verify=self.verify)
         self.raise_for_status(response)
         return response.json()
 
-    def get_view_metadata(self, view_name: str, log_warning: bool = True):
-        """get metadata for a view"""
+    def get_view_metadata(
+        self,
+        view_name: str,
+        materialization_version: int = None,
+        datastack_name: str = None,
+        log_warning: bool = True,
+    ):
+        """get metadata for a view
+
+        Args:
+            view_name (str): name of view to query
+            materialization_version (int, optional): version to query.
+                                        Defaults to None. (will use version set by client)
+            log_warning (bool, optional): whether to log warnings. Defaults to True.
+        Returns:
+            dict: metadata of view
+
+        """
+        if datastack_name is None:
+            datastack_name = self.datastack_name
+        if materialization_version is None:
+            materialization_version = self.version
+
         endpoint_mapping = self.default_url_mapping
         endpoint_mapping["view_name"] = view_name
+        endpoint_mapping["datastack_name"] = datastack_name
+        endpoint_mapping["version"] = materialization_version
+
         url = self._endpoints["get_view_metadata"].format_map(endpoint_mapping)
         response = self.session.get(url, verify=self.verify)
         self.raise_for_status(response, log_warning=log_warning)
         return response.json()
 
+    def get_view_schema(
+        self,
+        view_name: str,
+        materialization_version: int = None,
+        datastack_name: str = None,
+        log_warning: bool = True,
+    ):
+        """get schema for a view
+
+        Args:
+            view_name (str): name of view to query
+            materialization_version (int, optional): version to query.
+                                        Defaults to None. (will version set by client)
+            log_warning (bool, optional): whether to log warnings. Defaults to True.
+        Returns:
+            dict: schema of view
+        """
+        if datastack_name is None:
+            datastack_name = self.datastack_name
+        if materialization_version is None:
+            materialization_version = self.version
+
+        endpoint_mapping = self.default_url_mapping
+        endpoint_mapping["view_name"] = view_name
+        endpoint_mapping["datastack_name"] = datastack_name
+        endpoint_mapping["version"] = materialization_version
+
+        url = self._endpoints["view_schema"].format_map(endpoint_mapping)
+        response = self.session.get(url, verify=self.verify)
+        self.raise_for_status(response, log_warning=log_warning)
+        return response.json()
+
+    def get_view_schemas(
+        self,
+        materialization_version: int = None,
+        datastack_name: str = None,
+        log_warning: bool = True,
+    ):
+        """get schemas for all views
+
+        Args:
+            materialization_version (int, optional): version to query.
+                                        Defaults to None. (will version set by client)
+            log_warning (bool, optional): whether to log warnings. Defaults to True.
+        Returns:
+            dict: schemas of all views
+        """
+        if datastack_name is None:
+            datastack_name = self.datastack_name
+        if materialization_version is None:
+            materialization_version = self.version
+
+        endpoint_mapping = self.default_url_mapping
+        endpoint_mapping["datastack_name"] = datastack_name
+        endpoint_mapping["version"] = materialization_version
+
+        url = self._endpoints["view_schemas"].format_map(endpoint_mapping)
+        response = self.session.get(url, verify=self.verify)
+        self.raise_for_status(response, log_warning=log_warning)
+        return response.json()
+
     def query_view(
         self,
         view_name: str,
         filter_in_dict=None,
         filter_out_dict=None,
         filter_equal_dict=None,
         filter_spatial_dict=None,
```

### Comparing `caveclient-5.3.2/caveclient/session_config.py` & `caveclient-5.4.0/caveclient/session_config.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/timeit.py` & `caveclient-5.4.0/caveclient/timeit.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/tools/caching.py` & `caveclient-5.4.0/caveclient/tools/caching.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient/tools/stage.py` & `caveclient-5.4.0/caveclient/tools/stage.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/caveclient.egg-info/SOURCES.txt` & `caveclient-5.4.0/caveclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/setup.py` & `caveclient-5.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/tests/conftest.py` & `caveclient-5.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/tests/test_annotation.py` & `caveclient-5.4.0/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/tests/test_chunkedgraph.py` & `caveclient-5.4.0/tests/test_chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/tests/test_infoservice.py` & `caveclient-5.4.0/tests/test_infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.2/tests/test_materialization.py` & `caveclient-5.4.0/tests/test_materialization.py`

 * *Files identical despite different names*


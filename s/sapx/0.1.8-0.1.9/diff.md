# Comparing `tmp/sapx-0.1.8.tar.gz` & `tmp/sapx-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapx-0.1.8.tar", last modified: Mon Apr 17 14:56:23 2023, max compression
+gzip compressed data, was "sapx-0.1.9.tar", last modified: Mon Apr 24 11:24:07 2023, max compression
```

## Comparing `sapx-0.1.8.tar` & `sapx-0.1.9.tar`

### file list

```diff
@@ -1,56 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.179742 sapx-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-17 14:56:23.179742 sapx-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-17 14:56:06.000000 sapx-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-17 14:56:06.000000 sapx-0.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.175742 sapx-0.1.8/sap/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.175742 sapx-0.1.8/sap/beanie/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/link.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/beanie/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.175742 sapx-0.1.8/sap/chart/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/chart/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.175742 sapx-0.1.8/sap/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/fastapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.175742 sapx-0.1.8/sap/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/rest/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/rest/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.175742 sapx-0.1.8/sap/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/amqp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/crons.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/lambdas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-17 14:56:06.000000 sapx-0.1.8/sap/worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.179742 sapx-0.1.8/sapx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-17 14:56:23.000000 sapx-0.1.8/sapx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-17 14:56:23.000000 sapx-0.1.8/sapx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:56:23.000000 sapx-0.1.8/sapx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-17 14:56:23.000000 sapx-0.1.8/sapx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 14:56:23.000000 sapx-0.1.8/sapx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:56:23.179742 sapx-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-17 14:56:06.000000 sapx-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:56:23.179742 sapx-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-17 14:56:06.000000 sapx-0.1.8/tests/test_fastapi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-17 14:56:06.000000 sapx-0.1.8/tests/test_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-17 14:56:06.000000 sapx-0.1.8/tests/test_worker_lambdas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-17 14:56:06.000000 sapx-0.1.8/tests/test_worker_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:24:07.023272 sapx-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-24 11:24:07.023272 sapx-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-24 11:23:48.000000 sapx-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-24 11:23:48.000000 sapx-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:24:07.015272 sapx-0.1.9/sap/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:24:07.019272 sapx-0.1.9/sap/beanie/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/beanie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/beanie/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/beanie/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/beanie/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/beanie/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/beanie/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/beanie/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/beanie/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:24:07.019272 sapx-0.1.9/sap/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/chart/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:24:07.019272 sapx-0.1.9/sap/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/fastapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/fastapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/fastapi/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/fastapi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/fastapi/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/fastapi/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/fastapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:24:07.019272 sapx-0.1.9/sap/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/rest/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/rest/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:24:07.023272 sapx-0.1.9/sap/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/worker/amqp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/worker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/worker/crons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/worker/crons_airtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/worker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/worker/lambdas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/worker/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-24 11:23:48.000000 sapx-0.1.9/sap/worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:24:07.023272 sapx-0.1.9/sapx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-24 11:24:07.000000 sapx-0.1.9/sapx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-24 11:24:07.000000 sapx-0.1.9/sapx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 11:24:07.000000 sapx-0.1.9/sapx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 11:24:07.000000 sapx-0.1.9/sapx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-24 11:24:07.000000 sapx-0.1.9/sapx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 11:24:07.023272 sapx-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-24 11:23:48.000000 sapx-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:24:07.023272 sapx-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-24 11:23:48.000000 sapx-0.1.9/tests/test_fastapi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-24 11:23:48.000000 sapx-0.1.9/tests/test_rest_client.py
```

### Comparing `sapx-0.1.8/PKG-INFO` & `sapx-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapx
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library of re-usable utilities for python web apps.
 Home-page: https://github.com/trellixio/sap
 Author: Trellix Dev
 Author-email: contact@trellix.io
 License: COPYRIGHT @ Trellix
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
```

### Comparing `sapx-0.1.8/pyproject.toml` & `sapx-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/beanie/client.py` & `sapx-0.1.9/sap/beanie/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,63 @@
 """
 Beanie Client.
 
 Initialize connection to the Mongo Database.
 """
 import typing
+from dataclasses import dataclass
 
-from motor.motor_asyncio import AsyncIOMotorClient
+import pymongo.errors
+from motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorDatabase
 
 import beanie
 
+from sap.loggers import logger
 from sap.settings import DatabaseParams
 
 
+@dataclass
+class MongoConnection:
+    """Define a standard cron task response."""
+
+    client: AsyncIOMotorClient
+    database: AsyncIOMotorDatabase
+
+
 class BeanieClient:
     """Set up a connection to the MongoDB server."""
 
-    connections: typing.ClassVar[dict[str, AsyncIOMotorClient]] = {}
+    connections: typing.ClassVar[dict[str, MongoConnection]] = {}
 
     @classmethod
-    async def get_db_default(cls) -> AsyncIOMotorClient:
+    async def get_db_default(cls) -> AsyncIOMotorDatabase:
         """Return the default db connection."""
-        return cls.connections["default"]
+        return cls.connections["default"].database
 
     @classmethod
     async def init(
         cls,
         mongo_params: DatabaseParams,
         document_models: list[typing.Union[typing.Type[beanie.Document], typing.Type[beanie.View], str]],
+        force: bool = False,
     ) -> None:
         """Open and maintain a connection to the database.
 
         :force bool: Use it for force a connection initialization
         """
-        # TODO: Check if connection exist, return existing connection
-        if "default" in cls.connections:
-            # connection = cls.connections["default"]
-            return
+
+        if "default" in cls.connections and not force:
+            database: AsyncIOMotorDatabase = cls.connections["default"].database
+
+            try:
+                await database.command("ping")
+            except pymongo.errors.ConnectionFailure:
+                logger.debug("--> Invalidate existing MongoDB connection")
+            else:
+                logger.debug("--> Using existing MongoDB connection")
+                return
 
         client = AsyncIOMotorClient(mongo_params.get_dns())
-        connection = client[mongo_params.db]
-        cls.connections["default"] = connection
-        await beanie.init_beanie(connection, document_models=document_models)
-        print("--> Initialized beanie")
+        database = client[mongo_params.db]
+        cls.connections["default"] = MongoConnection(client=client, database=database)
+        await beanie.init_beanie(database, document_models=document_models, allow_index_dropping=True)
+        logger.info("--> Establishing new MongoDB connection")
```

### Comparing `sapx-0.1.8/sap/beanie/document.py` & `sapx-0.1.9/sap/beanie/document.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/beanie/link.py` & `sapx-0.1.9/sap/beanie/link.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/beanie/mixins.py` & `sapx-0.1.9/sap/beanie/mixins.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/beanie/patch.py` & `sapx-0.1.9/sap/beanie/patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,16 @@
                 link_type=LinkTypes.LIST,
             )
     return None
 
 
 def init_document_fields(cls) -> None:
     """
-    Init class fields
+    Init class fields.
+
     :return: None
     """
     cls.update_forward_refs()
 
     def check_nested_links(link_info: LinkInfo, prev_models: List[Type[BaseModel]]) -> None:
         if link_info.model_class in prev_models:
             return
```

### Comparing `sapx-0.1.8/sap/beanie/query.py` & `sapx-0.1.9/sap/beanie/query.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/chart/serializers.py` & `sapx-0.1.9/sap/chart/serializers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Stat Serializer. 
+Stat Serializer.
 
 A serializer that helps normalize the format of statistics objects
 """
 
 import typing
 from decimal import Decimal
```

### Comparing `sapx-0.1.8/sap/fastapi/__init__.py` & `sapx-0.1.9/sap/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/fastapi/auth.py` & `sapx-0.1.9/sap/fastapi/auth.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/fastapi/exceptions.py` & `sapx-0.1.9/sap/fastapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/fastapi/forms.py` & `sapx-0.1.9/sap/fastapi/forms.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/fastapi/middleware.py` & `sapx-0.1.9/sap/fastapi/middleware.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/fastapi/pagination.py` & `sapx-0.1.9/sap/fastapi/pagination.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/fastapi/serializers.py` & `sapx-0.1.9/sap/fastapi/serializers.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/fastapi/utils.py` & `sapx-0.1.9/sap/fastapi/utils.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/rest/client.py` & `sapx-0.1.9/sap/rest/client.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/rest/exceptions.py` & `sapx-0.1.9/sap/rest/exceptions.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/settings.py` & `sapx-0.1.9/sap/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -44,12 +44,14 @@
         query: str = f"?{self.params}" if self.params else ""
         return f"{self.protocol}://{credentials}{self.host}{port}/{self.db}{query}"
 
 
 class SapSettings:
     """Settings params for SAP."""
 
+    APP_ENV: str = os.getenv("APP_ENV", "").upper()
+
     # True is environment is set to DEV
-    is_env_dev: bool = os.getenv("APP_ENV", "").upper() == "DEV"
+    is_env_dev: bool = APP_ENV == "DEV"
 
     # True is environment is set to PROD
-    is_env_prod: bool = os.getenv("APP_ENV", "").upper() == "PROD"
+    is_env_prod: bool = APP_ENV == "PROD"
```

### Comparing `sapx-0.1.8/sap/worker/__init__.py` & `sapx-0.1.9/sap/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/worker/amqp.py` & `sapx-0.1.9/sap/worker/amqp.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/worker/config.py` & `sapx-0.1.9/sap/worker/config.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/worker/lambdas.py` & `sapx-0.1.9/sap/worker/lambdas.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/worker/packet.py` & `sapx-0.1.9/sap/worker/packet.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sap/worker/utils.py` & `sapx-0.1.9/sap/worker/utils.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/sapx.egg-info/PKG-INFO` & `sapx-0.1.9/sapx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapx
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library of re-usable utilities for python web apps.
 Home-page: https://github.com/trellixio/sap
 Author: Trellix Dev
 Author-email: contact@trellix.io
 License: COPYRIGHT @ Trellix
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
```

### Comparing `sapx-0.1.8/sapx.egg-info/SOURCES.txt` & `sapx-0.1.9/sapx.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -26,20 +26,19 @@
 sap/rest/__init__.py
 sap/rest/client.py
 sap/rest/exceptions.py
 sap/worker/__init__.py
 sap/worker/amqp.py
 sap/worker/config.py
 sap/worker/crons.py
+sap/worker/crons_airtable.py
 sap/worker/exceptions.py
 sap/worker/lambdas.py
 sap/worker/packet.py
 sap/worker/utils.py
 sapx.egg-info/PKG-INFO
 sapx.egg-info/SOURCES.txt
 sapx.egg-info/dependency_links.txt
 sapx.egg-info/requires.txt
 sapx.egg-info/top_level.txt
 tests/test_fastapi_utils.py
-tests/test_rest_client.py
-tests/test_worker_lambdas.py
-tests/test_worker_packet.py
+tests/test_rest_client.py
```

### Comparing `sapx-0.1.8/setup.py` & `sapx-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 
 setup(
     name="sapx",
     version=VERSION,
     packages=find_packages(include=("sap.*", "sap")),
     package_data={"sap": ["py.typed"]},
     include_package_data=True,
```

### Comparing `sapx-0.1.8/tests/test_fastapi_utils.py` & `sapx-0.1.9/tests/test_fastapi_utils.py`

 * *Files identical despite different names*

### Comparing `sapx-0.1.8/tests/test_rest_client.py` & `sapx-0.1.9/tests/test_rest_client.py`

 * *Files identical despite different names*


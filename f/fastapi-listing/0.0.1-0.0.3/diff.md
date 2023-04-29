# Comparing `tmp/fastapi-listing-0.0.1.tar.gz` & `tmp/fastapi-listing-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-listing-0.0.1.tar", last modified: Tue Apr 11 07:55:43 2023, max compression
+gzip compressed data, was "fastapi-listing-0.0.3.tar", last modified: Sat Apr 29 18:29:23 2023, max compression
```

## Comparing `fastapi-listing-0.0.1.tar` & `fastapi-listing-0.0.3.tar`

### file list

```diff
@@ -1,50 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.731464 fastapi-listing-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-11 07:55:43.731464 fastapi-listing-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.723464 fastapi-listing-0.0.1/fastapi_listing/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.727464 fastapi-listing-0.0.1/fastapi_listing/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/base_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/listing_meta_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.727464 fastapi-listing-0.0.1/fastapi_listing/factory/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/factory/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/factory/generic_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/factory/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.727464 fastapi-listing-0.0.1/fastapi_listing/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/filters/generic_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/generic_dao.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.731464 fastapi-listing-0.0.1/fastapi_listing/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/listing_main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.731464 fastapi-listing-0.0.1/fastapi_listing/paginator/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/paginator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/paginator/naive_page_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.731464 fastapi-listing-0.0.1/fastapi_listing/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/plugins/filter_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/plugins/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/plugins/sorter_machanics.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.731464 fastapi-listing-0.0.1/fastapi_listing/sorter/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/sorter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/sorter/naive_page_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.723464 fastapi-listing-0.0.1/fastapi_listing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-11 07:55:43.000000 fastapi-listing-0.0.1/fastapi_listing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-11 07:55:43.000000 fastapi-listing-0.0.1/fastapi_listing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:55:43.000000 fastapi-listing-0.0.1/fastapi_listing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-11 07:55:43.000000 fastapi-listing-0.0.1/fastapi_listing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 07:55:43.000000 fastapi-listing-0.0.1/fastapi_listing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 07:55:43.731464 fastapi-listing-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.429780 fastapi-listing-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-29 18:29:23.429780 fastapi-listing-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.421779 fastapi-listing-0.0.3/fastapi_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.421779 fastapi-listing-0.0.3/fastapi_listing/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/abstracts/base_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/abstracts/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/abstracts/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/abstracts/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/abstracts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/abstracts/sorter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.421779 fastapi-listing-0.0.3/fastapi_listing/dao/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/dao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/dao/generic_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/factory/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/factory/generic_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/factory/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/filters/generic_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/interface/listing_meta_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/mechanics/filter_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/mechanics/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/mechanics/sorter_mechanics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/paginator/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/paginator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/paginator/naive_page_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/service/listing_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/sorter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/sorter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/sorter/naive_page_sorter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.425780 fastapi-listing-0.0.3/fastapi_listing/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/strategies/query_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/fastapi_listing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:29:23.421779 fastapi-listing-0.0.3/fastapi_listing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-29 18:29:23.000000 fastapi-listing-0.0.3/fastapi_listing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-29 18:29:23.000000 fastapi-listing-0.0.3/fastapi_listing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:29:23.000000 fastapi-listing-0.0.3/fastapi_listing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-29 18:29:23.000000 fastapi-listing-0.0.3/fastapi_listing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 18:29:23.000000 fastapi-listing-0.0.3/fastapi_listing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:29:23.429780 fastapi-listing-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-29 18:29:14.000000 fastapi-listing-0.0.3/setup.py
```

### Comparing `fastapi-listing-0.0.1/PKG-INFO` & `fastapi-listing-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-listing
-Version: 0.0.1
+Version: 0.0.3
 Summary: Data Listing Library for FastAPI
 Home-page: https://github.com/danielhasan1/fastapi-listing
 Author: Danish Hasan
 Author-email: dh813030@gmail.com
 Keywords: starlette,fastapi,starlite,pydantic
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `fastapi-listing-0.0.1/fastapi_listing/abstracts/dao.py` & `fastapi-listing-0.0.3/fastapi_listing/abstracts/dao.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.1/fastapi_listing/factory/generic_factory.py` & `fastapi-listing-0.0.3/fastapi_listing/factory/generic_factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import Any, Callable
 
 object_creation_collector: dict[str, Callable[..., Any]] = {}
 
 
 def register(key: str, creator: Callable[..., Any]) -> None:
+    print(creator)
     """Register a new game character type."""
     if key in object_creation_collector:
         raise ValueError(f"Factory can not have duplicate builder key {key} for instance {creator.__name__}")
     object_creation_collector[key] = creator
 
 
 def unregister(key: str) -> None:
```

### Comparing `fastapi-listing-0.0.1/fastapi_listing/factory/strategy.py` & `fastapi-listing-0.0.3/fastapi_listing/factory/strategy.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.1/fastapi_listing/filters/generic_filters.py` & `fastapi-listing-0.0.3/fastapi_listing/filters/generic_filters.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.1/fastapi_listing/generic_dao.py` & `fastapi-listing-0.0.3/fastapi_listing/dao/generic_dao.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,71 @@
-from fastapi_listing.abstracts import DaoAbstract
-from sqlalchemy.orm import Session
-
-from fastapi_listing.typing import SqlAlchemyModel
-
-
-class GenericDao(DaoAbstract):
-
-    """
-    Dao stands for data access object.
-    This layers encapsulates all logic that a user may write
-    in order to interact with databases.
-    Dao has only one responsibility that is to communicate with
-    database, all logic regarding data manipulation should live at
-    service layer. This also acts as a gateway to database
-    a wrapper on top of existing orm where generic logic could be defined.
-
-    This is a demo class showing how one can benefit from it.
-    Please note that this is just a basic implementation
-    i.e., a basic recipe, if one want they can spice it up as they like.
-
-    A dao should only have a primary table as we are speaking in terms of orm
-    we will call it a model.
-    so a dao should only be associated with single model or model class.
-    i.e., one primary model per dao instance. please note that this is different from
-    joining multiple models or tables. we are strictly  speaking in terms of
-    objects context here that one dao object should only have one primary model
-    but one dao object can talk to multiple models with having first primary model.
-
-    Note - no data validation should happen at this layer. That should be prior to pushing
-    at this layer.
-    """
-
-    def __init__(self, model, **kwargs):
-        # considering that we are dealing with separate read and write dbs.
-        # we must have two sessions one for read replica and one for master or write replica
-        # we should define our reusable attributes here that we will use in each dao method definition
-        self._read_db: Session = kwargs.get("read_db_session")
-        self._write_db: Session = kwargs.get("write_db_session")
-        self.model = model
-
-    def create(self, values: dict[str, str | int]) -> SqlAlchemyModel:
-        """
-        A light method that enters values in primary model table.
-        single value at a time receives a dict implementation could map the dict with model values and
-        insert that mapping or single row into the table.
-        :param values: dict of values where keys are columns of table and value should be row values
-        :return: created object i.e., instrumented row object.
-        """
-        pass
-
-    def update(self, identifier: dict[str, str | int | list], values: dict) -> bool:
-        """
-        Similar to create method this receives an identifier
-        :param identifier:
-        :param values:
-        :return:
-        """
-        pass
-
-    def read(self, identifier: dict[str, str | int | list], fields: list | str = "__all__") -> SqlAlchemyModel:
-        pass
-
-    def delete(self, ids: list[int]) -> bool:
-        pass
+from fastapi_listing.abstracts import DaoAbstract
+from sqlalchemy.orm import Session
+
+from fastapi_listing.typing import SqlAlchemyModel
+
+
+class GenericDao(DaoAbstract):
+    """
+    Dao stands for data access object.
+    This layers encapsulates all logic that a user may write
+    in order to interact with databases.
+    Dao has only one responsibility that is to communicate with
+    database, all logic regarding data manipulation should live at
+    service layer. This also acts as a gateway to database
+    a wrapper on top of existing orm where generic logic could be defined.
+
+    This is a demo class showing how one can benefit from it.
+    Please note that this is just a basic implementation
+    i.e., a basic recipe, if one want they can spice it up as they like.
+
+    A dao should only have a primary table as we are speaking in terms of orm
+    we will call it a model.
+    so a dao should only be associated with single model or model class.
+    i.e., one primary model per dao instance. please note that this is different from
+    joining multiple models or tables. we are strictly  speaking in terms of
+    objects context here that one dao object should only have one primary model
+    but one dao object can talk to multiple models with having first primary model.
+
+    Note - no data validation should happen at this layer. That should be prior to pushing
+    at this layer.
+    """
+
+    model_kls: SqlAlchemyModel = None
+
+    def __init__(self, **kwargs):
+        # considering that we are dealing with separate read and write dbs.
+        # we must have two sessions one for read replica and one for master or write replica
+        # we should define our reusable attributes here that we will use in each dao method definition
+        self._read_db: Session = kwargs.get("read_db")
+        self._write_db: Session = kwargs.get("write_db")
+        if self.model_kls is None:
+            raise ValueError("model class is not set!")
+        self.model = self.model_kls
+
+    def create(self, values: dict[str, str | int]) -> SqlAlchemyModel:
+        """
+        A light method that enters values in primary model table.
+        single value at a time receives a dict implementation could map the dict with model values and
+        insert that mapping or single row into the table.
+        :param values: dict of values where keys are columns of table and value should be row values
+        :return: created object i.e., instrumented row object.
+        """
+        pass
+
+    def update(self, identifier: dict[str, str | int | list], values: dict) -> bool:
+        """
+        Similar to create method this receives an identifier
+        :param identifier:
+        :param values:
+        :return:
+        """
+        pass
+
+    def read(self, identifier: dict[str, str | int | list], fields: list | str = "__all__") -> SqlAlchemyModel:
+        pass
+
+    def delete(self, ids: list[int]) -> bool:
+        pass
+
+    def get_naive_read(self, fields_to_read: list):
+        return self._read_db.query(*fields_to_read)
```

### Comparing `fastapi-listing-0.0.1/fastapi_listing/listing_main.py` & `fastapi-listing-0.0.3/fastapi_listing/service/listing_main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,64 @@
-from typing import Type, Optional
 from fastapi import Request
 from sqlalchemy.orm import Query
 from json import JSONDecodeError
+from typing import Type, Optional
 
 from fastapi_listing import utils
-from fastapi_listing.abstracts import TableDataPaginatingStrategy, TableDataSortingStrategy
+from fastapi_listing.abstracts import TableDataPaginatingStrategy
 from fastapi_listing.sorter import SortingOrderStrategy
-from fastapi_listing.typing import ListingResponseType
-from fastapi_listing.abstracts import ListingBase, ListingMetaInfo
-from fastapi_listing.factory import strategy_factory, filter_factory
+from fastapi_listing.typing import ListingResponseType, SqlAlchemyModel
+from fastapi_listing.abstracts import ListingBase, ListingServiceBase
+from fastapi_listing.factory import strategy_factory
 from fastapi_listing.errors import ListingFilterError, ListingSorterError
-from fastapi_listing.filters import CommonFilterImpl
-from fastapi_listing.generic_dao import GenericDao
-from fastapi_listing.plugins import loader
+from fastapi_listing.dao.generic_dao import GenericDao
+from fastapi_listing.interface.listing_meta_info import ListingMetaInfo
 from fastapi_listing.factory import generic_factory
+from fastapi_listing.mechanics import loader
 
 try:
     from pydantic import BaseModel
 
     HAS_PYDANTIC = True
 except ImportError:
     HAS_PYDANTIC = False
     BaseModel: Optional[Type] = None
 
-N_SRT_STRATEGY_DSC = "naive_sort_dsc"
-N_SRT_STRATEGY_ASC = "naive_sort_asc"
-
 
 class FastapiListing(ListingBase):
 
-    def __init__(self, request: Request, dao: GenericDao, pydantic_serializer: Type[BaseModel] = None,
-                 custom_fields: bool = False) -> None:
+    def __init__(self, request: Request, dao: GenericDao, pydantic_serializer: Optional[Type[BaseModel]] = None,
+                 custom_fields: Optional[bool] = False) -> None:
         self.request = request
         self.dao = dao
-        if HAS_PYDANTIC:
+        if HAS_PYDANTIC and pydantic_serializer:
             self.fields_to_fetch = list(pydantic_serializer.__fields__.keys())
         else:
-            self.fields_to_fetch = None  # can't deduce automatically tell this in query strategy
+            self.fields_to_fetch = None
         self.custom_fields = custom_fields
 
-    def replace_aliases(self, mapper: dict[str, str], req_params: list[dict[str, str]]) -> list[dict[str, str]]:
+    def _replace_aliases(self, mapper: dict[str, str], req_params: list[dict[str, str]]) -> list[dict[str, str]]:
         req_prms_cpy = req_params.copy()
         for param in req_prms_cpy:
             param["field"] = mapper[param["field"]]
         return req_prms_cpy
 
-    def apply_sorting(self, query: Query, listing_meta_info: ListingMetaInfo) -> Query:
+    def _apply_sorting(self, query: Query, listing_meta_info: ListingMetaInfo) -> Query:
         try:
             sorting_params: list[dict] = utils.jsonify_query_params(self.request.query_params.get("sort"))
         except JSONDecodeError:
             raise ListingSorterError("sorter param is not a valid json!")
 
         if temp := set(item.get("field") for item in sorting_params) - set(
                 listing_meta_info.sorting_column_mapper.keys()):
             raise ListingSorterError(f"Sorter'(s) not registered with listing: {temp}, Did you forget to do it?")
         if sorting_params:
-            sorting_params = self.replace_aliases(listing_meta_info.sorting_column_mapper, sorting_params)
+            sorting_params = self._replace_aliases(listing_meta_info.sorting_column_mapper, sorting_params)
         else:
             sorting_params = [listing_meta_info.default_sort_val]
-        loader.load_plugins(listing_meta_info.sorter_plugins)
 
         # ideally sorting should only happen on one field multi field sorting puts
         # unwanted strain on table when the size is big and not really popular
         # among various clients. Still leaving room for extension won't hurt
         # by default even if client is sending multiple sorting params we prioritize
         # the latest one which is last column that client requested to sort on.
         # if user want they can implement their own asc or dsc sorting order strategy and
@@ -79,145 +75,200 @@
 
         # fix this code
         # query = sorting_strategy.sort(value=sorting_params[-1],
         #                               query=query)
         def launch_mechanics(qry):
             # for mechanics in listing_meta_info.sorter_plugins:
             #     mecha: str = mechanics.split(".")[-1]
-            mecha: str = listing_meta_info.sorter_plugins[-1].split(".")[-1]
-            mecha_obj = generic_factory.create(mecha, query=qry, strategy=listing_meta_info.sorting_strategy,
-                                               sorting_params=sorting_params)
-            qry = mecha_obj.apply()
+            mecha: str = listing_meta_info.sorter_plugin
+            mecha_obj = generic_factory.create(mecha)
+            qry = mecha_obj.apply(query=qry, strategy=listing_meta_info.sorting_strategy,
+                                  sorting_params=sorting_params, extra_context=listing_meta_info.extra_context)
             return qry
 
         query = launch_mechanics(query)
         return query
 
     # no means to send allowed filte dictionary to client as this was handled by core.
     # same goes for allowed sorts.
     # need to add that in listing response.
     # naive strategies are not registered, register them.
     # we can leave multi sorting for later release for now only allow sort on a singular field.
     # this class name is not looking to good think of a different name if possible.
     # FilterApplicationEngine
-    def apply_filters(self, query: Query, filter_field_mapper: dict[str, str], filter_plugins: list[str]) -> Query:
+    def _apply_filters(self, query: Query, listing_meta_info: ListingMetaInfo) -> Query:
         try:
             fltrs: list[dict] = utils.jsonify_query_params(self.request.query_params.get("filter"))
         except JSONDecodeError:
             raise ListingFilterError(f"filter param is not a valid json!")
 
-        if temp := set(item.get("field") for item in fltrs) - set(filter_field_mapper.keys()):
+        if temp := set(item.get("field") for item in fltrs) - set(listing_meta_info.filter_column_mapper.keys()):
             raise ListingFilterError(f"Filter'(s) not registered with listing: {temp}, Did you forget to do it?")
 
-        fltrs = self.replace_aliases(filter_field_mapper, fltrs)
-
-        loader.load_plugins(filter_plugins)
+        fltrs = self._replace_aliases(listing_meta_info.filter_column_mapper, fltrs)
 
         def launch_mechanics(qry):
-            mecha: str = filter_plugins[-1].split(".")[-1]
-            mecha_obj = generic_factory.create(mecha, query=qry, filter_params=fltrs, dao=self.dao,
-                                               request=self.request)
-            qry = mecha_obj.apply()
+            mecha_obj = generic_factory.create(listing_meta_info.filter_plugin)
+            qry = mecha_obj.apply(query=qry, filter_params=fltrs, dao=self.dao,
+                                  request=self.request, extra_context=listing_meta_info.extra_context)
             return qry
 
         query = launch_mechanics(query)
-
-        # for applied_filter in fltrs:
-        #     filter_obj: CommonFilterImpl = filter_factory.create(filter_field_mapper[applied_filter.get("field")],
-        #                                                          dao=self.dao,
-        #                                                          request=self.request)
-        #     query = filter_obj.filter(field=filter_field_mapper[applied_filter.get("field")],
-        #                               value=applied_filter.get("value"),
-        #                               query=query)
         return query
 
-    def paginate(self, query: Query, paginate_strategy: TableDataPaginatingStrategy) -> ListingResponseType:
-        query = paginate_strategy.paginate(query, self.request)
-        return query
+    def _paginate(self, query: Query, paginate_strategy: TableDataPaginatingStrategy,
+                  extra_context: dict) -> ListingResponseType:
+        page = paginate_strategy.paginate(query, self.request, extra_context)
+        return page
 
-    def prepare_query(self, listing_meta_info: ListingMetaInfo) -> Query:
-        base_query: Query = listing_meta_info.query_strategy.get_query(field_list=self.fields_to_fetch,
-                                                                       request=self.request,
+    def _prepare_query(self, listing_meta_info: ListingMetaInfo) -> Query:
+        base_query: Query = listing_meta_info.query_strategy.get_query(request=self.request,
                                                                        dao=self.dao,
-                                                                       custom_fields=self.custom_fields)
-        fltr_query: Query = self.apply_filters(base_query, listing_meta_info.filter_column_mapper)
-        srtd_query: Query = self.apply_sorting(fltr_query, listing_meta_info)
+                                                                       extra_context=listing_meta_info.extra_context)
+        fltr_query: Query = self._apply_filters(base_query, listing_meta_info)
+        srtd_query: Query = self._apply_sorting(fltr_query, listing_meta_info)
         return srtd_query
 
-    # def prepare_response(self, query, paginating_strategy) -> ListingResponseType:
-    #     """
-    #     Prepares a page response to return to the client
-    #     :param query sqlalchemy query
-    #     """
-    #     pgntd_resp: ListingResponseType = self.paginate(query, paginating_strategy)
-    #     return pgntd_resp
+    @staticmethod
+    def _set_vals_in_extra_context(extra_context: dict, **kwargs):
+        extra_context.update(kwargs)
 
     def get_response(self, listing_meta_info: ListingMetaInfo) -> ListingResponseType:
-        fnl_query: Query = self.prepare_query(listing_meta_info)
-        response: ListingResponseType = self.paginate(fnl_query, listing_meta_info.paginating_strategy)
+        self._set_vals_in_extra_context(listing_meta_info.extra_context,
+                                        field_list=self.fields_to_fetch,
+                                        custom_fields=self.custom_fields
+                                        )
+        fnl_query: Query = self._prepare_query(listing_meta_info)
+        response: ListingResponseType = self._paginate(fnl_query, listing_meta_info.paginating_strategy,
+                                                       listing_meta_info.extra_context)
         return response
 
 
-class ListingService:
-    filter_mapper = {}
-    sort_mapper = {}
+class ListingService(ListingServiceBase):
+    filter_mapper: dict = {}
+    sort_mapper: dict = {}
     # here resource creation should be based on factory and not inline as we are separating creation from usage.
     # factory should deliver sorting resource
-    DEFAULT_SRT_ON = "created_at"
-    DEFAULT_SRT_ORD = "dsc"
-    PAGINATE_STRATEGY = "naive_paginator"
-    QUERY_STRATEGY = "naive_query"
-    SORTING_STRATEGY = "naive_sorter"
-    SORTER_PLUGIN = ["fastapi_listing.plugins.sorter_mechanics"]
-    FILTER_PLUGIN = ["fastapi_listing.plugins.filter_mechanics"]
-
-    def __init__(self, dao, request, model, **kwargs):
-        self.dao = dao(model, **kwargs)
+    DEFAULT_SRT_ON: str = "created_at"
+    DEFAULT_SRT_ORD: str = "dsc"
+    PAGINATE_STRATEGY: str = "naive_paginator"
+    QUERY_STRATEGY: str = "naive_query"
+    SORTING_STRATEGY: str = "naive_sorter"
+    SORT_MECHA: str = "sorter_mechanics"
+    FILTER_MECHA: str = "filter_mechanics"
+    dao_kls: GenericDao = GenericDao
+
+    # pydantic_serializer: Type[BaseModel] = None
+    # allowed_pydantic_custom_fields: bool = False
+    # it is possible to have more than one serializer for particular endpoint depending upon
+    # user or a query/path param condition we could switch json schema so allowing this
+    # flexibility for the user to be able to switch between schema Fastapilisting object
+    # should get initialized at user level and not implicit.
+
+    def __init__(self, request, **kwargs) -> None:
+        self.dao = self.dao_kls(**kwargs)
+        # pop out db sessions as they are concrete property of data access layer and not service layer.
+        # once injected to dao popping out here
+        kwargs.pop("read_db", None)
+        kwargs.pop("write_db", None)
         self.request = request
+        self.extra_context = kwargs
 
     def get_listing(self):
-        raise NotImplementedError
+        """
+        implement at child class level.
 
-    # def choose_sorting_strategy(self):
-    #     try:
-    #         sorting_param: list[dict] = utils.jsonify_query_params(self.request.query_params.get("sort"))
-    #     except JSONDecodeError:
-    #         # CashifyLogger.error(f"Error occurred during sort decode:{e}")
-    #         raise ListingSorterError("sorter param is not a valid json!")
-    #     srt_strtg: str = "dsc"
-    #     if sorting_param:
-    #         srt_strtg = sorting_param[-1].get("type")
-    #     if srt_strtg == "asc":
-    #         return strategy_factory.create(self.SRT_STRATEGY_ASC, self.DEFAULT_SRT_ON)
-    #     else:
-    #         return strategy_factory.create(self.SRT_STRATEGY_DSC, self.DEFAULT_SRT_ON)
+        FastapiListing(self.request, self.dao, pydantic_serializer=some_pydantic_model_class,
+         custom_fields=True/False).get_response(self.MetaInfo(self))
+        custom_fields can be also called pydantic_custom_fields.
+        Note: what is pydantic_custom_fields?
+                These are the fields that gets generated at runtime from existing table/sqlalchemy model fields.
+                for example:
+                lets say you have a pydantic model class
+                class abc(BaseModel):
+                    id: int
+                    code: str
+
+                    @root_validator
+                    def generate_code(cls, values):
+                        values["code"] = f'FANCY{values["id"]}CODE'
+                here code gets generated at runtime, code is not a table field, code is a custom field that is
+                deduced with the help of id.
+        :return: page response for client to render
+        """
+        raise NotImplementedError("method should be implemented in child class and not here!")
+
+    def page_data_modifier(self, data: dict) -> dict:
+        raise NotImplementedError
 
     class MetaInfo:
-        def __init__(self, outer_instance) -> None:
-            # self.sorting_strategy = outer_instance.choose_sorting_strategy()
+
+        def __init__(self, outer_instance):
             self.paginating_strategy: TableDataPaginatingStrategy = strategy_factory.create(
                 outer_instance.PAGINATE_STRATEGY)
             self.filter_column_mapper: dict = outer_instance.filter_mapper
             self.query_strategy: Query = strategy_factory.create(outer_instance.QUERY_STRATEGY)
-            self.sorting_column_mapper: dict = outer_instance.sort_mapper
+            # self.sorting_column_mapper: dict = outer_instance.sort_mapper
             self.default_sort_val: dict[str, str] = dict(type=outer_instance.DEFAULT_SRT_ORD,
                                                          field=outer_instance.DEFAULT_SRT_ON)
             self.sorting_strategy: SortingOrderStrategy = strategy_factory.create(
                 outer_instance.SORTING_STRATEGY,
                 model=outer_instance.dao.model,
                 request=outer_instance.request
             )
-            self.sorter_plugins = outer_instance.SORTER_PLUGIN
-            self.filter_plugins = outer_instance.FILTER_PLUGIN
+            self.sorter_plugin: str = outer_instance.SORT_MECHA
+            self.filter_plugin: str = outer_instance.FILTER_MECHA
+            self.extra_context: dict = outer_instance.extra_context
 
-    def create_inner(self) -> MetaInfo:
-        return ListingService.MetaInfo(self)
+    def meta_info_generator(self) -> ListingMetaInfo:
+        return ListingService.MetaInfo(self) # type:ignore # noqa # some issue is coming in pycharm for return types
 
     @classmethod
     def get_aliased_filter_mapper(cls) -> dict[str, str]:
         return {key: key for key, val in cls.filter_mapper.items()}
 
     @classmethod
     def get_aliased_sort_mapper(cls) -> dict[str, str]:
         return {key: key for key, val in cls.sort_mapper.items()}
 
-# default strategy factory
+    @staticmethod
+    def get_sort_mecha_plugin_path() -> str:
+        """
+        hook to provide sort mecha plugin module path as py import path
+        overwrite allowed to provide custom path.
+        :return: import path as string ex. fastapi_listing.mechanics.sorter_mechanics.
+        """
+        return "fastapi_listing.mechanics.sorter_mechanics"
+
+    @staticmethod
+    def get_filter_mecha_plugin_path() -> str:
+        """
+       hook to provide filter mecha plugin module path as py import path
+       overwrite allowed to provide custom path.
+       :return: import path as string ex. fastapi_listing.mechanics.filter_mechanics.
+       """
+        return "fastapi_listing.mechanics.filter_mechanics"
+
+    @classmethod
+    def plugins_to_load(cls) -> list[str]:
+        """
+        Provided a hook to be called at module level of each listing service.
+        overwrite sort or filter plugin path getters to give your own custom
+        mechanic implementations.
+        refrain from overwriting it as this may change or it's fundamnetal
+        implementation is already broken down to pieces that can no longer
+        be broken any further. So instead of overwriting this
+        overwrite the individual pieces
+        :return: list plugins to load
+        currently only support sort/filter mecha loading
+        todo: can add pattern calling like %s_plugin_path for providing n number of plugin loading
+        """
+        return [cls.get_sort_mecha_plugin_path(), cls.get_filter_mecha_plugin_path()]
+
+
+# calling loader at module level so once the module is loaded all plugins get loaded and not further loading is required
+loader.load_plugins(ListingService.plugins_to_load())
+
+
+# todo: how to provide a hook in listing service so a person can easily overwrite the data list or manipulate it easily
+# todo: before wrapping it up in page response
+
```

### Comparing `fastapi-listing-0.0.1/fastapi_listing/paginator/naive_page_builder.py` & `fastapi-listing-0.0.3/fastapi_listing/paginator/naive_page_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,30 @@
+from json import JSONDecodeError
 from fastapi_listing import utils
 from fastapi_listing.abstracts import TableDataPaginatingStrategy
+from fastapi_listing.errors import ListingPaginatorError
+from fastapi_listing.typing import SqlAlchemyQuery, FastapiRequest
 
 
 class NaivePaginationStrategy(TableDataPaginatingStrategy):
+    """
+    Loosely coupled paginator module.
+    """
 
     default_pagination_params = {"pageSize": 10, "page": 0}
-    DEFAULT_PAGE_TEMPLATE = {"data": None, "hasNext": None, "totalCount": None,
-                             "currentPageSize": None, "currentPageNumber": None}
+    PAGE_TEMPLATE = {"data": None, "hasNext": None, "totalCount": None,
+                     "currentPageSize": None, "currentPageNumber": None}
 
-    def paginate(self, query, request):
+    def paginate(self, query: SqlAlchemyQuery, request: FastapiRequest, extra_context: dict):
         pagination_params = self.default_pagination_params
-        pagination_params = utils.jsonify_query_params(request.query_params.get('pagination')) \
-            if request.query_params.get('pagination') else pagination_params
+        try:
+            pagination_params = utils.jsonify_query_params(request.query_params.get('pagination')) \
+                if request.query_params.get('pagination') else pagination_params
+        except JSONDecodeError:
+            raise ListingPaginatorError("pagination params are not valid json!")
         count = query.count()
         has_next = True if count - ((pagination_params.get('page')) * pagination_params.get('pageSize')) > \
                            pagination_params.get('pageSize') else False
         current_page_size = pagination_params.get("pageSize")
         current_page_number = pagination_params.get("page")
         query = query.limit(
             pagination_params.get('pageSize')
```

### Comparing `fastapi-listing-0.0.1/fastapi_listing/plugins/filter_mechanics.py` & `fastapi-listing-0.0.3/fastapi_listing/mechanics/filter_mechanics.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from fastapi_listing.factory import filter_factory, generic_factory
 from fastapi_listing.filters import CommonFilterImpl
+from fastapi_listing.typing import SqlAlchemyQuery, FastapiRequest
 
 
 class FilterMechanics:
 
-    def apply(self, *, query, filter_params: list[dict[str, str]], dao, request):
+    def apply(self, *, query: SqlAlchemyQuery = None, filter_params: list[dict[str, str]], dao=None,
+              request: FastapiRequest = None, extra_context: dict = None) -> SqlAlchemyQuery:
         for applied_filter in filter_params:
             filter_obj: CommonFilterImpl = filter_factory.create(applied_filter.get("field"),
                                                                  dao=dao,
                                                                  request=request)
             query = filter_obj.filter(field=applied_filter.get("field"),
                                       value=applied_filter.get("value"),
                                       query=query)
         return query
 
 
 def register() -> None:
-    generic_factory.register("filter_mechanics", FilterMechanics)
+    generic_factory.register("filter_mechanics", FilterMechanics)
```

### Comparing `fastapi-listing-0.0.1/fastapi_listing/plugins/loader.py` & `fastapi-listing-0.0.3/fastapi_listing/mechanics/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 
 def import_module(name: str) -> ModuleInterface:
     """Imports a module given a name."""
     return importlib.import_module(name)  # type: ignore
 
 
 def load_plugins(plugins: list[str]) -> None:
-    """Loads the plugins defined in the plugins list."""
+    """Loads the mechanics defined in the mechanics list."""
+    print(plugins)
     for plugin_file in plugins:
         plugin = import_module(plugin_file)
         plugin.register()
```

### Comparing `fastapi-listing-0.0.1/fastapi_listing/plugins/sorter_machanics.py` & `fastapi-listing-0.0.3/fastapi_listing/mechanics/sorter_mechanics.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from fastapi_listing.abstracts import TableDataSortingStrategy
 from fastapi_listing.typing import SqlAlchemyQuery
 
 
 class SorterMechanics:
 
     def apply(self, *, query: SqlAlchemyQuery = None, strategy: TableDataSortingStrategy = None,
-              sorting_params: list[dict[str, str]] = None) -> SqlAlchemyQuery:
+              sorting_params: list[dict[str, str]] = None, extra_context: dict = None) -> SqlAlchemyQuery:
         latest = sorting_params[-1]
         query = strategy.sort(query=query, value=latest)
         return query
 
 
 def register() -> None:
     generic_factory.register("sorter_mechanics", SorterMechanics)
```

### Comparing `fastapi-listing-0.0.1/fastapi_listing/sorter/naive_page_sorter.py` & `fastapi-listing-0.0.3/fastapi_listing/sorter/naive_page_sorter.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,10 +33,9 @@
     def validate_srt_field(model: SqlAlchemyModel, sort_field: str):
         try:
             inst_field = getattr(model, sort_field)
         except AttributeError:
             inst_field = None
         if inst_field is None:
             raise ValueError(f"Provided sort field is not an attribute of {model}")  # todo improve this by custom exception
-            # raise CashifyApiException(LogisticsException.INVALID_SORT_FIELD, LogisticsDiagnoCode.PLG1013)
         return inst_field
```

### Comparing `fastapi-listing-0.0.1/fastapi_listing/typing.py` & `fastapi-listing-0.0.3/fastapi_listing/typing.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,32 @@
-from typing import Tuple, TypeVar, List, Dict
+from typing import TypeVar, List, Dict
 from typing_extensions import TypedDict
-from sqlalchemy.orm.decl_api import DeclarativeMeta
-from sqlalchemy.orm import Query
-from sqlalchemy.orm import Session
-from sqlalchemy.sql.sqltypes import TypeEngine
 from fastapi import Request
 
+# will support future imports as well like pymongo and other orm tools
 
-SqlAlchemyModel = TypeVar("SqlAlchemyModel", bound=DeclarativeMeta)
+try:
+    from sqlalchemy.orm.decl_api import DeclarativeMeta
+    from sqlalchemy.orm import Query
+    from sqlalchemy.orm import Session
+    from sqlalchemy.sql.sqltypes import TypeEngine
+except ImportError:
+    DeclarativeMeta = None
+    Query = None
+    Session = None
+    TypeEngine = None
 
 
 class ListingResponseType(TypedDict):
     data: List[Dict[str, int | str | list | dict]]
     currentPageNumber: int
     currentPageSize: int
     totalCount: int
     hasNext: bool
 
 
 SqlAlchemyQuery = TypeVar("SqlAlchemyQuery", bound=Query)
 SqlAlchemySession = TypeVar("SqlAlchemySession", bound=Session)
 FastapiRequest = TypeVar("FastapiRequest", bound=Request)
 AnySqlAlchemyColumn = TypeVar("AnySqlAlchemyColumn", bound=TypeEngine)
+SqlAlchemyModel = TypeVar("SqlAlchemyModel", bound=DeclarativeMeta)
```

### Comparing `fastapi-listing-0.0.1/fastapi_listing.egg-info/PKG-INFO` & `fastapi-listing-0.0.3/fastapi_listing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-listing
-Version: 0.0.1
+Version: 0.0.3
 Summary: Data Listing Library for FastAPI
 Home-page: https://github.com/danielhasan1/fastapi-listing
 Author: Danish Hasan
 Author-email: dh813030@gmail.com
 Keywords: starlette,fastapi,starlite,pydantic
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `fastapi-listing-0.0.1/fastapi_listing.egg-info/SOURCES.txt` & `fastapi-listing-0.0.3/fastapi_listing.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 README.md
 setup.py
 fastapi_listing/__init__.py
 fastapi_listing/errors.py
-fastapi_listing/generic_dao.py
-fastapi_listing/listing_main.py
 fastapi_listing/logger.py
 fastapi_listing/py.typed
 fastapi_listing/typing.py
 fastapi_listing/utils.py
 fastapi_listing.egg-info/PKG-INFO
 fastapi_listing.egg-info/SOURCES.txt
 fastapi_listing.egg-info/dependency_links.txt
 fastapi_listing.egg-info/requires.txt
 fastapi_listing.egg-info/top_level.txt
 fastapi_listing/abstracts/__init__.py
 fastapi_listing/abstracts/base_query.py
 fastapi_listing/abstracts/dao.py
 fastapi_listing/abstracts/filter.py
 fastapi_listing/abstracts/listing.py
-fastapi_listing/abstracts/listing_meta_info.py
 fastapi_listing/abstracts/paginator.py
 fastapi_listing/abstracts/sorter.py
+fastapi_listing/dao/__init__.py
+fastapi_listing/dao/generic_dao.py
 fastapi_listing/factory/__init__.py
 fastapi_listing/factory/filter.py
 fastapi_listing/factory/generic_factory.py
 fastapi_listing/factory/strategy.py
 fastapi_listing/filters/__init__.py
 fastapi_listing/filters/generic_filters.py
 fastapi_listing/interface/__init__.py
+fastapi_listing/interface/listing_meta_info.py
+fastapi_listing/mechanics/__init__.py
+fastapi_listing/mechanics/filter_mechanics.py
+fastapi_listing/mechanics/loader.py
+fastapi_listing/mechanics/sorter_mechanics.py
 fastapi_listing/paginator/__init__.py
 fastapi_listing/paginator/naive_page_builder.py
-fastapi_listing/plugins/__init__.py
-fastapi_listing/plugins/filter_mechanics.py
-fastapi_listing/plugins/loader.py
-fastapi_listing/plugins/sorter_machanics.py
+fastapi_listing/service/__init__.py
+fastapi_listing/service/listing_main.py
 fastapi_listing/sorter/__init__.py
-fastapi_listing/sorter/naive_page_sorter.py
+fastapi_listing/sorter/naive_page_sorter.py
+fastapi_listing/strategies/__init__.py
+fastapi_listing/strategies/query_strategy.py
```

### Comparing `fastapi-listing-0.0.1/setup.py` & `fastapi-listing-0.0.3/setup.py`

 * *Files identical despite different names*


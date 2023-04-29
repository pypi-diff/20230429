# Comparing `tmp/pypreql-0.0.1rc8.tar.gz` & `tmp/pypreql-0.0.1rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypreql-0.0.1rc8.tar", last modified: Mon Feb 20 18:02:35 2023, max compression
+gzip compressed data, was "pypreql-0.0.1rc9.tar", last modified: Fri Feb 24 01:18:14 2023, max compression
```

## Comparing `pypreql-0.0.1rc8.tar` & `pypreql-0.0.1rc9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:35.032112 pypreql-0.0.1rc8/
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-02-20 18:02:35.032112 pypreql-0.0.1rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:35.028112 pypreql-0.0.1rc8/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/demo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:35.032112 pypreql-0.0.1rc8/preql/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:35.032112 pypreql-0.0.1rc8/preql/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/core/env_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/core/graph_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/core/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    29847 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:35.032112 pypreql-0.0.1rc8/preql/core/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/core/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21384 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/core/processing/concept_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/core/processing/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/core/query_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:35.032112 pypreql-0.0.1rc8/preql/dialect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/dialect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12664 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/dialect/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/dialect/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/dialect/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/dialect/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/dialect/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/dialect/sql_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:35.032112 pypreql-0.0.1rc8/preql/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:35.032112 pypreql-0.0.1rc8/preql/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:35.032112 pypreql-0.0.1rc8/preql/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/parsing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21815 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/parsing/parse_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/preql/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:02:35.032112 pypreql-0.0.1rc8/pypreql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-02-20 18:02:34.000000 pypreql-0.0.1rc8/pypreql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-02-20 18:02:35.000000 pypreql-0.0.1rc8/pypreql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 18:02:34.000000 pypreql-0.0.1rc8/pypreql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-20 18:02:34.000000 pypreql-0.0.1rc8/pypreql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-20 18:02:34.000000 pypreql-0.0.1rc8/pypreql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 18:02:35.032112 pypreql-0.0.1rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-20 18:02:24.000000 pypreql-0.0.1rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.461750 pypreql-0.0.1rc9/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/demo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.461750 pypreql-0.0.1rc9/preql/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.461750 pypreql-0.0.1rc9/preql/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/env_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/graph_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29847 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/preql/core/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/processing/concept_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/processing/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/core/query_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/preql/dialect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/dialect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/dialect/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/dialect/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/dialect/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/dialect/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/dialect/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/dialect/sql_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/preql/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/preql/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/preql/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/parsing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21715 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/parsing/parse_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/preql/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:18:14.465750 pypreql-0.0.1rc9/pypreql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-02-24 01:18:14.000000 pypreql-0.0.1rc9/pypreql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-02-24 01:18:14.000000 pypreql-0.0.1rc9/pypreql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 01:18:14.000000 pypreql-0.0.1rc9/pypreql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-24 01:18:14.000000 pypreql-0.0.1rc9/pypreql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-24 01:18:14.000000 pypreql-0.0.1rc9/pypreql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 01:18:14.469751 pypreql-0.0.1rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-02-24 01:18:03.000000 pypreql-0.0.1rc9/setup.py
```

### Comparing `pypreql-0.0.1rc8/PKG-INFO` & `pypreql-0.0.1rc9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pypreql
-Version: 0.0.1rc8
-Summary: Declarative, typed query lanuage.
+Version: 0.0.1rc9
+Summary: Declarative, typed query language that compiles to SQL.
 Home-page: 
 Author: 
 Author-email: preql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -143,8 +143,9 @@
 ```
 
 
 ## Contributing
 
 
 ## Similar in space
-singleorigin
+
+- singleorigin
```

### Comparing `pypreql-0.0.1rc8/README.md` & `pypreql-0.0.1rc9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -130,8 +130,9 @@
 ```
 
 
 ## Contributing
 
 
 ## Similar in space
-singleorigin
+
+- singleorigin
```

### Comparing `pypreql-0.0.1rc8/preql/core/enums.py` & `pypreql-0.0.1rc9/preql/core/enums.py`

 * *Files identical despite different names*

### Comparing `pypreql-0.0.1rc8/preql/core/env_processor.py` & `pypreql-0.0.1rc9/preql/core/env_processor.py`

 * *Files identical despite different names*

### Comparing `pypreql-0.0.1rc8/preql/core/graph_models.py` & `pypreql-0.0.1rc9/preql/core/graph_models.py`

 * *Files identical despite different names*

### Comparing `pypreql-0.0.1rc8/preql/core/hooks.py` & `pypreql-0.0.1rc9/preql/core/hooks.py`

 * *Files identical despite different names*

### Comparing `pypreql-0.0.1rc8/preql/core/models.py` & `pypreql-0.0.1rc9/preql/core/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -28,19 +28,19 @@
     pass
 
 
 class Concept(BaseModel):
     name: str
     datatype: DataType
     purpose: Purpose
-    grain: "Grain" = Field(default=None)
     metadata: Optional[Metadata] = None
     lineage: Optional[Union["Function", "WindowItem"]] = None
     namespace: str = ""
     keys: Optional[List["Concept"]] = None
+    grain: "Grain" = Field(default=None)
 
     @validator("lineage")
     def lineage_validator(cls, v):
         if v and not isinstance(v, (Function, WindowItem)):
             raise ValueError
         return v
 
@@ -435,14 +435,15 @@
 
     def __str__(self):
         if self.abstract:
             return "Grain<Abstract>"
         return "Grain<" + ",".join([c.address for c in self.components]) + ">"
 
     def with_namespace(self, namespace: str) -> "Grain":
+
         return Grain(
             components=[c.with_namespace(namespace) for c in self.components],
             nested=self.nested,
         )
 
     @property
     def abstract(self):
@@ -523,15 +524,14 @@
             )
         if isinstance(self.address, str):
             self.address = Address(location=self.address)
         if not self.namespace:
             self.namespace = ""
 
     def with_namespace(self, namespace: str):
-
         return Datasource(
             identifier=self.identifier,
             namespace=namespace,
             grain=self.grain.with_namespace(namespace),
             address=self.address,
             columns=[c.with_namespace(namespace) for c in self.columns],
         )
```

### Comparing `pypreql-0.0.1rc8/preql/core/processing/concept_strategies.py` & `pypreql-0.0.1rc9/preql/core/processing/concept_strategies.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,23 +78,34 @@
     g: ReferenceGraph,
     whole_grain: bool = False,
 ) -> QueryDatasource:
     """Return a datasource that has a direct property/key relation
     If the datasource is a component of the grain, assume we can
     join it in the final query to the grain level"""
     all_concepts = concept_to_inputs(concept)
-    for datasource in environment.datasources.values():
-        # whole grain determins
-        # if we can get a partial grain match
-        # such as joining through a table with a PK to get properties
-        # sometimes we need a source with all grain keys, in which case we
-        # force this not to match
-        if datasource.grain.issubset(grain) and (
-            datasource.grain == grain or not whole_grain
-        ):
+    if whole_grain:
+        valid_matches = ["all"]
+    else:
+        valid_matches = ["all", "partial"]
+    for strategy in valid_matches:
+        for datasource in environment.datasources.values():
+            # whole grain determines
+            # if we can get a partial grain match
+            # such as joining through a table with a PK to get properties
+            # sometimes we need a source with all grain keys, in which case we
+            # force this not to match
+
+            if strategy == "partial":
+                if not datasource.grain.issubset(grain):
+                    continue
+            else:
+                # either an exact match
+                # or it's a key on the table
+                if not datasource.grain == grain:
+                    continue
             all_found = True
             for req_concept in all_concepts:
                 try:
                     path = nx.shortest_path(
                         g,
                         source=datasource_to_node(datasource),
                         target=concept_to_node(req_concept),
@@ -102,25 +113,33 @@
                 except nx.exception.NetworkXNoPath as e:
                     all_found = False
                     break
                 if len([p for p in path if g.nodes[p]["type"] == "datasource"]) != 1:
                     all_found = False
                     break
             if all_found:
-                logger.debug(f"Can satisfy query from property lookup for {concept}")
-                if whole_grain:
-                    outputs = datasource.grain.components
-                    filters = [concept]
-                else:
-                    outputs = [concept] + datasource.grain.components
-                    filters = []
+                logger.debug(
+                    f"Can satisfy query from property lookup for {concept} using {datasource.identifier}"
+                )
+                outputs = [concept] + datasource.grain.components
+
+                # also pull through any grain component that might exist
+                # to facilitate future joins
+                for concept in grain.components:
+                    if (
+                        concept.with_grain(datasource.grain)
+                        in datasource.output_concepts
+                    ):
+                        outputs.append(concept)
+                outputs = unique(outputs, "address")
+                filters: List[Concept] = []
                 return QueryDatasource(
                     input_concepts=all_concepts + datasource.grain.components,
                     output_concepts=outputs,
-                    source_map={concept.name: {datasource} for concept in all_concepts},
+                    source_map={concept.name: {datasource} for concept in outputs},
                     datasources=[datasource],
                     grain=datasource.grain,
                     joins=[],
                     filter_concepts=filters,
                 )
     raise ValueError(f"No property lookup for {concept}")
 
@@ -159,20 +178,16 @@
             #     final_grain = datasource.grain
             # else:
             #     final_grain = grain
             final_grain = grain
             logger.debug(
                 f"got {datasource.identifier} for {concept} from grouped select"
             )
-            if whole_grain:
-                outputs = grain.components
-                filters = [concept]
-            else:
-                outputs = [concept] + grain.components
-                filters = []
+            outputs = [concept] + grain.components
+            filters: List[Concept] = []
             return QueryDatasource(
                 input_concepts=all_concepts,
                 output_concepts=outputs,
                 source_map={concept.name: {datasource} for concept in all_concepts},
                 datasources=[datasource],
                 grain=final_grain,
                 joins=[],
```

### Comparing `pypreql-0.0.1rc8/preql/core/processing/utility.py` & `pypreql-0.0.1rc9/preql/core/processing/utility.py`

 * *Files identical despite different names*

### Comparing `pypreql-0.0.1rc8/preql/core/query_processor.py` & `pypreql-0.0.1rc9/preql/core/query_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,16 @@
         # we do the with_grain here to fix an issue
         # where a query with a grain of properties has the components of the grain
         # with the default key grain rather than the grain of the select
         # TODO - evaluate if we can fix this in select definition
         joinkeys = [
             JoinKey(c)
             for c in statement.grain.components
-            if c.with_grain(statement.grain) in cte.output_columns
+            if c.with_grain(cte.grain) in cte.output_columns
+            and cte.grain.issubset(statement.grain)
         ]
         if joinkeys:
             joins.append(
                 Join(
                     left_cte=base,
                     right_cte=cte,
                     joinkeys=joinkeys,
```

### Comparing `pypreql-0.0.1rc8/preql/dialect/base.py` & `pypreql-0.0.1rc9/preql/dialect/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 
 GENERIC_SQL_TEMPLATE = Template(
     """{%- if ctes %}
 WITH {% for cte in ctes %}
 {{cte.name}} as ({{cte.statement}}){% if not loop.last %},{% endif %}{% endfor %}{% endif %}
 SELECT
-{%- if limit %}
+{%- if limit is not none %}
 TOP {{ limit }}{% endif %}
 {%- for select in select_columns %}
     {{ select }}{% if not loop.last %},{% endif %}{% endfor %}
 FROM
     {{ base }}{% if joins %}{% for join in joins %}
 {{ join }}{% endfor %}{% endif %}
 {% if where %}WHERE
@@ -182,14 +182,15 @@
                 name=cte.name,
                 statement=self.SQL_TEMPLATE.render(
                     select_columns=[
                         self.render_concept_sql(c, cte) for c in cte.output_columns
                     ],
                     base=f"{cte.base_name} as {cte.base_alias}",
                     grain=cte.grain,
+                    limit=None,
                     joins=[
                         render_join(join, self.QUOTE_CHARACTER)
                         for join in (cte.joins or [])
                     ],
                     where=self.render_expr(where_assignment[cte.name], cte)
                     if cte.name in where_assignment
                     else None,
@@ -224,14 +225,15 @@
             if isinstance(statement, Select):
                 output.append(process_query(environment, statement, hooks))
                 # graph = generate_graph(environment, statement)
                 # output.append(graph_to_query(environment, graph, statement))
         return output
 
     def compile_statement(self, query: ProcessedQuery) -> str:
+
         select_columns: list[str] = []
         cte_output_map = {}
         selected = set()
         output_addresses = [c.address for c in query.output_columns]
 
         # valid joins are anything that is a subset of the final grain
         output_ctes = [cte for cte in query.ctes if cte.grain.issubset(query.grain)]
@@ -290,14 +292,20 @@
                     "Cannot generate complex query with filtering on grain that does not match any source."
                 )
         for join in query.joins:
 
             if join.right_cte.name in where_assignment:
                 # force filtering if the CTE has a where clause
                 join.jointype = JoinType.INNER
+                # if the left source is partial, make it a full join
+            elif (
+                join.left_cte.grain.issubset(query.grain)
+                and join.left_cte.grain != query.grain
+            ):
+                join.jointype = JoinType.FULL
         compiled_ctes = self.generate_ctes(query, where_assignment)
         return self.SQL_TEMPLATE.render(
             select_columns=select_columns,
             base=query.base.name,
             joins=[render_join(join, self.QUOTE_CHARACTER) for join in query.joins],
             ctes=compiled_ctes,
             limit=query.limit,
```

### Comparing `pypreql-0.0.1rc8/preql/dialect/bigquery.py` & `pypreql-0.0.1rc9/preql/dialect/bigquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 GROUP BY {% for group in group_by %}
     {{group}}{% if not loop.last %},{% endif %}
 {% endfor %}{% endif %}
 {%- if order_by %}
 ORDER BY {% for order in order_by %}
     {{ order }}{% if not loop.last %},{% endif %}
 {% endfor %}{% endif %}
-{%- if limit %}
+{%- if limit is not none %}
 LIMIT {{ limit }}{% endif %}
 """
 )
 
 
 class BigqueryDialect(BaseDialect):
     WINDOW_FUNCTION_MAP = WINDOW_FUNCTION_MAP
```

### Comparing `pypreql-0.0.1rc8/preql/dialect/common.py` & `pypreql-0.0.1rc9/preql/dialect/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from typing import List
-
-from preql.core.models import CTE
-from preql.core.models import Join, OrderItem
+from preql.core.models import Join
 
 
 def render_join(join: Join, quote_character: str = '"') -> str:
     # {% for key in join.joinkeys %}{{ key.inner }} = {{ key.outer}}{% endfor %}
     joinkeys = " AND ".join(
         [
             f"{join.left_cte.name}.{quote_character}{key.concept.safe_address}{quote_character} = {join.right_cte.name}.{quote_character}{key.concept.safe_address}{quote_character}"
```

### Comparing `pypreql-0.0.1rc8/preql/dialect/duckdb.py` & `pypreql-0.0.1rc9/preql/dialect/duckdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 }
 
 DUCKDB_TEMPLATE = Template(
     """{%- if ctes %}
 WITH {% for cte in ctes %}
 {{cte.name}} as ({{cte.statement}}){% if not loop.last %},{% endif %}{% endfor %}{% endif %}
 SELECT
-{%- if limit %}
+{%- if limit is not none %}
 TOP {{ limit }}{% endif %}
 {%- for select in select_columns %}
     {{ select }}{% if not loop.last %},{% endif %}{% endfor %}
 FROM
     {{ base }}{% if joins %}
 {% for join in joins %}
 {{ join }}
```

### Comparing `pypreql-0.0.1rc8/preql/dialect/sql_server.py` & `pypreql-0.0.1rc9/preql/dialect/sql_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 }
 
 TSQL_TEMPLATE = Template(
     """{%- if ctes %}
 WITH {% for cte in ctes %}
 {{cte.name}} as ({{cte.statement}}){% if not loop.last %},{% endif %}{% endfor %}{% endif %}
 SELECT
-{%- if limit %}
+{%- if limit is not none %}
 TOP {{ limit }}{% endif %}
 {%- for select in select_columns %}
     {{ select }}{% if not loop.last %},{% endif %}{% endfor %}
 FROM
     {{ base }}{% if joins %}
 {% for join in joins %}
 {{ join }}
@@ -87,13 +87,10 @@
     QUOTE_CHARACTER = '"'
     SQL_TEMPLATE = TSQL_TEMPLATE
 
     def compile_statement(self, query: ProcessedQuery) -> str:
         base = super().compile_statement(query)
         for cte in query.ctes:
             if len(cte.name) > MAX_IDENTIFIER_LENGTH:
-                print("replacing")
-                print(cte.name)
                 new_name = f"rhash_{string_to_hash(cte.name)}"
-                print(new_name)
                 base = base.replace(cte.name, new_name)
         return base
```

### Comparing `pypreql-0.0.1rc8/preql/executor.py` & `pypreql-0.0.1rc9/preql/executor.py`

 * *Files identical despite different names*

### Comparing `pypreql-0.0.1rc8/preql/parsing/parse_engine.py` & `pypreql-0.0.1rc9/preql/parsing/parse_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,14 +341,15 @@
     def column_assignment_list(self, args):
         return args
 
     def column_list(self, args) -> List:
         return args
 
     def grain_clause(self, args) -> Grain:
+        #            namespace=self.environment.namespace,
         return Grain(components=[self.environment.concepts[a] for a in args[0]])
 
     @v_args(meta=True)
     def datasource(self, meta: Meta, args):
         name = args[0]
         columns: List[ColumnAssignment] = args[1]
         grain: Optional[Grain] = None
@@ -453,30 +454,27 @@
 
     def import_statement(self, args):
         alias = args[-1]
         path = args[0].split(".")
 
         target = join(self.environment.working_path, *path) + ".preql"
         with open(target, "r", encoding="utf-8") as f:
+
             text = f.read()
-            nparser = ParseToObjects(
-                visit_tokens=True,
-                text=text,
-                environment=Environment(working_path=dirname(target), namespace=alias),
-            )
-            nparser.transform(PARSER.parse(text))
+        nparser = ParseToObjects(
+            visit_tokens=True,
+            text=text,
+            environment=Environment(working_path=dirname(target), namespace=alias),
+        )
+        nparser.transform(PARSER.parse(text))
 
-            for key, concept in nparser.environment.concepts.items():
-                self.environment.concepts[f"{alias}.{key}"] = concept.with_namespace(
-                    alias
-                )
-            for key, datasource in nparser.environment.datasources.items():
-                self.environment.datasources[
-                    f"{alias}.{key}"
-                ] = datasource.with_namespace(alias)
+        for key, concept in nparser.environment.concepts.items():
+            self.environment.concepts[f"{alias}.{key}"] = concept
+        for key, datasource in nparser.environment.datasources.items():
+            self.environment.datasources[f"{alias}.{key}"] = datasource
         return None
 
     @v_args(meta=True)
     def select(self, meta: Meta, args):
 
         select_items = None
         limit = None
```

### Comparing `pypreql-0.0.1rc8/pypreql.egg-info/PKG-INFO` & `pypreql-0.0.1rc9/pypreql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pypreql
-Version: 0.0.1rc8
-Summary: Declarative, typed query lanuage.
+Version: 0.0.1rc9
+Summary: Declarative, typed query language that compiles to SQL.
 Home-page: 
 Author: 
 Author-email: preql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -143,8 +143,9 @@
 ```
 
 
 ## Contributing
 
 
 ## Similar in space
-singleorigin
+
+- singleorigin
```

### Comparing `pypreql-0.0.1rc8/pypreql.egg-info/SOURCES.txt` & `pypreql-0.0.1rc9/pypreql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypreql-0.0.1rc8/setup.py` & `pypreql-0.0.1rc9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 setuptools.setup(
     name="pypreql",
     version=version,
     url="",
     author="",
     author_email="preql-community@gmail.com",
-    description="Declarative, typed query lanuage.",
+    description="Declarative, typed query language that compiles to SQL.",
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(exclude=["dist", "build", "*.tests", "*.tests.*", "tests.*", "tests", "docs", ".github", "", "examples"]),
     package_data={
         "": ["*.tf", "*.jinja", "py.typed"],
     },
     install_requires=install_requires,
```


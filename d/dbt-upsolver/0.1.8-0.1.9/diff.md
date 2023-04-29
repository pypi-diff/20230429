# Comparing `tmp/dbt-upsolver-0.1.8.tar.gz` & `tmp/dbt-upsolver-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-upsolver-0.1.8.tar", last modified: Fri Apr 21 12:24:47 2023, max compression
+gzip compressed data, was "dbt-upsolver-0.1.9.tar", last modified: Sat Apr 29 21:26:14 2023, max compression
```

## Comparing `dbt-upsolver-0.1.8.tar` & `dbt-upsolver-0.1.9.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:24:47.953438 dbt-upsolver-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-21 12:24:47.953438 dbt-upsolver-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:24:47.945438 dbt-upsolver-0.1.8/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:24:47.945438 dbt-upsolver-0.1.8/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:24:47.949438 dbt-upsolver-0.1.8/dbt/adapters/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/adapters/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/adapters/upsolver/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/adapters/upsolver/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/adapters/upsolver/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:24:47.949438 dbt-upsolver-0.1.8/dbt/adapters/upsolver/options/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/adapters/upsolver/options/connection_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/adapters/upsolver/options/copy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/adapters/upsolver/options/table_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/adapters/upsolver/options/transformation_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/adapters/upsolver/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:24:47.945438 dbt-upsolver-0.1.8/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:24:47.949438 dbt-upsolver-0.1.8/dbt/include/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/include/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/include/upsolver/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:24:47.949438 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:24:47.949438 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/connection.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:24:47.949438 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/materializedview.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:24:47.949438 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/utils/create_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/utils/render_options.sql
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/dbt/include/upsolver/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:24:47.953438 dbt-upsolver-0.1.8/dbt_upsolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-21 12:24:47.000000 dbt-upsolver-0.1.8/dbt_upsolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-21 12:24:47.000000 dbt-upsolver-0.1.8/dbt_upsolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:24:47.000000 dbt-upsolver-0.1.8/dbt_upsolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:24:47.000000 dbt-upsolver-0.1.8/dbt_upsolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 12:24:47.000000 dbt-upsolver-0.1.8/dbt_upsolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-21 12:24:47.000000 dbt-upsolver-0.1.8/dbt_upsolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:24:47.953438 dbt-upsolver-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-21 12:24:30.000000 dbt-upsolver-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.815418 dbt-upsolver-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-04-29 21:26:14.815418 dbt-upsolver-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.807418 dbt-upsolver-0.1.9/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.807418 dbt-upsolver-0.1.9/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.811418 dbt-upsolver-0.1.9/dbt/adapters/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.811418 dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/connection_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/copy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/materialized_view_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/table_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/transformation_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.807418 dbt-upsolver-0.1.9/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.811418 dbt-upsolver-0.1.9/dbt/include/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.811418 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.811418 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/connection.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.811418 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/materializedview.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.815418 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/utils/create_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/utils/render_options.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.815418 dbt-upsolver-0.1.9/dbt_upsolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-04-29 21:26:14.000000 dbt-upsolver-0.1.9/dbt_upsolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-29 21:26:14.000000 dbt-upsolver-0.1.9/dbt_upsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:26:14.000000 dbt-upsolver-0.1.9/dbt_upsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:26:14.000000 dbt-upsolver-0.1.9/dbt_upsolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-29 21:26:14.000000 dbt-upsolver-0.1.9/dbt_upsolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-29 21:26:14.000000 dbt-upsolver-0.1.9/dbt_upsolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 21:26:14.815418 dbt-upsolver-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/setup.py
```

### Comparing `dbt-upsolver-0.1.8/LICENSE` & `dbt-upsolver-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.8/dbt/adapters/upsolver/connections.py` & `dbt-upsolver-0.1.9/dbt/adapters/upsolver/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.8/dbt/adapters/upsolver/impl.py` & `dbt-upsolver-0.1.9/dbt/adapters/upsolver/impl.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dbt.adapters.upsolver.relation import UpsolverRelation
 from typing import List
 from dbt.adapters.base.meta import available
 from dbt.adapters.upsolver.options.copy_options import Copy_options
 from dbt.adapters.upsolver.options.connection_options import Connection_options
 from dbt.adapters.upsolver.options.transformation_options import Transformation_options
 from dbt.adapters.upsolver.options.table_options import Table_options
+from dbt.adapters.upsolver.options.materialized_view_options import Materialized_view_options
 import agate
 import datetime
 import re
 
 logger = AdapterLogger("Upsolver")
 LIST_RELATION_MACRO_NAME = "list_relation_without_caching"
 
@@ -28,28 +29,24 @@
     def date_function(cls):
         """
         Returns canonical date func
         """
         return "datenow()"
 
     def debug_query(self) -> None:
-        self.execute('SELECT * FROM logs.logs.task_executions limit 1;')
+        self.execute('SELECT * FROM system.information_schema.jobs limit1;')
+
 
     def create_schema(self, relation: UpsolverRelation) -> None:
         pass
 
     def drop_schema(self, relation: UpsolverRelation) -> None:
         pass
 
     @available
-    def alter_datetime(self):
-        datetime_now = datetime.datetime.now()
-        return 'Altered: ' + datetime_now.strftime('%Y-%m-%d %H:%M:%S')
-
-    @available
     def get_connection_from_sql(self, sql):
         connection_identifier = re.search('"(.*)"', sql).group().split('.')[2] \
                                   .translate(str.maketrans({'\"':'', '\'':''}))
 
         return connection_identifier
 
     @available
@@ -96,18 +93,30 @@
     def get_options(self, source, options_type):
         if options_type == 'connection_options':
             options = Connection_options[source.lower()]
         elif options_type == 'transformation_options':
             options = Transformation_options[source.lower()]
         elif options_type == 'table_options':
             options = Table_options
+        elif options_type == 'materialized_view_options':
+            options = Materialized_view_options
         else:
             options = Copy_options[source.lower()][options_type]
         return options
 
+    @available
+    def get_delete_placeholder(self, sql, delete_condition):
+        if delete_condition:
+            delete_placeholder= re.search('(nettotal < 0 [as|AS,\s]*\w*)', sql)[1] \
+              .lower().replace(" ", "") \
+              .replace(f"{delete_condition.lower().replace(' ', '')}as", "")
+            return delete_placeholder
+        else:
+            return False
+
     def list_relations_without_caching(
         self,
         schema_relation: UpsolverRelation,
         ) -> List[UpsolverRelation]:
         materializations = ["table", "job", "connection", "view"]
         results = agate.Table([],[])
         for type in materializations:
```

### Comparing `dbt-upsolver-0.1.8/dbt/adapters/upsolver/options/connection_options.py` & `dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/connection_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.8/dbt/adapters/upsolver/options/copy_options.py` & `dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/copy_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.8/dbt/adapters/upsolver/options/table_options.py` & `dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/table_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.8/dbt/adapters/upsolver/options/transformation_options.py` & `dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/transformation_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.8/dbt/adapters/upsolver/relation.py` & `dbt-upsolver-0.1.9/dbt/adapters/upsolver/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.8/dbt/include/upsolver/macros/adapters.sql` & `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/connection.sql` & `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/connection.sql`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 
   {% set connection_type = config.require('connection_type') %}
   {% set connection_options = config.require('connection_options') %}
   {% set enriched_options = adapter.enrich_options(connection_options, connection_type, 'connection_options') %}
   {% set enriched_editable_options = adapter.filter_options(enriched_options, 'editable') %}
 
 
-
-  {%- set curr_datetime = adapter.alter_datetime() -%}
-
   {%- set old_relation = adapter.get_relation(identifier=identifier,
                                               schema=schema,
                                               database=database) -%}
   {%- set target_relation = api.Relation.create(identifier=identifier,
                                                 schema=schema,
                                                 database=database,
                                                 type="connection") -%}
```

### Comparing `dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql` & `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/incremental/incremental.sql` & `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/incremental.sql`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
   {%- set identifier = model['alias'] -%}
   {% set incremental_strategy = config.get('incremental_strategy', False) %}
   {% set partition_by = config.get('partition_by', []) %}
   {% set sync = config.get('sync', False) %}
   {% set options = config.get('options', {}) %}
   {% set source = config.get('source', none) %}
+  {% set delete_condition = config.get('delete_condition', False) %}
   {% set partition_by = config.get('partition_by', []) %}
   {% set primary_key = config.get('primary_key', []) %}
   {% set map_columns_by_name = config.get('map_columns_by_name', False) %}
   {% set job_identifier = identifier + '_job' %}
 
   {%- set old_relation = adapter.get_relation(identifier=job_identifier,
                                               schema=schema,
@@ -35,15 +36,15 @@
     {% call statement('main') -%}
       {{ get_alter_job_sql(job_identifier, options, incremental_strategy, source) }}
     {%- endcall %}
   {% else %}
     {% call statement('main') -%}
       {% if incremental_strategy == 'merge' %}
         {{ get_create_merge_job_sql(job_identifier, table_relation, sync,
-                                    options, primary_key) }}
+                                    options, primary_key, delete_condition) }}
       {% elif incremental_strategy == 'insert' %}
         {{ get_create_incert_job_sql(job_identifier,
                                     table_relation, sync, options,
                                     map_columns_by_name) }}
 
       {% else  %}
         {{ get_create_copy_job_sql(job_identifier, sql,
```

### Comparing `dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/materializedview.sql` & `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/materializedview.sql`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 {% materialization materializedview, adapter='upsolver' %}
   {%- set identifier = model['alias'] -%}
-  {% set sync = config.get('sync', '') %}
-  {% set options = config.require('options') %}
-  {%- set curr_datetime = adapter.alter_datetime() -%}
+  {% set sync = config.get('sync', False) %}
+  {% set options = config.get('options', {}) %}
+  {% set enriched_options = adapter.enrich_options(options, None, 'materialized_view_options') %}
+  {% set enriched_editable_options = adapter.filter_options(enriched_options, 'editable') %}
 
   {%- set old_relation = adapter.get_relation(identifier=identifier,
                                               schema=schema,
                                               database=database) -%}
   {%- set target_relation = api.Relation.create(identifier=identifier,
                                                 schema=schema,
                                                 database=database,
                                                 type="materializedview") -%}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
     {% if old_relation %}
       {% call statement('main') -%}
-        ALTER MATERIALIZED VIEW {{target_relation.database}}.{{target_relation.schema}}.{{target_relation.identifier}}
-          {% for k, v in options.items() %}
-            SET {{k}} = {{v}}
-          {% endfor %}
+        ALTER MATERIALIZED VIEW {{target_relation}}
+          {{ render_options(enriched_editable_options, 'alter') }}
       {%- endcall %}
     {% else %}
       {% call statement('main') -%}
-        CREATE {{ sync }} MATERIALIZED VIEW  {{target_relation.database}}.{{target_relation.schema}}.{{target_relation.identifier}} AS
+        CREATE
+        {% if sync %}
+          SYNC
+        {% endif %}
+        MATERIALIZED VIEW  {{target_relation}} AS
         {{ sql }}
-        {% for k, v in options.items() %}
-          SET {{k}} = {{v}}
-        {% endfor %}
-
+        {{ render_options(enriched_options, 'create') }}
       {%- endcall %}
     {% endif %}
 
   {% do persist_docs(target_relation, model) %}
 
   {{ run_hooks(post_hooks, inside_transaction=False) }}
   {{ run_hooks(post_hooks, inside_transaction=True) }}
```

### Comparing `dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/utils/ater_job.sql` & `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/utils/ater_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.8/dbt/include/upsolver/macros/materializations/utils/create_table.sql` & `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/utils/create_table.sql`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 {% macro get_create_table_if_not_exists_sql(target_relation, partition_by, primary_key, options) -%}
 
 {%- set old_relation = adapter.get_relation(identifier=target_relation.identifier,
                                             schema=target_relation.schema,
                                             database=target_relation.database) -%}
 
-  {%- set curr_datetime = adapter.alter_datetime() -%}
   {%- set columns_with_types = adapter.get_columns_names_with_types(partition_by + primary_key) -%}
   {%- set columns_partitioned_by  = adapter.get_columns_names(partition_by) -%}
   {%- set columns_primary_key  = adapter.get_columns_names(primary_key) -%}
   {% set enriched_options = adapter.enrich_options(options, None, 'table_options') %}
   {% set enriched_editable_options = adapter.filter_options(enriched_options, 'editable') %}
 
   {% if old_relation %}
```

### Comparing `dbt-upsolver-0.1.8/dbt_upsolver.egg-info/SOURCES.txt` & `dbt-upsolver-0.1.9/dbt_upsolver.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 dbt/adapters/upsolver/__init__.py
 dbt/adapters/upsolver/__version__.py
 dbt/adapters/upsolver/connections.py
 dbt/adapters/upsolver/impl.py
 dbt/adapters/upsolver/relation.py
 dbt/adapters/upsolver/options/connection_options.py
 dbt/adapters/upsolver/options/copy_options.py
+dbt/adapters/upsolver/options/materialized_view_options.py
 dbt/adapters/upsolver/options/table_options.py
 dbt/adapters/upsolver/options/transformation_options.py
 dbt/include/upsolver/__init__.py
 dbt/include/upsolver/dbt_project.yml
 dbt/include/upsolver/profile_template.yml
 dbt/include/upsolver/macros/adapters.sql
 dbt/include/upsolver/macros/catalog.sql
```

### Comparing `dbt-upsolver-0.1.8/setup.py` & `dbt-upsolver-0.1.9/setup.py`

 * *Files identical despite different names*


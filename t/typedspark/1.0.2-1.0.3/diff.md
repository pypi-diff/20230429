# Comparing `tmp/typedspark-1.0.2.tar.gz` & `tmp/typedspark-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedspark-1.0.2.tar", last modified: Tue Apr 18 09:39:53 2023, max compression
+gzip compressed data, was "typedspark-1.0.3.tar", last modified: Sat Apr 29 18:03:11 2023, max compression
```

## Comparing `typedspark-1.0.2.tar` & `typedspark-1.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:53.691731 typedspark-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 09:39:40.000000 typedspark-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-18 09:39:53.691731 typedspark-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-18 09:39:40.000000 typedspark-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-18 09:39:40.000000 typedspark-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:39:53.691731 typedspark-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-18 09:39:40.000000 typedspark-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:53.687730 typedspark-1.0.2/typedspark/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:53.687730 typedspark-1.0.2/typedspark/_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_core/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_core/column_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_core/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_core/validate_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:53.687730 typedspark-1.0.2/typedspark/_schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_schema/dlt_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_schema/get_schema_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_schema/get_schema_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_schema/structfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:53.687730 typedspark-1.0.2/typedspark/_transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_transforms/structtype_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_transforms/transform_to_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_transforms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:53.687730 typedspark-1.0.2/typedspark/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_utils/create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_utils/load_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/_utils/register_schema_to_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:40.000000 typedspark-1.0.2/typedspark/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:39:53.687730 typedspark-1.0.2/typedspark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-18 09:39:53.000000 typedspark-1.0.2/typedspark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-18 09:39:53.000000 typedspark-1.0.2/typedspark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:39:53.000000 typedspark-1.0.2/typedspark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 09:39:53.000000 typedspark-1.0.2/typedspark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 09:39:53.000000 typedspark-1.0.2/typedspark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:03:11.155666 typedspark-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 18:02:57.000000 typedspark-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-29 18:03:11.155666 typedspark-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-29 18:02:57.000000 typedspark-1.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-29 18:02:57.000000 typedspark-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:03:11.155666 typedspark-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-29 18:02:57.000000 typedspark-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:03:11.155666 typedspark-1.0.3/typedspark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:03:11.155666 typedspark-1.0.3/typedspark/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_core/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_core/column_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_core/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_core/validate_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:03:11.155666 typedspark-1.0.3/typedspark/_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_schema/dlt_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_schema/get_schema_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_schema/get_schema_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_schema/structfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:03:11.155666 typedspark-1.0.3/typedspark/_transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_transforms/structtype_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_transforms/transform_to_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_transforms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:03:11.155666 typedspark-1.0.3/typedspark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_utils/create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_utils/load_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/_utils/register_schema_to_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:02:57.000000 typedspark-1.0.3/typedspark/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:03:11.155666 typedspark-1.0.3/typedspark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-29 18:03:11.000000 typedspark-1.0.3/typedspark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-29 18:03:11.000000 typedspark-1.0.3/typedspark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:03:11.000000 typedspark-1.0.3/typedspark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-29 18:03:11.000000 typedspark-1.0.3/typedspark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 18:03:11.000000 typedspark-1.0.3/typedspark.egg-info/top_level.txt
```

### Comparing `typedspark-1.0.2/LICENSE.txt` & `typedspark-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/PKG-INFO` & `typedspark-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.0.2
+Version: 1.0.3
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
@@ -54,14 +54,16 @@
 * Easy refactoring of column names
 * Easier unit testing through the generation of empty ``DataSets`` based on their schemas
 * Improved documentation of tables
 
 Installation
 ============
 
+You can install ``typedspark`` from `pypi <https://pypi.org/project/typedspark/>`_ by running:
+
 .. code-block:: bash
 
     pip install typedspark
 
 By default, ``typedspark`` does not list ``pyspark`` as a dependency, since many platforms (e.g. Databricks) come with ``pyspark`` preinstalled.  If you want to install ``typedspark`` with ``pyspark``, you can run:
 
 .. code-block:: bash
```

### Comparing `typedspark-1.0.2/README.rst` & `typedspark-1.0.3/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 * Easy refactoring of column names
 * Easier unit testing through the generation of empty ``DataSets`` based on their schemas
 * Improved documentation of tables
 
 Installation
 ============
 
+You can install ``typedspark`` from `pypi <https://pypi.org/project/typedspark/>`_ by running:
+
 .. code-block:: bash
 
     pip install typedspark
 
 By default, ``typedspark`` does not list ``pyspark`` as a dependency, since many platforms (e.g. Databricks) come with ``pyspark`` preinstalled.  If you want to install ``typedspark`` with ``pyspark``, you can run:
 
 .. code-block:: bash
```

### Comparing `typedspark-1.0.2/pyproject.toml` & `typedspark-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/setup.py` & `typedspark-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark/__init__.py` & `typedspark-1.0.3/typedspark/__init__.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark/_core/column.py` & `typedspark-1.0.3/typedspark/_core/column.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark/_core/column_meta.py` & `typedspark-1.0.3/typedspark/_core/column_meta.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark/_core/dataset.py` & `typedspark-1.0.3/typedspark/_core/dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark/_core/datatypes.py` & `typedspark-1.0.3/typedspark/_core/datatypes.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark/_core/validate_schema.py` & `typedspark-1.0.3/typedspark/_core/validate_schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark/_schema/get_schema_definition.py` & `typedspark-1.0.3/typedspark/_schema/get_schema_definition.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark/_schema/get_schema_imports.py` & `typedspark-1.0.3/typedspark/_schema/get_schema_imports.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,32 +28,44 @@
     encountered_datatypes: set[Type[DataType]] = set()
     for column in get_type_hints(schema).values():
         args = get_args(column)
         if not args:
             continue
 
         dtype = args[0]
-        origin: Optional[Type[DataType]] = get_origin(dtype)
-        if origin:
-            encountered_datatypes.add(origin)
-        else:
-            encountered_datatypes.add(dtype)
-
-        if origin == MapType:
-            key, value = get_args(dtype)
-            encountered_datatypes.add(key)
-            encountered_datatypes.add(value)
-
-        if origin == ArrayType:
-            element = get_args(dtype)[0]
-            encountered_datatypes.add(element)
-
-        if get_origin(dtype) == StructType:
-            subschema = get_args(dtype)[0]
-            encountered_datatypes |= _get_imported_dtypes(subschema)
+        encountered_datatypes |= _process_datatype(dtype)
+
+    return encountered_datatypes
+
+
+def _process_datatype(dtype: Type[DataType]) -> set[Type[DataType]]:
+    """Returns a set of DataTypes that are imported for a given DataType.
+
+    Handles nested DataTypes recursively.
+    """
+    encountered_datatypes: set[Type[DataType]] = set()
+
+    origin: Optional[Type[DataType]] = get_origin(dtype)
+    if origin:
+        encountered_datatypes.add(origin)
+    else:
+        encountered_datatypes.add(dtype)
+
+    if origin == MapType:
+        key, value = get_args(dtype)
+        encountered_datatypes |= _process_datatype(key)
+        encountered_datatypes |= _process_datatype(value)
+
+    if origin == ArrayType:
+        element = get_args(dtype)[0]
+        encountered_datatypes |= _process_datatype(element)
+
+    if get_origin(dtype) == StructType:
+        subschema = get_args(dtype)[0]
+        encountered_datatypes |= _get_imported_dtypes(subschema)
 
     return encountered_datatypes
 
 
 def _build_import_string(
     encountered_datatypes: set[Type[DataType]], include_documentation: bool
 ) -> str:
```

### Comparing `typedspark-1.0.2/typedspark/_schema/schema.py` & `typedspark-1.0.3/typedspark/_schema/schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark/_schema/structfield.py` & `typedspark-1.0.3/typedspark/_schema/structfield.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark/_transforms/structtype_column.py` & `typedspark-1.0.3/typedspark/_transforms/structtype_column.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark/_transforms/transform_to_schema.py` & `typedspark-1.0.3/typedspark/_transforms/transform_to_schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark/_transforms/utils.py` & `typedspark-1.0.3/typedspark/_transforms/utils.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark/_utils/create_dataset.py` & `typedspark-1.0.3/typedspark/_utils/create_dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark/_utils/load_table.py` & `typedspark-1.0.3/typedspark/_utils/load_table.py`

 * *Files identical despite different names*

```diff
@@ -59,13 +59,12 @@
     This allows for autocompletion on column names, amongst other
     things.
 
     .. code-block:: python
 
         df, Person = load_table(spark, "path.to.table")
     """
-
     dataframe = spark.table(table_name)
     schema = _create_schema(dataframe.schema)
     dataset = DataSet[schema](dataframe)  # type: ignore
     schema = register_schema_to_dataset(dataset, schema)
     return dataset, schema
```

### Comparing `typedspark-1.0.2/typedspark/_utils/register_schema_to_dataset.py` & `typedspark-1.0.3/typedspark/_utils/register_schema_to_dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.2/typedspark.egg-info/PKG-INFO` & `typedspark-1.0.3/typedspark.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.0.2
+Version: 1.0.3
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
@@ -54,14 +54,16 @@
 * Easy refactoring of column names
 * Easier unit testing through the generation of empty ``DataSets`` based on their schemas
 * Improved documentation of tables
 
 Installation
 ============
 
+You can install ``typedspark`` from `pypi <https://pypi.org/project/typedspark/>`_ by running:
+
 .. code-block:: bash
 
     pip install typedspark
 
 By default, ``typedspark`` does not list ``pyspark`` as a dependency, since many platforms (e.g. Databricks) come with ``pyspark`` preinstalled.  If you want to install ``typedspark`` with ``pyspark``, you can run:
 
 .. code-block:: bash
```

### Comparing `typedspark-1.0.2/typedspark.egg-info/SOURCES.txt` & `typedspark-1.0.3/typedspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*


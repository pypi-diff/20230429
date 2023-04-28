# Comparing `tmp/featurizerai-1.6.0.tar.gz` & `tmp/featurizerai-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.6.0.tar", last modified: Fri Apr 28 23:22:56 2023, max compression
+gzip compressed data, was "featurizerai-1.6.1.tar", last modified: Fri Apr 28 23:32:27 2023, max compression
```

## Comparing `featurizerai-1.6.0.tar` & `featurizerai-1.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:22:56.205982 featurizerai-1.6.0/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.6.0/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.6.0/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 23:22:56.206047 featurizerai-1.6.0/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.6.0/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 23:22:56.206264 featurizerai-1.6.0/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 23:22:49.000000 featurizerai-1.6.0/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:22:56.202070 featurizerai-1.6.0/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:22:56.204088 featurizerai-1.6.0/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.6.0/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.6.0/src/features/authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.6.0/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.6.0/src/features/custom_schema.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     5025 2023-04-28 23:22:42.000000 featurizerai-1.6.0/src/features/materialize.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:22:56.204956 featurizerai-1.6.0/src/features/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.6.0/src/features/tests/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     2766 2023-04-28 14:47:29.000000 featurizerai-1.6.0/src/features/tests/test_materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.6.0/src/features/tests/test_pipeline.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:22:56.205842 featurizerai-1.6.0/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 23:22:56.000000 featurizerai-1.6.0/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 23:22:56.000000 featurizerai-1.6.0/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 23:22:56.000000 featurizerai-1.6.0/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 23:22:56.000000 featurizerai-1.6.0/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 23:22:56.000000 featurizerai-1.6.0/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:32:27.410240 featurizerai-1.6.1/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.6.1/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.6.1/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 23:32:27.410308 featurizerai-1.6.1/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.6.1/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 23:32:27.410516 featurizerai-1.6.1/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 23:32:15.000000 featurizerai-1.6.1/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:32:27.405855 featurizerai-1.6.1/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:32:27.407925 featurizerai-1.6.1/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.6.1/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.6.1/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.6.1/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.6.1/src/features/custom_schema.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     5024 2023-04-28 23:32:08.000000 featurizerai-1.6.1/src/features/materialize.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:32:27.409244 featurizerai-1.6.1/src/features/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.6.1/src/features/tests/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     2766 2023-04-28 14:47:29.000000 featurizerai-1.6.1/src/features/tests/test_materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.6.1/src/features/tests/test_pipeline.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:32:27.410125 featurizerai-1.6.1/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 23:32:27.000000 featurizerai-1.6.1/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 23:32:27.000000 featurizerai-1.6.1/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 23:32:27.000000 featurizerai-1.6.1/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 23:32:27.000000 featurizerai-1.6.1/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 23:32:27.000000 featurizerai-1.6.1/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.6.0/LICENSE` & `featurizerai-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.6.0/PKG-INFO` & `featurizerai-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.6.0/setup.py` & `featurizerai-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.6.0',
+    version='1.6.1',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.6.0/src/features/authenticate.py` & `featurizerai-1.6.1/src/features/authenticate.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.6.0/src/features/create_stream.py` & `featurizerai-1.6.1/src/features/create_stream.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.6.0/src/features/custom_schema.py` & `featurizerai-1.6.1/src/features/custom_schema.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.6.0/src/features/materialize.py` & `featurizerai-1.6.1/src/features/materialize.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,30 +86,30 @@
         # Execute the dynamic Spark SQL
         for sql in self.sparksql:
             sql_base = sql.replace("{"+ self.groupby_attr + "}", str(self.groupby))
             hour = int(sql.split("_")[3])
             sql_with_timestamp = sql_base.replace("{timestamp}", str(int((start_time - timedelta(hours=hour)).timestamp())))
             sql_with_timestamp_base = sql_with_timestamp.replace("{timestamp_base}", str(int((start_time).timestamp())))
             c_count = self.spark.sql(sql_with_timestamp_base)
-            print(c_count)
+            c_count.show()
             result_df = result_df.join(c_count, self.groupby_attr, "full") \
                 .select(result_df.columns + [col for col in c_count.columns if col not in result_df.columns])
-            print(result_df)
+            result_df.show()
         # Convert the aggregated data to JSON
-        print(result_df)
+        result_df.show()
 
         if result_df.isEmpty():
             json_aggregated_data = "{'error': 'No data found'}"
         else:
             print(result_df.toJSON())
             json_aggregated_data = result_df.toJSON()
 
         if json_aggregated_data is not None:
             aggregated_data_collection.update_one(
-                {"date": start_time, self.groupby_attr: self.groupby},
+                {"date": start_time, "aggregated_key": self.groupby},
                 {"$set": {"aggregated_data": json_aggregated_data}},
                 upsert=True
             )
         else:
             logging.error("Serialized aggregated data is None, skipping update")
 
         return json_aggregated_data
```

### Comparing `featurizerai-1.6.0/src/features/tests/test_materialize.py` & `featurizerai-1.6.1/src/features/tests/test_materialize.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.6.0/src/features/tests/test_pipeline.py` & `featurizerai-1.6.1/src/features/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.6.0/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.6.1/src/featurizerai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```


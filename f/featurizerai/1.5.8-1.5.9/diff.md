# Comparing `tmp/featurizerai-1.5.8.tar.gz` & `tmp/featurizerai-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.5.8.tar", last modified: Fri Apr 28 21:55:39 2023, max compression
+gzip compressed data, was "featurizerai-1.5.9.tar", last modified: Fri Apr 28 22:00:35 2023, max compression
```

## Comparing `featurizerai-1.5.8.tar` & `featurizerai-1.5.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:55:39.098312 featurizerai-1.5.8/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.5.8/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.5.8/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 21:55:39.098383 featurizerai-1.5.8/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.5.8/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 21:55:39.098613 featurizerai-1.5.8/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 21:55:26.000000 featurizerai-1.5.8/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:55:39.094303 featurizerai-1.5.8/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:55:39.096418 featurizerai-1.5.8/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.5.8/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.5.8/src/features/authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.5.8/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.5.8/src/features/custom_schema.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4946 2023-04-28 21:54:27.000000 featurizerai-1.5.8/src/features/materialize.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:55:39.097208 featurizerai-1.5.8/src/features/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.5.8/src/features/tests/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     2766 2023-04-28 14:47:29.000000 featurizerai-1.5.8/src/features/tests/test_materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.5.8/src/features/tests/test_pipeline.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:55:39.098099 featurizerai-1.5.8/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 21:55:39.000000 featurizerai-1.5.8/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 21:55:39.000000 featurizerai-1.5.8/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 21:55:39.000000 featurizerai-1.5.8/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 21:55:39.000000 featurizerai-1.5.8/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 21:55:39.000000 featurizerai-1.5.8/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 22:00:35.324458 featurizerai-1.5.9/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.5.9/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.5.9/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 22:00:35.324525 featurizerai-1.5.9/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.5.9/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 22:00:35.324747 featurizerai-1.5.9/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 22:00:25.000000 featurizerai-1.5.9/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 22:00:35.320568 featurizerai-1.5.9/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 22:00:35.322729 featurizerai-1.5.9/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.5.9/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.5.9/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.5.9/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.5.9/src/features/custom_schema.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     5010 2023-04-28 22:00:25.000000 featurizerai-1.5.9/src/features/materialize.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 22:00:35.323395 featurizerai-1.5.9/src/features/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.5.9/src/features/tests/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     2766 2023-04-28 14:47:29.000000 featurizerai-1.5.9/src/features/tests/test_materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.5.9/src/features/tests/test_pipeline.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 22:00:35.324317 featurizerai-1.5.9/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 22:00:35.000000 featurizerai-1.5.9/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 22:00:35.000000 featurizerai-1.5.9/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 22:00:35.000000 featurizerai-1.5.9/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 22:00:35.000000 featurizerai-1.5.9/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 22:00:35.000000 featurizerai-1.5.9/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.5.8/LICENSE` & `featurizerai-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.8/PKG-INFO` & `featurizerai-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.5.8
+Version: 1.5.9
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.5.8/setup.py` & `featurizerai-1.5.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.5.8',
+    version='1.5.9',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.5.8/src/features/authenticate.py` & `featurizerai-1.5.9/src/features/authenticate.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.8/src/features/create_stream.py` & `featurizerai-1.5.9/src/features/create_stream.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.8/src/features/custom_schema.py` & `featurizerai-1.5.9/src/features/custom_schema.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.8/src/features/materialize.py` & `featurizerai-1.5.9/src/features/materialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,15 +95,17 @@
 
         # Convert the aggregated data to JSON
         print(result_df)
 
         if result_df.isEmpty():
             json_aggregated_data = "{'error': 'No data found'}"
         else:
-            json_aggregated_data = result_df.toJSON().collect()[-1]
+            print(result_df.toJSON())
+            json_aggregated_data = result_df.toJSON()
+            print(json_aggregated_data)
 
         if json_aggregated_data is not None:
             aggregated_data_collection.update_one(
                 {"date": start_time, self.groupby_attr: self.groupby},
                 {"$set": {"aggregated_data": json_aggregated_data}},
                 upsert=True
             )
```

### Comparing `featurizerai-1.5.8/src/features/tests/test_materialize.py` & `featurizerai-1.5.9/src/features/tests/test_materialize.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.8/src/features/tests/test_pipeline.py` & `featurizerai-1.5.9/src/features/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.8/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.5.9/src/featurizerai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.5.8
+Version: 1.5.9
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```


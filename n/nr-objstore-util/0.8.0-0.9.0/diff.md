# Comparing `tmp/nr_objstore_util-0.8.0.tar.gz` & `tmp/nr_objstore_util-0.9.0.tar.gz`

## Comparing `nr_objstore_util-0.8.0.tar` & `nr_objstore_util-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nr_objstore_util-0.8.0/requirements.txt
--rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 nr_objstore_util-0.8.0/src/NRUtil/NRObjStoreUtil.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nr_objstore_util-0.8.0/src/NRUtil/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nr_objstore_util-0.8.0/src/NRUtil/__init__.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 nr_objstore_util-0.8.0/src/NRUtil/constants.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 nr_objstore_util-0.8.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nr_objstore_util-0.8.0/LICENSE
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 nr_objstore_util-0.8.0/README.md
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nr_objstore_util-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 nr_objstore_util-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nr_objstore_util-0.9.0/requirements.txt
+-rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 nr_objstore_util-0.9.0/src/NRUtil/NRObjStoreUtil.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nr_objstore_util-0.9.0/src/NRUtil/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nr_objstore_util-0.9.0/src/NRUtil/__init__.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 nr_objstore_util-0.9.0/src/NRUtil/constants.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 nr_objstore_util-0.9.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nr_objstore_util-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 nr_objstore_util-0.9.0/README.md
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nr_objstore_util-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 nr_objstore_util-0.9.0/PKG-INFO
```

### Comparing `nr_objstore_util-0.8.0/src/NRUtil/NRObjStoreUtil.py` & `nr_objstore_util-0.9.0/src/NRUtil/NRObjStoreUtil.py`

 * *Files identical despite different names*

### Comparing `nr_objstore_util-0.8.0/src/NRUtil/constants.py` & `nr_objstore_util-0.9.0/src/NRUtil/constants.py`

 * *Files identical despite different names*

### Comparing `nr_objstore_util-0.8.0/.gitignore` & `nr_objstore_util-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nr_objstore_util-0.8.0/LICENSE` & `nr_objstore_util-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nr_objstore_util-0.8.0/README.md` & `nr_objstore_util-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nr_objstore_util-0.8.0/pyproject.toml` & `nr_objstore_util-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nr_objstore_util-0.8.0/PKG-INFO` & `nr_objstore_util-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nr_objstore_util
-Version: 0.8.0
+Version: 0.9.0
 Summary: Utility to bundle commonly used object store operations into an easy to use module
 Project-URL: Homepage, https://github.com/bcgov/nr-objectstore-util
 Project-URL: Bug Tracker, https://github.com/bcgov/nr-objectstore-util/issues
 Author-email: Kevin Netherton <kevin.netherton@gov.bc.ca>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: boto3==1.26.87
-Requires-Dist: minio==7.1.0
+Requires-Dist: boto3==1.26.99
+Requires-Dist: minio==7.1.14
 Requires-Dist: python-dotenv==1.0.0
 Description-Content-Type: text/markdown
 
 [![Lifecycle:Maturing](https://img.shields.io/badge/Lifecycle-Maturing-007EC6)](<Redirect-URL>)
 
 # Object Storage / S3 Utility Methods
```


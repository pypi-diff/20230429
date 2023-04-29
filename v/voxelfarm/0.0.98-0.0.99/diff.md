# Comparing `tmp/voxelfarm-0.0.98.tar.gz` & `tmp/voxelfarm-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxelfarm-0.0.98.tar", last modified: Fri Feb 17 20:19:43 2023, max compression
+gzip compressed data, was "voxelfarm-0.0.99.tar", last modified: Fri Feb 17 20:24:08 2023, max compression
```

## Comparing `voxelfarm-0.0.98.tar` & `voxelfarm-0.0.99.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-02-17 20:19:43.537032 voxelfarm-0.0.98/
--rw-rw-rw-   0        0        0     1093 2022-10-18 20:11:03.000000 voxelfarm-0.0.98/LICENSE
--rw-rw-rw-   0        0        0     2058 2023-02-17 20:19:43.534031 voxelfarm-0.0.98/PKG-INFO
--rw-rw-rw-   0        0        0     1457 2022-10-18 20:11:03.000000 voxelfarm-0.0.98/README.md
--rw-rw-rw-   0        0        0       86 2022-10-18 20:11:03.000000 voxelfarm-0.0.98/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-17 20:19:43.537032 voxelfarm-0.0.98/setup.cfg
--rw-rw-rw-   0        0        0     1059 2023-02-17 20:19:37.000000 voxelfarm-0.0.98/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-17 20:19:43.472900 voxelfarm-0.0.98/src/
-drwxrwxrwx   0        0        0        0 2023-02-17 20:19:43.513510 voxelfarm-0.0.98/src/voxelfarm/
--rw-rw-rw-   0        0        0    18490 2023-02-17 19:58:28.000000 voxelfarm-0.0.98/src/voxelfarm/__init__.py
--rw-rw-rw-   0        0        0     7204 2022-10-18 20:21:24.000000 voxelfarm-0.0.98/src/voxelfarm/block_model.py
--rw-rw-rw-   0        0        0     2719 2022-11-17 21:38:53.000000 voxelfarm-0.0.98/src/voxelfarm/generator_lambda.py
--rw-rw-rw-   0        0        0    16075 2023-02-17 20:19:33.000000 voxelfarm-0.0.98/src/voxelfarm/process_lambda.py
--rw-rw-rw-   0        0        0    16399 2023-02-02 17:44:21.000000 voxelfarm-0.0.98/src/voxelfarm/report_lambda.py
--rw-rw-rw-   0        0        0    15810 2023-02-01 19:43:58.000000 voxelfarm-0.0.98/src/voxelfarm/view_lambda.py
--rw-rw-rw-   0        0        0    68961 2023-02-16 21:54:40.000000 voxelfarm-0.0.98/src/voxelfarm/voxelfarmclient.py
--rw-rw-rw-   0        0        0    44460 2023-02-16 21:54:37.000000 voxelfarm-0.0.98/src/voxelfarm/workflow_lambda.py
-drwxrwxrwx   0        0        0        0 2023-02-17 20:19:43.530032 voxelfarm-0.0.98/src/voxelfarm.egg-info/
--rw-rw-rw-   0        0        0     2058 2023-02-17 20:19:43.000000 voxelfarm-0.0.98/src/voxelfarm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-02-17 20:19:43.000000 voxelfarm-0.0.98/src/voxelfarm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-17 20:19:43.000000 voxelfarm-0.0.98/src/voxelfarm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-02-17 20:19:43.000000 voxelfarm-0.0.98/src/voxelfarm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-17 20:19:43.000000 voxelfarm-0.0.98/src/voxelfarm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-17 20:24:08.400721 voxelfarm-0.0.99/
+-rw-rw-rw-   0        0        0     1093 2022-10-18 20:11:03.000000 voxelfarm-0.0.99/LICENSE
+-rw-rw-rw-   0        0        0     2058 2023-02-17 20:24:08.398722 voxelfarm-0.0.99/PKG-INFO
+-rw-rw-rw-   0        0        0     1457 2022-10-18 20:11:03.000000 voxelfarm-0.0.99/README.md
+-rw-rw-rw-   0        0        0       86 2022-10-18 20:11:03.000000 voxelfarm-0.0.99/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-02-17 20:24:08.401722 voxelfarm-0.0.99/setup.cfg
+-rw-rw-rw-   0        0        0     1059 2023-02-17 20:24:01.000000 voxelfarm-0.0.99/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-17 20:24:08.337724 voxelfarm-0.0.99/src/
+drwxrwxrwx   0        0        0        0 2023-02-17 20:24:08.379724 voxelfarm-0.0.99/src/voxelfarm/
+-rw-rw-rw-   0        0        0    18490 2023-02-17 19:58:28.000000 voxelfarm-0.0.99/src/voxelfarm/__init__.py
+-rw-rw-rw-   0        0        0     7204 2022-10-18 20:21:24.000000 voxelfarm-0.0.99/src/voxelfarm/block_model.py
+-rw-rw-rw-   0        0        0     2719 2022-11-17 21:38:53.000000 voxelfarm-0.0.99/src/voxelfarm/generator_lambda.py
+-rw-rw-rw-   0        0        0    16079 2023-02-17 20:23:56.000000 voxelfarm-0.0.99/src/voxelfarm/process_lambda.py
+-rw-rw-rw-   0        0        0    16399 2023-02-02 17:44:21.000000 voxelfarm-0.0.99/src/voxelfarm/report_lambda.py
+-rw-rw-rw-   0        0        0    15810 2023-02-01 19:43:58.000000 voxelfarm-0.0.99/src/voxelfarm/view_lambda.py
+-rw-rw-rw-   0        0        0    68961 2023-02-16 21:54:40.000000 voxelfarm-0.0.99/src/voxelfarm/voxelfarmclient.py
+-rw-rw-rw-   0        0        0    44460 2023-02-16 21:54:37.000000 voxelfarm-0.0.99/src/voxelfarm/workflow_lambda.py
+drwxrwxrwx   0        0        0        0 2023-02-17 20:24:08.395721 voxelfarm-0.0.99/src/voxelfarm.egg-info/
+-rw-rw-rw-   0        0        0     2058 2023-02-17 20:24:08.000000 voxelfarm-0.0.99/src/voxelfarm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-02-17 20:24:08.000000 voxelfarm-0.0.99/src/voxelfarm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-17 20:24:08.000000 voxelfarm-0.0.99/src/voxelfarm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-02-17 20:24:08.000000 voxelfarm-0.0.99/src/voxelfarm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-02-17 20:24:08.000000 voxelfarm-0.0.99/src/voxelfarm.egg-info/top_level.txt
```

### Comparing `voxelfarm-0.0.98/LICENSE` & `voxelfarm-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `voxelfarm-0.0.98/PKG-INFO` & `voxelfarm-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxelfarm
-Version: 0.0.98
+Version: 0.0.99
 Summary: Voxel Farm Python Lambdas
 Home-page: https://www.voxelfarm.com/help/PythonCookbook.html
 Author: Voxel Farm Contant
 Author-email: contant@voxelfarm.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/voxelfarm/voxelfarmclient/issues
 Platform: UNKNOWN
```

### Comparing `voxelfarm-0.0.98/README.md` & `voxelfarm-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `voxelfarm-0.0.98/setup.py` & `voxelfarm-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="voxelfarm",
-    version="0.0.98",
+    version="0.0.99",
     author="Voxel Farm Contant",
     author_email="contant@voxelfarm.com",
     description="Voxel Farm Python Lambdas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.voxelfarm.com/help/PythonCookbook.html",
     project_urls={
```

### Comparing `voxelfarm-0.0.98/src/voxelfarm/__init__.py` & `voxelfarm-0.0.99/src/voxelfarm/__init__.py`

 * *Files identical despite different names*

### Comparing `voxelfarm-0.0.98/src/voxelfarm/block_model.py` & `voxelfarm-0.0.99/src/voxelfarm/block_model.py`

 * *Files identical despite different names*

### Comparing `voxelfarm-0.0.98/src/voxelfarm/generator_lambda.py` & `voxelfarm-0.0.99/src/voxelfarm/generator_lambda.py`

 * *Files identical despite different names*

### Comparing `voxelfarm-0.0.98/src/voxelfarm/process_lambda.py` & `voxelfarm-0.0.99/src/voxelfarm/process_lambda.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,17 +453,17 @@
             fields=fields, 
             inputs=inputs,
             code=code,
             type='PROCESS',
             files=verified_files, 
             callback=None)
 
-    def create_entity_raw(self, type, name, fields, files):
+    def create_entity_raw(self, type, name, fields, files = None):
         result = self.vf_api.create_entity_raw(self.project, type, name, fields, self.crs)
-        if apiResult.success:
+        if result.success:
             # Attach files to the entity
             if files:
                 for file in files:
                     if (not os.path.exists(file)):
                         result.success = False
                         result.error_info = 'File not found: ' + file
                         return result
```

### Comparing `voxelfarm-0.0.98/src/voxelfarm/report_lambda.py` & `voxelfarm-0.0.99/src/voxelfarm/report_lambda.py`

 * *Files identical despite different names*

### Comparing `voxelfarm-0.0.98/src/voxelfarm/view_lambda.py` & `voxelfarm-0.0.99/src/voxelfarm/view_lambda.py`

 * *Files identical despite different names*

### Comparing `voxelfarm-0.0.98/src/voxelfarm/voxelfarmclient.py` & `voxelfarm-0.0.99/src/voxelfarm/voxelfarmclient.py`

 * *Files identical despite different names*

### Comparing `voxelfarm-0.0.98/src/voxelfarm/workflow_lambda.py` & `voxelfarm-0.0.99/src/voxelfarm/workflow_lambda.py`

 * *Files identical despite different names*

### Comparing `voxelfarm-0.0.98/src/voxelfarm.egg-info/PKG-INFO` & `voxelfarm-0.0.99/src/voxelfarm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxelfarm
-Version: 0.0.98
+Version: 0.0.99
 Summary: Voxel Farm Python Lambdas
 Home-page: https://www.voxelfarm.com/help/PythonCookbook.html
 Author: Voxel Farm Contant
 Author-email: contant@voxelfarm.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/voxelfarm/voxelfarmclient/issues
 Platform: UNKNOWN
```


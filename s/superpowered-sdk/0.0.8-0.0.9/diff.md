# Comparing `tmp/superpowered-sdk-0.0.8.tar.gz` & `tmp/superpowered-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpowered-sdk-0.0.8.tar", last modified: Thu Feb  2 08:50:13 2023, max compression
+gzip compressed data, was "superpowered-sdk-0.0.9.tar", last modified: Thu Feb  2 08:52:20 2023, max compression
```

## Comparing `superpowered-sdk-0.0.8.tar` & `superpowered-sdk-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:50:13.229709 superpowered-sdk-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:50:02.000000 superpowered-sdk-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-02-02 08:50:13.229709 superpowered-sdk-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-02 08:50:02.000000 superpowered-sdk-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-02 08:50:02.000000 superpowered-sdk-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 08:50:13.229709 superpowered-sdk-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-02-02 08:50:02.000000 superpowered-sdk-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:50:13.229709 superpowered-sdk-0.0.8/superpowered/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:50:02.000000 superpowered-sdk-0.0.8/superpowered/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-02-02 08:50:02.000000 superpowered-sdk-0.0.8/superpowered/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:50:13.229709 superpowered-sdk-0.0.8/superpowered_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-02-02 08:50:13.000000 superpowered-sdk-0.0.8/superpowered_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-02 08:50:13.000000 superpowered-sdk-0.0.8/superpowered_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 08:50:13.000000 superpowered-sdk-0.0.8/superpowered_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-02 08:50:13.000000 superpowered-sdk-0.0.8/superpowered_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:52:20.668043 superpowered-sdk-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:52:06.000000 superpowered-sdk-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-02-02 08:52:20.668043 superpowered-sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-02 08:52:06.000000 superpowered-sdk-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-02 08:52:06.000000 superpowered-sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 08:52:20.668043 superpowered-sdk-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-02-02 08:52:06.000000 superpowered-sdk-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:52:20.668043 superpowered-sdk-0.0.9/superpowered/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:52:06.000000 superpowered-sdk-0.0.9/superpowered/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-02-02 08:52:06.000000 superpowered-sdk-0.0.9/superpowered/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:52:20.668043 superpowered-sdk-0.0.9/superpowered_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-02-02 08:52:20.000000 superpowered-sdk-0.0.9/superpowered_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-02 08:52:20.000000 superpowered-sdk-0.0.9/superpowered_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 08:52:20.000000 superpowered-sdk-0.0.9/superpowered_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-02 08:52:20.000000 superpowered-sdk-0.0.9/superpowered_sdk.egg-info/top_level.txt
```

### Comparing `superpowered-sdk-0.0.8/PKG-INFO` & `superpowered-sdk-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Superpowered AI SDK
 Home-page: https://superpowered.ai
 Author: superpowered
 Author-email: justin@superpowered.ai
 License: Proprietary License
 Project-URL: Homepage, https://superpowered.ai
 Project-URL: Documentation, https://superpowered.ai/docs
```

### Comparing `superpowered-sdk-0.0.8/pyproject.toml` & `superpowered-sdk-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.0.8/setup.py` & `superpowered-sdk-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname), "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setuptools.setup(
     name="superpowered-sdk",
-    version="0.0.8",
+    version="0.0.9",
     description="Superpowered AI SDK",
     license="Proprietary License",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://superpowered.ai",
     project_urls={
         "Homepage": "https://superpowered.ai",
```

### Comparing `superpowered-sdk-0.0.8/superpowered/main.py` & `superpowered-sdk-0.0.9/superpowered/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,15 @@
 
 class ModelInstance:
     def __init__(self, model_id: str = None, supp_id: str = None, description: str = None, instance_id = None):
         self.supp_id = supp_id
         self.description = description
         self.instance_id = instance_id
         self.model_id = model_id
+        self.chat_history = []
         self.chat_history = self.get_chat_history()
         self.is_deployed = self.instance_id not in models['model_id'].model_instances
 
     def get_chat_history(self):
         # get chat history interactions with pagination
         url = BASE_URL + f'models/{self.model_id}/instances/{self.instance_id}/chat_history'
         response = _format_http_response(requests.get(url, headers=HEADERS))
```

### Comparing `superpowered-sdk-0.0.8/superpowered_sdk.egg-info/PKG-INFO` & `superpowered-sdk-0.0.9/superpowered_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Superpowered AI SDK
 Home-page: https://superpowered.ai
 Author: superpowered
 Author-email: justin@superpowered.ai
 License: Proprietary License
 Project-URL: Homepage, https://superpowered.ai
 Project-URL: Documentation, https://superpowered.ai/docs
```


# Comparing `tmp/jiggybase-0.0.14.tar.gz` & `tmp/jiggybase-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.14.tar", last modified: Fri Apr 28 16:17:28 2023, max compression
+gzip compressed data, was "jiggybase-0.0.15.tar", last modified: Sat Apr 29 03:41:17 2023, max compression
```

## Comparing `jiggybase-0.0.14.tar` & `jiggybase-0.0.15.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-28 16:17:28.053706 jiggybase-0.0.14/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.14/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)      542 2023-04-28 16:17:28.053398 jiggybase-0.0.14/PKG-INFO
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-28 16:17:28.046454 jiggybase-0.0.14/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.14/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1769 2023-04-28 15:29:35.000000 jiggybase-0.0.14/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     4935 2023-04-24 00:27:42.000000 jiggybase-0.0.14/jiggybase/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)     2726 2023-04-05 03:30:00.000000 jiggybase-0.0.14/jiggybase/config.py
--rw-r--r--   0 wsk        (501) staff       (20)     4479 2023-04-28 15:41:35.000000 jiggybase-0.0.14/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.14/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-28 16:17:28.052442 jiggybase-0.0.14/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.14/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.14/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.14/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.14/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.14/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.14/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.14/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.14/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.14/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     1523 2023-04-26 01:38:56.000000 jiggybase-0.0.14/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3452 2023-04-10 19:09:18.000000 jiggybase-0.0.14/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.14/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.14/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.14/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4315 2023-04-24 00:03:45.000000 jiggybase-0.0.14/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-28 16:17:28.047811 jiggybase-0.0.14/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)      542 2023-04-28 16:17:28.000000 jiggybase-0.0.14/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      744 2023-04-28 16:17:28.000000 jiggybase-0.0.14/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-28 16:17:28.000000 jiggybase-0.0.14/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-04-28 16:17:28.000000 jiggybase-0.0.14/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-04-28 16:17:28.000000 jiggybase-0.0.14/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      675 2023-04-28 15:25:50.000000 jiggybase-0.0.14/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-28 16:17:28.053794 jiggybase-0.0.14/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-28 16:17:28.052858 jiggybase-0.0.14/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.14/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 03:41:17.439918 jiggybase-0.0.15/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.15/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)      532 2023-04-29 03:41:17.439513 jiggybase-0.0.15/PKG-INFO
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 03:41:17.432381 jiggybase-0.0.15/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.15/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1769 2023-04-28 15:29:35.000000 jiggybase-0.0.15/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     7227 2023-04-29 03:02:52.000000 jiggybase-0.0.15/jiggybase/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2726 2023-04-05 03:30:00.000000 jiggybase-0.0.15/jiggybase/config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4530 2023-04-29 01:57:08.000000 jiggybase-0.0.15/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.15/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 03:41:17.438523 jiggybase-0.0.15/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.15/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.15/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.15/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.15/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.15/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.15/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.15/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.15/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.15/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.15/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3452 2023-04-10 19:09:18.000000 jiggybase-0.0.15/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.15/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.15/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.15/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4315 2023-04-24 00:03:45.000000 jiggybase-0.0.15/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 03:41:17.433770 jiggybase-0.0.15/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)      532 2023-04-29 03:41:17.000000 jiggybase-0.0.15/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      744 2023-04-29 03:41:17.000000 jiggybase-0.0.15/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-29 03:41:17.000000 jiggybase-0.0.15/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-04-29 03:41:17.000000 jiggybase-0.0.15/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-04-29 03:41:17.000000 jiggybase-0.0.15/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      665 2023-04-29 03:40:54.000000 jiggybase-0.0.15/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-29 03:41:17.440014 jiggybase-0.0.15/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 03:41:17.438977 jiggybase-0.0.15/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.15/test/test.py
```

### Comparing `jiggybase-0.0.14/LICENSE` & `jiggybase-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/PKG-INFO` & `jiggybase-0.0.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.14
+Version: 0.0.15
 Summary: Client for jiggy.ai JiggyBase including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
-Project-URL: Bug Tracker, https://github.com/jiggy-ai/jiggybase/issues
+Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jiggybase-0.0.14/jiggybase/client.py` & `jiggybase-0.0.15/jiggybase/client.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/jiggybase/collection.py` & `jiggybase-0.0.15/jiggybase/collection.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from typing import Optional
 from pydantic import BaseModel, Field, BaseConfig, HttpUrl
 from enum import Enum
 from .models import collection, CollectionChatConfig, PatchCollectionChatConfig
+from .jiggybase_session import JiggyBaseSession
+from .models import UpsertResponse,  Query, QueryRequest, QueryResponse, UpsertRequest, Document, DocumentChunk, DeleteRequest, DeleteResponse, DocumentMetadataFilter
+import os
+import mimetypes
 
-
+from typing import Union, List
 class PluginAuthType(Enum):
     bearer :str = "bearer"
     none   :str = "none"
     oauth  :str = "oauth"
 
         
 class CollectionPostRequest(BaseModel):
@@ -51,15 +55,16 @@
     """
     class Config(BaseConfig):
         extra = "allow"
 
     def __init__(self, session, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.session = session
-        
+        self.plugin_session = JiggyBaseSession(host=f'https://{kwargs["fqdn"]}', api='')
+
     def set_description(self, description:str) -> "Collection":
         """
         Update an existing collection using its ID and the provided description.
         """
         patch_request = CollectionPatchRequest(description=description)
         rsp = self.session.patch(f"/orgs/{self.org_id}/collections/{self.id}", model=patch_request)
         return Collection(**rsp.json())
@@ -99,8 +104,46 @@
     def update_chat_config(self, model: str, prompt_task_id: int) -> CollectionChatConfig:
         """
         Update the chat configuration for this collection.
         """
         rsp = self.session.patch(f"/orgs/{self.org_id}/collections/{self.id}/chat_config/{model}", model=PatchCollectionChatConfig(prompt_task_id=prompt_task_id))
         return CollectionChatConfig(**rsp.json())
 
-    
+ 
+    def upsert_file(self, file_path: str, mimetype: str = None) -> UpsertResponse:
+        if not os.path.exists(file_path):
+            raise ValueError("File not found")
+             
+        with open(file_path, "rb") as file:
+            files = {"file": (os.path.basename(file_path), file, mimetype)}
+            rsp = self.plugin_session.post("/upsert-file", files=files)
+        return UpsertResponse.parse_obj(rsp.json())
+
+    def upsert(self, documents: List[Document]) -> UpsertResponse:
+        upsert_request = UpsertRequest(documents=documents)
+        rsp = self.plugin_session.post("/upsert", model=upsert_request)
+        return  UpsertResponse.parse_obj(rsp.json())
+    
+    def query(self, queries: Union[str, List[str]]) -> QueryResponse:
+        if isinstance(queries, str):
+            queries = [queries]
+        query_requests = [Query(query=q) for q in queries]
+        qr = QueryRequest(queries=query_requests)
+        rsp = self.plugin_session.post("/query", model=qr)
+        return  QueryResponse.parse_obj(rsp.json())
+
+    def get_chunks(self, 
+                   start: int = 0, 
+                   limit: int = 10, 
+                   reverse: bool = True) -> List[DocumentChunk]:
+        params = {"start": start, "limit": limit, "reverse": reverse}
+        rsp = self.plugin_session.get("/chunks", params=params)
+        return [DocumentChunk.parse_obj(chunk) for chunk in rsp.json()]
+
+    def delete_docs(self, 
+                        ids                      : Optional[List[str]] = None, 
+                        document_metadata_filter : Optional[DocumentMetadataFilter] = None, 
+                        delete_all               : bool = False) -> DeleteResponse:
+        delete_request = DeleteRequest(ids=ids, filter=document_metadata_filter, delete_all=delete_all)
+        rsp = self.plugin_session.delete("/delete", model=delete_request)
+        return DeleteResponse.parse_obj(rsp.json())
+
```

### Comparing `jiggybase-0.0.14/jiggybase/config.py` & `jiggybase-0.0.15/jiggybase/config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/jiggybase/jiggybase_session.py` & `jiggybase-0.0.15/jiggybase/jiggybase_session.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from requests.auth import HTTPBasicAuth
 from requests.packages.urllib3 import Retry
 from requests.adapters import HTTPAdapter
 import requests
 from .login import window_open
 
-GPTG_HOST     = 'https://api.gpt-gateway.com'   # transition to jiggy.ai in progress
+JIGGYBASE_HOST     = 'https://api.gpt-gateway.com'   # transition to jiggy.ai in progress
 
 JB_KEY_FILE = os.path.expanduser('~') + '/.jb'   # local file to store user entered apikey 
 
 
 class ClientError(Exception):
     """
     API returned 4xx client error
@@ -20,29 +20,32 @@
 class ServerError(Exception):
     """
     API returned 5xx Server error
     """
 
     
 class JiggyBaseSession(requests.Session):
-    def __init__(self, gptg_api='gpt-gateway-v1', gptg_host=GPTG_HOST, *args, **kwargs):
+    def __init__(self, host=JIGGYBASE_HOST, api='gpt-gateway-v1',  *args, **kwargs):
         """
         Extend requests.Session with common GPTG authentication, retry, and exceptions.
 
-        gptg_api:  The gptg api & version to use.
-        
-        gptg_host: The url host prefix of the form "https:/api.gpt-gateway.com"
-                    if gptg_host arg is not set, will use 
-                    GPTG_HOST environment variable or "api.gpt-gateway.com" as final default.
-        
-        final url prefix are of the form "https:/{gptg_host}/{gptg_api}"
+        host: The url host prefix of the form "https:/api.gpt-gateway.com"
+              if host arg is not set, will use 
+                    JIGGYBASE_HOST environment variable or "api.gpt-gateway.com" as final default.
+
+        api:  The api & version to use. defaults to 'gpt-gateway-v1'
+                
+        final url prefix are of the form "https:/{host}/{api}"
         """
         super(JiggyBaseSession, self).__init__(*args, **kwargs)
-        self.host = gptg_host
-        self.prefix_url = f"{gptg_host}/{gptg_api}"
+        self.host = host
+        if api:
+            self.prefix_url = f"{host}/{api}"
+        else:
+            self.prefix_url = host            
         test_url = f"{self.prefix_url}/docs"
         if requests.head(test_url).status_code != 200:
             raise Exception(f"Invalid or unreachable api: {self.prefix_url}")
             
         self.bearer_token = None
         super(JiggyBaseSession, self).mount('https://',
                                         HTTPAdapter(max_retries=Retry(connect=5,
@@ -50,19 +53,18 @@
                                                                       status=5,
                                                                       redirect=2,
                                                                       backoff_factor=.001,
                                                                       status_forcelist=(500, 502, 503, 504))))
 
     def _set_bearer(self, jwt):
         self.bearer_token = jwt
-        print(jwt)
         self.headers['Authorization'] = f"Bearer {jwt}"
 
     def _getjwt(self, key):        
-        resp = requests.post(f"{self.host}/gpt-gateway-v1/auth", json={'key': key})
+        resp = requests.post(f"{JIGGYBASE_HOST}/gpt-gateway-v1/auth", json={'key': key})
         if resp.status_code == 200:
             self._set_bearer(resp.json()['jwt'])
         elif resp.status_code == 401:
             raise ClientError("Invalid API Key")
         else:
             raise ServerError(resp.content)
```

### Comparing `jiggybase-0.0.14/jiggybase/login.py` & `jiggybase-0.0.15/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/jiggybase/models/auth.py` & `jiggybase-0.0.15/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/jiggybase/models/chat.py` & `jiggybase-0.0.15/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/jiggybase/models/chunk.py` & `jiggybase-0.0.15/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/jiggybase/models/collection.py` & `jiggybase-0.0.15/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/jiggybase/models/metadata.py` & `jiggybase-0.0.15/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/jiggybase/models/org.py` & `jiggybase-0.0.15/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/jiggybase/models/plugin_config.py` & `jiggybase-0.0.15/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/jiggybase/models/prompt.py` & `jiggybase-0.0.15/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/jiggybase/models/providers.py` & `jiggybase-0.0.15/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/jiggybase/models/user.py` & `jiggybase-0.0.15/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/jiggybase/org.py` & `jiggybase-0.0.15/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.15/jiggybase.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.14
+Version: 0.0.15
 Summary: Client for jiggy.ai JiggyBase including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
-Project-URL: Bug Tracker, https://github.com/jiggy-ai/jiggybase/issues
+Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jiggybase-0.0.14/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.15/jiggybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.14/pyproject.toml` & `jiggybase-0.0.15/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.14"
+version = "0.0.15"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pedantic[email]', 'requests']
 description = "Client for jiggy.ai JiggyBase including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
@@ -17,8 +17,8 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/jiggy-ai/jiggybase"
-"Bug Tracker" = "https://github.com/jiggy-ai/jiggybase/issues"
+"Bug Tracker" = "https://github.com/jiggy-ai/issues"
```

### Comparing `jiggybase-0.0.14/test/test.py` & `jiggybase-0.0.15/test/test.py`

 * *Files identical despite different names*


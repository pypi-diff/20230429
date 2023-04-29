# Comparing `tmp/jiggybase-0.0.15.tar.gz` & `tmp/jiggybase-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.15.tar", last modified: Sat Apr 29 03:41:17 2023, max compression
+gzip compressed data, was "jiggybase-0.0.17.tar", last modified: Sat Apr 29 04:16:05 2023, max compression
```

## Comparing `jiggybase-0.0.15.tar` & `jiggybase-0.0.17.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 03:41:17.439918 jiggybase-0.0.15/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.15/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)      532 2023-04-29 03:41:17.439513 jiggybase-0.0.15/PKG-INFO
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 03:41:17.432381 jiggybase-0.0.15/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.15/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1769 2023-04-28 15:29:35.000000 jiggybase-0.0.15/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     7227 2023-04-29 03:02:52.000000 jiggybase-0.0.15/jiggybase/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)     2726 2023-04-05 03:30:00.000000 jiggybase-0.0.15/jiggybase/config.py
--rw-r--r--   0 wsk        (501) staff       (20)     4530 2023-04-29 01:57:08.000000 jiggybase-0.0.15/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.15/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 03:41:17.438523 jiggybase-0.0.15/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.15/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.15/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.15/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.15/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.15/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.15/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.15/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.15/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.15/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.15/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3452 2023-04-10 19:09:18.000000 jiggybase-0.0.15/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.15/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.15/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.15/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4315 2023-04-24 00:03:45.000000 jiggybase-0.0.15/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 03:41:17.433770 jiggybase-0.0.15/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)      532 2023-04-29 03:41:17.000000 jiggybase-0.0.15/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      744 2023-04-29 03:41:17.000000 jiggybase-0.0.15/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-29 03:41:17.000000 jiggybase-0.0.15/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-04-29 03:41:17.000000 jiggybase-0.0.15/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-04-29 03:41:17.000000 jiggybase-0.0.15/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      665 2023-04-29 03:40:54.000000 jiggybase-0.0.15/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-29 03:41:17.440014 jiggybase-0.0.15/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 03:41:17.438977 jiggybase-0.0.15/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.15/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 04:16:05.818916 jiggybase-0.0.17/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.17/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)      533 2023-04-29 04:16:05.818577 jiggybase-0.0.17/PKG-INFO
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 04:16:05.812430 jiggybase-0.0.17/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.17/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1769 2023-04-28 15:29:35.000000 jiggybase-0.0.17/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     8278 2023-04-29 04:07:23.000000 jiggybase-0.0.17/jiggybase/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2726 2023-04-05 03:30:00.000000 jiggybase-0.0.17/jiggybase/config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.17/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.17/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 04:16:05.817708 jiggybase-0.0.17/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.17/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.17/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.17/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.17/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.17/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.17/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.17/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.17/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.17/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.17/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3452 2023-04-10 19:09:18.000000 jiggybase-0.0.17/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.17/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.17/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.17/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4315 2023-04-24 00:03:45.000000 jiggybase-0.0.17/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 04:16:05.813788 jiggybase-0.0.17/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)      533 2023-04-29 04:16:05.000000 jiggybase-0.0.17/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      744 2023-04-29 04:16:05.000000 jiggybase-0.0.17/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-29 04:16:05.000000 jiggybase-0.0.17/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-04-29 04:16:05.000000 jiggybase-0.0.17/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-04-29 04:16:05.000000 jiggybase-0.0.17/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      669 2023-04-29 04:14:16.000000 jiggybase-0.0.17/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-29 04:16:05.819006 jiggybase-0.0.17/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 04:16:05.818062 jiggybase-0.0.17/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.17/test/test.py
```

### Comparing `jiggybase-0.0.15/LICENSE` & `jiggybase-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/PKG-INFO` & `jiggybase-0.0.17/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.15
-Summary: Client for jiggy.ai JiggyBase including ChatGPT Retriever Plugins
+Version: 0.0.17
+Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `jiggybase-0.0.15/jiggybase/client.py` & `jiggybase-0.0.17/jiggybase/client.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase/collection.py` & `jiggybase-0.0.17/jiggybase/collection.py`

 * *Files 18% similar despite different names*

```diff
@@ -106,44 +106,68 @@
         Update the chat configuration for this collection.
         """
         rsp = self.session.patch(f"/orgs/{self.org_id}/collections/{self.id}/chat_config/{model}", model=PatchCollectionChatConfig(prompt_task_id=prompt_task_id))
         return CollectionChatConfig(**rsp.json())
 
  
     def upsert_file(self, file_path: str, mimetype: str = None) -> UpsertResponse:
+        """
+        Add a file to the collection.
+        """
         if not os.path.exists(file_path):
             raise ValueError("File not found")
              
         with open(file_path, "rb") as file:
             files = {"file": (os.path.basename(file_path), file, mimetype)}
             rsp = self.plugin_session.post("/upsert-file", files=files)
         return UpsertResponse.parse_obj(rsp.json())
 
     def upsert(self, documents: List[Document]) -> UpsertResponse:
+        """
+        Add a list of Document objects to the collection.
+        """
         upsert_request = UpsertRequest(documents=documents)
         rsp = self.plugin_session.post("/upsert", model=upsert_request)
         return  UpsertResponse.parse_obj(rsp.json())
     
-    def query(self, queries: Union[str, List[str]]) -> QueryResponse:
+    def query(self, queries: Union[str, List[str], Query], top_k : int = 10) -> QueryResponse:
+        """
+        Query the collection returning the top_k results for each query.
+        queries can be either a single string, a list of strings, or a list of Query objects.
+        if it is a string or list of strings, the specified top_k will be used for each of the queries.
+        Returns a QueryResponse object.
+        """
         if isinstance(queries, str):
-            queries = [queries]
-        query_requests = [Query(query=q) for q in queries]
-        qr = QueryRequest(queries=query_requests)
+            queries = [Query(query=queries, top_k=top_k)]
+        elif isinstance(queries, Query):
+            queries = [Query(query=q, top_k=top_k) for q in queries]
+        qr = QueryRequest(queries=queries)
         rsp = self.plugin_session.post("/query", model=qr)
         return  QueryResponse.parse_obj(rsp.json())
 
     def get_chunks(self, 
                    start: int = 0, 
                    limit: int = 10, 
                    reverse: bool = True) -> List[DocumentChunk]:
+        """
+        low level interface for iterating through the chunks in a collection
+        start - Offset of the first result to return
+        limit - Number of results to return starting from the offset
+        reverse - Reverse the order of the items returned
+        """
         params = {"start": start, "limit": limit, "reverse": reverse}
         rsp = self.plugin_session.get("/chunks", params=params)
         return [DocumentChunk.parse_obj(chunk) for chunk in rsp.json()]
 
+
     def delete_docs(self, 
-                        ids                      : Optional[List[str]] = None, 
-                        document_metadata_filter : Optional[DocumentMetadataFilter] = None, 
-                        delete_all               : bool = False) -> DeleteResponse:
+                    ids                      : Optional[List[str]] = None, 
+                    document_metadata_filter : Optional[DocumentMetadataFilter] = None, 
+                    delete_all               : Optional[bool] = False) -> DeleteResponse:
+        """
+        Delete items in the collection by document id's or document metadata filter.
+        A delete_all option is also provided to delete all documents in the collection.
+        """
         delete_request = DeleteRequest(ids=ids, filter=document_metadata_filter, delete_all=delete_all)
         rsp = self.plugin_session.delete("/delete", model=delete_request)
         return DeleteResponse.parse_obj(rsp.json())
```

### Comparing `jiggybase-0.0.15/jiggybase/config.py` & `jiggybase-0.0.17/jiggybase/config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase/jiggybase_session.py` & `jiggybase-0.0.17/jiggybase/jiggybase_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from requests.packages.urllib3 import Retry
 from requests.adapters import HTTPAdapter
 import requests
 from .login import window_open
 
 JIGGYBASE_HOST     = 'https://api.gpt-gateway.com'   # transition to jiggy.ai in progress
 
-JB_KEY_FILE = os.path.expanduser('~') + '/.jb'   # local file to store user entered apikey 
+JB_KEY_FILE = os.path.expanduser('~') + '/.jiggybase'   # local file to store user entered apikey 
 
 
 class ClientError(Exception):
     """
     API returned 4xx client error
     """
 
@@ -72,15 +72,15 @@
         if 'JIGGYBASE_API_KEY' in os.environ:
             self._getjwt(os.environ['JIGGYBASE_API_KEY'])
         elif os.path.exists(JB_KEY_FILE):
             self._getjwt(open(JB_KEY_FILE).read())
         else:
             while True:
                 window_open("https://jiggy.ai/authorize")
-                key_input = input("Enter your gpt-gateway.com API Key: ")
+                key_input = input("Enter your JiggyBase API Key: ")
                 if key_input[:4] == "jgy-":
                     # try using the key to see if it is valid
                     try:
                         self._getjwt(key_input)
                         # key validated, save to key file
                         open(JB_KEY_FILE, 'w').write(key_input)
                         os.chmod(JB_KEY_FILE, 0o600)  # -rw-------
```

### Comparing `jiggybase-0.0.15/jiggybase/login.py` & `jiggybase-0.0.17/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase/models/auth.py` & `jiggybase-0.0.17/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase/models/chat.py` & `jiggybase-0.0.17/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase/models/chunk.py` & `jiggybase-0.0.17/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase/models/collection.py` & `jiggybase-0.0.17/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase/models/metadata.py` & `jiggybase-0.0.17/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase/models/org.py` & `jiggybase-0.0.17/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase/models/plugin.py` & `jiggybase-0.0.17/jiggybase/models/plugin.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase/models/plugin_config.py` & `jiggybase-0.0.17/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase/models/prompt.py` & `jiggybase-0.0.17/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase/models/providers.py` & `jiggybase-0.0.17/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase/models/user.py` & `jiggybase-0.0.17/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase/org.py` & `jiggybase-0.0.17/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.17/jiggybase.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.15
-Summary: Client for jiggy.ai JiggyBase including ChatGPT Retriever Plugins
+Version: 0.0.17
+Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `jiggybase-0.0.15/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.17/jiggybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.15/pyproject.toml` & `jiggybase-0.0.17/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.15"
+version = "0.0.17"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pedantic[email]', 'requests']
-description = "Client for jiggy.ai JiggyBase including ChatGPT Retriever Plugins"
+description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 
 [project.urls]
-"Homepage" = "https://github.com/jiggy-ai/jiggybase"
+"Homepage"    = "https://github.com/jiggy-ai/jiggybase"
 "Bug Tracker" = "https://github.com/jiggy-ai/issues"
```

### Comparing `jiggybase-0.0.15/test/test.py` & `jiggybase-0.0.17/test/test.py`

 * *Files identical despite different names*


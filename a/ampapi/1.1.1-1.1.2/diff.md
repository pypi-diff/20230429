# Comparing `tmp/ampapi-1.1.1.tar.gz` & `tmp/ampapi-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampapi-1.1.1.tar", last modified: Fri Apr 28 08:04:01 2023, max compression
+gzip compressed data, was "ampapi-1.1.2.tar", last modified: Sat Apr 29 04:17:39 2023, max compression
```

## Comparing `ampapi-1.1.1.tar` & `ampapi-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-28 08:04:01.074105 ampapi-1.1.1/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1074 2023-04-28 07:48:40.000000 ampapi-1.1.1/LICENCE
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     4131 2023-04-28 08:04:01.074105 ampapi-1.1.1/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     3620 2023-04-28 07:47:28.000000 ampapi-1.1.1/README.md
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-28 08:04:01.070104 ampapi-1.1.1/ampapi/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2023-04-28 01:28:45.000000 ampapi-1.1.1/ampapi/__init__.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)   158791 2023-04-28 08:03:46.000000 ampapi-1.1.1/ampapi/ampapi.py
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-28 08:04:01.074105 ampapi-1.1.1/ampapi.egg-info/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     4131 2023-04-28 08:04:01.000000 ampapi-1.1.1/ampapi.egg-info/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      198 2023-04-28 08:04:01.000000 ampapi-1.1.1/ampapi.egg-info/SOURCES.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-04-28 08:04:01.000000 ampapi-1.1.1/ampapi.egg-info/dependency_links.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        7 2023-04-28 08:04:01.000000 ampapi-1.1.1/ampapi.egg-info/top_level.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      111 2023-04-28 01:28:45.000000 ampapi-1.1.1/pyproject.toml
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      600 2023-04-28 08:04:01.074105 ampapi-1.1.1/setup.cfg
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-29 04:17:39.713090 ampapi-1.1.2/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1074 2023-04-29 04:12:37.000000 ampapi-1.1.2/LICENCE
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     4131 2023-04-29 04:17:39.713090 ampapi-1.1.2/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     3620 2023-04-29 04:12:37.000000 ampapi-1.1.2/README.md
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-29 04:17:39.713090 ampapi-1.1.2/ampapi/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2023-04-29 04:12:37.000000 ampapi-1.1.2/ampapi/__init__.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)   160315 2023-04-29 04:17:25.000000 ampapi-1.1.2/ampapi/ampapi.py
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-29 04:17:39.713090 ampapi-1.1.2/ampapi.egg-info/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     4131 2023-04-29 04:17:39.000000 ampapi-1.1.2/ampapi.egg-info/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      198 2023-04-29 04:17:39.000000 ampapi-1.1.2/ampapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-04-29 04:17:39.000000 ampapi-1.1.2/ampapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        7 2023-04-29 04:17:39.000000 ampapi-1.1.2/ampapi.egg-info/top_level.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      111 2023-04-29 04:12:37.000000 ampapi-1.1.2/pyproject.toml
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      600 2023-04-29 04:17:39.717090 ampapi-1.1.2/setup.cfg
```

### Comparing `ampapi-1.1.1/LICENCE` & `ampapi-1.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `ampapi-1.1.1/PKG-INFO` & `ampapi-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampapi
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python implemenation of the Cubecoders AMP API.
 Home-page: https://github.com/p0t4t0sandwich/ampapi-python
 Author: Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 Author-email: p0t4t0sandwich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ampapi-1.1.1/README.md` & `ampapi-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ampapi-1.1.1/ampapi/ampapi.py` & `ampapi-1.1.2/ampapi/ampapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1593,26 +1593,26 @@
         })
 
     def ADSModule_UpgradeInstance(self, InstanceName: str):
         """
         :param InstanceName: 
         :type InstanceName: strFalse
             AMP Type: String
-        :returns: AMP Type: Task<ActionResult>
+        :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/UpgradeInstance", data={
             "InstanceName": InstanceName, 
         })
 
     async def ADSModule_UpgradeInstanceAsync(self, InstanceName: str):
         """
         :param InstanceName: 
         :type InstanceName: strFalse
             AMP Type: String
-        :returns: AMP Type: Task<ActionResult>
+        :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/UpgradeInstance", data={
             "InstanceName": InstanceName, 
         })
 
     def ADSModule_StartAllInstances(self):
         """
@@ -1683,48 +1683,48 @@
         })
 
     def ADSModule_RestartInstance(self, InstanceName: str):
         """
         :param InstanceName: 
         :type InstanceName: strFalse
             AMP Type: String
-        :returns: AMP Type: Task<ActionResult>
+        :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/RestartInstance", data={
             "InstanceName": InstanceName, 
         })
 
     async def ADSModule_RestartInstanceAsync(self, InstanceName: str):
         """
         :param InstanceName: 
         :type InstanceName: strFalse
             AMP Type: String
-        :returns: AMP Type: Task<ActionResult>
+        :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/RestartInstance", data={
             "InstanceName": InstanceName, 
         })
 
     def ADSModule_StopInstance(self, InstanceName: str):
         """
         :param InstanceName: 
         :type InstanceName: strFalse
             AMP Type: String
-        :returns: AMP Type: Task<ActionResult>
+        :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="ADSModule/StopInstance", data={
             "InstanceName": InstanceName, 
         })
 
     async def ADSModule_StopInstanceAsync(self, InstanceName: str):
         """
         :param InstanceName: 
         :type InstanceName: strFalse
             AMP Type: String
-        :returns: AMP Type: Task<ActionResult>
+        :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="ADSModule/StopInstance", data={
             "InstanceName": InstanceName, 
         })
 
     def ADSModule_DeleteInstanceUsers(self, InstanceId: str):
         """
@@ -2046,52 +2046,88 @@
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/AppendFileChunk", data={
             "Filename": Filename, 
             "Data": Data, 
             "Delete": Delete, 
         })
 
-    def FileManagerPlugin_WriteFileChunk(self, Filename: str, Position: int, Data: str):
+    def FileManagerPlugin_ReadFileChunk(self, Filename: str, Offset: int):
         """
         :param Filename: 
         :type Filename: strFalse
             AMP Type: String
-        :param Position: 
-        :type Position: intFalse
+        :param Offset: 
+        :type Offset: intFalse
             AMP Type: Int64
+        :returns: AMP Type: ActionResult<String>
+        """
+        return self.APICall(endpoint="FileManagerPlugin/ReadFileChunk", data={
+            "Filename": Filename, 
+            "Offset": Offset, 
+        })
+
+    async def FileManagerPlugin_ReadFileChunkAsync(self, Filename: str, Offset: int):
+        """
+        :param Filename: 
+        :type Filename: strFalse
+            AMP Type: String
+        :param Offset: 
+        :type Offset: intFalse
+            AMP Type: Int64
+        :returns: AMP Type: ActionResult<String>
+        """
+        return await self.APICallAsync(endpoint="FileManagerPlugin/ReadFileChunk", data={
+            "Filename": Filename, 
+            "Offset": Offset, 
+        })
+
+    def FileManagerPlugin_WriteFileChunk(self, Filename: str, Data: str, Offset: int, FinalChunk: bool):
+        """
+        :param Filename: 
+        :type Filename: strFalse
+            AMP Type: String
         :param Data: 
         :type Data: strFalse
             AMP Type: String
-        :returns: AMP Type: Void
-        :rtype: None
+        :param Offset: 
+        :type Offset: intFalse
+            AMP Type: Int64
+        :param FinalChunk: 
+        :type FinalChunk: boolFalse
+            AMP Type: Boolean
+        :returns: AMP Type: ActionResult
         """
         return self.APICall(endpoint="FileManagerPlugin/WriteFileChunk", data={
             "Filename": Filename, 
-            "Position": Position, 
             "Data": Data, 
+            "Offset": Offset, 
+            "FinalChunk": FinalChunk, 
         })
 
-    async def FileManagerPlugin_WriteFileChunkAsync(self, Filename: str, Position: int, Data: str):
+    async def FileManagerPlugin_WriteFileChunkAsync(self, Filename: str, Data: str, Offset: int, FinalChunk: bool):
         """
         :param Filename: 
         :type Filename: strFalse
             AMP Type: String
-        :param Position: 
-        :type Position: intFalse
-            AMP Type: Int64
         :param Data: 
         :type Data: strFalse
             AMP Type: String
-        :returns: AMP Type: Void
-        :rtype: None
+        :param Offset: 
+        :type Offset: intFalse
+            AMP Type: Int64
+        :param FinalChunk: 
+        :type FinalChunk: boolFalse
+            AMP Type: Boolean
+        :returns: AMP Type: ActionResult
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/WriteFileChunk", data={
             "Filename": Filename, 
-            "Position": Position, 
             "Data": Data, 
+            "Offset": Offset, 
+            "FinalChunk": FinalChunk, 
         })
 
     def FileManagerPlugin_DownloadFileFromURL(self, Source: str, TargetDirectory: str):
         """
         :param Source: 
         :type Source: strFalse
             AMP Type: Uri
@@ -4438,14 +4474,26 @@
     async def Core_GetDiagnosticsInfoAsync(self):
         """
         :returns: AMP Type: Dictionary<String, String>
         :rtype: dict[str, str]
         """
         return await self.APICallAsync(endpoint="Core/GetDiagnosticsInfo")
 
+    def Core_GetWebserverMetrics(self):
+        """
+        :returns: AMP Type: Object
+        """
+        return self.APICall(endpoint="Core/GetWebserverMetrics")
+
+    async def Core_GetWebserverMetricsAsync(self):
+        """
+        :returns: AMP Type: Object
+        """
+        return await self.APICallAsync(endpoint="Core/GetWebserverMetrics")
+
     def Core_CreateTestTask(self):
         """DEV: Creates a non-ending task with 50% progress for testing purposes
             
         :returns: AMP Type: Void
         :rtype: None
         """
         return self.APICall(endpoint="Core/CreateTestTask")
@@ -4630,15 +4678,15 @@
             "rememberMe": True
         })
 
         if loginResult != None and "success" in loginResult.keys() and loginResult["success"] == True:
             return AMPAPIHandler(
                 baseUri=self.baseUri + f"API/ADSModule/Servers/{instance_id}",
                 username=self.username,
-                password=self.password,
+                password="",
                 rememberMeToken=loginResult["rememberMeToken"],
                 sessionId=loginResult["sessionID"]
             )
         else:
             return None
 
     async def InstanceLoginAsync(self, instance_id: str) -> AMPAPIHandlerType | None:
@@ -4655,13 +4703,13 @@
             "rememberMe": True
         })
 
         if loginResult != None and "success" in loginResult.keys() and loginResult["success"] == True:
             return AMPAPIHandler(
                 baseUri=self.baseUri + f"API/ADSModule/Servers/{instance_id}",
                 username=self.username,
-                password=self.password,
+                password="",
                 rememberMeToken=loginResult["rememberMeToken"],
                 sessionId=loginResult["sessionID"]
             )
         else:
             return None
```

### Comparing `ampapi-1.1.1/ampapi.egg-info/PKG-INFO` & `ampapi-1.1.2/ampapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampapi
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python implemenation of the Cubecoders AMP API.
 Home-page: https://github.com/p0t4t0sandwich/ampapi-python
 Author: Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 Author-email: p0t4t0sandwich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ampapi-1.1.1/setup.cfg` & `ampapi-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ampapi
-version = 1.1.1
+version = 1.1.2
 author = Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 author_email = p0t4t0sandwich@gmail.com
 description = A Python implemenation of the Cubecoders AMP API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/p0t4t0sandwich/ampapi-python
 classifiers =
```


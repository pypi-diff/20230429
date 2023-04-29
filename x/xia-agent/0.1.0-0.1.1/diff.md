# Comparing `tmp/xia_agent-0.1.0-cp39-none-win_amd64.whl.zip` & `tmp/xia_agent-0.1.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 134324 bytes, number of entries: 7
--rw-r--r--  2.0 unx      146 b- defN 23-Apr-28 19:21 xia_agent/__init__.py
--rw-r--r--  2.0 unx   328192 b- defN 23-Apr-28 19:24 xia_agent/agent.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-28 19:24 xia_agent-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      686 b- defN 23-Apr-28 19:24 xia_agent-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-28 19:24 xia_agent-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-28 19:24 xia_agent-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      568 b- defN 23-Apr-28 19:24 xia_agent-0.1.0.dist-info/RECORD
-7 files, 329853 bytes uncompressed, 133314 bytes compressed:  59.6%
+Zip file size: 134139 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      146 b- defN 23-Apr-29 16:51 xia_agent/__init__.py
+-rw-r--r--  2.0 unx   327680 b- defN 23-Apr-29 16:54 xia_agent/agent.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-29 16:54 xia_agent-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      686 b- defN 23-Apr-29 16:54 xia_agent-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-29 16:54 xia_agent-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-29 16:54 xia_agent-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      568 b- defN 23-Apr-29 16:54 xia_agent-0.1.1.dist-info/RECORD
+7 files, 329341 bytes uncompressed, 133129 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_agent/__init__.py
 Comment: 
 
 Filename: xia_agent/agent.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_agent-0.1.0.dist-info/LICENSE.txt
+Filename: xia_agent-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_agent-0.1.0.dist-info/METADATA
+Filename: xia_agent-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: xia_agent-0.1.0.dist-info/WHEEL
+Filename: xia_agent-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: xia_agent-0.1.0.dist-info/top_level.txt
+Filename: xia_agent-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_agent-0.1.0.dist-info/RECORD
+Filename: xia_agent-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_agent/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_agent.agent import Agent, AgentFunction, MetaFunction
 
 __all__ = [
     "Agent", "AgentFunction", "MetaFunction"
 ]
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## Comparing `xia_agent-0.1.0.dist-info/METADATA` & `xia_agent-0.1.1.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-agent
-Version: 0.1.0
+Version: 0.1.1
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-agent/0.1.0/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-agent/0.1.1/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_agent-0.1.0.dist-info/RECORD` & `xia_agent-0.1.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_agent/__init__.py,sha256=eRaVzVyb1Y9v9p1X3fGoqIAiXLPDFVm2qPFQPH88olM,146
-xia_agent/agent.cp39-win_amd64.pyd,sha256=gxcUSuk6yh1PMRHGSp8IbISMQ72DIiDAX9IAZKCW1-U,328192
-xia_agent-0.1.0.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
-xia_agent-0.1.0.dist-info/METADATA,sha256=_FrbBpWZIW1uFCH8LDVu8VJ-o6e2i-UjQnsbrUGyVGI,686
-xia_agent-0.1.0.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_agent-0.1.0.dist-info/top_level.txt,sha256=uiK8HE2yj2wekdrxVgGRL0zCqajqbV6xrgTp7HlCXYU,10
-xia_agent-0.1.0.dist-info/RECORD,,
+xia_agent/__init__.py,sha256=PFSSHLgY5zIYNG_hTWy-YS5aWS4u95maCbJw8A6AHBw,146
+xia_agent/agent.cp39-win_amd64.pyd,sha256=H_jyLLCTb4YKPMe3LjCR3AljgCgR6Kgol-ZO2ZY_N9o,327680
+xia_agent-0.1.1.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_agent-0.1.1.dist-info/METADATA,sha256=lisoxhG3T1sLus-qCgo9e2hcO_MH6pfPeHzFGpuQcrQ,686
+xia_agent-0.1.1.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_agent-0.1.1.dist-info/top_level.txt,sha256=uiK8HE2yj2wekdrxVgGRL0zCqajqbV6xrgTp7HlCXYU,10
+xia_agent-0.1.1.dist-info/RECORD,,
```


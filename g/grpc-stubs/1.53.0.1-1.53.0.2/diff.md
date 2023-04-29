# Comparing `tmp/grpc-stubs-1.53.0.1.tar.gz` & `tmp/grpc-stubs-1.53.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpc-stubs-1.53.0.1.tar", last modified: Fri Apr  7 10:12:31 2023, max compression
+gzip compressed data, was "grpc-stubs-1.53.0.2.tar", last modified: Sat Apr 29 10:45:36 2023, max compression
```

## Comparing `grpc-stubs-1.53.0.1.tar` & `grpc-stubs-1.53.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-07 10:12:31.661166 grpc-stubs-1.53.0.1/
--rw-rw-r--   0 bl        (1000) bl        (1000)     1080 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/LICENSE
--rw-rw-r--   0 bl        (1000) bl        (1000)     3428 2023-04-07 10:12:31.661166 grpc-stubs-1.53.0.1/PKG-INFO
--rw-rw-r--   0 bl        (1000) bl        (1000)     2872 2023-04-07 10:11:59.000000 grpc-stubs-1.53.0.1/README.md
-drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-07 10:12:31.657166 grpc-stubs-1.53.0.1/grpc-stubs/
--rw-rw-r--   0 bl        (1000) bl        (1000)    24256 2023-04-07 10:11:11.000000 grpc-stubs-1.53.0.1/grpc-stubs/__init__.pyi
-drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-07 10:12:31.657166 grpc-stubs-1.53.0.1/grpc-stubs/aio/
--rw-rw-r--   0 bl        (1000) bl        (1000)    16499 2023-04-07 10:11:11.000000 grpc-stubs-1.53.0.1/grpc-stubs/aio/__init__.pyi
--rw-rw-r--   0 bl        (1000) bl        (1000)        8 2023-04-07 10:11:11.000000 grpc-stubs-1.53.0.1/grpc-stubs/aio/py.typed
--rw-rw-r--   0 bl        (1000) bl        (1000)        8 2023-03-05 04:14:41.000000 grpc-stubs-1.53.0.1/grpc-stubs/py.typed
-drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-07 10:12:31.661166 grpc-stubs-1.53.0.1/grpc_channelz-stubs/
--rw-rw-r--   0 bl        (1000) bl        (1000)       56 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/grpc_channelz-stubs/__init__.pyi
--rw-rw-r--   0 bl        (1000) bl        (1000)        0 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/grpc_channelz-stubs/py.typed
-drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-07 10:12:31.661166 grpc-stubs-1.53.0.1/grpc_channelz-stubs/v1/
--rw-rw-r--   0 bl        (1000) bl        (1000)       56 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/grpc_channelz-stubs/v1/__init__.pyi
--rw-rw-r--   0 bl        (1000) bl        (1000)     1330 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/grpc_channelz-stubs/v1/_servicer.pyi
--rw-rw-r--   0 bl        (1000) bl        (1000)       84 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/grpc_channelz-stubs/v1/channelz.pyi
-drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-07 10:12:31.661166 grpc-stubs-1.53.0.1/grpc_health-stubs/
--rw-rw-r--   0 bl        (1000) bl        (1000)       56 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/grpc_health-stubs/__init__.pyi
--rw-rw-r--   0 bl        (1000) bl        (1000)        0 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/grpc_health-stubs/py.typed
-drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-07 10:12:31.661166 grpc-stubs-1.53.0.1/grpc_health-stubs/v1/
--rw-rw-r--   0 bl        (1000) bl        (1000)       56 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/grpc_health-stubs/v1/__init__.pyi
--rw-rw-r--   0 bl        (1000) bl        (1000)     1332 2022-04-16 02:10:26.000000 grpc-stubs-1.53.0.1/grpc_health-stubs/v1/health.pyi
-drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-07 10:12:31.661166 grpc-stubs-1.53.0.1/grpc_reflection-stubs/
--rw-rw-r--   0 bl        (1000) bl        (1000)       56 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/grpc_reflection-stubs/__init__.pyi
--rw-rw-r--   0 bl        (1000) bl        (1000)        0 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/grpc_reflection-stubs/py.typed
-drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-07 10:12:31.661166 grpc-stubs-1.53.0.1/grpc_reflection-stubs/v1alpha/
--rw-rw-r--   0 bl        (1000) bl        (1000)       56 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/grpc_reflection-stubs/v1alpha/__init__.pyi
--rw-rw-r--   0 bl        (1000) bl        (1000)      628 2023-01-14 22:59:05.000000 grpc-stubs-1.53.0.1/grpc_reflection-stubs/v1alpha/reflection.pyi
-drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-07 10:12:31.661166 grpc-stubs-1.53.0.1/grpc_status-stubs/
--rw-rw-r--   0 bl        (1000) bl        (1000)       56 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/grpc_status-stubs/__init__.pyi
--rw-rw-r--   0 bl        (1000) bl        (1000)        0 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/grpc_status-stubs/py.typed
--rw-rw-r--   0 bl        (1000) bl        (1000)      455 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.1/grpc_status-stubs/rpc_status.pyi
-drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-07 10:12:31.661166 grpc-stubs-1.53.0.1/grpc_stubs.egg-info/
--rw-rw-r--   0 bl        (1000) bl        (1000)     3428 2023-04-07 10:12:31.000000 grpc-stubs-1.53.0.1/grpc_stubs.egg-info/PKG-INFO
--rw-rw-r--   0 bl        (1000) bl        (1000)      841 2023-04-07 10:12:31.000000 grpc-stubs-1.53.0.1/grpc_stubs.egg-info/SOURCES.txt
--rw-rw-r--   0 bl        (1000) bl        (1000)        1 2023-04-07 10:12:31.000000 grpc-stubs-1.53.0.1/grpc_stubs.egg-info/dependency_links.txt
--rw-rw-r--   0 bl        (1000) bl        (1000)        7 2023-04-07 10:12:31.000000 grpc-stubs-1.53.0.1/grpc_stubs.egg-info/requires.txt
--rw-rw-r--   0 bl        (1000) bl        (1000)       89 2023-04-07 10:12:31.000000 grpc-stubs-1.53.0.1/grpc_stubs.egg-info/top_level.txt
--rw-rw-r--   0 bl        (1000) bl        (1000)      194 2023-04-07 10:12:31.661166 grpc-stubs-1.53.0.1/setup.cfg
--rw-rw-r--   0 bl        (1000) bl        (1000)     1864 2023-04-07 10:12:12.000000 grpc-stubs-1.53.0.1/setup.py
+drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-29 10:45:36.427962 grpc-stubs-1.53.0.2/
+-rw-rw-r--   0 bl        (1000) bl        (1000)     1080 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/LICENSE
+-rw-rw-r--   0 bl        (1000) bl        (1000)     3428 2023-04-29 10:45:36.427962 grpc-stubs-1.53.0.2/PKG-INFO
+-rw-rw-r--   0 bl        (1000) bl        (1000)     2872 2023-04-07 10:11:59.000000 grpc-stubs-1.53.0.2/README.md
+drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-29 10:45:36.427962 grpc-stubs-1.53.0.2/grpc-stubs/
+-rw-rw-r--   0 bl        (1000) bl        (1000)    24256 2023-04-07 10:11:11.000000 grpc-stubs-1.53.0.2/grpc-stubs/__init__.pyi
+drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-29 10:45:36.427962 grpc-stubs-1.53.0.2/grpc-stubs/aio/
+-rw-rw-r--   0 bl        (1000) bl        (1000)    16499 2023-04-07 10:11:11.000000 grpc-stubs-1.53.0.2/grpc-stubs/aio/__init__.pyi
+-rw-rw-r--   0 bl        (1000) bl        (1000)        8 2023-04-07 10:11:11.000000 grpc-stubs-1.53.0.2/grpc-stubs/aio/py.typed
+-rw-rw-r--   0 bl        (1000) bl        (1000)        8 2023-03-05 04:14:41.000000 grpc-stubs-1.53.0.2/grpc-stubs/py.typed
+drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-29 10:45:36.427962 grpc-stubs-1.53.0.2/grpc_channelz-stubs/
+-rw-rw-r--   0 bl        (1000) bl        (1000)       56 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/grpc_channelz-stubs/__init__.pyi
+-rw-rw-r--   0 bl        (1000) bl        (1000)        0 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/grpc_channelz-stubs/py.typed
+drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-29 10:45:36.427962 grpc-stubs-1.53.0.2/grpc_channelz-stubs/v1/
+-rw-rw-r--   0 bl        (1000) bl        (1000)       56 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/grpc_channelz-stubs/v1/__init__.pyi
+-rw-rw-r--   0 bl        (1000) bl        (1000)     1330 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/grpc_channelz-stubs/v1/_servicer.pyi
+-rw-rw-r--   0 bl        (1000) bl        (1000)       84 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/grpc_channelz-stubs/v1/channelz.pyi
+drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-29 10:45:36.427962 grpc-stubs-1.53.0.2/grpc_health-stubs/
+-rw-rw-r--   0 bl        (1000) bl        (1000)       56 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/grpc_health-stubs/__init__.pyi
+-rw-rw-r--   0 bl        (1000) bl        (1000)        0 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/grpc_health-stubs/py.typed
+drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-29 10:45:36.427962 grpc-stubs-1.53.0.2/grpc_health-stubs/v1/
+-rw-rw-r--   0 bl        (1000) bl        (1000)       56 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/grpc_health-stubs/v1/__init__.pyi
+-rw-rw-r--   0 bl        (1000) bl        (1000)     1332 2022-04-16 02:10:26.000000 grpc-stubs-1.53.0.2/grpc_health-stubs/v1/health.pyi
+drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-29 10:45:36.427962 grpc-stubs-1.53.0.2/grpc_reflection-stubs/
+-rw-rw-r--   0 bl        (1000) bl        (1000)       56 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/grpc_reflection-stubs/__init__.pyi
+-rw-rw-r--   0 bl        (1000) bl        (1000)        0 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/grpc_reflection-stubs/py.typed
+drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-29 10:45:36.427962 grpc-stubs-1.53.0.2/grpc_reflection-stubs/v1alpha/
+-rw-rw-r--   0 bl        (1000) bl        (1000)       56 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/grpc_reflection-stubs/v1alpha/__init__.pyi
+-rw-rw-r--   0 bl        (1000) bl        (1000)      792 2023-04-29 10:44:37.000000 grpc-stubs-1.53.0.2/grpc_reflection-stubs/v1alpha/reflection.pyi
+drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-29 10:45:36.427962 grpc-stubs-1.53.0.2/grpc_status-stubs/
+-rw-rw-r--   0 bl        (1000) bl        (1000)       56 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/grpc_status-stubs/__init__.pyi
+-rw-rw-r--   0 bl        (1000) bl        (1000)        0 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/grpc_status-stubs/py.typed
+-rw-rw-r--   0 bl        (1000) bl        (1000)      455 2020-06-11 15:14:53.000000 grpc-stubs-1.53.0.2/grpc_status-stubs/rpc_status.pyi
+drwxrwxr-x   0 bl        (1000) bl        (1000)        0 2023-04-29 10:45:36.427962 grpc-stubs-1.53.0.2/grpc_stubs.egg-info/
+-rw-rw-r--   0 bl        (1000) bl        (1000)     3428 2023-04-29 10:45:36.000000 grpc-stubs-1.53.0.2/grpc_stubs.egg-info/PKG-INFO
+-rw-rw-r--   0 bl        (1000) bl        (1000)      841 2023-04-29 10:45:36.000000 grpc-stubs-1.53.0.2/grpc_stubs.egg-info/SOURCES.txt
+-rw-rw-r--   0 bl        (1000) bl        (1000)        1 2023-04-29 10:45:36.000000 grpc-stubs-1.53.0.2/grpc_stubs.egg-info/dependency_links.txt
+-rw-rw-r--   0 bl        (1000) bl        (1000)        7 2023-04-29 10:45:36.000000 grpc-stubs-1.53.0.2/grpc_stubs.egg-info/requires.txt
+-rw-rw-r--   0 bl        (1000) bl        (1000)       89 2023-04-29 10:45:36.000000 grpc-stubs-1.53.0.2/grpc_stubs.egg-info/top_level.txt
+-rw-rw-r--   0 bl        (1000) bl        (1000)      194 2023-04-29 10:45:36.427962 grpc-stubs-1.53.0.2/setup.cfg
+-rw-rw-r--   0 bl        (1000) bl        (1000)     1864 2023-04-29 10:44:23.000000 grpc-stubs-1.53.0.2/setup.py
```

### Comparing `grpc-stubs-1.53.0.1/LICENSE` & `grpc-stubs-1.53.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grpc-stubs-1.53.0.1/PKG-INFO` & `grpc-stubs-1.53.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpc-stubs
-Version: 1.53.0.1
+Version: 1.53.0.2
 Summary: Mypy stubs for gRPC
 Home-page: https://github.com/shabbyrobe/grpc-stubs
 Author: Blake Williams
 Author-email: code@shabbyrobe.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `grpc-stubs-1.53.0.1/README.md` & `grpc-stubs-1.53.0.2/README.md`

 * *Files identical despite different names*

### Comparing `grpc-stubs-1.53.0.1/grpc-stubs/__init__.pyi` & `grpc-stubs-1.53.0.2/grpc-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `grpc-stubs-1.53.0.1/grpc-stubs/aio/__init__.pyi` & `grpc-stubs-1.53.0.2/grpc-stubs/aio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `grpc-stubs-1.53.0.1/grpc_channelz-stubs/v1/_servicer.pyi` & `grpc-stubs-1.53.0.2/grpc_channelz-stubs/v1/_servicer.pyi`

 * *Files identical despite different names*

### Comparing `grpc-stubs-1.53.0.1/grpc_health-stubs/v1/health.pyi` & `grpc-stubs-1.53.0.2/grpc_health-stubs/v1/health.pyi`

 * *Files identical despite different names*

### Comparing `grpc-stubs-1.53.0.1/grpc_reflection-stubs/v1alpha/reflection.pyi` & `grpc-stubs-1.53.0.2/grpc_reflection-stubs/v1alpha/reflection.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,27 @@
+import typing
+
+import grpc
+from grpc import aio
 from google.protobuf import descriptor_pool
-from grpc import Server, ServicerContext
 from grpc_reflection.v1alpha import reflection_pb2 as _reflection_pb2
 from grpc_reflection.v1alpha._base import BaseReflectionServicer
-from typing import Iterable, List, Optional
 
 SERVICE_NAME: str
 
+AnyServer = typing.Union[grpc.Server, aio.Server]
+AnyServicerContext = typing.Union[grpc.ServicerContext, aio.ServicerContext]
+
 class ReflectionServicer(BaseReflectionServicer):
-    def ServerReflectionInfo(self, request_iterator: Iterable[_reflection_pb2.ServerReflectionRequest], context: ServicerContext) -> None:
+    def ServerReflectionInfo(
+        self,
+        request_iterator: typing.Iterable[_reflection_pb2.ServerReflectionRequest],
+        context: AnyServicerContext,
+    ) -> None:
         ...
 
-def enable_server_reflection(service_names: List[str], server: Server, pool: Optional[descriptor_pool.DescriptorPool] = ...) -> None:
+def enable_server_reflection(
+    service_names: typing.List[str],
+    server: AnyServer,
+    pool: typing.Optional[descriptor_pool.DescriptorPool] = ...,
+) -> None:
     ...
```

### Comparing `grpc-stubs-1.53.0.1/grpc_stubs.egg-info/PKG-INFO` & `grpc-stubs-1.53.0.2/grpc_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpc-stubs
-Version: 1.53.0.1
+Version: 1.53.0.2
 Summary: Mypy stubs for gRPC
 Home-page: https://github.com/shabbyrobe/grpc-stubs
 Author: Blake Williams
 Author-email: code@shabbyrobe.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `grpc-stubs-1.53.0.1/grpc_stubs.egg-info/SOURCES.txt` & `grpc-stubs-1.53.0.2/grpc_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpc-stubs-1.53.0.1/setup.py` & `grpc-stubs-1.53.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from typing import List
 
 from setuptools import find_packages
 from distutils.core import setup
 
-__version__ = "1.53.0.1"
+__version__ = "1.53.0.2"
 
 dependencies = [
     'grpcio',
 ]
 
 
 def find_stub_files(name: str) -> List[str]:
```


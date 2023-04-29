# Comparing `tmp/goxlrutilityapi-1.0.0.dev6.tar.gz` & `tmp/goxlrutilityapi-1.0.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.0.0.dev6.tar", last modified: Sat Apr 29 01:57:34 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.0.0.dev7.tar", last modified: Sat Apr 29 12:07:28 2023, max compression
```

## Comparing `goxlrutilityapi-1.0.0.dev6.tar` & `goxlrutilityapi-1.0.0.dev7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:57:34.087793 goxlrutilityapi-1.0.0.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 01:57:34.087793 goxlrutilityapi-1.0.0.dev6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:57:34.083793 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-29 01:57:32.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:57:34.087793 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13435 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:57:34.083793 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 01:57:34.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-29 01:57:34.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 01:57:34.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-29 01:57:34.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 01:57:34.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 01:57:34.087793 goxlrutilityapi-1.0.0.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:07:28.598775 goxlrutilityapi-1.0.0.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 12:07:28.598775 goxlrutilityapi-1.0.0.dev7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:07:28.594775 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-29 12:07:27.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:07:28.598775 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13324 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:07:28.594775 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 12:07:28.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-29 12:07:28.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 12:07:28.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-29 12:07:28.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 12:07:28.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 12:07:28.598775 goxlrutilityapi-1.0.0.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/setup.py
```

### Comparing `goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/__main__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/const.py` & `goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/const.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/helper.py` & `goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/helper.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/models/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,18 +45,18 @@
     device_type: str
     usb_device: UsbDevice
 
 
 class FaderStatus(DefaultBaseModel):
     """Fader Status Model"""
 
-    channel: str = Field(..., alias="Channel")
-    mute_type: str = Field(..., alias="MuteType")
-    scribble: Optional[Any] = Field(None, alias="Scribble")
-    mute_state: str = Field(..., alias="MuteState")
+    channel: str
+    mute_type: str
+    scribble: Optional[Any] = Field(None)
+    mute_state: str
 
 
 class FaderStatuses(DefaultBaseModel):
     """Fader Statuses Model"""
 
     a: FaderStatus = Field(..., alias="A")
     b: FaderStatus = Field(..., alias="B")
```

### Comparing `goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/websocket_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 import asyncio
 import socket
 from collections.abc import Awaitable, Callable
 from typing import Any, Optional
 
 import aiohttp
+import async_timeout
+from pydantic import ValidationError
 
 from .base import Base
 from .const import (
     DEFAULT_HOST,
     DEFAULT_PORT,
     KEY_DATA,
     KEY_ID,
@@ -105,15 +107,18 @@
             Response[Any]
         ] = asyncio.get_running_loop().create_future()
         self._responses[request.id] = future, response_type
         await self._websocket.send_str(request.json())
         self._logger.debug("Sent message: %s", request.json())
         if wait_for_response:
             try:
-                return await future
+                async with async_timeout.timeout(10):
+                    return await future
+            except asyncio.TimeoutError as error:
+                raise BadMessageException("Timeout waiting for response") from error
             finally:
                 self._responses.pop(request.id)
         return Response[None](
             id=request.id,
             data=None,
             type=None,
         )
@@ -167,15 +172,15 @@
                     raise BadMessageException("Message data is missing")
 
                 try:
                     if isinstance(response.data, list):
                         response.data = [model(**item) for item in response.data]
                     else:
                         response.data = model(**response.data)
-                except TypeError as error:
+                except (TypeError, ValidationError) as error:
                     raise BadMessageException(
                         f"Failed to create model '{message_type}' with data:\n{response.data}"
                     ) from error
 
                 self._logger.info(
                     "Response: %s",
                     response.json(
@@ -205,17 +210,17 @@
                                     "Future already set for response ID: %s",
                                     message_id,
                                 )
 
                 if patch_callback is not None and message_type == RESPONSE_TYPE_PATCH:
                     try:
                         await patch_callback(Response[Patch](**response.dict()))
-                    except TypeError as error:
+                    except (TypeError, ValidationError) as error:
                         raise BadMessageException(
-                            f"Failed to create model '{message_type}' with data:\n{response.data}"
+                            f"Failed to create model patch response with data:\n{response.data}"
                         ) from error
 
         await self._listen_for_messages(callback=_message_callback)
 
     async def _listen_for_messages(
         self,
         callback: Callable[[dict[Any, Any]], Awaitable[None]],
```

### Comparing `goxlrutilityapi-1.0.0.dev6/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.0.0.dev7/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev6/pyproject.toml` & `goxlrutilityapi-1.0.0.dev7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev6/setup.py` & `goxlrutilityapi-1.0.0.dev7/setup.py`

 * *Files identical despite different names*


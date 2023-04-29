# Comparing `tmp/goxlrutilityapi-1.0.0.dev8.tar.gz` & `tmp/goxlrutilityapi-1.0.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.0.0.dev8.tar", last modified: Sat Apr 29 13:26:08 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.0.0.dev9.tar", last modified: Sat Apr 29 15:19:07 2023, max compression
```

## Comparing `goxlrutilityapi-1.0.0.dev8.tar` & `goxlrutilityapi-1.0.0.dev9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:26:08.262676 goxlrutilityapi-1.0.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 13:26:08.262676 goxlrutilityapi-1.0.0.dev8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:26:08.258676 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-29 13:26:06.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:26:08.262676 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:26:08.258676 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 13:26:08.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-29 13:26:08.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:26:08.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-29 13:26:08.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 13:26:08.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 13:26:08.262676 goxlrutilityapi-1.0.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:19:07.143836 goxlrutilityapi-1.0.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 15:19:07.143836 goxlrutilityapi-1.0.0.dev9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:19:07.143836 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-29 15:19:05.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:19:07.143836 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:19:07.143836 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 15:19:07.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-29 15:19:07.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:19:07.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-29 15:19:07.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 15:19:07.000000 goxlrutilityapi-1.0.0.dev9/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:19:07.143836 goxlrutilityapi-1.0.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-29 15:18:50.000000 goxlrutilityapi-1.0.0.dev9/setup.py
```

### Comparing `goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/__main__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/const.py` & `goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/const.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/helper.py` & `goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/helper.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/models/status.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.0.0.dev9/goxlrutilityapi/websocket_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,16 +210,22 @@
                                 self._logger.debug(
                                     "Future already set for response ID: %s",
                                     message_id,
                                 )
 
                 if patch_callback is not None and message_type == RESPONSE_TYPE_PATCH:
                     try:
-                        self._logger.debug("Patch response: %s", response)
-                        await patch_callback(response)
+                        for item in response.data:
+                            patch_response = Response[Patch](
+                                id=response.id,
+                                type=response.type,
+                                data=item,
+                            )
+                            self._logger.debug("Patch callback: %s", patch_response)
+                            await patch_callback(patch_response)
                     except (TypeError, ValidationError) as error:
                         raise BadMessageException(
                             f"Failed to create model patch response with data:\n{response.data}"
                         ) from error
 
         await self._listen_for_messages(callback=_message_callback)
```

### Comparing `goxlrutilityapi-1.0.0.dev8/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.0.0.dev9/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev8/pyproject.toml` & `goxlrutilityapi-1.0.0.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev8/setup.py` & `goxlrutilityapi-1.0.0.dev9/setup.py`

 * *Files identical despite different names*


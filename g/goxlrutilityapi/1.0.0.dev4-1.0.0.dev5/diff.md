# Comparing `tmp/goxlrutilityapi-1.0.0.dev4.tar.gz` & `tmp/goxlrutilityapi-1.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.0.0.dev4.tar", last modified: Fri Apr 28 21:42:21 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.0.0.dev5.tar", last modified: Fri Apr 28 23:17:40 2023, max compression
```

## Comparing `goxlrutilityapi-1.0.0.dev4.tar` & `goxlrutilityapi-1.0.0.dev5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:42:21.658695 goxlrutilityapi-1.0.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 21:42:21.658695 goxlrutilityapi-1.0.0.dev4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:42:21.654695 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 21:42:09.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-28 21:42:09.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 21:42:20.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-28 21:42:09.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-28 21:42:09.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 21:42:09.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 21:42:09.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:42:21.658695 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 21:42:09.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-28 21:42:09.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 21:42:09.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-28 21:42:09.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-04-28 21:42:09.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-28 21:42:09.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:42:21.658695 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 21:42:21.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-28 21:42:21.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:42:21.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 21:42:21.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 21:42:21.000000 goxlrutilityapi-1.0.0.dev4/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-28 21:42:09.000000 goxlrutilityapi-1.0.0.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 21:42:21.658695 goxlrutilityapi-1.0.0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-28 21:42:09.000000 goxlrutilityapi-1.0.0.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:17:40.846442 goxlrutilityapi-1.0.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 23:17:40.846442 goxlrutilityapi-1.0.0.dev5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:17:40.842442 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 23:17:39.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:17:40.846442 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:17:40.842442 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 23:17:40.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-28 23:17:40.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:17:40.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 23:17:40.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 23:17:40.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:17:40.846442 goxlrutilityapi-1.0.0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/setup.py
```

### Comparing `goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,29 +25,31 @@
 loop = asyncio.new_event_loop()
 asyncio.set_event_loop(loop)
 websocket_client = WebsocketClient()
 
 
 def setup_websocket(
     callback: Optional[Callable[[Response[Patch]], Awaitable[None]]] = None
-) -> None:
+) -> bool:
     """Listen for messages on another thread"""
     try:
         loop.run_until_complete(websocket_client.connect())
         loop.create_task(
             websocket_client.listen(callback),
             name="Websocket Listener",
         )
     except (
         BadMessageException,
         ConnectionClosedException,
         ConnectionErrorException,
     ) as error:
         typer.secho(f"Error: {error}", fg=typer.colors.RED)
         loop.stop()
+        return False
+    return True
 
 
 async def patch_callback(response: Response[Patch]) -> None:
     """Patch response callback function"""
     typer.secho(
         response.json(
             include={
@@ -62,15 +64,17 @@
 
 
 @app.command(name="get_status", short_help="Get Status of GoXLR")
 def get_status(debug: bool = False) -> None:
     """Get Status of GoXLR"""
     if debug:
         setup_logger("DEBUG")
-    setup_websocket()
+    if setup_websocket() is False:
+        typer.secho("Failed to connect to GoXLR", fg=typer.colors.RED)
+        return
     try:
         status: Status = loop.run_until_complete(websocket_client.get_status())
     except BadMessageException as error:
         typer.secho(
             f"Failed to get status from GoXLR: {error}",
             fg=typer.colors.RED,
         )
```

### Comparing `goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/const.py` & `goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/const.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/models/status.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev4/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/websocket_client.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev4/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.0.0.dev5/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 setup.py
 goxlrutilityapi/__init__.py
 goxlrutilityapi/__main__.py
 goxlrutilityapi/_version.py
 goxlrutilityapi/base.py
 goxlrutilityapi/const.py
 goxlrutilityapi/exceptions.py
+goxlrutilityapi/helper.py
 goxlrutilityapi/logger.py
 goxlrutilityapi/websocket_client.py
 goxlrutilityapi.egg-info/PKG-INFO
 goxlrutilityapi.egg-info/SOURCES.txt
 goxlrutilityapi.egg-info/dependency_links.txt
 goxlrutilityapi.egg-info/requires.txt
 goxlrutilityapi.egg-info/top_level.txt
```

### Comparing `goxlrutilityapi-1.0.0.dev4/pyproject.toml` & `goxlrutilityapi-1.0.0.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev4/setup.py` & `goxlrutilityapi-1.0.0.dev5/setup.py`

 * *Files identical despite different names*


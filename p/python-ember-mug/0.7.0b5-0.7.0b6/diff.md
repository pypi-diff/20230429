# Comparing `tmp/python_ember_mug-0.7.0b5.tar.gz` & `tmp/python_ember_mug-0.7.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ember_mug-0.7.0b5.tar", max compression
+gzip compressed data, was "python_ember_mug-0.7.0b6.tar", max compression
```

## Comparing `python_ember_mug-0.7.0b5.tar` & `python_ember_mug-0.7.0b6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/LICENSE
--rw-r--r--   0        0        0     5282 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/README.md
--rwxr-xr-x   0        0        0      189 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/__init__.py
--rw-r--r--   0        0        0      106 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/__main__.py
--rw-r--r--   0        0        0      296 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/cli/__init__.py
--rw-r--r--   0        0        0     8933 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/cli/commands.py
--rw-r--r--   0        0        0     2910 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/cli/helpers.py
--rw-r--r--   0        0        0     5436 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/consts.py
--rw-r--r--   0        0        0     8946 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/data.py
--rw-r--r--   0        0        0      605 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/formatting.py
--rw-r--r--   0        0        0    18888 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/mug.py
--rw-r--r--   0        0        0     2212 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/scanner.py
--rw-r--r--   0        0        0     2707 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/ember_mug/utils.py
--rw-r--r--   0        0        0     2896 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/cli/__init__.py
--rw-r--r--   0        0        0     7846 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/cli/test_commands.py
--rw-r--r--   0        0        0     2663 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/cli/test_helpers.py
--rw-r--r--   0        0        0     1199 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/conftest.py
--rw-r--r--   0        0        0    19254 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/test_connection.py
--rw-r--r--   0        0        0     1115 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/test_consts.py
--rw-r--r--   0        0        0     2395 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/test_data.py
--rw-r--r--   0        0        0      534 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/test_formatting.py
--rw-r--r--   0        0        0     3428 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/test_mug_data.py
--rw-r--r--   0        0        0     2012 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/test_scanner.py
--rw-r--r--   0        0        0      801 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/test_utils.py
--rw-r--r--   0        0        0     6490 1970-01-01 00:00:00.000000 python_ember_mug-0.7.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/LICENSE
+-rw-r--r--   0        0        0     5282 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/README.md
+-rwxr-xr-x   0        0        0      189 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/__init__.py
+-rw-r--r--   0        0        0      106 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/__main__.py
+-rw-r--r--   0        0        0      296 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/cli/__init__.py
+-rw-r--r--   0        0        0     8933 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/cli/commands.py
+-rw-r--r--   0        0        0     2910 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/cli/helpers.py
+-rw-r--r--   0        0        0     5436 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/consts.py
+-rw-r--r--   0        0        0     8946 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/data.py
+-rw-r--r--   0        0        0      605 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/formatting.py
+-rw-r--r--   0        0        0    18898 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/mug.py
+-rw-r--r--   0        0        0     2212 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/scanner.py
+-rw-r--r--   0        0        0     3528 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/utils.py
+-rw-r--r--   0        0        0     2896 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/cli/__init__.py
+-rw-r--r--   0        0        0     7846 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/cli/test_commands.py
+-rw-r--r--   0        0        0     2663 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/cli/test_helpers.py
+-rw-r--r--   0        0        0     1199 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/conftest.py
+-rw-r--r--   0        0        0    19254 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/test_connection.py
+-rw-r--r--   0        0        0     1115 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/test_consts.py
+-rw-r--r--   0        0        0     2395 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/test_data.py
+-rw-r--r--   0        0        0      534 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/test_formatting.py
+-rw-r--r--   0        0        0     3428 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/test_mug_data.py
+-rw-r--r--   0        0        0     2012 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/test_scanner.py
+-rw-r--r--   0        0        0     2289 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/test_utils.py
+-rw-r--r--   0        0        0     6490 1970-01-01 00:00:00.000000 python_ember_mug-0.7.0b6/PKG-INFO
```

### Comparing `python_ember_mug-0.7.0b5/LICENSE` & `python_ember_mug-0.7.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/README.md` & `python_ember_mug-0.7.0b6/README.md`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/ember_mug/cli/commands.py` & `python_ember_mug-0.7.0b6/ember_mug/cli/commands.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/ember_mug/cli/helpers.py` & `python_ember_mug-0.7.0b6/ember_mug/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/ember_mug/consts.py` & `python_ember_mug-0.7.0b6/ember_mug/consts.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/ember_mug/data.py` & `python_ember_mug-0.7.0b6/ember_mug/data.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/ember_mug/formatting.py` & `python_ember_mug-0.7.0b6/ember_mug/formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/ember_mug/mug.py` & `python_ember_mug-0.7.0b6/ember_mug/mug.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     VolumeLevel,
 )
 from .data import BatteryInfo, Change, Colour, Model, MugData, MugFirmwareInfo, MugMeta
 from .utils import (
     bytes_to_big_int,
     bytes_to_little_int,
     decode_byte_string,
+    discover_services,
     encode_byte_string,
-    log_services,
     temp_from_bytes,
 )
 
 logger = logging.getLogger(__name__)
 
 DISCONNECT_DELAY = 120
 
@@ -105,15 +105,15 @@
                     device=self.device,
                     name=f'{self.data.name} ({self.device.address})',
                     use_services_cache=True,
                     disconnected_callback=self._disconnect_callback,  # type: ignore
                     ble_device_callback=lambda: self.device,
                 )
                 if self.debug is True:
-                    await log_services(client)
+                    await discover_services(client)
                 self._expected_disconnect = False
             except (asyncio.TimeoutError, BleakError) as error:
                 logger.error("%s: Failed to connect to the mug: %s", self.device, error)
                 raise error
             # Attempt to pair for good measure
             try:
                 await client.pair()
```

### Comparing `python_ember_mug-0.7.0b5/ember_mug/scanner.py` & `python_ember_mug-0.7.0b6/ember_mug/scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/ember_mug/utils.py` & `python_ember_mug-0.7.0b6/ember_mug/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Helpful utils for processing mug data."""
 from __future__ import annotations
 
 import base64
 import contextlib
 import logging
 import re
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
+
+from bleak import BleakError
 
 if TYPE_CHECKING:
-    from bleak import BleakClient, BleakError
+    from bleak import BleakClient
 
 logger = logging.getLogger(__name__)
 
 
 def decode_byte_string(data: bytes | bytearray) -> str:
     """Convert bytes to text as Ember expects."""
     if not data:
@@ -44,34 +46,55 @@
     temp = float(bytes_to_little_int(temp_bytes)) * 0.01
     if metric is False:
         # Convert to fahrenheit
         temp = (temp * 9 / 5) + 32
     return round(temp, 2)
 
 
-async def log_services(client: BleakClient) -> None:
+async def discover_services(client: BleakClient) -> dict[str, Any]:
     """Log all services and all values for debugging/development."""
     logger.info("Logging all services that were discovered")
+    services: dict[str, Any] = {}
     for service in client.services:
-        logger.info("[Service] %s: %s", service.uuid, service.description)
+        logger.debug("[Service] %s: %s", service.uuid, service.description)
+        characteristics: dict[str, Any] = {}
+        services[service.uuid] = {
+            'uuid': service.uuid,
+            'characteristics': characteristics,
+        }
         for characteristic in service.characteristics:
-            value: bytearray | BleakError | None = None
+            value: bytes | BleakError | None = None
             if "read" in characteristic.properties:
                 try:
-                    value = await client.read_gatt_char(characteristic.uuid)
+                    value = bytes(await client.read_gatt_char(characteristic.uuid))
                 except BleakError as e:
                     value = e
-            logger.info(
-                "\t[Characteristic] %s: %s | Name: %s | Value: '%s'",
+            logger.debug(
+                "\t[Characteristic] %s: %s | Description: %s | Value: '%s'",
                 characteristic.uuid,
                 ",".join(characteristic.properties),
                 characteristic.description,
                 value,
             )
+            descriptors: list[dict[str, Any]] = []
+            characteristics[characteristic.uuid] = {
+                'uuid': characteristic.uuid,
+                'properties': characteristic.properties,
+                'value': value,
+                'descriptors': descriptors,
+            }
             for descriptor in characteristic.descriptors:
-                value = await client.read_gatt_descriptor(descriptor.handle)
-                logger.info(
+                value = bytes(await client.read_gatt_descriptor(descriptor.handle))
+                logger.debug(
                     "\t\t[Descriptor] %s: Handle: %s | Value: '%s'",
                     descriptor.uuid,
                     descriptor.handle,
                     value,
                 )
+                descriptors.append(
+                    {
+                        'uuid': descriptor.uuid,
+                        'handle': descriptor.handle,
+                        'value': value,
+                    },
+                )
+    return services
```

### Comparing `python_ember_mug-0.7.0b5/pyproject.toml` & `python_ember_mug-0.7.0b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "python-ember-mug"
-version = "0.7.0b5"
+version = "0.7.0b6"
 homepage = "https://github.com/sopelj/python-ember-mug"
 description = "Python Library for Ember Mugs."
 authors = ["Jesse Sopel <jesse.sopel@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `python_ember_mug-0.7.0b5/tests/cli/test_commands.py` & `python_ember_mug-0.7.0b6/tests/cli/test_commands.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/tests/cli/test_helpers.py` & `python_ember_mug-0.7.0b6/tests/cli/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/tests/conftest.py` & `python_ember_mug-0.7.0b6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/tests/test_connection.py` & `python_ember_mug-0.7.0b6/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/tests/test_consts.py` & `python_ember_mug-0.7.0b6/tests/test_consts.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/tests/test_data.py` & `python_ember_mug-0.7.0b6/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/tests/test_formatting.py` & `python_ember_mug-0.7.0b6/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/tests/test_mug_data.py` & `python_ember_mug-0.7.0b6/tests/test_mug_data.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/tests/test_scanner.py` & `python_ember_mug-0.7.0b6/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b5/PKG-INFO` & `python_ember_mug-0.7.0b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ember-mug
-Version: 0.7.0b5
+Version: 0.7.0b6
 Summary: Python Library for Ember Mugs.
 Home-page: https://github.com/sopelj/python-ember-mug
 License: MIT
 Author: Jesse Sopel
 Author-email: jesse.sopel@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```


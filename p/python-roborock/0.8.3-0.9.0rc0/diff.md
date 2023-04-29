# Comparing `tmp/python_roborock-0.8.3.tar.gz` & `tmp/python_roborock-0.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.8.3.tar", max compression
+gzip compressed data, was "python_roborock-0.9.0rc0.tar", max compression
```

## Comparing `python_roborock-0.8.3.tar` & `python_roborock-0.9.0rc0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-04-28 00:36:07.290760 python_roborock-0.8.3/LICENSE
--rw-r--r--   0        0        0     2122 2023-04-28 00:36:07.290760 python_roborock-0.8.3/README.md
--rw-r--r--   0        0        0     1370 2023-04-28 00:36:08.494767 python_roborock-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-28 00:36:07.290760 python_roborock-0.8.3/roborock/__init__.py
--rw-r--r--   0        0        0    20956 2023-04-28 00:36:07.290760 python_roborock-0.8.3/roborock/api.py
--rw-r--r--   0        0        0     3991 2023-04-28 00:36:07.290760 python_roborock-0.8.3/roborock/cli.py
--rw-r--r--   0        0        0     7649 2023-04-28 00:36:07.290760 python_roborock-0.8.3/roborock/cloud_api.py
--rw-r--r--   0        0        0     4620 2023-04-28 00:36:07.290760 python_roborock-0.8.3/roborock/code_mappings.py
--rw-r--r--   0        0        0      209 2023-04-28 00:36:07.290760 python_roborock-0.8.3/roborock/const.py
--rw-r--r--   0        0        0    10730 2023-04-28 00:36:07.290760 python_roborock-0.8.3/roborock/containers.py
--rw-r--r--   0        0        0     1483 2023-04-28 00:36:07.290760 python_roborock-0.8.3/roborock/exceptions.py
--rw-r--r--   0        0        0     6578 2023-04-28 00:36:07.290760 python_roborock-0.8.3/roborock/local_api.py
--rw-r--r--   0        0        0      694 2023-04-28 00:36:07.290760 python_roborock-0.8.3/roborock/roborock_future.py
--rw-r--r--   0        0        0     6232 2023-04-28 00:36:07.290760 python_roborock-0.8.3/roborock/roborock_message.py
--rw-r--r--   0        0        0    12651 2023-04-28 00:36:07.290760 python_roborock-0.8.3/roborock/typing.py
--rw-r--r--   0        0        0      783 2023-04-28 00:36:07.290760 python_roborock-0.8.3/roborock/util.py
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-15 23:23:41.026106 python_roborock-0.9.0rc0/LICENSE
+-rw-r--r--   0        0        0     2122 2023-04-17 23:50:22.944797 python_roborock-0.9.0rc0/README.md
+-rw-r--r--   0        0        0     1373 2023-04-29 00:38:52.377261 python_roborock-0.9.0rc0/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-17 23:50:22.945724 python_roborock-0.9.0rc0/roborock/__init__.py
+-rw-r--r--   0        0        0    20953 2023-04-29 00:19:12.443894 python_roborock-0.9.0rc0/roborock/api.py
+-rw-r--r--   0        0        0     4102 2023-04-29 00:14:20.401256 python_roborock-0.9.0rc0/roborock/cli.py
+-rw-r--r--   0        0        0     7261 2023-04-29 00:18:57.528713 python_roborock-0.9.0rc0/roborock/cloud_api.py
+-rw-r--r--   0        0        0     4620 2023-04-29 00:15:07.502108 python_roborock-0.9.0rc0/roborock/code_mappings.py
+-rw-r--r--   0        0        0      209 2023-04-27 14:49:49.843263 python_roborock-0.9.0rc0/roborock/const.py
+-rw-r--r--   0        0        0    10730 2023-04-27 14:49:49.843775 python_roborock-0.9.0rc0/roborock/containers.py
+-rw-r--r--   0        0        0     1483 2023-04-27 14:49:49.930465 python_roborock-0.9.0rc0/roborock/exceptions.py
+-rw-r--r--   0        0        0     5635 2023-04-29 00:24:11.618489 python_roborock-0.9.0rc0/roborock/local_api.py
+-rw-r--r--   0        0        0      694 2023-04-22 02:10:16.435351 python_roborock-0.9.0rc0/roborock/roborock_future.py
+-rw-r--r--   0        0        0     6358 2023-04-29 00:14:58.499142 python_roborock-0.9.0rc0/roborock/roborock_message.py
+-rw-r--r--   0        0        0     4626 2023-04-29 00:06:49.142059 python_roborock-0.9.0rc0/roborock/test.py
+-rw-r--r--   0        0        0    18391 2023-04-29 00:18:15.411897 python_roborock-0.9.0rc0/roborock/typing.py
+-rw-r--r--   0        0        0      783 2023-04-25 18:03:12.110531 python_roborock-0.9.0rc0/roborock/util.py
+-rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 python_roborock-0.9.0rc0/PKG-INFO
```

### Comparing `python_roborock-0.8.3/LICENSE` & `python_roborock-0.9.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.3/README.md` & `python_roborock-0.9.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.3/pyproject.toml` & `python_roborock-0.9.0rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.8.3"
+version = "0.9.0-rc"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `python_roborock-0.8.3/roborock/api.py` & `python_roborock-0.9.0rc0/roborock/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import json
 import logging
 import math
 import secrets
 import struct
 import time
 from random import randint
-from typing import Any, Callable, Coroutine, Mapping, Optional
+from typing import Any, Callable, Coroutine, Optional
 
 import aiohttp
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import unpad
 
 from .code_mappings import RoborockDockTypeCode, RoborockEnum
 from .containers import (
@@ -81,106 +81,123 @@
                 data=data,
                 headers=_headers,
             ) as resp:
                 return await resp.json()
 
 
 class RoborockClient:
-    def __init__(self, endpoint: str, devices_info: Mapping[str, RoborockDeviceInfo]) -> None:
-        self.devices_info = devices_info
+    def __init__(self, endpoint: str, device_info: RoborockDeviceInfo) -> None:
+        self.device_info = device_info
         self._endpoint = endpoint
         self._nonce = secrets.token_bytes(16)
         self._waiting_queue: dict[int, RoborockFuture] = {}
         self._last_device_msg_in = self.time_func()
         self._last_disconnection = self.time_func()
         self.keep_alive = KEEPALIVE
 
+    def __del__(self) -> None:
+        self.sync_disconnect()
+
     @property
     def time_func(self) -> Callable[[], float]:
         try:
             # Use monotonic clock if available
             time_func = time.monotonic
         except AttributeError:
             time_func = time.time
         return time_func
 
+    async def async_connect(self):
+        raise NotImplementedError
+
+    def sync_disconnect(self) -> Any:
+        raise NotImplementedError
+
     async def async_disconnect(self) -> Any:
         raise NotImplementedError
 
-    def on_message(self, messages: list[RoborockMessage]) -> None:
+    def on_message_received(self, messages: list[RoborockMessage]) -> None:
         try:
             self._last_device_msg_in = self.time_func()
             for data in messages:
                 protocol = data.protocol
                 if protocol == 102 or protocol == 4:
                     payload = json.loads(data.payload.decode())
                     for data_point_number, data_point in payload.get("dps").items():
                         if data_point_number == "102":
                             data_point_response = json.loads(data_point)
                             request_id = data_point_response.get("id")
                             queue = self._waiting_queue.get(request_id)
-                            if queue:
-                                if queue.protocol == protocol:
-                                    error = data_point_response.get("error")
-                                    if error:
-                                        queue.resolve(
-                                            (
-                                                None,
-                                                VacuumError(
-                                                    error.get("code"),
-                                                    error.get("message"),
-                                                ),
-                                            )
+                            if queue and queue.protocol == protocol:
+                                error = data_point_response.get("error")
+                                if error:
+                                    queue.resolve(
+                                        (
+                                            None,
+                                            VacuumError(
+                                                error.get("code"),
+                                                error.get("message"),
+                                            ),
                                         )
-                                    else:
-                                        result = data_point_response.get("result")
-                                        if isinstance(result, list) and len(result) == 1:
-                                            result = result[0]
-                                        queue.resolve((result, None))
+                                    )
+                                else:
+                                    result = data_point_response.get("result")
+                                    if isinstance(result, list) and len(result) == 1:
+                                        result = result[0]
+                                    queue.resolve((result, None))
                 elif protocol == 301:
                     payload = data.payload[0:24]
                     [endpoint, _, request_id, _] = struct.unpack("<15sBH6s", payload)
                     if endpoint.decode().startswith(self._endpoint):
                         iv = bytes(AES.block_size)
                         decipher = AES.new(self._nonce, AES.MODE_CBC, iv)
                         decrypted = unpad(decipher.decrypt(data.payload[24:]), AES.block_size)
                         decrypted = gzip.decompress(decrypted)
                         queue = self._waiting_queue.get(request_id)
                         if queue:
                             if isinstance(decrypted, list):
                                 decrypted = decrypted[0]
                             queue.resolve((decrypted, None))
+                else:
+                    queue = self._waiting_queue.get(data.seq)
+                    if queue:
+                        queue.resolve((data.payload, None))
         except Exception as ex:
             _LOGGER.exception(ex)
 
-    def on_disconnect(self, exc: Optional[Exception]) -> None:
+    def on_connection_lost(self, exc: Optional[Exception]) -> None:
         self._last_disconnection = self.time_func()
         _LOGGER.warning("Roborock client disconnected")
         if exc is not None:
             _LOGGER.warning(exc)
 
     def should_keepalive(self) -> bool:
         now = self.time_func()
         # noinspection PyUnresolvedReferences
         if now - self._last_disconnection > self.keep_alive**2 and now - self._last_device_msg_in > self.keep_alive:
             return False
         return True
 
+    async def validate_connection(self) -> None:
+        if not self.should_keepalive():
+            await self.async_disconnect()
+        await self.async_connect()
+
     async def _async_response(self, request_id: int, protocol_id: int = 0) -> tuple[Any, VacuumError | None]:
         try:
             queue = RoborockFuture(protocol_id)
             self._waiting_queue[request_id] = queue
             (response, err) = await queue.async_get(QUEUE_TIMEOUT)
             return response, err
         except (asyncio.TimeoutError, asyncio.CancelledError):
             raise RoborockTimeout(f"Timeout after {QUEUE_TIMEOUT} seconds waiting for response") from None
         finally:
             del self._waiting_queue[request_id]
 
-    def _get_payload(self, method: RoborockCommand, params: Optional[list] = None, secured=False):
+    def _get_payload(self, method: RoborockCommand, params: Optional[list | dict] = None, secured=False):
         timestamp = math.floor(time.time())
         request_id = randint(10000, 99999)
         inner = {
             "id": request_id,
             "method": method,
             "params": params or [],
         }
@@ -196,165 +213,164 @@
                     "t": timestamp,
                 },
                 separators=(",", ":"),
             ).encode()
         )
         return request_id, timestamp, payload
 
-    async def send_command(self, device_id: str, method: RoborockCommand, params: Optional[list] = None):
+    async def send_command(self, method: RoborockCommand, params: Optional[list | dict] = None):
         raise NotImplementedError
 
-    async def get_status(self, device_id: str) -> Status | None:
-        status = await self.send_command(device_id, RoborockCommand.GET_STATUS)
+    async def get_status(self) -> Status | None:
+        status = await self.send_command(RoborockCommand.GET_STATUS)
         if isinstance(status, dict):
             return Status.from_dict(status)
         return None
 
-    async def get_dnd_timer(self, device_id: str) -> DNDTimer | None:
+    async def get_dnd_timer(self) -> DNDTimer | None:
         try:
-            dnd_timer = await self.send_command(device_id, RoborockCommand.GET_DND_TIMER)
+            dnd_timer = await self.send_command(RoborockCommand.GET_DND_TIMER)
             if isinstance(dnd_timer, dict):
                 return DNDTimer.from_dict(dnd_timer)
         except RoborockTimeout as e:
             _LOGGER.error(e)
         return None
 
-    async def get_clean_summary(self, device_id: str) -> CleanSummary | None:
+    async def get_clean_summary(self) -> CleanSummary | None:
         try:
-            clean_summary = await self.send_command(device_id, RoborockCommand.GET_CLEAN_SUMMARY)
+            clean_summary = await self.send_command(RoborockCommand.GET_CLEAN_SUMMARY)
             if isinstance(clean_summary, dict):
                 return CleanSummary.from_dict(clean_summary)
             elif isinstance(clean_summary, list):
                 clean_time, clean_area, clean_count, records = unpack_list(clean_summary, 4)
                 return CleanSummary(
                     clean_time=clean_time, clean_area=clean_area, clean_count=clean_count, records=records
                 )
         except RoborockTimeout as e:
             _LOGGER.error(e)
         return None
 
-    async def get_clean_record(self, device_id: str, record_id: int) -> CleanRecord | None:
+    async def get_clean_record(self, record_id: int) -> CleanRecord | None:
         try:
-            clean_record = await self.send_command(device_id, RoborockCommand.GET_CLEAN_RECORD, [record_id])
+            clean_record = await self.send_command(RoborockCommand.GET_CLEAN_RECORD, [record_id])
             if isinstance(clean_record, dict):
                 return CleanRecord.from_dict(clean_record)
         except RoborockTimeout as e:
             _LOGGER.error(e)
         return None
 
-    async def get_consumable(self, device_id: str) -> Consumable | None:
+    async def get_consumable(self) -> Consumable | None:
         try:
-            consumable = await self.send_command(device_id, RoborockCommand.GET_CONSUMABLE)
+            consumable = await self.send_command(RoborockCommand.GET_CONSUMABLE)
             if isinstance(consumable, dict):
                 return Consumable.from_dict(consumable)
         except RoborockTimeout as e:
             _LOGGER.error(e)
         return None
 
-    async def get_wash_towel_mode(self, device_id: str) -> WashTowelMode | None:
+    async def get_wash_towel_mode(self) -> WashTowelMode | None:
         try:
-            washing_mode = await self.send_command(device_id, RoborockCommand.GET_WASH_TOWEL_MODE)
+            washing_mode = await self.send_command(RoborockCommand.GET_WASH_TOWEL_MODE)
             if isinstance(washing_mode, dict):
                 return WashTowelMode.from_dict(washing_mode)
         except RoborockTimeout as e:
             _LOGGER.error(e)
         return None
 
-    async def get_dust_collection_mode(self, device_id: str) -> DustCollectionMode | None:
+    async def get_dust_collection_mode(self) -> DustCollectionMode | None:
         try:
-            dust_collection = await self.send_command(device_id, RoborockCommand.GET_DUST_COLLECTION_MODE)
+            dust_collection = await self.send_command(RoborockCommand.GET_DUST_COLLECTION_MODE)
             if isinstance(dust_collection, dict):
                 return DustCollectionMode.from_dict(dust_collection)
         except RoborockTimeout as e:
             _LOGGER.error(e)
         return None
 
-    async def get_smart_wash_params(self, device_id: str) -> SmartWashParams | None:
+    async def get_smart_wash_params(self) -> SmartWashParams | None:
         try:
-            mop_wash_mode = await self.send_command(device_id, RoborockCommand.GET_SMART_WASH_PARAMS)
+            mop_wash_mode = await self.send_command(RoborockCommand.GET_SMART_WASH_PARAMS)
             if isinstance(mop_wash_mode, dict):
                 return SmartWashParams.from_dict(mop_wash_mode)
         except RoborockTimeout as e:
             _LOGGER.error(e)
         return None
 
-    async def get_dock_summary(self, device_id: str, dock_type: RoborockEnum) -> DockSummary | None:
+    async def get_dock_summary(self, dock_type: RoborockEnum) -> DockSummary | None:
         """Gets the status summary from the dock with the methods available for a given dock.
 
-        :param device_id: Device id
         :param dock_type: RoborockDockTypeCode"""
         try:
             commands: list[
                 Coroutine[
                     Any,
                     Any,
                     DustCollectionMode | WashTowelMode | SmartWashParams | None,
                 ]
-            ] = [self.get_dust_collection_mode(device_id)]
+            ] = [self.get_dust_collection_mode()]
             if dock_type == RoborockDockTypeCode["3"]:
                 commands += [
-                    self.get_wash_towel_mode(device_id),
-                    self.get_smart_wash_params(device_id),
+                    self.get_wash_towel_mode(),
+                    self.get_smart_wash_params(),
                 ]
             [dust_collection_mode, wash_towel_mode, smart_wash_params] = unpack_list(
                 list(await asyncio.gather(*commands)), 3
             )
 
             return DockSummary(dust_collection_mode, wash_towel_mode, smart_wash_params)
         except RoborockTimeout as e:
             _LOGGER.error(e)
         return None
 
-    async def get_prop(self, device_id: str) -> DeviceProp | None:
+    async def get_prop(self) -> DeviceProp | None:
         [status, dnd_timer, clean_summary, consumable] = await asyncio.gather(
             *[
-                self.get_status(device_id),
-                self.get_dnd_timer(device_id),
-                self.get_clean_summary(device_id),
-                self.get_consumable(device_id),
+                self.get_status(),
+                self.get_dnd_timer(),
+                self.get_clean_summary(),
+                self.get_consumable(),
             ]
         )
         last_clean_record = None
         if clean_summary and clean_summary.records and len(clean_summary.records) > 0:
-            last_clean_record = await self.get_clean_record(device_id, clean_summary.records[0])
+            last_clean_record = await self.get_clean_record(clean_summary.records[0])
         dock_summary = None
         if status and status.dock_type is not None and status.dock_type != RoborockDockTypeCode["0"]:
-            dock_summary = await self.get_dock_summary(device_id, status.dock_type)
+            dock_summary = await self.get_dock_summary(status.dock_type)
         if any([status, dnd_timer, clean_summary, consumable]):
             return DeviceProp(
                 status,
                 dnd_timer,
                 clean_summary,
                 consumable,
                 last_clean_record,
                 dock_summary,
             )
         return None
 
-    async def get_multi_maps_list(self, device_id) -> MultiMapsList | None:
+    async def get_multi_maps_list(self) -> MultiMapsList | None:
         try:
-            multi_maps_list = await self.send_command(device_id, RoborockCommand.GET_MULTI_MAPS_LIST)
+            multi_maps_list = await self.send_command(RoborockCommand.GET_MULTI_MAPS_LIST)
             if isinstance(multi_maps_list, dict):
                 return MultiMapsList.from_dict(multi_maps_list)
         except RoborockTimeout as e:
             _LOGGER.error(e)
         return None
 
-    async def get_networking(self, device_id) -> NetworkInfo | None:
+    async def get_networking(self) -> NetworkInfo | None:
         try:
-            networking_info = await self.send_command(device_id, RoborockCommand.GET_NETWORK_INFO)
+            networking_info = await self.send_command(RoborockCommand.GET_NETWORK_INFO)
             if isinstance(networking_info, dict):
                 return NetworkInfo.from_dict(networking_info)
         except RoborockTimeout as e:
             _LOGGER.error(e)
         return None
 
-    async def get_room_mapping(self, device_id: str) -> list[RoomMapping]:
+    async def get_room_mapping(self) -> list[RoomMapping]:
         """Gets the mapping from segment id -> iot id. Only works on local api."""
-        mapping = await self.send_command(device_id, RoborockCommand.GET_ROOM_MAPPING)
+        mapping = await self.send_command(RoborockCommand.GET_ROOM_MAPPING)
         if isinstance(mapping, list):
             return [
                 RoomMapping(segment_id=segment_id, iot_id=iot_id)  # type: ignore
                 for segment_id, iot_id in [unpack_list(room, 2) for room in mapping]
             ]
         return []
```

### Comparing `python_roborock-0.8.3/roborock/cli.py` & `python_roborock-0.9.0rc0/roborock/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,34 +98,38 @@
 async def list_devices(ctx):
     context: RoborockContext = ctx.obj
     login_data = context.login_data()
     if not login_data.home_data:
         await _discover(ctx)
         login_data = context.login_data()
     home_data = login_data.home_data
-    click.echo(f"Known devices {', '.join([device.name for device in home_data.devices + home_data.received_devices])}")
+    device_name_id = ", ".join(
+        [f"{device.name}: {device.duid}" for device in home_data.devices + home_data.received_devices]
+    )
+    click.echo(f"Known devices {device_name_id}")
 
 
 @click.command()
+@click.option("--device_id", required=True)
 @click.option("--cmd", required=True)
 @click.option("--params", required=False)
 @click.pass_context
 @run_sync()
-async def command(ctx, cmd, params):
+async def command(ctx, cmd, device_id, params):
     context: RoborockContext = ctx.obj
     login_data = context.login_data()
     if not login_data.home_data:
         await _discover(ctx)
         login_data = context.login_data()
     home_data = login_data.home_data
-    device_map: dict[str, RoborockDeviceInfo] = {}
-    for device in home_data.devices + home_data.received_devices:
-        device_map[device.duid] = RoborockDeviceInfo(device=device)
-    mqtt_client = RoborockMqttClient(login_data.user_data, device_map)
-    await mqtt_client.send_command(home_data.devices[0].duid, cmd, params)
+    devices = home_data.devices + home_data.received_devices
+    device = next((device for device in devices if device.duid == device_id), None)
+    device_info = RoborockDeviceInfo(device=device)
+    mqtt_client = RoborockMqttClient(login_data.user_data, device_info)
+    await mqtt_client.send_command(cmd, params)
     mqtt_client.__del__()
 
 
 cli.add_command(login)
 cli.add_command(discover)
 cli.add_command(list_devices)
 cli.add_command(command)
```

### Comparing `python_roborock-0.8.3/roborock/cloud_api.py` & `python_roborock-0.9.0rc0/roborock/cloud_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import base64
 import logging
 import threading
 import uuid
 from asyncio import Lock
-from typing import Mapping, Optional
+from typing import Optional
 from urllib.parse import urlparse
 
 import paho.mqtt.client as mqtt
 
 from .api import KEEPALIVE, SPECIAL_COMMANDS, RoborockClient, md5hex
 from .containers import RoborockDeviceInfo, UserData
 from .exceptions import CommandVacuumError, RoborockException, VacuumError
@@ -20,92 +20,86 @@
 _LOGGER = logging.getLogger(__name__)
 CONNECT_REQUEST_ID = 0
 DISCONNECT_REQUEST_ID = 1
 
 
 class RoborockMqttClient(RoborockClient, mqtt.Client):
     _thread: threading.Thread
+    _client_id: str
 
-    def __init__(self, user_data: UserData, devices_info: Mapping[str, RoborockDeviceInfo]) -> None:
+    def __init__(self, user_data: UserData, device_info: RoborockDeviceInfo) -> None:
         rriot = user_data.rriot
         if rriot is None:
             raise RoborockException("Got no rriot data from user_data")
         endpoint = base64.b64encode(md5bin(rriot.k)[8:14]).decode()
-        RoborockClient.__init__(self, endpoint, devices_info)
+        RoborockClient.__init__(self, endpoint, device_info)
         mqtt.Client.__init__(self, protocol=mqtt.MQTTv5)
         self._mqtt_user = rriot.u
         self._hashed_user = md5hex(self._mqtt_user + ":" + rriot.k)[2:10]
         url = urlparse(rriot.r.m)
         if not isinstance(url.hostname, str):
             raise RoborockException("Url parsing returned an invalid hostname")
-        self._mqtt_host = url.hostname
+        self._mqtt_host = str(url.hostname)
         self._mqtt_port = url.port
         self._mqtt_ssl = url.scheme == "ssl"
         if self._mqtt_ssl:
             super().tls_set()
         self._mqtt_password = rriot.s
         self._hashed_password = md5hex(self._mqtt_password + ":" + rriot.k)[16:]
         super().username_pw_set(self._hashed_user, self._hashed_password)
         self._endpoint = base64.b64encode(md5bin(rriot.k)[8:14]).decode()
         self._waiting_queue: dict[int, RoborockFuture] = {}
         self._mutex = Lock()
         self.update_client_id()
 
-    def __del__(self) -> None:
-        self.sync_disconnect()
-
-    def on_connect(self, *args, **kwargs) -> None:
+    def on_connect(self, *args, **kwargs):
         _, __, ___, rc, ____ = args
         connection_queue = self._waiting_queue.get(CONNECT_REQUEST_ID)
         if rc != mqtt.MQTT_ERR_SUCCESS:
             message = f"Failed to connect (rc: {rc})"
             _LOGGER.error(message)
             if connection_queue:
                 connection_queue.resolve((None, VacuumError(rc, message)))
             return
         _LOGGER.info(f"Connected to mqtt {self._mqtt_host}:{self._mqtt_port}")
-        topic = f"rr/m/o/{self._mqtt_user}/{self._hashed_user}/#"
+        topic = f"rr/m/o/{self._mqtt_user}/{self._hashed_user}/{self.device_info.device.duid}"
         (result, mid) = self.subscribe(topic)
         if result != 0:
             message = f"Failed to subscribe (rc: {result})"
             _LOGGER.error(message)
             if connection_queue:
                 connection_queue.resolve((None, VacuumError(rc, message)))
             return
         _LOGGER.info(f"Subscribed to topic {topic}")
         if connection_queue:
             connection_queue.resolve((True, None))
 
-    def on_message(self, *args, **kwargs) -> None:
+    def on_message(self, *args, **kwargs):
         _, __, msg = args
-        device_id = msg.topic.split("/").pop()
-        messages, _ = RoborockParser.decode(msg.payload, self.devices_info[device_id].device.local_key)
-        super().on_message(messages)
+        try:
+            messages, _ = RoborockParser.decode(msg.payload, self.device_info.device.local_key)
+            super().on_message_received(messages)
+        except Exception as ex:
+            _LOGGER.exception(ex)
 
-    def on_disconnect(self, *args, **kwargs) -> None:
+    def on_disconnect(self, *args, **kwargs):
+        _, __, rc, ___ = args
         try:
-            _, __, rc, ___ = args
-            super().on_disconnect(RoborockException(f"(rc: {rc})"))
+            super().on_connection_lost(RoborockException(f"(rc: {rc})"))
             if rc == mqtt.MQTT_ERR_PROTOCOL:
                 self.update_client_id()
             connection_queue = self._waiting_queue.get(DISCONNECT_REQUEST_ID)
             if connection_queue:
                 connection_queue.resolve((True, None))
         except Exception as ex:
             _LOGGER.exception(ex)
 
     def update_client_id(self):
         self._client_id = mqtt.base62(uuid.uuid4().int, padding=22)
 
-    def _check_keepalive(self) -> None:
-        if not self.should_keepalive():
-            self._ping_t = self.time_func() - KEEPALIVE
-            # noinspection PyUnresolvedReferences
-        super()._check_keepalive()  # type: ignore[misc]
-
     def sync_stop_loop(self) -> None:
         if self._thread:
             _LOGGER.info("Stopping mqtt loop")
             super().loop_stop()
 
     def sync_start_loop(self) -> None:
         if not self._thread or not self._thread.is_alive():
@@ -144,40 +138,37 @@
         async with self._mutex:
             connecting = self.sync_connect()
             if connecting:
                 (_, err) = await self._async_response(CONNECT_REQUEST_ID)
                 if err:
                     raise RoborockException(err) from err
 
-    async def validate_connection(self) -> None:
-        await self.async_connect()
-
-    def _send_msg_raw(self, device_id, msg) -> None:
-        info = self.publish(f"rr/m/i/{self._mqtt_user}/{self._hashed_user}/{device_id}", msg)
+    def _send_msg_raw(self, msg: bytes) -> None:
+        info = self.publish(f"rr/m/i/{self._mqtt_user}/{self._hashed_user}/{self.device_info.device.duid}", msg)
         if info.rc != mqtt.MQTT_ERR_SUCCESS:
             raise RoborockException(f"Failed to publish (rc: {info.rc})")
 
-    async def send_command(self, device_id: str, method: RoborockCommand, params: Optional[list] = None):
+    async def send_command(self, method: RoborockCommand, params: Optional[list | dict] = None):
         await self.validate_connection()
         request_id, timestamp, payload = super()._get_payload(method, params, True)
         _LOGGER.debug(f"id={request_id} Requesting method {method} with {params}")
         request_protocol = 101
         response_protocol = 301 if method in SPECIAL_COMMANDS else 102
         roborock_message = RoborockMessage(timestamp=timestamp, protocol=request_protocol, payload=payload)
-        local_key = self.devices_info[device_id].device.local_key
+        local_key = self.device_info.device.local_key
         msg = RoborockParser.encode(roborock_message, local_key)
-        self._send_msg_raw(device_id, msg)
+        self._send_msg_raw(msg)
         (response, err) = await self._async_response(request_id, response_protocol)
         if err:
             raise CommandVacuumError(method, err) from err
         if response_protocol == 301:
             _LOGGER.debug(f"id={request_id} Response from {method}: {len(response)} bytes")
         else:
             _LOGGER.debug(f"id={request_id} Response from {method}: {response}")
         return response
 
-    async def get_map_v1(self, device_id):
+    async def get_map_v1(self):
         try:
-            return await self.send_command(device_id, RoborockCommand.GET_MAP_V1)
+            return await self.send_command(RoborockCommand.GET_MAP_V1)
         except RoborockException as e:
             _LOGGER.error(e)
         return None
```

### Comparing `python_roborock-0.8.3/roborock/code_mappings.py` & `python_roborock-0.9.0rc0/roborock/code_mappings.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.3/roborock/containers.py` & `python_roborock-0.9.0rc0/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.3/roborock/exceptions.py` & `python_roborock-0.9.0rc0/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.3/roborock/local_api.py` & `python_roborock-0.9.0rc0/roborock/local_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,73 @@
 from __future__ import annotations
 
 import asyncio
 import logging
-import socket
 from asyncio import Lock, Transport
-from typing import Callable, Mapping, Optional
+from typing import Optional
 
 import async_timeout
 
 from .api import QUEUE_TIMEOUT, SPECIAL_COMMANDS, RoborockClient
 from .containers import RoborockLocalDeviceInfo
 from .exceptions import CommandVacuumError, RoborockConnectionException, RoborockException
 from .roborock_message import RoborockMessage, RoborockParser
 from .typing import CommandInfoMap, RoborockCommand
 from .util import get_running_loop_or_create_one
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class RoborockLocalClient(RoborockClient):
-    def __init__(self, devices_info: Mapping[str, RoborockLocalDeviceInfo]):
-        super().__init__("abc", devices_info)
+class RoborockLocalClient(RoborockClient, asyncio.Protocol):
+    def __init__(self, device_info: RoborockLocalDeviceInfo):
+        super().__init__("abc", device_info)
         self.loop = get_running_loop_or_create_one()
-        self.device_listener: dict[str, RoborockSocketListener] = {
-            device_id: RoborockSocketListener(
-                device_info.network_info.ip, device_info.device.local_key, self.on_message, self.on_disconnect
-            )
-            for device_id, device_info in devices_info.items()
-        }
+        self.ip = device_info.network_info.ip
         self._batch_structs: list[RoborockMessage] = []
         self._executing = False
+        self.remaining = b""
+        self.transport: Transport | None = None
+        self._mutex = Lock()
+
+    def data_received(self, message):
+        if self.remaining:
+            message = self.remaining + message
+            self.remaining = b""
+        (parser_msg, remaining) = RoborockParser.decode(message, self.device_info.device.local_key)
+        self.remaining = remaining
+        self.on_message_received(parser_msg)
+
+    def connection_lost(self, exc: Optional[Exception]):
+        self.on_connection_lost(exc)
+
+    def is_connected(self):
+        return self.transport and self.transport.is_reading()
 
     async def async_connect(self) -> None:
-        await asyncio.gather(*[listener.connect() for listener in self.device_listener.values()])
+        async with self._mutex:
+            try:
+                if not self.is_connected():
+                    async with async_timeout.timeout(QUEUE_TIMEOUT):
+                        _LOGGER.info(f"Connecting to {self.ip}")
+                        self.transport, _ = await self.loop.create_connection(  # type: ignore
+                            lambda: self, self.ip, 58867
+                        )
+                        _LOGGER.info(f"Connected to {self.ip}")
+            except Exception as e:
+                raise RoborockConnectionException(f"Failed connecting to {self.ip}") from e
+
+    def sync_disconnect(self) -> None:
+        if self.transport and not self.loop.is_closed():
+            self.transport.close()
 
     async def async_disconnect(self) -> None:
-        for listener in self.device_listener.values():
-            listener.disconnect()
+        async with self._mutex:
+            self.sync_disconnect()
 
-    def build_roborock_message(self, method: RoborockCommand, params: Optional[list] = None) -> RoborockMessage:
+    def build_roborock_message(self, method: RoborockCommand, params: Optional[list | dict] = None) -> RoborockMessage:
         secured = True if method in SPECIAL_COMMANDS else False
         request_id, timestamp, payload = self._get_payload(method, params, secured)
         _LOGGER.debug(f"id={request_id} Requesting method {method} with {params}")
         command_info = CommandInfoMap.get(method)
         if not command_info:
             raise RoborockException(f"Request {method} have unknown prefix. Can't execute in offline mode")
         command = CommandInfoMap.get(method)
@@ -53,113 +78,55 @@
         return RoborockMessage(
             prefix=prefix,
             timestamp=timestamp,
             protocol=request_protocol,
             payload=payload,
         )
 
-    async def send_command(self, device_id: str, method: RoborockCommand, params: Optional[list] = None):
+    async def ping(self):
+        command_info = CommandInfoMap[RoborockCommand.NONE]
+        roborock_message = RoborockMessage(prefix=command_info.prefix, protocol=0, payload=b"")
+        return (await self.send_message(roborock_message))[0]
+
+    async def send_command(self, method: RoborockCommand, params: Optional[list | dict] = None):
         roborock_message = self.build_roborock_message(method, params)
-        return (await self.send_message(device_id, roborock_message))[0]
+        return (await self.send_message(roborock_message))[0]
 
     async def async_local_response(self, roborock_message: RoborockMessage):
         request_id = roborock_message.get_request_id()
-        if request_id is not None:
-            # response_protocol = 5 if roborock_message.prefix == secured_prefix else 4
-            response_protocol = 4
-            (response, err) = await self._async_response(request_id, response_protocol)
-            if err:
-                raise CommandVacuumError("", err) from err
-            _LOGGER.debug(f"id={request_id} Response from {roborock_message.get_method()}: {response}")
-            return response
+        if request_id is None:
+            request_id = roborock_message.seq
+        # response_protocol = 5 if roborock_message.prefix == secured_prefix else 4
+        response_protocol = 4
+        (response, err) = await self._async_response(request_id, response_protocol)
+        if err:
+            raise CommandVacuumError("", err) from err
+        _LOGGER.debug(f"id={request_id} Response from {roborock_message.get_method()}: {response}")
+        return response
+
+    def _send_msg_raw(self, data: bytes):
+        try:
+            if not self.transport:
+                raise RoborockException("Can not send message without connection")
+            self.transport.write(data)
+        except Exception as e:
+            raise RoborockException(e) from e
 
-    async def send_message(self, device_id: str, roborock_messages: list[RoborockMessage] | RoborockMessage):
+    async def send_message(self, roborock_messages: list[RoborockMessage] | RoborockMessage):
+        await self.validate_connection()
         if isinstance(roborock_messages, RoborockMessage):
             roborock_messages = [roborock_messages]
-        local_key = self.devices_info[device_id].device.local_key
+        local_key = self.device_info.device.local_key
         msg = RoborockParser.encode(roborock_messages, local_key)
         # Send the command to the Roborock device
-        listener = self.device_listener.get(device_id)
-        if listener is None:
-            raise RoborockException(f"No device listener for {device_id}")
-        if not self.should_keepalive():
-            listener.disconnect()
-
         _LOGGER.debug(f"Requesting device with {roborock_messages}")
-        await listener.send_message(msg)
+        self._send_msg_raw(msg)
 
         responses = await asyncio.gather(
             *[self.async_local_response(roborock_message) for roborock_message in roborock_messages],
             return_exceptions=True,
         )
         exception = next((response for response in responses if isinstance(response, BaseException)), None)
         if exception:
-            listener.disconnect()
+            await self.async_disconnect()
             raise exception
         return responses
-
-
-class RoborockSocket(socket.socket):
-    _closed = None
-
-    @property
-    def is_closed(self):
-        return self._closed
-
-
-class RoborockSocketListener(asyncio.Protocol):
-    roborock_port = 58867
-
-    def __init__(
-        self,
-        ip: str,
-        local_key: str,
-        on_message: Callable[[list[RoborockMessage]], None],
-        on_disconnect: Callable[[Optional[Exception]], None],
-        timeout: float | int = QUEUE_TIMEOUT,
-    ):
-        self.ip = ip
-        self.local_key = local_key
-        self.loop = get_running_loop_or_create_one()
-        self.on_message = on_message
-        self.on_disconnect = on_disconnect
-        self.timeout = timeout
-        self.remaining = b""
-        self.transport: Transport | None = None
-        self._mutex = Lock()
-
-    def data_received(self, message):
-        if self.remaining:
-            message = self.remaining + message
-            self.remaining = b""
-        (parser_msg, remaining) = RoborockParser.decode(message, self.local_key)
-        self.remaining = remaining
-        self.on_message(parser_msg)
-
-    def connection_lost(self, exc: Optional[Exception]):
-        self.on_disconnect(exc)
-
-    def is_connected(self):
-        return self.transport and self.transport.is_reading()
-
-    async def connect(self):
-        try:
-            if not self.is_connected():
-                async with async_timeout.timeout(self.timeout):
-                    _LOGGER.info(f"Connecting to {self.ip}")
-                    self.transport, _ = await self.loop.create_connection(lambda: self, self.ip, 58867)  # type: ignore
-        except Exception as e:
-            raise RoborockConnectionException(f"Failed connecting to {self.ip}") from e
-
-    def disconnect(self):
-        if self.transport:
-            self.transport.close()
-
-    async def send_message(self, data: bytes) -> None:
-        async with self._mutex:
-            await self.connect()
-            try:
-                if not self.transport:
-                    raise RoborockException("Can not send message without connection")
-                self.transport.write(data)
-            except Exception as e:
-                raise RoborockException(e) from e
```

### Comparing `python_roborock-0.8.3/roborock/roborock_future.py` & `python_roborock-0.9.0rc0/roborock/roborock_future.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.3/roborock/roborock_message.py` & `python_roborock-0.9.0rc0/roborock/roborock_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 if data_point_number in ["101", "102"]:
                     data_point_response = json.loads(data_point)
                     return data_point_response.get("id")
         return None
 
     def get_method(self) -> RoborockCommand | None:
         protocol = self.protocol
-        if protocol in [4, 101, 102]:
+        if protocol in [4, 5, 101, 102]:
             payload = json.loads(self.payload.decode())
             for data_point_number, data_point in payload.get("dps").items():
                 if data_point_number in ["101", "102"]:
                     data_point_response = json.loads(data_point)
                     return data_point_response.get("method")
         return None
 
@@ -107,60 +107,63 @@
         return msg
 
     @staticmethod
     def decode(msg: bytes, local_key: str, index=0) -> tuple[list[RoborockMessage], bytes]:
         prefix = b""
         original_index = index
         if len(msg) - index < 17:
-            ## broken message
+            # broken message
             return [], msg[original_index:]
 
         if msg[index + 4 : index + 7] == "1.0".encode():
             prefix = msg[index : index + 4]
             index += 4
         elif msg[index : index + 3] != "1.0".encode():
             raise RoborockException(f"Unknown protocol version {msg[0:3]!r}")
-        if len(msg) - index in [17]:
+        message_size = len(msg) - index
+        if message_size == 17:
             [version, request_id, random, timestamp, protocol] = struct.unpack_from("!3sIIIH", msg, index)
             return [
                 RoborockMessage(
                     prefix=prefix,
                     version=version,
                     seq=request_id,
                     random=random,
                     timestamp=timestamp,
                     protocol=protocol,
                     payload=b"",
                 )
             ], b""
 
         if len(msg) - index < 19:
-            ## broken message
+            # broken message
             return [], msg[original_index:]
 
+        _format = "!3sIIIHH"
         [
             version,
             request_id,
             random,
             timestamp,
             protocol,
             payload_len,
-        ] = struct.unpack_from("!3sIIIHH", msg, index)
-        index += 19
+        ] = struct.unpack_from(_format, msg, index)
+        format_size = struct.calcsize(_format)
+        index += format_size
 
         if payload_len + index + 4 > len(msg):
             ## broken message
             return [], msg[original_index:]
 
         payload = b""
         if payload_len == 0:
             index += 2
         else:
             [payload, expected_crc32] = struct.unpack_from(f"!{payload_len}sI", msg, index)
-            crc32 = binascii.crc32(msg[index - 19 : index + payload_len])
+            crc32 = binascii.crc32(msg[index - format_size : index + payload_len])
             index += 4 + payload_len
             if crc32 != expected_crc32:
                 raise RoborockException(f"Wrong CRC32 {crc32}, expected {expected_crc32}")
 
         if payload:
             aes_key = md5bin(encode_timestamp(timestamp) + local_key + salt)
             decipher = AES.new(aes_key, AES.MODE_ECB)
```

### Comparing `python_roborock-0.8.3/roborock/util.py` & `python_roborock-0.9.0rc0/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.3/PKG-INFO` & `python_roborock-0.9.0rc0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.8.3
+Version: 0.9.0rc0
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 0.8.3 Summary: A package
-to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
-python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
-humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries Requires-Dist: aiohttp
-Requires-Dist: async-timeout Requires-Dist: click (>=8) Requires-Dist: dacite
-(>=1.8.0,<1.9.0) Requires-Dist: paho-mqtt (>=1.6.1,<1.7.0) Requires-Dist:
-pycryptodome (>=3.17.0,<3.18.0) Requires-Dist: pycryptodomex (>=3.17.0,<3.18.0)
-; sys_platform == "darwin" Project-URL: Repository, https://github.com/
-humbertogontijo/python-roborock Description-Content-Type: text/markdown #
-Roborock
+Metadata-Version: 2.1 Name: python-roborock Version: 0.9.0rc0 Summary: A
+package to control Roborock vacuums. Home-page: https://github.com/
+humbertogontijo/python-roborock License: GPL-3.0-only Author: humbertogontijo
+Author-email: humbertogontijo@users.noreply.github.com Requires-Python:
+>=3.9,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: GNU
+General Public License v3 (GPLv3) Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
+Dist: aiohttp Requires-Dist: async-timeout Requires-Dist: click (>=8) Requires-
+Dist: dacite (>=1.8.0,<1.9.0) Requires-Dist: paho-mqtt (>=1.6.1,<1.7.0)
+Requires-Dist: pycryptodome (>=3.17.0,<3.18.0) Requires-Dist: pycryptodomex
+(>=3.17.0,<3.18.0) ; sys_platform == "darwin" Project-URL: Repository, https://
+github.com/humbertogontijo/python-roborock Description-Content-Type: text/
+markdown # Roborock
              [PyPI_Version] [Supported Python versions] [License]
 Roborock library for online and offline control of your vacuums. ##
 Installation Install this via pip (or your favourite package manager): `pip
 install python-roborock` ## Functionality This package can encrypt and decrypt
 the following commands: - GET_CLEAN_RECORD - GET_CONSUMABLE -
 GET_MULTI_MAPS_LIST - APP_START - APP_PAUSE - APP_STOP - APP_CHARGE - APP_SPOT
 - FIND_ME - RESUME_ZONED_CLEAN - RESUME_SEGMENT_CLEAN - SET_CUSTOM_MODE -
```


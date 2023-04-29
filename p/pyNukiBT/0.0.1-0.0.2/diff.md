# Comparing `tmp/pyNukiBT-0.0.1.tar.gz` & `tmp/pynukibt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNukiBT-0.0.1.tar", last modified: Tue Apr 25 17:37:32 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pyNukiBT-0.0.1.tar` & `pynukibt-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,11 @@
-drwxrwxr-x   0 roneng    (1000) roneng    (1000)        0 2023-04-25 17:37:32.930588 pyNukiBT-0.0.1/
--rw-rw-r--   0 roneng    (1000) roneng    (1000)     1064 2023-04-25 17:34:19.000000 pyNukiBT-0.0.1/LICENSE
--rw-rw-r--   0 roneng    (1000) roneng    (1000)      459 2023-04-25 17:37:32.930588 pyNukiBT-0.0.1/PKG-INFO
--rw-rw-r--   0 roneng    (1000) roneng    (1000)       30 2023-04-25 17:34:19.000000 pyNukiBT-0.0.1/README.md
-drwxrwxr-x   0 roneng    (1000) roneng    (1000)        0 2023-04-25 17:37:32.930588 pyNukiBT-0.0.1/pyNukiBT/
--rw-rw-r--   0 roneng    (1000) roneng    (1000)      229 2023-04-25 17:34:19.000000 pyNukiBT-0.0.1/pyNukiBT/__init__.py
--rw-rw-r--   0 roneng    (1000) roneng    (1000)    39075 2023-04-25 17:34:19.000000 pyNukiBT-0.0.1/pyNukiBT/const.py
--rw-rw-r--   0 roneng    (1000) roneng    (1000)    22892 2023-04-25 17:34:55.000000 pyNukiBT-0.0.1/pyNukiBT/nuki.py
-drwxrwxr-x   0 roneng    (1000) roneng    (1000)        0 2023-04-25 17:37:32.930588 pyNukiBT-0.0.1/pyNukiBT.egg-info/
--rw-rw-r--   0 roneng    (1000) roneng    (1000)      459 2023-04-25 17:37:32.000000 pyNukiBT-0.0.1/pyNukiBT.egg-info/PKG-INFO
--rw-rw-r--   0 roneng    (1000) roneng    (1000)      241 2023-04-25 17:37:32.000000 pyNukiBT-0.0.1/pyNukiBT.egg-info/SOURCES.txt
--rw-rw-r--   0 roneng    (1000) roneng    (1000)        1 2023-04-25 17:37:32.000000 pyNukiBT-0.0.1/pyNukiBT.egg-info/dependency_links.txt
--rw-rw-r--   0 roneng    (1000) roneng    (1000)       62 2023-04-25 17:37:32.000000 pyNukiBT-0.0.1/pyNukiBT.egg-info/requires.txt
--rw-rw-r--   0 roneng    (1000) roneng    (1000)        9 2023-04-25 17:37:32.000000 pyNukiBT-0.0.1/pyNukiBT.egg-info/top_level.txt
--rw-rw-r--   0 roneng    (1000) roneng    (1000)       38 2023-04-25 17:37:32.930588 pyNukiBT-0.0.1/setup.cfg
--rw-rw-r--   0 roneng    (1000) roneng    (1000)      738 2023-04-25 17:34:19.000000 pyNukiBT-0.0.1/setup.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pynukibt-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 pynukibt-0.0.2/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pynukibt-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pynukibt-0.0.2/pyNukiBT/__init__.py
+-rw-r--r--   0        0        0    38869 2020-02-02 00:00:00.000000 pynukibt-0.0.2/pyNukiBT/const.py
+-rw-r--r--   0        0        0    24696 2020-02-02 00:00:00.000000 pynukibt-0.0.2/pyNukiBT/nuki.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pynukibt-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pynukibt-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 pynukibt-0.0.2/README.md
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pynukibt-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 pynukibt-0.0.2/PKG-INFO
```

### Comparing `pyNukiBT-0.0.1/LICENSE` & `pynukibt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyNukiBT-0.0.1/pyNukiBT/const.py` & `pynukibt-0.0.2/pyNukiBT/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,26 +275,26 @@
     LogEntryCount = Struct(
         "logging_enabled" / Int8ul,
         "count" / Int16ul,
         "door_sensor_enabled" / Int8ul,
         "door_sensor_logging_enabled" / Int8ul,
     )
 
-    NukiChallenge = Struct(
+    Challenge = Struct(
         "nonce" / Bytes(32)
     )
 
-    NukiPublicKey = Struct(
+    PublicKey = Struct(
         "public_key" / Bytes(32)
     )
 
     AuthorizationId = Struct(
         "authenticator" / Bytes(32),
         "auth_id" / Bytes(4),
-        "uuuid" / Bytes(16),
+        "uuid" / Bytes(16),
         "nonce" / Bytes(32),
     )
 
     NukiCommandStatus = Struct(
         "status" / StatusCode
     )
 
@@ -419,17 +419,14 @@
         "command" / NukiCommand
     )
 
     RequestConfig = Struct(
         "nonce" / Bytes(32)
     )
 
-    Challenge = Struct(
-        "nonce" / Bytes(32)
-    )
     LockState = NotImplemented
     LockAction = NotImplemented
     KeyturnerStates = NotImplemented
     Config = NotImplemented
 
     @functools.cached_property
     def LockActionMsg(self):
@@ -488,15 +485,15 @@
                                     self.LogEntryType.DOOR_SENSOR_LOGGING_ENABLED_DISABLED : self.LogEntryExt1,
                                     }),
         )
     @functools.cached_property
     def message_types(self):
         return {
         self.NukiCommand.REQUEST_DATA                  : self.RequestData,
-        # self.NukiCommand.PUBLIC_KEY                    : self.PublicKey,
+        self.NukiCommand.PUBLIC_KEY                    : self.PublicKey,
         self.NukiCommand.CHALLENGE                     : self.Challenge,
         # self.NukiCommand.AUTHORIZATION_AUTHENTICATOR   : self.AuthorizationAuthenticator,
         # self.NukiCommand.AUTHORIZATION_DATA            : self.AuthorizationData,
         self.NukiCommand.AUTHORIZATION_ID              : self.AuthorizationId,
         # self.NukiCommand.REMOVE_USER_AUTHORIZATION     : self.RemoveUserAuthorization,
         # self.NukiCommand.REQUEST_AUTHORIZATION_ENTRIES : self.RequestAuthorizationEntries,
         self.NukiCommand.AUTHORIZATION_ENTRY           : self.AuthorizationEntry,
@@ -552,22 +549,26 @@
         return Struct(
             "auth_id" / Bytes(4),
             "command" / self.NukiCommand,
             "payload" / Switch(this.command, self.message_types),
             "crc" / NukiChecksum(Int16ul,
                              lambda data: crc16.xmodem(data, 0xFFFF),
                              lambda x: x._io.getvalue()[:x._io.tell()])
-            # "crc" / Checksum(Int16ul,
-            #                  lambda data: crc16.xmodem(data, 0xFFFF),
-            #                  # In current construct.Checksum parsing implementation, the filed is parsed before
-            #                  # checksum is calculated, so we need to subtract crc.sizeof bytes from getvalue
-            #                  lambda x: x._io.getvalue()[:
-            #                         x._io.tell() - int(x._parsing) * x._subcons.crc.sizeof()
-            #                         ])
         )
+
+    @functools.cached_property
+    def NukiUnencryptedMessage(self):
+        return Struct(
+            "command" / self.NukiCommand,
+            "payload" / Switch(this.command, self.message_types),
+            "crc" / NukiChecksum(Int16ul,
+                             lambda data: crc16.xmodem(data, 0xFFFF),
+                             lambda x: x._io.getvalue()[:x._io.tell()])
+        )
+
     @functools.cached_property
     def NukiMessage2(self):
         return Struct(
             "auth_id" / Bytes(4),
             "command" / self.NukiCommand,
             "payload" / Switch(this.command, self.message_types),
             "crc" / Int16ul,
```

### Comparing `pyNukiBT-0.0.1/pyNukiBT/nuki.py` & `pynukibt-0.0.2/pyNukiBT/nuki.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import asyncio
 import hashlib
 import logging
 import hmac
 import time
+import construct
 from asyncio import CancelledError, TimeoutError
 from typing import Callable
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData
+from bleak.backends.characteristic import BleakGATTCharacteristic
 
 import async_timeout
 
 # from bleak_retry_connector import BLEAK_RETRY_EXCEPTIONS
 
 from fastcrc import crc16
 import nacl.utils
@@ -29,65 +31,62 @@
         address,
         auth_id,
         nuki_public_key,
         bridge_public_key,
         bridge_private_key,
         app_id,
         name,
-        type_id: NukiConst.NukiClientType = NukiConst.NukiClientType.BRIDGE,
+        client_type: NukiConst.NukiClientType = NukiConst.NukiClientType.BRIDGE,
         ble_device=None,
-        model=None,
     ):
-        self.address = address
-        self.auth_id = auth_id
-        self.nuki_public_key = nuki_public_key
-        self.bridge_public_key = bridge_public_key
-        self.bridge_private_key = bridge_private_key
-        self.app_id = app_id
-        self.id = None
-        self.name = None
-        self.type_id = type_id
+        self._address = address
+        self._auth_id = auth_id
+        self._nuki_public_key = nuki_public_key
+        self._bridge_public_key = bridge_public_key
+        self._bridge_private_key = bridge_private_key
+        self._app_id = app_id
+        self._name = name
+        self._client_type = client_type
 
-        self.username = None
         self.rssi = None
         self.last_state = None
         self.config = {}
         self._poll_needed = False
         self.last_action_status = None
-
-        self.name = name
         self._device_type = None
+
         self._pairing_handle = None
         self._client = None
         self._expected_response: NukiConst.NukiCommand = None
+        self._aggregate_messages = list(),
         self.retry = 5
         self.connection_timeout = 30
         self.command_timeout = 30
         self.command_response_timeout = 10
 
         self._send_cmd_lock = asyncio.Lock()
         self._connect_lock = asyncio.Lock()
         self._operation_lock = asyncio.Lock()
         self._update_state_lock = asyncio.Lock()
         self._update_config_lock = asyncio.Lock()
+        self._notify_future = None
+        self._messages = []
 
         self._callbacks = []
 
         if nuki_public_key and bridge_private_key:
             self._create_shared_key()
 
         self._last_ibeacon = None
-        if model:
-            self.device_type = model
 
         if ble_device:
             self.set_ble_device(ble_device)
 
-    async def parse_advertisement_data(self, device, advertisement_data):
-        if device.address == self.address:
+    def parse_advertisement_data(self, device, advertisement_data):
+        if device.address == self._address:
             manufacturer_data = advertisement_data.manufacturer_data.get(76, None)
             if manufacturer_data is None:
                 logger.info(
                     f"No manufacturer_data (76) in advertisement_data: {advertisement_data}"
                 )
                 return
             if manufacturer_data[0] != 0x02:
@@ -119,25 +118,27 @@
             self._last_ibeacon = time.time()
         return seen_recently
 
     @property
     def device_type(self):
         return self._device_type
 
-    @device_type.setter
-    def device_type(self, device_type: NukiConst.NukiDeviceType):
-        if device_type == NukiConst.NukiDeviceType.OPENER:
-            self._const = NukiOpenerConst
-        else:
-            self._const = NukiLockConst
-        self._device_type = device_type
-        logger.info(f"Device type: {self.device_type}")
+    # @device_type.setter
+    # def device_type(self, device_type: NukiConst.NukiDeviceType):
+    #     if device_type == NukiConst.NukiDeviceType.OPENER:
+    #         self._const = NukiOpenerConst
+    #     else:
+    #         self._const = NukiLockConst
+    #     self._device_type = device_type
+    #     logger.info(f"Device type: {self._device_type}")
 
     def _create_shared_key(self):
-        self._shared_key = crypto_box_beforenm(self.nuki_public_key, self.bridge_private_key)
+        self._shared_key = crypto_box_beforenm(
+            self._nuki_public_key, self._bridge_private_key
+        )
         self._box = nacl.secret.SecretBox(self._shared_key)
 
     @property
     def is_battery_critical(self):
         return bool(self.last_state["critical_battery_state"] & 1)
 
     @property
@@ -161,37 +162,49 @@
     @staticmethod
     def _prepare_command(cmd: NukiConst.NukiCommand, payload=bytes()):
         message = NukiConst.NukiCommand.build(cmd) + payload
         crc = crc16.xmodem(message, 0xFFFF).to_bytes(2, "little")
         message += crc
         return message
 
-    async def _send_encrtypted_command(self, cmd: NukiConst.NukiCommand, payload : dict, expected_response : NukiConst.NukiCommand = None):
-        unencrypted = self._const.NukiMessage.build({
-            "auth_id" : self.auth_id,
-            "command" : cmd,
-            "payload" : payload,
-        })
+    async def _send_encrtypted_command(
+        self,
+        cmd: NukiConst.NukiCommand,
+        payload: dict,
+        aggregate_messages = list(),
+        expected_response: NukiConst.NukiCommand = None,
+    ):
+        unencrypted = self._const.NukiMessage.build(
+            {
+                "auth_id": self._auth_id,
+                "command": cmd,
+                "payload": payload,
+            }
+        )
         nonce = nacl.utils.random(24)
         encrypted = self._box.encrypt(unencrypted, nonce)[24:]
         length = len(encrypted).to_bytes(2, "little")
-        message = nonce + self.auth_id + length + encrypted
+        message = nonce + self._auth_id + length + encrypted
         logger.info(f"sending encrypted command {cmd}")
-        return await self._send_command(self._const.BLE_CHAR, message, expected_response)
+        return await self._send_command(
+            self._const.BLE_CHAR, message, aggregate_messages=aggregate_messages, expected_response=expected_response,
+        )
 
-    def _decrypt_message(self, data):
+    def _decrypt_message(self, data: bytes):
         msg = self._const.NukiEncryptedMessage.parse(data)
         decrypted = self._box.decrypt(msg.nonce + msg.encrypted)
         return decrypted
 
-    def _parse_message(self, data):
+    def _parse_message(self, data: bytes, encrypted: bool):
         msg_sz = None
         try:
-            msg = self._const.NukiMessage.parse(data)
-
+            if encrypted:
+                msg = self._const.NukiMessage.parse(self._decrypt_message(data))
+            else:
+                msg = self._const.NukiUnencryptedMessage.parse(data)
             # keyturner_state usually has crc=0. if we got crc=0 in other command we want to know about it.
             if msg.crc == 0 and msg.command != self._const.NukiCommand.KEYTURNER_STATES:
                 logger.warning(f"got message with crc=0. cmd:{msg.command}")
                 try:
                     msg = self._const.NukiMessage2.parse(data)
                     msg_sz = len(self._const.NukiMessage2.build(msg))
                 except TypeError:
@@ -205,134 +218,150 @@
                 msg_sz = 0
             if msg_sz == len(data):
                 # If we got the len we expected, this is probably a real crc error.
                 # Otherwise it is probably not a real crc error, we are just missing some fields in the message format
                 raise
 
         if msg_sz and msg_sz != len(data):
-            logger.warning(f"Got unexpected message length for command {msg.command}. got length:{len(data)} expecting length:{msg_sz}")
+            logger.warning(
+                f"Got unexpected message length for command {msg.command}. got length:{len(data)} expecting length:{msg_sz}"
+            )
             unhandled_bytes = len(data) - msg_sz
-            logger.warning(f"got {unhandled_bytes} unknown bytes with value: {data[-unhandled_bytes-2:-2]}")
+            logger.warning(
+                f"Got {unhandled_bytes} unknown bytes with value: {data[-unhandled_bytes-2:-2]}"
+            )
 
         return msg
 
     def _fire_callbacks(self) -> None:
         """Fire callbacks."""
-        logger.debug("%s: Fire callbacks", self.name)
+        logger.debug("%s: Fire callbacks", self._name)
         for callback in self._callbacks:
             callback()
 
     def subscribe(self, callback: Callable[[], None]) -> Callable[[], None]:
         """Subscribe to device notifications."""
         self._callbacks.append(callback)
 
         def _unsub() -> None:
             """Unsubscribe from device notifications."""
             self._callbacks.remove(callback)
 
         return _unsub
 
-    def set_ble_device(self, ble_device:BLEDevice, advertisement_data:AdvertisementData=None):
+    def set_ble_device(
+        self, ble_device: BLEDevice, advertisement_data: AdvertisementData = None
+    ):
         if not self._client:
             self._client = BleakClient(ble_device, timeout=self.connection_timeout)
-        if not self.device_type and advertisement_data:
+        if (not self._device_type or not self._const) and advertisement_data:
             if NukiOpenerConst.BLE_PAIRING_CHAR in advertisement_data.service_uuids:
-                self.device_type = NukiConst.NukiDeviceType.OPENER
+                self._device_type = NukiConst.NukiDeviceType.OPENER
+                self._const = NukiOpenerConst
             else:
-                self.device_type = NukiConst.NukiDeviceType.SMARTLOCK_1_2
+                self._device_type = NukiConst.NukiDeviceType.SMARTLOCK_1_2
+                self._const = NukiLockConst
 
         return self._client
 
-    async def _notification_handler(self, sender, data):
+    async def _notification_handler(self, sender: BleakGATTCharacteristic, data):
         logger.debug(f"Notification handler: {sender}, data: {data}")
-        if self._client.services[self._const.BLE_PAIRING_CHAR] and \
-                sender == self._client.services[self._const.BLE_PAIRING_CHAR].handle:
-            # The pairing handler is not encrypted
-            msg = self._parse_message(bytes(data))
-        else:
-            msg = self._parse_message(self._decrypt_message(bytes(data)))
+
+        # The pairing handler is not encrypted
+        encrypted = sender.uuid != self._const.BLE_PAIRING_CHAR
+        msg = self._parse_message(bytes(data), encrypted)
 
         if msg.command == self._const.NukiCommand.ERROR_REPORT:
             if msg.payload.error_code == self._const.ErrorCode.P_ERROR_NOT_PAIRING:
-                logger.error(f"********************************************************************")
-                logger.error(f"*                                                                  *")
-                logger.error(f"*                            UNPAIRED!                             *")
-                logger.error(f"*    Put Nuki in pairing mode by pressing the button 6 seconds     *")
-                logger.error(f"*                         Then try again                           *")
-                logger.error(f"*                                                                  *")
-                logger.error(f"********************************************************************")
-                exit(0)
+                logger.error("UNPAIRED! Put Nuki in pairing mode by pressing the button 6 seconds, Then try again")
             else:
-                logger.error(f"Error {msg.payload.error_code}, command {msg.payload.command_identifier}")
-            ex = NukiErrorException(error_code=msg.payload.error_code, command=msg.payload.command_identifier)
+                logger.error(
+                    f"Error {msg.payload.error_code}, command {msg.payload.command_identifier}"
+                )
+            ex = NukiErrorException(
+                error_code=msg.payload.error_code,
+                command=msg.payload.command_identifier,
+            )
             if self._notify_future and not self._notify_future.done():
                 self._notify_future.set_exception(ex)
                 return
             else:
                 raise ex
 
         elif msg.command == self._const.NukiCommand.STATUS:
-            logger.info(f"Last action: {msg.payload.status}")
+            logger.debug(f"Last action: {msg.payload.status}")
             self.last_action_status = msg.payload.status
 
         if self._notify_future and not self._notify_future.done():
             if msg.command == self._expected_response:
-                self._notify_future.set_result(msg)
+                self._notify_future.set_result(msg.payload)
+                return
+            if msg.command in self._aggregate_messages:
+                self._messages.append(msg.payload)
                 return
 
         if msg.command == self._const.NukiCommand.KEYTURNER_STATES:
-            update_config = not self.config or (self.last_state["config_update_count"] != msg.payload["config_update_count"])
+            update_config = not self.config or (
+                self.last_state["config_update_count"]
+                != msg.payload["config_update_count"]
+            )
             self.last_state = msg.payload
             logger.debug(f"State: {self.last_state}")
             if update_config:
                 # todo: update config directly?
                 self.poll_needed = True
 
         elif msg.command == self._const.NukiCommand.STATUS:
             logger.info(f"Last action: {msg.payload.status}")
 
         else:
-            logger.error("%s: Received unsolicited notification: %s", self.name, msg)
+            logger.error("%s: Received unsolicited notification: %s", self._name, msg)
             logger.error("was expecting %s", self._expected_response)
 
-    async def _send_command(self, characteristic, command, expected_response : NukiConst.NukiCommand = None):
+    async def _send_command(
+        self, characteristic, command,
+        aggregate_messages = list(),
+        expected_response: NukiConst.NukiCommand = None
+    ):
         async with self._send_cmd_lock:
             self._notify_future = asyncio.Future()
+            self._aggregate_messages = aggregate_messages
             self._expected_response = expected_response
+            self._messages = list()
             msg = None
 
             # Sometimes the connection to the smartlock fails, retry 3 times
             _characteristic = characteristic
             for i in range(1, self.retry + 1):
-                logger.info(f'Trying to send data. Attempt {i}')
+                logger.info(f"Trying to send data. Attempt {i}")
                 try:
                     await self.connect()
                     if _characteristic is None:
                         _characteristic = self._const.BLE_CHAR
-                    logger.info(f'Sending data to Nuki')
+                    logger.info(f"Sending data to Nuki")
                     await self._client.write_gatt_char(_characteristic, command)
                 except (TimeoutError, CancelledError):
-                    logger.error(f'Timeout while sending data on attempt {i}')
+                    logger.error(f"Timeout while sending data on attempt {i}")
                     await asyncio.sleep(0.2)
                 except BleakDBusError as ex:
-                    logger.error(f'DBus Error {ex}')
+                    logger.error(f"DBus Error {ex}")
                     await asyncio.sleep(0.2)
                 # except BLEAK_RETRY_EXCEPTIONS as ex:
                 #     logger.error(f'Bleak retry error {ex}')
                 #     await asyncio.sleep(0.2)
                 except BleakError as exc:
                     logger.error(f"Bleak Error while sending data on attempt {i}")
                     logger.exception(exc)
                     await asyncio.sleep(0.7)
                 except Exception as exc:
-                    logger.error(f'Error while sending data on attempt {i}')
+                    logger.error(f"Error while sending data on attempt {i}")
                     logger.exception(exc)
                     await asyncio.sleep(0.2)
                 else:
-                    logger.info(f'Data sent on attempt {i}')
+                    logger.info(f"Data sent on attempt {i}")
                     break
         if expected_response:
             async with async_timeout.timeout(self.command_response_timeout):
                 msg = await self._notify_future
         self._notify_future = None
         self._expected_response = None
         return msg
@@ -345,53 +374,67 @@
         # Haven't researched further the reason and consequences of this exception
         except EOFError:
             logger.info("EOFError during notification")
 
     async def connect(self):
         async with self._connect_lock:
             if not self._client:
-                self._client = BleakClient(self.address, timeout=self.connection_timeout)
+                self._client = BleakClient(
+                    self._address, timeout=self.connection_timeout
+                )
             if self._client.is_connected:
                 logger.info("Connected")
                 return
             await self._client.connect()
             logger.debug(f"Services {[str(s) for s in self._client.services]}")
-            logger.debug(f"Characteristics {[str(v) for v in self._client.services.characteristics.values()]}")
-            if not self.device_type:
+            logger.debug(
+                f"Characteristics {[str(v) for v in self._client.services.characteristics.values()]}"
+            )
+            if (not self._device_type or not self._const):
                 services = self._client.services
                 if services.get_characteristic(NukiOpenerConst.BLE_PAIRING_CHAR):
-                    self.device_type = NukiConst.NukiDeviceType.OPENER
+                    self._device_type = NukiConst.NukiDeviceType.OPENER
+                    self._const = NukiOpenerConst
                 else:
-                    self.device_type = NukiConst.NukiDeviceType.SMARTLOCK_1_2
-            await self._safe_start_notify(self._const.BLE_PAIRING_CHAR, self._notification_handler)
-            await self._safe_start_notify(self._const.BLE_CHAR, self._notification_handler)
+                    self._device_type = NukiConst.NukiDeviceType.SMARTLOCK_1_2
+                    self._const = NukiLockConst
+            await self._safe_start_notify(
+                self._const.BLE_PAIRING_CHAR, self._notification_handler
+            )
+            await self._safe_start_notify(
+                self._const.BLE_CHAR, self._notification_handler
+            )
             logger.info("Connected")
 
     async def disconnect(self):
         if self._client and self._client.is_connected:
             logger.info(f"Nuki disconnecting...")
             try:
                 await self._client.disconnect()
                 logger.info("Nuki disconnected")
             except Exception as e:
-                logger.error(f'Error while disconnecting')
+                logger.error(f"Error while disconnecting")
                 logger.exception(e)
 
     async def update_state(self):
         logger.info("Querying Nuki state")
         if self._update_state_lock.locked():
             logger.info("update state already in progress. ignoring")
             return
         async with self._update_state_lock, self._operation_lock:
             msg = await self._send_encrtypted_command(
                 self._const.NukiCommand.REQUEST_DATA,
-                {"command" : self._const.NukiCommand.KEYTURNER_STATES},
-                self._const.NukiCommand.KEYTURNER_STATES)
-            update_config = not self.config or (self.last_state["config_update_count"] != msg.payload["config_update_count"])
-            self.last_state = msg.payload
+                {"command": self._const.NukiCommand.KEYTURNER_STATES},
+                expected_response=self._const.NukiCommand.KEYTURNER_STATES,
+            )
+            update_config = not self.config or (
+                self.last_state["config_update_count"]
+                != msg["config_update_count"]
+            )
+            self.last_state = msg
             logger.debug(f"State: {self.last_state}")
             self._poll_needed = False
         if update_config:
             await self.update_config()
         self._fire_callbacks()
 
     async def lock(self):
@@ -405,123 +448,164 @@
         )
 
     async def unlatch(self):
         return await self.lock_action(
             self._const.LockAction.UNLATCH, self._const.LockState.UNLATCHING
         )
 
-    async def lock_action(self, action : NukiConst.LockAction, new_lock_state : NukiConst.LockState = None):
+    async def lock_action(
+        self, action: NukiConst.LockAction, new_lock_state: NukiConst.LockState = None, name_suffix: str = None
+    ):
         logger.info(f"Lock action {action}")
         async with self._operation_lock:
             if new_lock_state:
-                self.last_state['lock_state'] = new_lock_state
+                self.last_state["lock_state"] = new_lock_state
             msg = await self._send_encrtypted_command(
                 self._const.NukiCommand.REQUEST_DATA,
                 {"command": self._const.NukiCommand.CHALLENGE},
-                self._const.NukiCommand.CHALLENGE,
+                expected_response=self._const.NukiCommand.CHALLENGE,
             )
             payload = {
                 "lock_action": action,
-                "app_id": self.app_id,
+                "app_id": self._app_id,
                 "flags": 0,
-                "name_suffix": self.username,
-                "nonce": msg.payload.nonce,
+                "name_suffix": name_suffix,
+                "nonce": msg.nonce,
             }
-            msg = await self._send_encrtypted_command(self._const.NukiCommand.LOCK_ACTION, payload, self._const.NukiCommand.STATUS)
-            logger.info(f"{msg.payload.status}")
-        return msg.payload
+            msg = await self._send_encrtypted_command(
+                self._const.NukiCommand.LOCK_ACTION,
+                payload,
+                expected_response=self._const.NukiCommand.STATUS,
+            )
+            logger.info(f"{msg.status}")
+        return msg
 
     async def update_config(self):
         logger.info("Retrieve nuki configuration")
         if self._update_config_lock.locked():
             logger.info("get config already in progress")
             return
         async with self._operation_lock, self._update_config_lock:
+            await self.connect() # connect so we can identify the device type and update self._const accordingly
             msg = await self._send_encrtypted_command(
                 self._const.NukiCommand.REQUEST_DATA,
                 {"command": self._const.NukiCommand.CHALLENGE},
-                self._const.NukiCommand.CHALLENGE,
+                expected_response=self._const.NukiCommand.CHALLENGE,
             )
             msg = await self._send_encrtypted_command(
                 self._const.NukiCommand.REQUEST_CONFIG,
-                {"nonce": msg.payload["nonce"]},
-                self._const.NukiCommand.CONFIG,
+                {"nonce": msg["nonce"]},
+                expected_response=self._const.NukiCommand.CONFIG,
             )
-            self.config = msg.payload
+            self.config = msg
             logger.debug(f"Config: {self.config}")
 
-    async def pair(self, callback):
+    async def pair(self):
         async with self._operation_lock:
+            await self.connect() # connect so we can identify the device type and update self._const accordingly
             payload = self._const.NukiCommand.build(self._const.NukiCommand.PUBLIC_KEY)
             cmd = self._prepare_command(self._const.NukiCommand.REQUEST_DATA, payload)
-            msg = await self._send_command(self._const.BLE_PAIRING_CHAR, cmd, self._const.NukiCommand.PUBLIC_KEY)
-            self.nuki_public_key = msg.payload["public_key"]
+            msg = await self._send_command(
+                self._const.BLE_PAIRING_CHAR, cmd, expected_response=self._const.NukiCommand.PUBLIC_KEY
+            )
+            self._nuki_public_key = msg["public_key"]
             self._create_shared_key()
-            logger.info(f"Nuki {self.address} public key: {self.nuki_public_key.hex()}")
-            cmd = self._prepare_command(self._const.NukiCommand.PUBLIC_KEY, self.bridge_public_key)
-            msg = await self._send_command(self._const.BLE_PAIRING_CHAR, cmd, self._const.NukiCommand.CHALLENGE)
-            value_r = self.bridge_public_key + self.nuki_public_key + msg.payload["nonce"]
-            payload = hmac.new(self._shared_key, msg=value_r, digestmod=hashlib.sha256).digest()
-            cmd = self._prepare_command(self._const.NukiCommand.AUTH_AUTHENTICATOR, payload)
-            msg = await self._send_command(self._const.BLE_PAIRING_CHAR, cmd, self._const.NukiCommand.CHALLENGE)
-            app_id = self.app_id.to_bytes(4, "little")
-            type_id = self._const.NukiClientType.build(self.type_id)
-            name = self.name.encode("utf-8").ljust(32, b"\0")
+            logger.info(f"Nuki {self._address} public key: {self._nuki_public_key.hex()}")
+            cmd = self._prepare_command(
+                self._const.NukiCommand.PUBLIC_KEY, self._bridge_public_key
+            )
+            msg = await self._send_command(
+                self._const.BLE_PAIRING_CHAR, cmd, expected_response=self._const.NukiCommand.CHALLENGE
+            )
+            value_r = (
+                self._bridge_public_key + self._nuki_public_key + msg["nonce"]
+            )
+            payload = hmac.new(
+                self._shared_key, msg=value_r, digestmod=hashlib.sha256
+            ).digest()
+            cmd = self._prepare_command(
+                self._const.NukiCommand.AUTHORIZATION_AUTHENTICATOR, payload
+            )
+            msg = await self._send_command(
+                self._const.BLE_PAIRING_CHAR, cmd, expected_response=self._const.NukiCommand.CHALLENGE
+            )
+            app_id = self._app_id.to_bytes(4, "little")
+            type_id = self._const.NukiClientType.build(self._client_type)
+            name = self._name.encode("utf-8").ljust(32, b"\0")
             nonce = nacl.utils.random(32)
-            value_r = type_id + app_id + name + nonce + msg.payload["nonce"]
-            payload = hmac.new(self._shared_key, msg=value_r, digestmod=hashlib.sha256).digest()
+            value_r = type_id + app_id + name + nonce + msg["nonce"]
+            payload = hmac.new(
+                self._shared_key, msg=value_r, digestmod=hashlib.sha256
+            ).digest()
             payload += type_id + app_id + name + nonce
-            cmd = self._prepare_command(self._const.NukiCommand.AUTH_DATA, payload)
-            msg = await self._send_command(self._const.BLE_PAIRING_CHAR, cmd, self._const.NukiCommand.AUTHORIZATION_ID)
-            self.auth_id = msg.payload["auth_id"]
-            value_r = self.auth_id + msg.payload["nonce"]
-            payload = hmac.new(self._shared_key, msg=value_r, digestmod=hashlib.sha256).digest()
-            payload += self.auth_id
-            cmd = self._prepare_command(self._const.NukiCommand.AUTH_ID_CONFIRM, payload)
-            msg = await self._send_command(self._const.BLE_PAIRING_CHAR, cmd, self._const.NukiCommand.STATUS)
-        if callback:
-            callback(self)
+            cmd = self._prepare_command(self._const.NukiCommand.AUTHORIZATION_DATA, payload)
+            msg = await self._send_command(
+                self._const.BLE_PAIRING_CHAR,
+                cmd,
+                expected_response=self._const.NukiCommand.AUTHORIZATION_ID,
+            )
+            self._auth_id = msg["auth_id"]
+            value_r = self._auth_id + msg["nonce"]
+            payload = hmac.new(
+                self._shared_key, msg=value_r, digestmod=hashlib.sha256
+            ).digest()
+            payload += self._auth_id
+            cmd = self._prepare_command(
+                self._const.NukiCommand.AUTHORIZATION_ID_CONFIRMATION, payload
+            )
+            msg = await self._send_command(
+                self._const.BLE_PAIRING_CHAR, cmd, expected_response=self._const.NukiCommand.STATUS
+            )
+            await self.disconnect()
+        return {"nuki_public_key": self._nuki_public_key, "auth_id": self._auth_id}
 
-    async def verify_pin(self, pin):
-        logger.info(f"verify PIN {pin}")
+    async def verify_security_pin(self, security_pin):
+        logger.info(f"verify security PIN")
         async with self._operation_lock:
             msg = await self._send_encrtypted_command(
                 self._const.NukiCommand.REQUEST_DATA,
                 {"command": self._const.NukiCommand.CHALLENGE},
-                self._const.NukiCommand.CHALLENGE,
+                expected_response=self._const.NukiCommand.CHALLENGE,
             )
             payload = {
-                "nonce" : msg.payload["nonce"],
-                "security_pin" : pin,
+                "nonce": msg["nonce"],
+                "security_pin": security_pin,
             }
             try:
-                msg = await self._send_encrtypted_command(self._const.NukiCommand.VERIFY_SECURITY_PIN, payload, self._const.NukiCommand.STATUS)
+                msg = await self._send_encrtypted_command(
+                    self._const.NukiCommand.VERIFY_SECURITY_PIN,
+                    payload,
+                    expected_response=self._const.NukiCommand.STATUS,
+                )
             except NukiErrorException as ex:
                 if ex.error_code == self._const.ErrorCode.K_ERROR_BAD_PIN:
                     return False
                 else:
                     raise
-            return msg.command == self._const.NukiCommand.STATUS and msg.payload.status == self._const.StatusCode.COMPLETED
+            return msg.status == self._const.StatusCode.COMPLETED
 
-    async def request_last_log_entry(self, pin):
+    async def request_log_entry(self, security_pin, sort_order=0x01, count=1):
         logger.info(f"request last log entry")
         async with self._operation_lock:
             msg = await self._send_encrtypted_command(
                 self._const.NukiCommand.REQUEST_DATA,
                 {"command": self._const.NukiCommand.CHALLENGE},
-                self._const.NukiCommand.CHALLENGE,
+                expected_response=self._const.NukiCommand.CHALLENGE,
             )
             payload = {
                 "start_index": 0,
-                "count": 1,
-                "sort_order": 0x01,
+                "count": count,
+                "sort_order": sort_order,
                 "total_count": 0,
-                "nonce": msg.payload.nonce,
-                "security_pin": pin,
+                "nonce": msg.nonce,
+                "security_pin": security_pin,
             }
             msg = await self._send_encrtypted_command(
                 self._const.NukiCommand.REQUEST_LOG_ENTRIES,
                 payload,
-                self._const.NukiCommand.LOG_ENTRY,
+                aggregate_messages=[self._const.NukiCommand.LOG_ENTRY,],
+                expected_response=self._const.NukiCommand.STATUS,
             )
-            logger.debug(msg.payload)
-        return msg.payload
+            logger.debug(msg)
+            logger.debug(self._messages)
+            ret = self._messages
+        return ret
```

### Comparing `pyNukiBT-0.0.1/setup.py` & `pynukibt-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     author_email="ronengr@gmail.com",
     description="Nuki Bluetooth API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ronengr/pyNukiBT",
     packages=find_packages(),
     install_requires=[
-        "bleak>=0.20.1",
+        "bleak>=0.20",
         "fastcrc>=0.2.1",
         "PyNaCl>=1.3.0",
         "construct>=2.10.68",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
-)
+)
```


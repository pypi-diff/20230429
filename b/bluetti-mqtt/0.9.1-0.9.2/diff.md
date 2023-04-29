# Comparing `tmp/bluetti_mqtt-0.9.1.tar.gz` & `tmp/bluetti_mqtt-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetti_mqtt-0.9.1.tar", last modified: Mon Oct 17 13:24:06 2022, max compression
+gzip compressed data, was "bluetti_mqtt-0.9.2.tar", last modified: Sun Oct 23 16:38:52 2022, max compression
```

## Comparing `bluetti_mqtt-0.9.1.tar` & `bluetti_mqtt-0.9.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:24:06.465666 bluetti_mqtt-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4075 2022-10-17 13:24:06.465666 bluetti_mqtt-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3598 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:24:06.465666 bluetti_mqtt-0.9.1/bluetti_mqtt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:24:06.465666 bluetti_mqtt-0.9.1/bluetti_mqtt/bluetooth/
--rw-r--r--   0 runner    (1001) docker     (121)     1722 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/bluetooth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5101 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/bluetooth/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/bluetooth/exc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/bluetooth/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/bus.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:24:06.465666 bluetti_mqtt-0.9.1/bluetti_mqtt/core/
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2654 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/core/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:24:06.465666 bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3686 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/ac200m.py
--rw-r--r--   0 runner    (1001) docker     (121)     4771 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/ac300.py
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/ac500.py
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/bluetti_device.py
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/eb3a.py
--rw-r--r--   0 runner    (1001) docker     (121)     4641 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/ep500.py
--rw-r--r--   0 runner    (1001) docker     (121)     4643 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/ep500p.py
--rw-r--r--   0 runner    (1001) docker     (121)     4523 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/struct.py
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/core/response.py
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4041 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/device_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4335 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/logger_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    16125 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4140 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/bluetti_mqtt/server_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 13:24:06.465666 bluetti_mqtt-0.9.1/bluetti_mqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4075 2022-10-17 13:24:06.000000 bluetti_mqtt-0.9.1/bluetti_mqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-10-17 13:24:06.000000 bluetti_mqtt-0.9.1/bluetti_mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 13:24:06.000000 bluetti_mqtt-0.9.1/bluetti_mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-17 13:24:06.000000 bluetti_mqtt-0.9.1/bluetti_mqtt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 13:24:06.000000 bluetti_mqtt-0.9.1/bluetti_mqtt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-17 13:24:06.000000 bluetti_mqtt-0.9.1/bluetti_mqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-17 13:24:06.000000 bluetti_mqtt-0.9.1/bluetti_mqtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-10-17 13:24:06.465666 bluetti_mqtt-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-10-17 13:23:57.000000 bluetti_mqtt-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 16:38:52.110690 bluetti_mqtt-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4075 2022-10-23 16:38:52.110690 bluetti_mqtt-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3598 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 16:38:52.106690 bluetti_mqtt-0.9.2/bluetti_mqtt/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 16:38:52.106690 bluetti_mqtt-0.9.2/bluetti_mqtt/bluetooth/
+-rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/bluetooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5102 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/bluetooth/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/bluetooth/exc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/bluetooth/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1607 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/bus.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 16:38:52.106690 bluetti_mqtt-0.9.2/bluetti_mqtt/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2654 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/core/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 16:38:52.110690 bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3687 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/ac200m.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4772 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/ac300.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/ac500.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2052 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/bluetti_device.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2910 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/eb3a.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4642 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/ep500.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4644 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/ep500p.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4519 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/struct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/core/response.py
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4042 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/device_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4337 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/logger_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16426 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4142 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/bluetti_mqtt/server_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 16:38:52.106690 bluetti_mqtt-0.9.2/bluetti_mqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4075 2022-10-23 16:38:52.000000 bluetti_mqtt-0.9.2/bluetti_mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-10-23 16:38:52.000000 bluetti_mqtt-0.9.2/bluetti_mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 16:38:52.000000 bluetti_mqtt-0.9.2/bluetti_mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-23 16:38:52.000000 bluetti_mqtt-0.9.2/bluetti_mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 16:38:51.000000 bluetti_mqtt-0.9.2/bluetti_mqtt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-23 16:38:52.000000 bluetti_mqtt-0.9.2/bluetti_mqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-23 16:38:52.000000 bluetti_mqtt-0.9.2/bluetti_mqtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      724 2022-10-23 16:38:52.110690 bluetti_mqtt-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-10-23 16:38:35.000000 bluetti_mqtt-0.9.2/setup.py
```

### Comparing `bluetti_mqtt-0.9.1/LICENSE` & `bluetti_mqtt-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt-0.9.1/PKG-INFO` & `bluetti_mqtt-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetti_mqtt
-Version: 0.9.1
+Version: 0.9.2
 Summary: MQTT interface to Bluetti power stations
 Home-page: http://github.com/warhammerkid/bluetti_mqtt
 Author: Stephen Augenstein
 Author-email: perl.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bluetti_mqtt-0.9.1/README.rst` & `bluetti_mqtt-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/bluetooth/__init__.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/bluetooth/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,14 +30,21 @@
     logging.debug(f'Found devices: {filtered}')
 
     if len(filtered) != len(addresses):
         return []
 
     def build_device(device: BLEDevice) -> BluettiDevice:
         match = DEVICE_NAME_RE.match(device.name)
-        if match[1] == 'AC200M': return AC200M(device.address, match[2])
-        if match[1] == 'AC300': return AC300(device.address, match[2])
-        if match[1] == 'AC500': return AC500(device.address, match[2])
-        if match[1] == 'EP500': return EP500(device.address, match[2])
-        if match[1] == 'EP500P': return EP500P(device.address, match[2])
-        if match[1] == 'EB3A': return EB3A(device.address, match[2])
+        if match[1] == 'AC200M':
+            return AC200M(device.address, match[2])
+        if match[1] == 'AC300':
+            return AC300(device.address, match[2])
+        if match[1] == 'AC500':
+            return AC500(device.address, match[2])
+        if match[1] == 'EP500':
+            return EP500(device.address, match[2])
+        if match[1] == 'EP500P':
+            return EP500P(device.address, match[2])
+        if match[1] == 'EB3A':
+            return EB3A(device.address, match[2])
+
     return [build_device(d) for d in filtered]
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/bluetooth/client.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/bluetooth/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             # Register for notifications and run command loop
             try:
                 await self.client.start_notify(
                     self.NOTIFY_UUID,
                     self._notification_handler)
                 await self._perform_commands(self.client)
             except (BleakError, asyncio.TimeoutError) as err:
-                logging.error('Reconnecting after error: {err}')
+                logging.error(f'Reconnecting after error: {err}')
                 continue
             except BadConnectionError as err:
                 logging.error(f'Delayed reconnect after error: {err}')
                 await asyncio.sleep(1)
             finally:
                 await self.client.disconnect()
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/bluetooth/manager.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/bluetooth/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import logging
 from typing import Dict, List
 from bluetti_mqtt.core import BluettiDevice, DeviceCommand
 from .client import BluetoothClient
 
+
 class MultiDeviceManager:
     clients: Dict[BluettiDevice, BluetoothClient]
 
     def __init__(self, devices: List[BluettiDevice]):
         self.devices = devices
         self.clients = {}
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/bus.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/bus.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import asyncio
 from dataclasses import dataclass
 import logging
 from typing import Callable, List, Union
 from bluetti_mqtt.core import BluettiDevice, DeviceCommand
 
+
 @dataclass(frozen=True)
 class ParserMessage:
     device: BluettiDevice
     parsed: dict
 
+
 @dataclass(frozen=True)
 class CommandMessage:
     device: BluettiDevice
     command: DeviceCommand
 
+
 class EventBus:
     parser_listeners: List[Callable[[ParserMessage], None]]
     command_listeners: List[Callable[[CommandMessage], None]]
     queue: asyncio.Queue
 
     def __init__(self):
         self.parser_listeners = []
@@ -41,11 +44,11 @@
         if not self.queue:
             self.queue = asyncio.Queue()
 
         while True:
             msg = await self.queue.get()
             logging.debug(f'queue size: {self.queue.qsize()}')
             if isinstance(msg, ParserMessage):
-                await asyncio.gather(*[l(msg) for l in self.parser_listeners])
+                await asyncio.gather(*[pl(msg) for pl in self.parser_listeners])
             elif isinstance(msg, CommandMessage):
-                await asyncio.gather(*[l(msg) for l in self.command_listeners])
+                await asyncio.gather(*[cl(msg) for cl in self.command_listeners])
             self.queue.task_done()
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/core/commands.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/core/commands.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/ac200m.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/ac200m.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.struct.add_sn_field('serial_number', 0x00, 0x11)
         self.struct.add_version_field('arm_version', 0x00, 0x17)
         self.struct.add_version_field('dsp_version', 0x00, 0x19)
         self.struct.add_uint_field('dc_input_power', 0x00, 0x24)
         self.struct.add_uint_field('ac_input_power', 0x00, 0x25)
         self.struct.add_uint_field('ac_output_power', 0x00, 0x26)
         self.struct.add_uint_field('dc_output_power', 0x00, 0x27)
-        self.struct.add_decimal_field('power_generation', 0x00, 0x29, 1) # Total power generated since last reset in kwh
+        self.struct.add_decimal_field('power_generation', 0x00, 0x29, 1)  # Total power generated since last reset (kwh)
         self.struct.add_uint_field('total_battery_percent', 0x00, 0x2B)
         self.struct.add_bool_field('ac_output_on', 0x00, 0x30)
         self.struct.add_bool_field('dc_output_on', 0x00, 0x31)
 
         # Page 0x00 - Details
         self.struct.add_enum_field('ac_output_mode', 0x00, 0x46, OutputMode)
         self.struct.add_uint_field('internal_ac_voltage', 0x00, 0x47)
@@ -49,15 +49,15 @@
         self.struct.add_uint_field('internal_dc_input_voltage', 0x00, 0x56)
         self.struct.add_decimal_field('internal_dc_input_power', 0x00, 0x57, 1)
         self.struct.add_decimal_field('internal_dc_input_current', 0x00, 0x58, 2)
 
         # Page 0x00 - Battery Data
         self.struct.add_uint_field('pack_num_max', 0x00, 0x5B)
         self.struct.add_uint_field('pack_num', 0x00, 0x60)
-        self.struct.add_decimal_field('pack_voltage', 0x00, 0x62, 2) # Full pack voltage
+        self.struct.add_decimal_field('pack_voltage', 0x00, 0x62, 2)  # Full pack voltage
         self.struct.add_uint_field('pack_battery_percent', 0x00, 0x63)
         self.struct.add_decimal_array_field('cell_voltages', 0x00, 0x69, 16, 2)
 
         # Page 0x0B - Controls
         self.struct.add_uint_field('pack_num', 0x0B, 0xBE)
         self.struct.add_bool_field('ac_output_on', 0x0B, 0xBF)
         self.struct.add_bool_field('dc_output_on', 0x0B, 0xC0)
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/ac300.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/ac300.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.struct.add_sn_field('serial_number', 0x00, 0x11)
         self.struct.add_version_field('arm_version', 0x00, 0x17)
         self.struct.add_version_field('dsp_version', 0x00, 0x19)
         self.struct.add_uint_field('dc_input_power', 0x00, 0x24)
         self.struct.add_uint_field('ac_input_power', 0x00, 0x25)
         self.struct.add_uint_field('ac_output_power', 0x00, 0x26)
         self.struct.add_uint_field('dc_output_power', 0x00, 0x27)
-        self.struct.add_decimal_field('power_generation', 0x00, 0x29, 1) # Total power generated since last reset in kwh
+        self.struct.add_decimal_field('power_generation', 0x00, 0x29, 1)  # Total power generated since last reset (kwh)
         self.struct.add_uint_field('total_battery_percent', 0x00, 0x2B)
         self.struct.add_bool_field('ac_output_on', 0x00, 0x30)
         self.struct.add_bool_field('dc_output_on', 0x00, 0x31)
 
         # Page 0x00 - Details
         self.struct.add_enum_field('ac_output_mode', 0x00, 0x46, OutputMode)
         self.struct.add_decimal_field('internal_ac_voltage', 0x00, 0x47, 1)
@@ -63,15 +63,15 @@
         self.struct.add_decimal_field('internal_dc_input_voltage', 0x00, 0x56, 1)
         self.struct.add_uint_field('internal_dc_input_power', 0x00, 0x57)
         self.struct.add_decimal_field('internal_dc_input_current', 0x00, 0x58, 1)
 
         # Page 0x00 - Battery Data
         self.struct.add_uint_field('pack_num_max', 0x00, 0x5B)
         self.struct.add_uint_field('pack_num', 0x00, 0x60)
-        self.struct.add_decimal_field('pack_voltage', 0x00, 0x62, 2) # Full pack voltage
+        self.struct.add_decimal_field('pack_voltage', 0x00, 0x62, 2)  # Full pack voltage
         self.struct.add_uint_field('pack_battery_percent', 0x00, 0x63)
         self.struct.add_decimal_array_field('cell_voltages', 0x00, 0x69, 16, 2)
         self.struct.add_version_field('pack_bms_version', 0x00, 0xC9)
 
         # Page 0x0B - Controls
         self.struct.add_enum_field('ups_mode', 0x0B, 0xB9, UpsMode)
         self.struct.add_uint_field('pack_num', 0x0B, 0xBE)
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/ac500.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/ac500.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         self.struct = DeviceStruct()
 
         # Page 0x00 - Core
         self.struct.add_uint_field('dc_input_power', 0x00, 0x24)
         self.struct.add_uint_field('ac_input_power', 0x00, 0x25)
         self.struct.add_uint_field('ac_output_power', 0x00, 0x26)
         self.struct.add_uint_field('dc_output_power', 0x00, 0x27)
-        self.struct.add_decimal_field('power_generation', 0x00, 0x29, 1) # Total power generated since last reset in kwh
+        self.struct.add_decimal_field('power_generation', 0x00, 0x29, 1)  # Total power generated since last reset (kwh)
         self.struct.add_uint_field('total_battery_percent', 0x00, 0x2B)
         self.struct.add_bool_field('ac_output_on', 0x00, 0x30)
         self.struct.add_bool_field('dc_output_on', 0x00, 0x31)
 
         super().__init__(address, 'AC500', sn)
 
     @property
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/bluetti_device.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/bluetti_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,41 +10,41 @@
         self.address = address
         self.type = type
         self.sn = sn
 
     def parse(self, page: int, offset: int, data: bytes) -> dict:
         return self.struct.parse(page, offset, data)
 
-    """
-    A given device has a maximum number of battery packs, including the
-    internal battery if it has one. We can provide this information statically
-    so it's not necessary to poll the device.
-    """
     @property
     def pack_num_max(self):
+        """
+        A given device has a maximum number of battery packs, including the
+        internal battery if it has one. We can provide this information statically
+        so it's not necessary to poll the device.
+        """
         return 1
 
-    """A given device has an optimal set of commands for polling"""
     @property
     def polling_commands(self) -> List[QueryRangeCommand]:
+        """A given device has an optimal set of commands for polling"""
         raise NotImplementedError
 
-    """A given device may have a set of commands for polling pack data"""
     @property
     def pack_polling_commands(self) -> List[QueryRangeCommand]:
+        """A given device may have a set of commands for polling pack data"""
         return []
 
-    """A given device has an optimal set of commands for debug logging"""
     @property
     def logging_commands(self) -> List[QueryRangeCommand]:
+        """A given device has an optimal set of commands for debug logging"""
         raise NotImplementedError
 
-    """A given device may have a set of commands for logging pack data"""
     @property
     def pack_logging_commands(self) -> List[QueryRangeCommand]:
+        """A given device may have a set of commands for logging pack data"""
         return []
 
     def has_field_setter(self, field: str):
         return any(f.page == 0x0B and f.name == field for f in self.struct.fields)
 
     def build_setter_command(self, field: str, value: Any):
         device_field = next(f for f in self.struct.fields if f.page == 0x0B and f.name == field)
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/eb3a.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/eb3a.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,56 +9,76 @@
 class LedMode(Enum):
     LOW = 1
     HIGH = 2
     SOS = 3
     OFF = 4
 
 
+@unique
+class EcoShutdown(Enum):
+    ONE_HOUR = 1
+    TWO_HOURS = 2
+    THREE_HOURS = 3
+    FOUR_HOURS = 4
+
+
+@unique
+class ChargingMode(Enum):
+    STANDARD = 0
+    SILENT = 1
+    TURBO = 2
+
+
 class EB3A(BluettiDevice):
     def __init__(self, address: str, sn: str):
         self.struct = DeviceStruct()
 
         # Page 0x00 - Core
         self.struct.add_string_field('device_type', 0x00, 0x0A, 6)
         self.struct.add_sn_field('serial_number', 0x00, 0x11)
         self.struct.add_version_field('arm_version', 0x00, 0x17)
         self.struct.add_version_field('dsp_version', 0x00, 0x19)
         self.struct.add_uint_field('dc_input_power', 0x00, 0x24)
         self.struct.add_uint_field('ac_input_power', 0x00, 0x25)
         self.struct.add_uint_field('ac_output_power', 0x00, 0x26)
         self.struct.add_uint_field('dc_output_power', 0x00, 0x27)
-        self.struct.add_decimal_field('power_generation', 0x00, 0x29, 1) # Total power generated since last reset in kwh
+        self.struct.add_decimal_field('power_generation', 0x00, 0x29, 1)  # Total power generated since last reset (kwh)
         self.struct.add_uint_field('total_battery_percent', 0x00, 0x2B)
         self.struct.add_bool_field('ac_output_on', 0x00, 0x30)
         self.struct.add_bool_field('dc_output_on', 0x00, 0x31)
 
         # Page 0x00 - Details
         self.struct.add_decimal_field('ac_input_voltage', 0x00, 0x4D, 1)
-        self.struct.add_decimal_field('dc_input_voltage', 0x00, 0x56, 1)
+        self.struct.add_decimal_field('internal_dc_input_voltage', 0x00, 0x56, 2)
 
         # Page 0x00 - Battery Data
         self.struct.add_uint_field('pack_num_max', 0x00, 0x5B)
 
         # Page 0x0B - Controls
         self.struct.add_bool_field('ac_output_on', 0x0B, 0xBF)
         self.struct.add_bool_field('dc_output_on', 0x0B, 0xC0)
         self.struct.add_enum_field('led_mode', 0x0B, 0xDA, LedMode)
+        self.struct.add_bool_field('power_off', 0x0B, 0xF4)
+        self.struct.add_bool_field('eco_on', 0x0B, 0xF7)
+        self.struct.add_enum_field('eco_shutdown', 0x0B, 0xF8, EcoShutdown)
+        self.struct.add_enum_field('charging_mode', 0x0B, 0xF9, ChargingMode)
+        self.struct.add_bool_field('power_lifting_on', 0x0B, 0xFA)
 
         super().__init__(address, 'EB3A', sn)
 
     @property
     def polling_commands(self) -> List[QueryRangeCommand]:
         return [
             QueryRangeCommand(0x00, 0x0A, 0x28),
             QueryRangeCommand(0x00, 0x46, 0x15),
-            QueryRangeCommand(0x0B, 0xDA, 1)
+            QueryRangeCommand(0x0B, 0xDA, 0x01),
+            QueryRangeCommand(0x0B, 0xF4, 0x07)
         ]
 
     @property
     def logging_commands(self) -> List[QueryRangeCommand]:
         return [
             QueryRangeCommand(0x00, 0x0A, 0x35),
             QueryRangeCommand(0x00, 0x46, 0x42),
             QueryRangeCommand(0x00, 0x88, 0x4A),
-            QueryRangeCommand(0x0B, 0xB9, 0x3D)
+            QueryRangeCommand(0x0B, 0xB8, 0x43)
         ]
-
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/ep500.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/ep500.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.struct.add_sn_field('serial_number', 0x00, 0x11)
         self.struct.add_version_field('arm_version', 0x00, 0x17)
         self.struct.add_version_field('dsp_version', 0x00, 0x19)
         self.struct.add_uint_field('dc_input_power', 0x00, 0x24)
         self.struct.add_uint_field('ac_input_power', 0x00, 0x25)
         self.struct.add_uint_field('ac_output_power', 0x00, 0x26)
         self.struct.add_uint_field('dc_output_power', 0x00, 0x27)
-        self.struct.add_decimal_field('power_generation', 0x00, 0x29, 1) # Total power generated since last reset in kwh
+        self.struct.add_decimal_field('power_generation', 0x00, 0x29, 1)  # Total power generated since last reset (kwh)
         self.struct.add_uint_field('total_battery_percent', 0x00, 0x2B)
         self.struct.add_bool_field('ac_output_on', 0x00, 0x30)
         self.struct.add_bool_field('dc_output_on', 0x00, 0x31)
 
         # Page 0x00 - Details
         self.struct.add_enum_field('ac_output_mode', 0x00, 0x46, OutputMode)
         self.struct.add_decimal_field('internal_ac_voltage', 0x00, 0x47, 1)
@@ -62,15 +62,15 @@
         self.struct.add_decimal_field('ac_input_frequency', 0x00, 0x50, 2)
         self.struct.add_decimal_field('internal_dc_input_voltage', 0x00, 0x56, 1)
         self.struct.add_uint_field('internal_dc_input_power', 0x00, 0x57)
         self.struct.add_decimal_field('internal_dc_input_current', 0x00, 0x58, 1)
 
         # Page 0x00 - Battery Data
         self.struct.add_uint_field('pack_num_max', 0x00, 0x5B)
-        self.struct.add_decimal_field('pack_voltage', 0x00, 0x5C, 1) # Full pack voltage
+        self.struct.add_decimal_field('pack_voltage', 0x00, 0x5C, 1)  # Full pack voltage
         self.struct.add_uint_field('pack_battery_percent', 0x00, 0x5E)
         self.struct.add_uint_field('pack_num', 0x00, 0x60)
         self.struct.add_decimal_array_field('cell_voltages', 0x00, 0x69, 16, 2)
 
         # Page 0x0B - Controls
         self.struct.add_enum_field('ups_mode', 0x0B, 0xB9, UpsMode)
         self.struct.add_uint_field('pack_num', 0x0B, 0xBE)
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/ep500p.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/ep500p.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.struct.add_sn_field('serial_number', 0x00, 0x11)
         self.struct.add_version_field('arm_version', 0x00, 0x17)
         self.struct.add_version_field('dsp_version', 0x00, 0x19)
         self.struct.add_uint_field('dc_input_power', 0x00, 0x24)
         self.struct.add_uint_field('ac_input_power', 0x00, 0x25)
         self.struct.add_uint_field('ac_output_power', 0x00, 0x26)
         self.struct.add_uint_field('dc_output_power', 0x00, 0x27)
-        self.struct.add_decimal_field('power_generation', 0x00, 0x29, 1) # Total power generated since last reset in kwh
+        self.struct.add_decimal_field('power_generation', 0x00, 0x29, 1)  # Total power generated since last reset (kwh)
         self.struct.add_uint_field('total_battery_percent', 0x00, 0x2B)
         self.struct.add_bool_field('ac_output_on', 0x00, 0x30)
         self.struct.add_bool_field('dc_output_on', 0x00, 0x31)
 
         # Page 0x00 - Details
         self.struct.add_enum_field('ac_output_mode', 0x00, 0x46, OutputMode)
         self.struct.add_decimal_field('internal_ac_voltage', 0x00, 0x47, 1)
@@ -62,15 +62,15 @@
         self.struct.add_decimal_field('ac_input_frequency', 0x00, 0x50, 2)
         self.struct.add_decimal_field('internal_dc_input_voltage', 0x00, 0x56, 1)
         self.struct.add_uint_field('internal_dc_input_power', 0x00, 0x57)
         self.struct.add_decimal_field('internal_dc_input_current', 0x00, 0x58, 1)
 
         # Page 0x00 - Battery Data
         self.struct.add_uint_field('pack_num_max', 0x00, 0x5B)
-        self.struct.add_decimal_field('pack_voltage', 0x00, 0x5C, 1) # Full pack voltage
+        self.struct.add_decimal_field('pack_voltage', 0x00, 0x5C, 1)  # Full pack voltage
         self.struct.add_uint_field('pack_battery_percent', 0x00, 0x5E)
         self.struct.add_uint_field('pack_num', 0x00, 0x60)
         self.struct.add_decimal_array_field('cell_voltages', 0x00, 0x69, 16, 2)
 
         # Page 0x0B - Controls
         self.struct.add_enum_field('ups_mode', 0x0B, 0xB9, UpsMode)
         self.struct.add_uint_field('pack_num', 0x0B, 0xBE)
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/core/devices/struct.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/core/devices/struct.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
         super().__init__(name, page, offset, size)
 
     def parse(self, data: bytes) -> Decimal:
         values = list(struct.unpack(f'!{self.size}H', data))
         return [Decimal(v) / 10 ** self.scale for v in values]
 
 
-"""Fixed-width null-terminated string field"""
 class StringField(DeviceField):
+    """Fixed-width null-terminated string field"""
     def parse(self, data: bytes) -> str:
         return data.rstrip(b'\0').decode('ascii')
 
 
 class VersionField(DeviceField):
     def __init__(self, name: str, page: int, offset: int):
         super().__init__(name, page, offset, 2)
@@ -120,15 +120,15 @@
         # need to divide the byte size by 2
         data_size = int(len(data) / 2)
 
         # Filter out fields not in range
         r = range(offset, offset + data_size)
         fields = [f for f in self.fields
                   if f.page == page and f.offset in r and f.offset + f.size - 1 in r]
-        
+
         # Parse fields
         parsed = {}
         for f in fields:
             data_start = 2 * (f.offset - offset)
             field_data = data[data_start:data_start + 2 * f.size]
             parsed[f.name] = f.parse(field_data)
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/core/response.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/core/response.py`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/device_handler.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/device_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
             start_time = time.monotonic()
             for pack in range(1, device.pack_num_max + 1):
                 # Send pack set command if the device supports more than 1 pack
                 if device.pack_num_max > 1:
                     command = device.build_setter_command('pack_num', pack)
                     await self.manager.perform_nowait(device, command)
-                    await asyncio.sleep(10) # We need to wait after switching packs for the data to be available
+                    await asyncio.sleep(10)  # We need to wait after switching packs for the data to be available
 
                 # Poll
                 for command in device.pack_logging_commands:
                     await self._poll_with_command(device, command)
             elapsed = time.monotonic() - start_time
 
             # Limit polling rate if interval provided
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/logger_cli.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/logger_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                 continue
 
             for pack in range(1, device.pack_num_max + 1):
                 # Send pack set command if the device supports more than 1 pack
                 if device.pack_num_max > 1:
                     command = device.build_setter_command('pack_num', pack)
                     await log_command(client, device, command, log_file)
-                    await asyncio.sleep(10) # We need to wait after switching packs for the data to be available
+                    await asyncio.sleep(10)  # We need to wait after switching packs for the data to be available
 
                 for command in device.pack_logging_commands:
                     await log_command(client, device, command, log_file)
 
 
 def main():
     parser = argparse.ArgumentParser(
@@ -115,9 +115,10 @@
     if args.scan:
         asyncio.run(scan_devices())
     elif args.log:
         asyncio.run(log(args.address, args.log))
     else:
         parser.print_help()
 
+
 if __name__ == "__main__":
     main(sys.argv)
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/mqtt_client.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/mqtt_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,30 @@
 from asyncio_mqtt import Client, MqttError
 from paho.mqtt.client import MQTTMessage
 from bluetti_mqtt.bus import CommandMessage, EventBus, ParserMessage
 from bluetti_mqtt.core import BluettiDevice, DeviceCommand
 
 
 COMMAND_TOPIC_RE = re.compile(r'^bluetti/command/(\w+)-(\d+)/([a-z_]+)$')
+ENUM_SETTER_FIELDS = {
+    'ups_mode',
+    'auto_sleep_mode',
+    'led_mode',
+    'eco_shutdown',
+    'charging_mode'
+}
+BOOL_SETTER_FIELDS = {
+    'ac_output_on',
+    'dc_output_on',
+    'grid_charge_on',
+    'time_control_on',
+    'power_off',
+    'eco_on',
+    'power_lifting_on'
+}
 
 
 class MQTTClient:
     message_queue: asyncio.Queue
 
     def __init__(
         self,
@@ -31,15 +47,20 @@
         self.username = username
         self.password = password
 
     async def run(self):
         while True:
             logging.info('Connecting to MQTT broker...')
             try:
-                async with Client(hostname=self.hostname, port=self.port, username=self.username, password=self.password) as client:
+                async with Client(
+                    hostname=self.hostname,
+                    port=self.port,
+                    username=self.username,
+                    password=self.password
+                ) as client:
                     logging.info('Connected to MQTT broker')
 
                     # Connect to event bus
                     self.message_queue = asyncio.Queue()
                     self.bus.add_parser_listener(self.handle_message)
 
                     # Announce device to Home Assistant
@@ -60,19 +81,19 @@
     async def _handle_commands(self, client: Client):
         async with client.filtered_messages('bluetti/command/#') as messages:
             await client.subscribe('bluetti/command/#')
             async for mqtt_message in messages:
                 await self._handle_command(mqtt_message)
 
     async def _handle_messages(self, client: Client):
-            while True:
-                msg: ParserMessage = await self.message_queue.get()
-                await self._handle_message(client, msg)
-                self.message_queue.task_done()
-    
+        while True:
+            msg: ParserMessage = await self.message_queue.get()
+            await self._handle_message(client, msg)
+            self.message_queue.task_done()
+
     async def _handle_command(self, mqtt_message: MQTTMessage):
         # Parse the mqtt_message.topic
         m = COMMAND_TOPIC_RE.match(mqtt_message.topic)
         if not m:
             logging.warn(f'unknown command topic: {mqtt_message.topic}')
             return
 
@@ -80,33 +101,31 @@
         device = next((d for d in self.devices if d.type == m[1] and d.sn == m[2]), None)
         if not device:
             logging.warn(f'unknown device: {m[1]} {m[2]}')
             return
 
         # Check if the device supports setting this field
         if not device.has_field_setter(m[3]):
-            logging.warn(f'Recevied command for unknown topic: {m[3]} - {mqtt_message.topic}')
+            logging.warn(f'Received command for unknown topic: {m[3]} - {mqtt_message.topic}')
             return
 
         cmd: DeviceCommand = None
-        if m[3] == 'ups_mode' or m[3] == 'auto_sleep_mode' or m[3] == 'led_mode':
+        if m[3] in ENUM_SETTER_FIELDS:
             value = mqtt_message.payload.decode('ascii')
             cmd = device.build_setter_command(m[3], value)
-        elif m[3] == 'ac_output_on' or m[3] == 'dc_output_on' or m[3] == 'grid_charge_on' or m[3] == 'time_control_on':
+        elif m[3] in BOOL_SETTER_FIELDS:
             value = mqtt_message.payload == b'ON'
             cmd = device.build_setter_command(m[3], value)
         else:
             logging.warn(f'Recevied command for unhandled topic: {m[3]} - {mqtt_message.topic}')
             return
 
         await self.bus.put(CommandMessage(device, cmd))
 
     async def _send_discovery_message(self, client: Client):
-
-        
         def payload(id: str, device: BluettiDevice, **kwargs) -> str:
             # Unknown keys are allowed but ignored by Home Assistant
             payload_dict = {
                 'state_topic': f'bluetti/state/{device.type}-{device.sn}/{id}',
                 'command_topic': f'bluetti/command/{device.type}-{device.sn}/{id}',
                 'device': {
                     'identifiers': [
@@ -123,112 +142,119 @@
             for key, value in kwargs.items():
                 payload_dict[key] = value
 
             return json.dumps(payload_dict)
 
         # Loop through devices
         for d in self.devices:
-            await client.publish(f'homeassistant/sensor/{d.sn}_ac_input_power/config',
-                                 payload=payload(
-                                     id='ac_input_power',
-                                     device=d,
-                                     name='AC Input Power',
-                                     unit_of_measurement='W',
-                                     device_class='power',
-                                     state_class='measurement',
-                                     force_update=True)
-                                     .encode(),
-                                 retain=True
-                                 )
-
-            await client.publish(f'homeassistant/sensor/{d.sn}_dc_input_power/config',
-                                 payload=payload(
-                                     id='dc_input_power',
-                                     device=d,
-                                     name='DC Input Power',
-                                     unit_of_measurement='W',
-                                     device_class='power',
-                                     state_class='measurement',
-                                     force_update=True)
-                                     .encode(),
-                                 retain=True
-                                 )
-
-            await client.publish(f'homeassistant/sensor/{d.sn}_ac_output_power/config',
-                        payload=payload(
-                            id='ac_output_power',
-                            device=d,
-                            name='AC Output Power',
-                            unit_of_measurement='W',
-                            device_class='power',
-                            state_class='measurement',
-                            force_update=True)
-                            .encode(),
-                        retain=True
-                        )
-
-            await client.publish(f'homeassistant/sensor/{d.sn}_dc_output_power/config',
-                        payload=payload(
-                            id='dc_output_power',
-                            device=d,
-                            name='DC Output Power',
-                            unit_of_measurement='W',
-                            device_class='power',
-                            state_class='measurement',
-                            force_update=True)
-                            .encode(),
-                        retain=True
-                        )
-
-            await client.publish(f'homeassistant/sensor/{d.sn}_total_battery_percent/config',
-                        payload=payload(
-                            id='total_battery_percent',
-                            device=d,
-                            name='Total Battery Percent',
-                            unit_of_measurement='%',
-                            device_class='battery',
-                            state_class='measurement')
-                            .encode(),
-                        retain=True
-                        )
-
-            await client.publish(f'homeassistant/switch/{d.sn}_ac_output_on/config',
-                        payload=payload(
-                            id='ac_output_on',
-                            device=d,
-                            name='AC Output',
-                            device_class='outlet')
-                            .encode(),
-                        retain=True
-                        )
-
-            await client.publish(f'homeassistant/switch/{d.sn}_dc_output_on/config',
-                        payload=payload(
-                            id='dc_output_on',
-                            device=d,
-                            name='DC Output',
-                            device_class='outlet')
-                            .encode(),
-                        retain=True
-                        )
+            await client.publish(
+                f'homeassistant/sensor/{d.sn}_ac_input_power/config',
+                payload=payload(
+                    id='ac_input_power',
+                    device=d,
+                    name='AC Input Power',
+                    unit_of_measurement='W',
+                    device_class='power',
+                    state_class='measurement',
+                    force_update=True
+                ).encode(),
+                retain=True
+            )
+
+            await client.publish(
+                f'homeassistant/sensor/{d.sn}_dc_input_power/config',
+                payload=payload(
+                    id='dc_input_power',
+                    device=d,
+                    name='DC Input Power',
+                    unit_of_measurement='W',
+                    device_class='power',
+                    state_class='measurement',
+                    force_update=True
+                ).encode(),
+                retain=True
+            )
+
+            await client.publish(
+                f'homeassistant/sensor/{d.sn}_ac_output_power/config',
+                payload=payload(
+                    id='ac_output_power',
+                    device=d,
+                    name='AC Output Power',
+                    unit_of_measurement='W',
+                    device_class='power',
+                    state_class='measurement',
+                    force_update=True
+                ).encode(),
+                retain=True
+            )
+
+            await client.publish(
+                f'homeassistant/sensor/{d.sn}_dc_output_power/config',
+                payload=payload(
+                    id='dc_output_power',
+                    device=d,
+                    name='DC Output Power',
+                    unit_of_measurement='W',
+                    device_class='power',
+                    state_class='measurement',
+                    force_update=True
+                ).encode(),
+                retain=True
+            )
+
+            await client.publish(
+                f'homeassistant/sensor/{d.sn}_total_battery_percent/config',
+                payload=payload(
+                    id='total_battery_percent',
+                    device=d,
+                    name='Total Battery Percent',
+                    unit_of_measurement='%',
+                    device_class='battery',
+                    state_class='measurement'
+                ).encode(),
+                retain=True
+            )
+
+            await client.publish(
+                f'homeassistant/switch/{d.sn}_ac_output_on/config',
+                payload=payload(
+                    id='ac_output_on',
+                    device=d,
+                    name='AC Output',
+                    device_class='outlet'
+                ).encode(),
+                retain=True
+            )
+
+            await client.publish(
+                f'homeassistant/switch/{d.sn}_dc_output_on/config',
+                payload=payload(
+                    id='dc_output_on',
+                    device=d,
+                    name='DC Output',
+                    device_class='outlet'
+                ).encode(),
+                retain=True
+            )
             if d.has_field_setter('led_mode'):
-                await client.publish(f'homeassistant/select/{d.sn}_led_mode/config',
-                            payload=payload(
-                                id='led_mode',
-                                device=d,
-                                name='LED Mode',
-                                icon='mdi:lightbulb',
-                                options= [ 'LOW', 'HIGH', 'SOS', 'OFF' ],
-                                force_update=True)
-                            .encode(),
-                            retain=True
-                            )
+                await client.publish(
+                    f'homeassistant/select/{d.sn}_led_mode/config',
+                    payload=payload(
+                        id='led_mode',
+                        device=d,
+                        name='LED Mode',
+                        icon='mdi:lightbulb',
+                        options=['LOW', 'HIGH', 'SOS', 'OFF'],
+                        force_update=True
+                    ).encode(),
+                    retain=True
+                )
             logging.info(f'Sent discovery message of {d.type}-{d.sn} to Home Assistant')
 
-
     async def _handle_message(self, client: Client, msg: ParserMessage):
         logging.debug(f'Got a message from {msg.device}: {msg.parsed}')
         topic_prefix = f'bluetti/state/{msg.device.type}-{msg.device.sn}/'
 
         if 'ac_input_power' in msg.parsed:
             await client.publish(
                 topic_prefix + 'ac_input_power',
@@ -374,7 +400,27 @@
                 payload=msg.parsed['auto_sleep_mode'].name.encode()
             )
         if 'led_mode' in msg.parsed:
             await client.publish(
                 topic_prefix + 'led_mode',
                 payload=msg.parsed['led_mode'].name.encode()
             )
+        if 'eco_on' in msg.parsed:
+            await client.publish(
+                topic_prefix + 'eco_on',
+                payload=('ON' if msg.parsed['eco_on'] else 'OFF').encode()
+            )
+        if 'eco_shutdown' in msg.parsed:
+            await client.publish(
+                topic_prefix + 'eco_shutdown',
+                payload=msg.parsed['eco_shutdown'].name.encode()
+            )
+        if 'charging_mode' in msg.parsed:
+            await client.publish(
+                topic_prefix + 'charging_mode',
+                payload=msg.parsed['charging_mode'].name.encode()
+            )
+        if 'power_lifting_on' in msg.parsed:
+            await client.publish(
+                topic_prefix + 'power_lifting_on',
+                payload=('ON' if msg.parsed['power_lifting_on'] else 'OFF').encode()
+            )
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt/server_cli.py` & `bluetti_mqtt-0.9.2/bluetti_mqtt/server_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,9 +118,10 @@
         warnings.simplefilter('always')
     else:
         logging.basicConfig(level=logging.INFO)
 
     cli = CommandLineHandler(argv)
     cli.execute()
 
+
 if __name__ == "__main__":
-    main(sys.argv)
+    main(sys.argv)
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt.egg-info/PKG-INFO` & `bluetti_mqtt-0.9.2/bluetti_mqtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetti-mqtt
-Version: 0.9.1
+Version: 0.9.2
 Summary: MQTT interface to Bluetti power stations
 Home-page: http://github.com/warhammerkid/bluetti_mqtt
 Author: Stephen Augenstein
 Author-email: perl.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bluetti_mqtt-0.9.1/bluetti_mqtt.egg-info/SOURCES.txt` & `bluetti_mqtt-0.9.2/bluetti_mqtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluetti_mqtt-0.9.1/setup.cfg` & `bluetti_mqtt-0.9.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bluetti_mqtt
-version = 0.9.1
+version = 0.9.2
 url = http://github.com/warhammerkid/bluetti_mqtt
 author = Stephen Augenstein
 author_email = perl.programmer@gmail.com
 description = MQTT interface to Bluetti power stations
 long_description = file: README.rst
 license = MIT
 classifiers =
```


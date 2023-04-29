# Comparing `tmp/python_ember_mug-0.7.0b4.tar.gz` & `tmp/python_ember_mug-0.7.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ember_mug-0.7.0b4.tar", max compression
+gzip compressed data, was "python_ember_mug-0.7.0b5.tar", max compression
```

## Comparing `python_ember_mug-0.7.0b4.tar` & `python_ember_mug-0.7.0b5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-27 02:53:54.686303 python_ember_mug-0.7.0b4/LICENSE
--rw-r--r--   0        0        0     5282 2023-04-27 02:53:54.686303 python_ember_mug-0.7.0b4/README.md
--rwxr-xr-x   0        0        0      189 2023-04-27 02:53:54.686303 python_ember_mug-0.7.0b4/ember_mug/__init__.py
--rw-r--r--   0        0        0      106 2023-04-27 02:53:54.686303 python_ember_mug-0.7.0b4/ember_mug/__main__.py
--rw-r--r--   0        0        0      296 2023-04-27 02:53:54.686303 python_ember_mug-0.7.0b4/ember_mug/cli/__init__.py
--rw-r--r--   0        0        0     8480 2023-04-27 02:53:54.686303 python_ember_mug-0.7.0b4/ember_mug/cli/commands.py
--rw-r--r--   0        0        0     2910 2023-04-27 02:53:54.686303 python_ember_mug-0.7.0b4/ember_mug/cli/helpers.py
--rw-r--r--   0        0        0     5394 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/ember_mug/consts.py
--rw-r--r--   0        0        0     8782 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/ember_mug/data.py
--rw-r--r--   0        0        0      605 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/ember_mug/formatting.py
--rw-r--r--   0        0        0    18205 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/ember_mug/mug.py
--rw-r--r--   0        0        0     2212 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/ember_mug/scanner.py
--rw-r--r--   0        0        0     1973 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/ember_mug/utils.py
--rw-r--r--   0        0        0     2896 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/cli/__init__.py
--rw-r--r--   0        0        0     7846 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/cli/test_commands.py
--rw-r--r--   0        0        0     2663 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/cli/test_helpers.py
--rw-r--r--   0        0        0     1199 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/conftest.py
--rw-r--r--   0        0        0    19254 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/test_connection.py
--rw-r--r--   0        0        0      776 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/test_consts.py
--rw-r--r--   0        0        0     2395 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/test_data.py
--rw-r--r--   0        0        0      534 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/test_formatting.py
--rw-r--r--   0        0        0     3372 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/test_mug_data.py
--rw-r--r--   0        0        0     2012 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/test_scanner.py
--rw-r--r--   0        0        0      801 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/test_utils.py
--rw-r--r--   0        0        0     6490 1970-01-01 00:00:00.000000 python_ember_mug-0.7.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/LICENSE
+-rw-r--r--   0        0        0     5282 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/README.md
+-rwxr-xr-x   0        0        0      189 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/__init__.py
+-rw-r--r--   0        0        0      106 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/__main__.py
+-rw-r--r--   0        0        0      296 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/cli/__init__.py
+-rw-r--r--   0        0        0     8933 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/cli/commands.py
+-rw-r--r--   0        0        0     2910 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/cli/helpers.py
+-rw-r--r--   0        0        0     5436 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/consts.py
+-rw-r--r--   0        0        0     8946 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/data.py
+-rw-r--r--   0        0        0      605 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/formatting.py
+-rw-r--r--   0        0        0    18888 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/mug.py
+-rw-r--r--   0        0        0     2212 2023-04-29 00:50:10.745538 python_ember_mug-0.7.0b5/ember_mug/scanner.py
+-rw-r--r--   0        0        0     2707 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/ember_mug/utils.py
+-rw-r--r--   0        0        0     2896 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/cli/__init__.py
+-rw-r--r--   0        0        0     7846 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/cli/test_commands.py
+-rw-r--r--   0        0        0     2663 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/cli/test_helpers.py
+-rw-r--r--   0        0        0     1199 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/conftest.py
+-rw-r--r--   0        0        0    19254 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/test_connection.py
+-rw-r--r--   0        0        0     1115 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/test_consts.py
+-rw-r--r--   0        0        0     2395 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/test_data.py
+-rw-r--r--   0        0        0      534 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/test_formatting.py
+-rw-r--r--   0        0        0     3428 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/test_mug_data.py
+-rw-r--r--   0        0        0     2012 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/test_scanner.py
+-rw-r--r--   0        0        0      801 2023-04-29 00:50:10.749538 python_ember_mug-0.7.0b5/tests/test_utils.py
+-rw-r--r--   0        0        0     6490 1970-01-01 00:00:00.000000 python_ember_mug-0.7.0b5/PKG-INFO
```

### Comparing `python_ember_mug-0.7.0b4/LICENSE` & `python_ember_mug-0.7.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b4/README.md` & `python_ember_mug-0.7.0b5/README.md`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b4/ember_mug/cli/commands.py` & `python_ember_mug-0.7.0b5/ember_mug/cli/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import re
 import sys
 from argparse import ArgumentParser, ArgumentTypeError, FileType, Namespace
 from typing import TYPE_CHECKING
 
 from bleak import BleakError
 
-from ..consts import ATTR_LABELS, EXTRA_ATTRS
+from ..consts import ATTR_LABELS, EXTRA_ATTRS, VolumeLevel
 from ..data import Colour
 from ..mug import EmberMug
 from ..scanner import discover_mugs, find_mug
 from .helpers import CommandLoop, print_changes, print_info, print_table, validate_mac
 
 if TYPE_CHECKING:
     from bleak.backends.device import BLEDevice
@@ -99,39 +99,47 @@
 async def get_mug_value(args: Namespace) -> None:
     """Get values from the mug and print them."""
     mug = await get_mug(args)
     data = {}
     attributes = [a.replace('-', '_') for a in args.attributes]
     async with mug.connection(adapter=args.adapter):
         for attr in attributes:
-            value = await getattr(mug, f'get_{attr}')()
+            try:
+                value = await getattr(mug, f'get_{attr}')()
+            except NotImplementedError as e:
+                print(e)
+                sys.exit(1)
             setattr(mug.data, attr, value)
             data[attr] = value
     if args.raw:
         print('\n'.join(str(v) for v in data.values()))
     else:
         print_table([(ATTR_LABELS.get(attr, attr), str(mug.data.get_formatted_attr(attr))) for attr in data])
 
 
 async def set_mug_value(args: Namespace) -> None:
     """Set one or more values on the mug."""
-    attrs = ('name', 'target_temp', 'temperature_unit', 'led_colour')
+    attrs = ('name', 'target_temp', 'temperature_unit', 'led_colour', 'volume_level')
     values = [(attr, value) for attr in attrs if (value := getattr(args, attr))]
     if not values:
         print('Please specify at least one attribute and value to set.')
         options = [f'--{a}' for a in attrs]
         print(f'Options: {", ".join(options)}')
         sys.exit(1)
 
     mug = await get_mug(args)
     async with mug.connection(adapter=args.adapter):
         for attr, value in values:
             method = getattr(mug, f'set_{attr.replace("-", "_")}')
             print(f'Setting {attr} to {value}')
-            await method(value)
+            try:
+                await method(value)
+            except NotImplementedError as e:
+                print(e)
+                sys.exit(1)
 
 
 def colour_type(value: str) -> Colour:
     """Convert a hex or rgb colour to a Colour object."""
     print(value)
     if match := re.match(r'#?([0-9a-f]{6})', value, re.IGNORECASE):
         colour = match.group(1)
@@ -201,14 +209,20 @@
         get_parser = subparsers.add_parser('get', description='Get mug value', parents=[shared_parser, info_parsers])
         get_parser.add_argument(dest='attributes', metavar='ATTRIBUTE', choices=get_attribute_names, nargs='+')
         set_parser = subparsers.add_parser('set', description='Set mug value', parents=[shared_parser, info_parsers])
         set_parser.add_argument('--name', help='Name', required=False)
         set_parser.add_argument('--target-temp', help='Target Temperature', type=float, required=False)
         set_parser.add_argument('--temperature-unit', help='Temperature Unit', choices=['C', 'F'], required=False)
         set_parser.add_argument('--led-colour', help='LED Colour', type=colour_type, required=False)
+        set_parser.add_argument(
+            '--volume-level',
+            help='Volume Level',
+            choices=[v.value for v in VolumeLevel],
+            required=False,
+        )
 
     async def run(self) -> None:
         """Run the specified command based on subparser."""
         args = self.parser.parse_args()
         if args.debug:
             logging.basicConfig(
                 stream=args.log_file,
```

### Comparing `python_ember_mug-0.7.0b4/ember_mug/cli/helpers.py` & `python_ember_mug-0.7.0b5/ember_mug/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b4/ember_mug/consts.py` & `python_ember_mug-0.7.0b5/ember_mug/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,10 +201,11 @@
     "liquid_level",
     "liquid_state",
 }
 EXTRA_ATTRS = {'dsk', 'udsk', 'battery_voltage', 'date_time_zone'}
 
 # Validation
 MUG_NAME_REGEX = re.compile(r"^[A-Za-z0-9,.\[\]#()!\"\';:|\-_+<>%= ]{1,16}$")
+MUG_NAME_PATTERN = MUG_NAME_REGEX.pattern
 MAC_ADDRESS_REGEX = re.compile(r"^([0-9A-Fa-f]{2}:){5}([0-9A-Fa-f]{2})$")
 
 IS_LINUX = platform.system() == "Linux"
```

### Comparing `python_ember_mug-0.7.0b4/ember_mug/data.py` & `python_ember_mug-0.7.0b5/ember_mug/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,14 +152,19 @@
     def initial_attributes(self) -> set[str]:
         """Initial attributes based on model and extra."""
         if self.include_extra is False:
             return INITIAL_ATTRS - EXTRA_ATTRS
         return INITIAL_ATTRS
 
     @cached_property
+    def all_attributes(self) -> set[str]:
+        """All attributes."""
+        return self.initial_attributes | self.update_attributes
+
+    @cached_property
     def update_attributes(self) -> set[str]:
         """Attributes to update based on model and extra."""
         attributes = UPDATE_ATTRS
         if self.include_extra is False:
             attributes = attributes - EXTRA_ATTRS
         if self.is_cup:
             # The Cup cannot be named
@@ -275,12 +280,13 @@
         return {label: self.get_formatted_attr(attr) for attr, label in self.model.attribute_labels.items()}
 
     def as_dict(self) -> dict[str, Any]:
         """Dump all attributes as dict for info/debugging."""
         data = {k: asdict(v) if is_dataclass(v) else v for k, v in asdict(self).items()}
         data.update(
             {
-                f'{attr}_display': getattr(self, f'{attr}_display')
-                for attr in ('led_colour', 'liquid_state', 'liquid_level', 'current_temp', 'target_temp')
+                f'{attr}_display': getattr(self, f'{attr}_display', None)
+                for attr in self.model.all_attributes
+                if hasattr(self, f'{attr}_display')
             },
         )
         return data
```

### Comparing `python_ember_mug-0.7.0b4/ember_mug/formatting.py` & `python_ember_mug-0.7.0b5/ember_mug/formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b4/ember_mug/mug.py` & `python_ember_mug-0.7.0b5/ember_mug/mug.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,14 +65,18 @@
         self._expected_disconnect = False
         self._callbacks: dict[Callable[[MugData], None], Callable[[], None]] = {}
         self._client: BleakClient = None  # type: ignore[assignment]
         self._queued_updates: set[str] = set()
         self._latest_events: dict[int, float] = {}
         self._client_kwargs: dict[str, str] = {}
 
+        # Just shortcuts, the value doesn't change once initialized
+        self.is_travel_mug = self.data.model.is_travel_mug
+        self.is_cup = self.data.model.is_cup
+
         logger.debug("New mug connection initialized.")
         self.set_client_options(**kwargs)
 
     def set_device(self, ble_device: BLEDevice) -> None:
         """Set the ble device."""
         logger.debug("Set new device from %s to %s", self.device, ble_device)
         self.device = ble_device
@@ -101,15 +105,15 @@
                     device=self.device,
                     name=f'{self.data.name} ({self.device.address})',
                     use_services_cache=True,
                     disconnected_callback=self._disconnect_callback,  # type: ignore
                     ble_device_callback=lambda: self.device,
                 )
                 if self.debug is True:
-                    log_services(client.services)
+                    await log_services(client)
                 self._expected_disconnect = False
             except (asyncio.TimeoutError, BleakError) as error:
                 logger.error("%s: Failed to connect to the mug: %s", self.device, error)
                 raise error
             # Attempt to pair for good measure
             try:
                 await client.pair()
@@ -191,18 +195,22 @@
 
     async def get_battery(self) -> BatteryInfo:
         """Get Battery percent from mug gatt."""
         return BatteryInfo.from_bytes(await self._read(MugCharacteristic.BATTERY))
 
     async def get_led_colour(self) -> Colour:
         """Get RGBA colours from mug gatt."""
+        if self.is_travel_mug is True:
+            raise NotImplementedError('The Travel Mug does not have an LED colour attribute')
         return Colour.from_bytes(await self._read(MugCharacteristic.LED))
 
     async def set_led_colour(self, colour: Colour) -> None:
         """Set new target temp for mug."""
+        if self.is_travel_mug is True:
+            raise NotImplementedError('The Travel Mug does not have an LED colour attribute')
         colour = Colour(*colour[:3], 255)  # It always expects 255 for alpha
         await self._write(MugCharacteristic.LED, colour.as_bytearray())
         self.data.led_colour = colour
 
     async def get_target_temp(self) -> float:
         """Get target temp form mug gatt."""
         temp_bytes = await self._read(MugCharacteristic.TARGET_TEMPERATURE)
@@ -222,47 +230,49 @@
     async def get_liquid_level(self) -> int:
         """Get liquid level from mug gatt."""
         liquid_level_bytes = await self._read(MugCharacteristic.LIQUID_LEVEL)
         return bytes_to_little_int(liquid_level_bytes)
 
     async def get_volume_level(self) -> VolumeLevel | None:
         """Get volume level from mug gatt."""
-        try:
-            volume_bytes = await self._read(MugCharacteristic.VOLUME)
-        except BleakError as e:
-            if not self.data.model.is_travel_mug:
-                raise NotImplementedError('Ony the travel mug has a volume')
-            logger.error('Failed to fetch volume attribute: %s', e)
-            return None
+        if self.is_travel_mug is False:
+            raise NotImplementedError('The Mug and Cup do not have a volume level attribute')
+        volume_bytes = await self._read(MugCharacteristic.VOLUME)
         volume_int = bytes_to_little_int(volume_bytes)
         return VolumeLevel.from_state(volume_int)
 
     async def set_volume_level(self, volume: int | VolumeLevel) -> None:
         """Set volume_level on Travel Mug."""
         if volume not in (0, 1, 2):
             raise ValueError('Volume level must be between 0 and 2 inclusively')
+        if self.is_travel_mug is False:
+            raise NotImplementedError('The Mug and Cup do not have a volume level attribute')
         volume_level = volume if isinstance(volume, VolumeLevel) else VolumeLevel.from_state(volume)
-        await self._write(MugCharacteristic.VOLUME, bytearray(bytearray([volume_level.state])))
+        await self._write(MugCharacteristic.VOLUME, bytearray([volume_level.state]))
         self.data.volume_level = volume_level
 
     async def get_liquid_state(self) -> LiquidState:
         """Get liquid state from mug gatt."""
         liquid_state_bytes = await self._read(MugCharacteristic.LIQUID_STATE)
         state = bytes_to_little_int(liquid_state_bytes)
         return LiquidState(state)
 
     async def get_name(self) -> str:
         """Get mug name from gatt."""
+        if self.is_cup is True:
+            raise NotImplementedError('The Cup does not have a name attribute')
         name_bytes: bytearray = await self._read(MugCharacteristic.MUG_NAME)
         return bytes(name_bytes).decode("utf8")
 
     async def set_name(self, name: str) -> None:
         """Assign new name to mug."""
         if MUG_NAME_REGEX.match(name) is None:
-            raise ValueError('Name cannot contain any special characters')
+            raise ValueError('Name cannot contain any special characters and must be 16 characters or less')
+        if self.is_cup is True:
+            raise NotImplementedError('The Cup does not have a name attribute')
         await self._write(MugCharacteristic.MUG_NAME, bytearray(name.encode("utf8")))
         self.data.name = name
 
     async def get_udsk(self) -> str:
         """Get mug udsk from gatt."""
         try:
             return decode_byte_string(await self._read(MugCharacteristic.UDSK))
```

### Comparing `python_ember_mug-0.7.0b4/ember_mug/scanner.py` & `python_ember_mug-0.7.0b5/ember_mug/scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b4/ember_mug/utils.py` & `python_ember_mug-0.7.0b5/ember_mug/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import base64
 import contextlib
 import logging
 import re
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from bleak import BleakGATTServiceCollection
+    from bleak import BleakClient, BleakError
 
 logger = logging.getLogger(__name__)
 
 
 def decode_byte_string(data: bytes | bytearray) -> str:
     """Convert bytes to text as Ember expects."""
     if not data:
@@ -44,19 +44,34 @@
     temp = float(bytes_to_little_int(temp_bytes)) * 0.01
     if metric is False:
         # Convert to fahrenheit
         temp = (temp * 9 / 5) + 32
     return round(temp, 2)
 
 
-def log_services(services: BleakGATTServiceCollection) -> None:
-    """Log services for debugging."""
-    logger.debug("Logging all services that were discovered")
-    for service in services:
-        logger.debug(
-            "Service '%s' (UUID: %s) has the characteristics:\n %s",
-            service.description,
-            service.uuid,
-            "\n".join(
-                f'{characteristic.uuid}: {characteristic.description}' for characteristic in service.characteristics
-            ),
-        )
+async def log_services(client: BleakClient) -> None:
+    """Log all services and all values for debugging/development."""
+    logger.info("Logging all services that were discovered")
+    for service in client.services:
+        logger.info("[Service] %s: %s", service.uuid, service.description)
+        for characteristic in service.characteristics:
+            value: bytearray | BleakError | None = None
+            if "read" in characteristic.properties:
+                try:
+                    value = await client.read_gatt_char(characteristic.uuid)
+                except BleakError as e:
+                    value = e
+            logger.info(
+                "\t[Characteristic] %s: %s | Name: %s | Value: '%s'",
+                characteristic.uuid,
+                ",".join(characteristic.properties),
+                characteristic.description,
+                value,
+            )
+            for descriptor in characteristic.descriptors:
+                value = await client.read_gatt_descriptor(descriptor.handle)
+                logger.info(
+                    "\t\t[Descriptor] %s: Handle: %s | Value: '%s'",
+                    descriptor.uuid,
+                    descriptor.handle,
+                    value,
+                )
```

### Comparing `python_ember_mug-0.7.0b4/pyproject.toml` & `python_ember_mug-0.7.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "python-ember-mug"
-version = "0.7.0b4"
+version = "0.7.0b5"
 homepage = "https://github.com/sopelj/python-ember-mug"
 description = "Python Library for Ember Mugs."
 authors = ["Jesse Sopel <jesse.sopel@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `python_ember_mug-0.7.0b4/tests/cli/test_commands.py` & `python_ember_mug-0.7.0b5/tests/cli/test_commands.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b4/tests/cli/test_helpers.py` & `python_ember_mug-0.7.0b5/tests/cli/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b4/tests/conftest.py` & `python_ember_mug-0.7.0b5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b4/tests/test_connection.py` & `python_ember_mug-0.7.0b5/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b4/tests/test_data.py` & `python_ember_mug-0.7.0b5/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b4/tests/test_formatting.py` & `python_ember_mug-0.7.0b5/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b4/tests/test_mug_data.py` & `python_ember_mug-0.7.0b5/tests/test_mug_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         'led_colour': Colour(red=255, green=255, blue=255),
         'led_colour_display': '#ffffff',
         'liquid_level': 0,
         'liquid_level_display': '0.00%',
         'liquid_state': LiquidState.UNKNOWN,
         'liquid_state_display': 'Unknown',
         'meta': {'mug_id': 'test_id', 'serial_number': 'serial number'},
+        'meta_display': 'Serial Number: serial number',
         'name': '',
         'target_temp': 0.0,
         'target_temp_display': '0.00°C',
         'temperature_unit': TemperatureUnit.CELSIUS,
         'udsk': '',
         'volume_level': None,
     }
```

### Comparing `python_ember_mug-0.7.0b4/tests/test_scanner.py` & `python_ember_mug-0.7.0b5/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b4/tests/test_utils.py` & `python_ember_mug-0.7.0b5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b4/PKG-INFO` & `python_ember_mug-0.7.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ember-mug
-Version: 0.7.0b4
+Version: 0.7.0b5
 Summary: Python Library for Ember Mugs.
 Home-page: https://github.com/sopelj/python-ember-mug
 License: MIT
 Author: Jesse Sopel
 Author-email: jesse.sopel@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```


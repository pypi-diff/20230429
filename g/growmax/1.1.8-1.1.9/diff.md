# Comparing `tmp/growmax-1.1.8.tar.gz` & `tmp/growmax-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "growmax-1.1.8.tar", last modified: Mon Mar 13 01:06:24 2023, max compression
+gzip compressed data, was "growmax-1.1.9.tar", last modified: Sun Mar 26 02:48:31 2023, max compression
```

## Comparing `growmax-1.1.8.tar` & `growmax-1.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:06:24.306501 growmax-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-13 01:06:10.000000 growmax-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-03-13 01:06:24.306501 growmax-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-13 01:06:10.000000 growmax-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-13 01:06:10.000000 growmax-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-13 01:06:24.306501 growmax-1.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:06:24.302502 growmax-1.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:06:24.302502 growmax-1.1.8/src/growmax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:06:24.306501 growmax-1.1.8/src/growmax/atlas_ph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/atlas_ph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/atlas_ph/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/atlas_ph/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/atlas_ph/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/atlas_ph/import_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/atlas_ph/set_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/atlas_ph/uart_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:06:24.306501 growmax-1.1.8/src/growmax/displays/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/displays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/displays/sh1107.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/displays/ssd1327.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/moisture.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/ntpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/pump.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/routine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:06:24.306501 growmax-1.1.8/src/growmax/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/sensors/adafruit_scd4x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:06:24.306501 growmax-1.1.8/src/growmax/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/utils/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/utils/displays.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/utils/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/utils/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/utils/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/utils/water.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-13 01:06:10.000000 growmax-1.1.8/src/growmax/utils/wifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:06:24.306501 growmax-1.1.8/src/growmax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-03-13 01:06:24.000000 growmax-1.1.8/src/growmax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-13 01:06:24.000000 growmax-1.1.8/src/growmax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 01:06:24.000000 growmax-1.1.8/src/growmax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-13 01:06:24.000000 growmax-1.1.8/src/growmax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.922046 growmax-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-26 02:48:16.000000 growmax-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-03-26 02:48:31.922046 growmax-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-26 02:48:16.000000 growmax-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-26 02:48:16.000000 growmax-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-26 02:48:31.922046 growmax-1.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.918046 growmax-1.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.918046 growmax-1.1.9/src/growmax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.922046 growmax-1.1.9/src/growmax/atlas_ph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/atlas_ph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/atlas_ph/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/atlas_ph/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/atlas_ph/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/atlas_ph/import_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/atlas_ph/set_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/atlas_ph/uart_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.922046 growmax-1.1.9/src/growmax/displays/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/displays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/displays/sh1107.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/displays/ssd1327.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/moisture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/ntpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/pump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/routine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.922046 growmax-1.1.9/src/growmax/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/sensors/adafruit_scd4x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.922046 growmax-1.1.9/src/growmax/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/displays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/water.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.918046 growmax-1.1.9/src/growmax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-03-26 02:48:31.000000 growmax-1.1.9/src/growmax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-26 02:48:31.000000 growmax-1.1.9/src/growmax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 02:48:31.000000 growmax-1.1.9/src/growmax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-26 02:48:31.000000 growmax-1.1.9/src/growmax.egg-info/top_level.txt
```

### Comparing `growmax-1.1.8/LICENSE` & `growmax-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/PKG-INFO` & `growmax-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growmax
-Version: 1.1.8
+Version: 1.1.9
 Summary: Micropython routines for automated plant watering and monitoring.
 Home-page: https://github.com/opensensor/growmax
 Author: Matt Davis and OpenSensor.io
 Author-email: matteius@gmail.com
 Project-URL: Bug Tracker, https://github.com/opensensor/growmax/-/issues
 Project-URL: repository, https://github.com/opensensor/growmax
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
```

### Comparing `growmax-1.1.8/README.md` & `growmax-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/setup.cfg` & `growmax-1.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = growmax
-version = 1.1.8
+version = 1.1.9
 author = Matt Davis and OpenSensor.io
 author_email = matteius@gmail.com
 description = Micropython routines for automated plant watering and monitoring.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/opensensor/growmax
 project_urls =
```

### Comparing `growmax-1.1.8/src/growmax/atlas_ph/calibration.py` & `growmax-1.1.9/src/growmax/atlas_ph/calibration.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/src/growmax/atlas_ph/i2c.py` & `growmax-1.1.9/src/growmax/atlas_ph/i2c.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/src/growmax/config.py` & `growmax-1.1.9/src/growmax/config.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/src/growmax/constants.py` & `growmax-1.1.9/src/growmax/constants.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/src/growmax/displays/sh1107.py` & `growmax-1.1.9/src/growmax/displays/sh1107.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/src/growmax/displays/ssd1327.py` & `growmax-1.1.9/src/growmax/displays/ssd1327.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/src/growmax/moisture.py` & `growmax-1.1.9/src/growmax/moisture.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/src/growmax/ntpclient.py` & `growmax-1.1.9/src/growmax/ntpclient.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/src/growmax/pump.py` & `growmax-1.1.9/src/growmax/pump.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/src/growmax/routine.py` & `growmax-1.1.9/src/growmax/routine.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import gc
 import random
 import utime
 from machine import Pin
 
 from growmax.moisture import Moisture
 from growmax.pump import Pump
+from growmax.utils import api
 from growmax.utils.configs import get_moisture_threshold_for_position
 from growmax.utils.displays import boot_sequence, display_basic_stats, display_ph_reading
 from growmax.utils.water import statistically_has_water
 from growmax.utils.wifi import ensure_wifi_connected
 
 # User's config file
 import config
@@ -63,19 +64,23 @@
                 if (config.PUMP_WHEN_DRY or has_water) and soil_moisture >= moisture_config:
                     print("position: ", pump_position)
                     pumps[position].dose(1, config.PUMP_CYCLE_DURATION)
                 utime.sleep(2)
             except Exception as e:
                 print("Exception: ", str(e))
 
-        if scd40x:
-            if config.OPEN_SENSOR_COLLECT_DATA:
-                from growmax.utils.api import read_and_report_adafruit_scd4x
-                read_and_report_adafruit_scd4x(scd40x)
-            else:
+        if config.OPEN_SENSOR_COLLECT_DATA:
+            report_data = api.get_device_metadata()
+            if scd40x:
+                api.read_adafruit_scd4x_(scd40x, report_data)
+            report_data["moisture"] = {
+                "readings": soil_moistures
+            }
+            api.report_environment_data(report_data)
+        elif scd40x:
                 from growmax.utils.sensors import read_adafruit_scd4x
                 read_adafruit_scd4x(scd40x)
         if atlas_ph:
             ph_reading = atlas_ph.obtain_ph_reading()
             display_ph_reading(ph_reading)
             utime.sleep(3)
```

### Comparing `growmax-1.1.8/src/growmax/sensors/adafruit_scd4x.py` & `growmax-1.1.9/src/growmax/sensors/adafruit_scd4x.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/src/growmax/utils/api.py` & `growmax-1.1.9/src/growmax/utils/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,44 +3,56 @@
 import time
 from growmax.utils import sensors
 
 import config
 
 headers = {'content-type': 'application/json'}
 
-def read_and_report_adafruit_scd4x(scd4x):
-    """This method requires installing urequests and ujson from pypi."""
+
+def get_device_metadata():
+    report_data = {}
     try:
-        import urequests
-        import ujson
-        data = sensors.read_adafruit_scd4x(scd4x)
         time.sleep(1.0)
         device_id = ubinascii.hexlify(machine.unique_id()).decode()
         time.sleep(1.0)
-        report_data = {
-            "device_metadata": {
-                "device_id": device_id,
-                "name": config.DEVICE_NAME,
-            },
-            "temp": {
-                "temp": data[0],
-                "unit": "C"
-            },
-            "rh": {
-                "rh": data[1],
-            },
-            "co2": {
-                "ppm": data[2],
-            }
+        report_data["device_metadata"] = {
+            "device_id": device_id,
+            "name": config.DEVICE_NAME,
         }
+    except Exception as e:
+        print(e)
+    return report_data
+
+
+def read_adafruit_scd4x_(scd4x, report_data):
+    try:
+        time.sleep(1.0)
+        data = sensors.read_adafruit_scd4x(scd4x)
+        time.sleep(1.0)
+        report_data["temp"] = {
+            "temp": data[0],
+            "unit": "C"
+        }
+        report_data["rh"] = {
+            "rh": data[1],
+        }
+        report_data["co2"] = {
+            "ppm": data[2],
+        }
+    except Exception as e:
+        print(e)
+
+
+def report_environment_data(report_data):
+    """This method requires installing urequests and ujson from pypi."""
+    try:
+        import urequests
+        import ujson
         time.sleep(1.0)
         resp = urequests.post(
             "https://api.opensensor.io/environment/",
             headers=headers,
             data=ujson.dumps(report_data))
         print(resp.status_code)
         resp.close()
-        return data
     except Exception as e:
         print(e)
-    return None
-
```

### Comparing `growmax-1.1.8/src/growmax/utils/displays.py` & `growmax-1.1.9/src/growmax/utils/displays.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/src/growmax/utils/sensors.py` & `growmax-1.1.9/src/growmax/utils/sensors.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/src/growmax/utils/wifi.py` & `growmax-1.1.9/src/growmax/utils/wifi.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.8/src/growmax.egg-info/PKG-INFO` & `growmax-1.1.9/src/growmax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growmax
-Version: 1.1.8
+Version: 1.1.9
 Summary: Micropython routines for automated plant watering and monitoring.
 Home-page: https://github.com/opensensor/growmax
 Author: Matt Davis and OpenSensor.io
 Author-email: matteius@gmail.com
 Project-URL: Bug Tracker, https://github.com/opensensor/growmax/-/issues
 Project-URL: repository, https://github.com/opensensor/growmax
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
```

### Comparing `growmax-1.1.8/src/growmax.egg-info/SOURCES.txt` & `growmax-1.1.9/src/growmax.egg-info/SOURCES.txt`

 * *Files identical despite different names*


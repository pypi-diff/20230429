# Comparing `tmp/plugwise-0.9.4a8.tar.gz` & `tmp/plugwise-0.9.4a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugwise-0.9.4a8.tar", last modified: Sun Mar 21 19:28:51 2021, max compression
+gzip compressed data, was "plugwise-0.9.4a9.tar", last modified: Mon Mar 22 18:31:04 2021, max compression
```

## Comparing `plugwise-0.9.4a8.tar` & `plugwise-0.9.4a9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-21 19:28:51.416805 plugwise-0.9.4a8/
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      754 2021-03-21 19:28:51.416805 plugwise-0.9.4a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4567 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-21 19:28:51.408805 plugwise-0.9.4a8/plugwise/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-21 19:28:51.412805 plugwise-0.9.4a8/plugwise/connections/
--rw-r--r--   0 runner    (1001) docker     (121)     4280 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2861 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/connections/serial.py
--rw-r--r--   0 runner    (1001) docker     (121)     2873 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/connections/socket.py
--rw-r--r--   0 runner    (1001) docker     (121)    14064 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    15574 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    36993 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-21 19:28:51.412805 plugwise-0.9.4a8/plugwise/messages/
--rw-r--r--   0 runner    (1001) docker     (121)      824 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12735 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/messages/requests.py
--rw-r--r--   0 runner    (1001) docker     (121)    15766 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/messages/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-21 19:28:51.416805 plugwise-0.9.4a8/plugwise/nodes/
--rw-r--r--   0 runner    (1001) docker     (121)    14721 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22509 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/nodes/circle.py
--rw-r--r--   0 runner    (1001) docker     (121)     5546 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/nodes/circle_plus.py
--rw-r--r--   0 runner    (1001) docker     (121)     4935 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/nodes/scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     5575 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/nodes/sed.py
--rw-r--r--   0 runner    (1001) docker     (121)     3456 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/nodes/sense.py
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/nodes/stealth.py
--rw-r--r--   0 runner    (1001) docker     (121)     2276 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/nodes/switch.py
--rw-r--r--   0 runner    (1001) docker     (121)     5348 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    19137 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/smile.py
--rw-r--r--   0 runner    (1001) docker     (121)    32571 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/stick.py
--rw-r--r--   0 runner    (1001) docker     (121)     9527 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/plugwise/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-21 19:28:51.408805 plugwise-0.9.4a8/plugwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      754 2021-03-21 19:28:51.000000 plugwise-0.9.4a8/plugwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      809 2021-03-21 19:28:51.000000 plugwise-0.9.4a8/plugwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-21 19:28:51.000000 plugwise-0.9.4a8/plugwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-21 19:28:51.000000 plugwise-0.9.4a8/plugwise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-03-21 19:28:51.000000 plugwise-0.9.4a8/plugwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-03-21 19:28:51.000000 plugwise-0.9.4a8/plugwise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3106 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      807 2021-03-21 19:28:51.416805 plugwise-0.9.4a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2021-03-21 19:28:50.000000 plugwise-0.9.4a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 18:31:04.851548 plugwise-0.9.4a9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2021-03-22 18:31:04.851548 plugwise-0.9.4a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4567 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 18:31:04.843548 plugwise-0.9.4a9/plugwise/
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 18:31:04.843548 plugwise-0.9.4a9/plugwise/connections/
+-rw-r--r--   0 runner    (1001) docker     (121)     4280 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2861 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/connections/serial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2873 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/connections/socket.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14064 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15574 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1838 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36937 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 18:31:04.851548 plugwise-0.9.4a9/plugwise/messages/
+-rw-r--r--   0 runner    (1001) docker     (121)      824 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12735 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/messages/requests.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15766 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/messages/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 18:31:04.851548 plugwise-0.9.4a9/plugwise/nodes/
+-rw-r--r--   0 runner    (1001) docker     (121)    14721 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22509 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/nodes/circle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5546 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/nodes/circle_plus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4935 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/nodes/scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5575 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/nodes/sed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3456 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/nodes/sense.py
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/nodes/stealth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2276 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/nodes/switch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5348 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19137 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/smile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32571 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/stick.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9527 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 18:31:04.843548 plugwise-0.9.4a9/plugwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      809 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/plugwise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3106 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2021-03-22 18:31:04.851548 plugwise-0.9.4a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1379 2021-03-22 18:31:04.000000 plugwise-0.9.4a9/setup.py
```

### Comparing `plugwise-0.9.4a8/LICENSE` & `plugwise-0.9.4a9/LICENSE`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/PKG-INFO` & `plugwise-0.9.4a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: plugwise
-Version: 0.9.4a8
+Version: 0.9.4a9
 Summary: Plugwise (Adam/Anna/P1/Stick/Stretch) API to use in conjunction with Home Assistant Core.
 Home-page: https://github.com/plugwise/python-plugwise
 Author: Plugwise-team
 Author-email: info@compa.nl
 License: MIT
 Description: Plugwise API to use in conjunction with Home Assistant, but it can also be used as a python-module.
 Keywords: HomeAssistant HA Home Assistant Anna Adam P1 Smile Stretch Stick Plugwise
```

### Comparing `plugwise-0.9.4a8/README.md` & `plugwise-0.9.4a9/README.md`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/connections/__init__.py` & `plugwise-0.9.4a9/plugwise/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/connections/serial.py` & `plugwise-0.9.4a9/plugwise/connections/serial.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/connections/socket.py` & `plugwise-0.9.4a9/plugwise/connections/socket.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/constants.py` & `plugwise-0.9.4a9/plugwise/constants.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/controller.py` & `plugwise-0.9.4a9/plugwise/controller.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/exceptions.py` & `plugwise-0.9.4a9/plugwise/exceptions.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/helper.py` & `plugwise-0.9.4a9/plugwise/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,14 @@
         self._timeout = None
 
         self._appliances = None
         self._domain_objects = None
         self._locations = None
         self._modules = None
 
-        self.active_device_present = False
         self.appl_data = {}
         self.gateway_id = None
         self.heater_id = None
         self.notifications = {}
         self.smile_hostname = None
         self.smile_name = None
         self.smile_type = None
@@ -430,16 +429,17 @@
 
         # The presence of either indicates a local active device, e.g. heat-pump or gas-fired heater
         self._cp_state = self._appliances.find(
             ".//logs/point_log[type='compressor_state']"
         )
         fl_state = self._appliances.find(".//logs/point_log[type='flame_state']")
         bl_state = self._appliances.find(".//services/boiler_state")
-        if self._cp_state or fl_state or bl_state:
-            self.active_device_present = True
+        self.active_device_present = (
+            self._cp_state is not None or fl_state is not None or bl_state is not None
+        )
 
         for appliance in self._appliances:
             appl = Munch()
             appl.pwclass = appliance.find("type").text
             # Nothing useful in opentherm so skip it
             if appl.pwclass == "open_therm_gateway":
                 continue
@@ -928,21 +928,19 @@
         tag = "zone_preset_based_on_time_and_presence_with_override"
         rule_ids = self.rule_ids_by_tag(tag, loc_id)
 
         if rule_ids is None:
             return available, selected, schedule_temperature
 
         for rule_id, dummy in rule_ids.items():
-            active = False
             name = self._domain_objects.find(f'rule[@id="{rule_id}"]/name').text
-            if (
+            active = (
                 self._domain_objects.find(f'rule[@id="{rule_id}"]/active').text
                 == "true"
-            ):
-                active = True
+            )
             schemas[name] = active
             schedules = {}
             locator = f'rule[@id="{rule_id}"]/directives'
             directives = self._domain_objects.find(locator)
             for directive in directives:
                 schedule = directive.find("then").attrib
                 keys, dummy = zip(*schedule.items())
```

### Comparing `plugwise-0.9.4a8/plugwise/messages/__init__.py` & `plugwise-0.9.4a9/plugwise/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/messages/requests.py` & `plugwise-0.9.4a9/plugwise/messages/requests.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/messages/responses.py` & `plugwise-0.9.4a9/plugwise/messages/responses.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/nodes/__init__.py` & `plugwise-0.9.4a9/plugwise/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/nodes/circle.py` & `plugwise-0.9.4a9/plugwise/nodes/circle.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/nodes/circle_plus.py` & `plugwise-0.9.4a9/plugwise/nodes/circle_plus.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/nodes/scan.py` & `plugwise-0.9.4a9/plugwise/nodes/scan.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/nodes/sed.py` & `plugwise-0.9.4a9/plugwise/nodes/sed.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/nodes/sense.py` & `plugwise-0.9.4a9/plugwise/nodes/sense.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/nodes/switch.py` & `plugwise-0.9.4a9/plugwise/nodes/switch.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/parser.py` & `plugwise-0.9.4a9/plugwise/parser.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/smile.py` & `plugwise-0.9.4a9/plugwise/smile.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/stick.py` & `plugwise-0.9.4a9/plugwise/stick.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise/util.py` & `plugwise-0.9.4a9/plugwise/util.py`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/plugwise.egg-info/PKG-INFO` & `plugwise-0.9.4a9/plugwise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: plugwise
-Version: 0.9.4a8
+Version: 0.9.4a9
 Summary: Plugwise (Adam/Anna/P1/Stick/Stretch) API to use in conjunction with Home Assistant Core.
 Home-page: https://github.com/plugwise/python-plugwise
 Author: Plugwise-team
 Author-email: info@compa.nl
 License: MIT
 Description: Plugwise API to use in conjunction with Home Assistant, but it can also be used as a python-module.
 Keywords: HomeAssistant HA Home Assistant Anna Adam P1 Smile Stretch Stick Plugwise
```

### Comparing `plugwise-0.9.4a8/plugwise.egg-info/SOURCES.txt` & `plugwise-0.9.4a9/plugwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/pyproject.toml` & `plugwise-0.9.4a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/setup.cfg` & `plugwise-0.9.4a9/setup.cfg`

 * *Files identical despite different names*

### Comparing `plugwise-0.9.4a8/setup.py` & `plugwise-0.9.4a9/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/hubitatcontrol-2.0.0.tar.gz` & `tmp/hubitatcontrol-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubitatcontrol-2.0.0.tar", max compression
+gzip compressed data, was "hubitatcontrol-2.1.0.tar", max compression
```

## Comparing `hubitatcontrol-2.0.0.tar` & `hubitatcontrol-2.1.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-03-12 19:21:22.061753 hubitatcontrol-2.0.0/LICENSE
--rw-r--r--   0        0        0     6247 2023-04-08 21:56:56.885073 hubitatcontrol-2.0.0/README.md
--rw-r--r--   0        0        0     1483 2023-04-08 21:56:56.889073 hubitatcontrol-2.0.0/hubitatcontrol/__init__.py
--rw-r--r--   0        0        0     3765 2023-04-08 21:56:56.889073 hubitatcontrol-2.0.0/hubitatcontrol/__main__.py
--rw-r--r--   0        0        0     1060 2023-03-30 01:32:16.534352 hubitatcontrol-2.0.0/hubitatcontrol/generic.py
--rw-r--r--   0        0        0     2902 2023-04-08 21:56:56.889073 hubitatcontrol-2.0.0/hubitatcontrol/hub.py
--rw-r--r--   0        0        0     2774 2023-03-30 01:32:16.534352 hubitatcontrol-2.0.0/hubitatcontrol/lights.py
--rw-r--r--   0        0        0      336 2023-03-30 01:32:16.534352 hubitatcontrol-2.0.0/hubitatcontrol/sensors.py
--rw-r--r--   0        0        0     2415 2023-04-08 21:57:32.752590 hubitatcontrol-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     7129 1970-01-01 00:00:00.000000 hubitatcontrol-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-03-12 19:21:22.061753 hubitatcontrol-2.1.0/LICENSE
+-rw-r--r--   0        0        0     6247 2023-04-23 03:06:31.100361 hubitatcontrol-2.1.0/README.md
+-rw-r--r--   0        0        0     1936 2023-04-29 01:57:50.164004 hubitatcontrol-2.1.0/hubitatcontrol/__init__.py
+-rw-r--r--   0        0        0     3765 2023-04-23 03:06:31.104361 hubitatcontrol-2.1.0/hubitatcontrol/__main__.py
+-rw-r--r--   0        0        0      172 2023-04-29 01:54:13.037854 hubitatcontrol-2.1.0/hubitatcontrol/environment.py
+-rw-r--r--   0        0        0     1060 2023-04-23 03:06:31.104361 hubitatcontrol-2.1.0/hubitatcontrol/generic.py
+-rw-r--r--   0        0        0     2902 2023-04-23 03:06:31.104361 hubitatcontrol-2.1.0/hubitatcontrol/hub.py
+-rw-r--r--   0        0        0     2774 2023-04-23 03:06:31.104361 hubitatcontrol-2.1.0/hubitatcontrol/lights.py
+-rw-r--r--   0        0        0      336 2023-04-29 01:51:56.296942 hubitatcontrol-2.1.0/hubitatcontrol/sensors.py
+-rw-r--r--   0        0        0     2606 2023-04-29 02:26:10.971754 hubitatcontrol-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7129 1970-01-01 00:00:00.000000 hubitatcontrol-2.1.0/PKG-INFO
```

### Comparing `hubitatcontrol-2.0.0/LICENSE` & `hubitatcontrol-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.0.0/README.md` & `hubitatcontrol-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.0.0/hubitatcontrol/__init__.py` & `hubitatcontrol-2.1.0/hubitatcontrol/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 def get_hub(host, token, app_id, cloud_token=None) -> Hub:
     return Hub(host=host, token=token, app_id=app_id, cloud_token=cloud_token)
 
 
 def lookup_device(hub_in, device_lookup):
+    # TODO Refactor to use ID, and and add interface for name search
     """
     Takes device NAME, not ID for lookup
     """
     d = hub_in.get_device(device_lookup)
     if d is None:
         raise Exception("Device Not Found")
     if "ColorControl" in d["capabilities"] and "ColorMode" in d["capabilities"]:
@@ -28,7 +29,16 @@
     if "PowerMeter" in d["capabilities"] and "Outlet" in d["capabilities"]:
         return hubitatcontrol.generic.ZigbeeOutlet(device_from_hub=d, hub=hub_in)
     if "Switch" in d["capabilities"]:
         return hubitatcontrol.generic.Switch(device_from_hub=d, hub=hub_in)
     if "TemperatureMeasurement" in d["capabilities"]:
         return hubitatcontrol.sensors.TemperatureSensor(device_from_hub=d, hub=hub_in)
     return d  # Fall through return # pragma: no cover
+
+
+def get_all_temperature_sensors(hub_in: hubitatcontrol.hub) -> list[hubitatcontrol.sensors.TemperatureSensor]:
+    """Returns list of all hub devices with associated helper functions"""
+    device_list = []
+    for i in hub_in.devices:
+        if "TemperatureMeasurement" in i["capabilities"]:
+            device_list.append(lookup_device(hub_in, i['name']))
+    return device_list
```

### Comparing `hubitatcontrol-2.0.0/hubitatcontrol/__main__.py` & `hubitatcontrol-2.1.0/hubitatcontrol/__main__.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.0.0/hubitatcontrol/generic.py` & `hubitatcontrol-2.1.0/hubitatcontrol/generic.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.0.0/hubitatcontrol/hub.py` & `hubitatcontrol-2.1.0/hubitatcontrol/hub.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.0.0/hubitatcontrol/lights.py` & `hubitatcontrol-2.1.0/hubitatcontrol/lights.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.0.0/pyproject.toml` & `hubitatcontrol-2.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hubitatcontrol"
-version = "2.0.0"
+version = "v2.1.0"
 description = "Hubitat Maker API Interface"
 authors = ["Jesse Schoepfer <jelloeater@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/Jelloeater/hubitatcontrol"
 keywords = ["hubitat", "makerapi","requests"]
 classifiers = ["Development Status :: 5 - Production/Stable",
@@ -41,14 +41,22 @@
 exclude =['./tests']
 max-line-length = 120
 count = false
 statistics = true
 diff = true
 format = "pylint"
 
+[tool.autoflake]
+check = true
+in-place = true
+expand-star-imports = false
+remove-unused-variables = true
+remove-duplicate-keys = true
+ignore-init-module-imports = false
+recursive = true
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = "True"
 force_grid_wrap = 0
 use_parentheses = "True"
 line_length = 120
@@ -76,18 +84,18 @@
 setuptools = "*"
 pytest = "*"
 pytest-cov = "*"
 python-dotenv = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest-pycharm = "*"
+autoflake = "*"
 pre-commit = "*"
 vulture = "*"
 isort = "*"
-radon = "*"
 xenon = "*"
 black = "*"
 typing_extensions ="*"
 #typeguard ="*" # Typing
 #mypy = "*" # Typing
 pdoc3 = "*"
 pylint = "*"
```

### Comparing `hubitatcontrol-2.0.0/PKG-INFO` & `hubitatcontrol-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubitatcontrol
-Version: 2.0.0
+Version: 2.1.0
 Summary: Hubitat Maker API Interface
 Home-page: https://github.com/Jelloeater/hubitatcontrol
 License: MIT
 Keywords: hubitat,makerapi,requests
 Author: Jesse Schoepfer
 Author-email: jelloeater@gmail.com
 Requires-Python: >=3.10,<4.0
```


# Comparing `tmp/estimenergy-2.0.5.tar.gz` & `tmp/estimenergy-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estimenergy-2.0.5.tar", max compression
+gzip compressed data, was "estimenergy-2.0.6.tar", max compression
```

## Comparing `estimenergy-2.0.5.tar` & `estimenergy-2.0.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1089 2023-04-28 18:18:17.069437 estimenergy-2.0.5/LICENSE
--rw-r--r--   0        0        0     4481 2023-04-28 18:18:17.069437 estimenergy-2.0.5/README.md
--rw-r--r--   0        0        0        0 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/__init__.py
--rw-r--r--   0        0        0       38 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/client/__init__.py
--rw-r--r--   0        0        0      631 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/client/client.py
--rw-r--r--   0        0        0      451 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/config.py
--rw-r--r--   0        0        0     6030 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/const.py
--rw-r--r--   0        0        0      665 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/db.py
--rw-r--r--   0        0        0      133 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/devices/__init__.py
--rw-r--r--   0        0        0     3108 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/devices/base_device.py
--rw-r--r--   0        0        0       99 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/devices/device_error.py
--rw-r--r--   0        0        0     4048 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/devices/device_registry.py
--rw-r--r--   0        0        0     6177 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/devices/glow_device.py
--rw-r--r--   0        0        0      540 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/helpers.py
--rw-r--r--   0        0        0      318 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/influx.py
--rw-r--r--   0        0        0      613 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/log.py
--rw-r--r--   0        0        0     2088 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/main.py
--rw-r--r--   0        0        0       94 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/models/config/__init__.py
--rw-r--r--   0        0        0     1500 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/models/config/config.py
--rw-r--r--   0        0        0       86 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/models/config/dev_config.py
--rw-r--r--   0        0        0      138 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/models/config/influx_config.py
--rw-r--r--   0        0        0      208 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/models/config/logging_config.py
--rw-r--r--   0        0        0      279 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/models/config/networking_config.py
--rw-r--r--   0        0        0      186 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/models/config/sql_config.py
--rw-r--r--   0        0        0      896 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/models/day.py
--rw-r--r--   0        0        0      912 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/models/device_config.py
--rw-r--r--   0        0        0       76 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/models/message.py
--rw-r--r--   0        0        0      874 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/models/month.py
--rw-r--r--   0        0        0      335 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/models/total.py
--rw-r--r--   0        0        0      799 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/models/year.py
--rw-r--r--   0        0        0      479 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/prometheus.py
--rw-r--r--   0        0        0        0 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/routers/__init__.py
--rw-r--r--   0        0        0     4261 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/routers/day_router.py
--rw-r--r--   0        0        0     4293 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/routers/device_router.py
--rw-r--r--   0        0        0     1466 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/routers/month_router.py
--rw-r--r--   0        0        0     1466 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/routers/total_router.py
--rw-r--r--   0        0        0     1436 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/routers/year_router.py
--rw-r--r--   0        0        0        0 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/services/__init__.py
--rw-r--r--   0        0        0     2663 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/services/data_service.py
--rw-r--r--   0        0        0     3098 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/services/influx_service.py
--rw-r--r--   0        0        0     4486 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/services/prediction_service.py
--rw-r--r--   0        0        0     1725 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/services/prometheus_service.py
--rw-r--r--   0        0        0    15611 2023-04-28 18:18:17.077437 estimenergy-2.0.5/estimenergy/services/sql_service.py
--rw-r--r--   0        0        0     2495 2023-04-28 18:19:08.425938 estimenergy-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     5876 1970-01-01 00:00:00.000000 estimenergy-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-28 18:46:02.102550 estimenergy-2.0.6/LICENSE
+-rw-r--r--   0        0        0     4481 2023-04-28 18:46:02.102550 estimenergy-2.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/__init__.py
+-rw-r--r--   0        0        0       38 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/client/__init__.py
+-rw-r--r--   0        0        0      639 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/client/client.py
+-rw-r--r--   0        0        0      451 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/config.py
+-rw-r--r--   0        0        0     6030 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/const.py
+-rw-r--r--   0        0        0      665 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/db.py
+-rw-r--r--   0        0        0      133 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/devices/__init__.py
+-rw-r--r--   0        0        0     3108 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/devices/base_device.py
+-rw-r--r--   0        0        0       99 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/devices/device_error.py
+-rw-r--r--   0        0        0     4048 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/devices/device_registry.py
+-rw-r--r--   0        0        0     6177 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/devices/glow_device.py
+-rw-r--r--   0        0        0      540 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/helpers.py
+-rw-r--r--   0        0        0      318 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/influx.py
+-rw-r--r--   0        0        0      613 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/log.py
+-rw-r--r--   0        0        0     2088 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/main.py
+-rw-r--r--   0        0        0       94 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/models/config/__init__.py
+-rw-r--r--   0        0        0     1500 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/models/config/config.py
+-rw-r--r--   0        0        0       86 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/models/config/dev_config.py
+-rw-r--r--   0        0        0      138 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/models/config/influx_config.py
+-rw-r--r--   0        0        0      208 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/models/config/logging_config.py
+-rw-r--r--   0        0        0      279 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/models/config/networking_config.py
+-rw-r--r--   0        0        0      186 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/models/config/sql_config.py
+-rw-r--r--   0        0        0      896 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/models/day.py
+-rw-r--r--   0        0        0      912 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/models/device_config.py
+-rw-r--r--   0        0        0       76 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/models/message.py
+-rw-r--r--   0        0        0      874 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/models/month.py
+-rw-r--r--   0        0        0      335 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/models/total.py
+-rw-r--r--   0        0        0      799 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/models/year.py
+-rw-r--r--   0        0        0      479 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/prometheus.py
+-rw-r--r--   0        0        0        0 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/routers/__init__.py
+-rw-r--r--   0        0        0     4261 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/routers/day_router.py
+-rw-r--r--   0        0        0     4293 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/routers/device_router.py
+-rw-r--r--   0        0        0     1466 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/routers/month_router.py
+-rw-r--r--   0        0        0     1466 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/routers/total_router.py
+-rw-r--r--   0        0        0     1436 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/routers/year_router.py
+-rw-r--r--   0        0        0        0 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/services/__init__.py
+-rw-r--r--   0        0        0     2663 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/services/data_service.py
+-rw-r--r--   0        0        0     3098 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/services/influx_service.py
+-rw-r--r--   0        0        0     4486 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/services/prediction_service.py
+-rw-r--r--   0        0        0     1725 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/services/prometheus_service.py
+-rw-r--r--   0        0        0    15611 2023-04-28 18:46:02.106550 estimenergy-2.0.6/estimenergy/services/sql_service.py
+-rw-r--r--   0        0        0     2495 2023-04-28 18:46:35.382316 estimenergy-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5876 1970-01-01 00:00:00.000000 estimenergy-2.0.6/PKG-INFO
```

### Comparing `estimenergy-2.0.5/LICENSE` & `estimenergy-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/README.md` & `estimenergy-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/client/client.py` & `estimenergy-2.0.6/estimenergy/client/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 class EstimEnergyClient:
     def __init__(self, host, port):
         self.host = host
         self.port = port
 
     def get_device(self, name: str):
-        url = f"http://{self.host}:{self.port}/device/{name}"
+        url = f"http://{self.host}:{self.port}/api/device/{name}"
         response = requests.get(url, timeout=5)
         return response.json()
 
     def get_devices(self):
-        url = f"http://{self.host}:{self.port}/device"
+        url = f"http://{self.host}:{self.port}/api/device"
         response = requests.get(url, timeout=5)
         return response.json()
 
     def get_metrics(self):
         url = f"http://{self.host}:{self.port}/metrics"
         response = requests.get(url, timeout=5)
         return response.text
```

### Comparing `estimenergy-2.0.5/estimenergy/const.py` & `estimenergy-2.0.6/estimenergy/const.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/db.py` & `estimenergy-2.0.6/estimenergy/db.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/devices/base_device.py` & `estimenergy-2.0.6/estimenergy/devices/base_device.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/devices/device_registry.py` & `estimenergy-2.0.6/estimenergy/devices/device_registry.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/devices/glow_device.py` & `estimenergy-2.0.6/estimenergy/devices/glow_device.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/helpers.py` & `estimenergy-2.0.6/estimenergy/helpers.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/log.py` & `estimenergy-2.0.6/estimenergy/log.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/main.py` & `estimenergy-2.0.6/estimenergy/main.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/models/config/config.py` & `estimenergy-2.0.6/estimenergy/models/config/config.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/models/day.py` & `estimenergy-2.0.6/estimenergy/models/day.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/models/device_config.py` & `estimenergy-2.0.6/estimenergy/models/device_config.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/models/month.py` & `estimenergy-2.0.6/estimenergy/models/month.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/models/year.py` & `estimenergy-2.0.6/estimenergy/models/year.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/routers/day_router.py` & `estimenergy-2.0.6/estimenergy/routers/day_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/routers/device_router.py` & `estimenergy-2.0.6/estimenergy/routers/device_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/routers/month_router.py` & `estimenergy-2.0.6/estimenergy/routers/month_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/routers/total_router.py` & `estimenergy-2.0.6/estimenergy/routers/total_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/routers/year_router.py` & `estimenergy-2.0.6/estimenergy/routers/year_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/services/data_service.py` & `estimenergy-2.0.6/estimenergy/services/data_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/services/influx_service.py` & `estimenergy-2.0.6/estimenergy/services/influx_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/services/prediction_service.py` & `estimenergy-2.0.6/estimenergy/services/prediction_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/services/prometheus_service.py` & `estimenergy-2.0.6/estimenergy/services/prometheus_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/estimenergy/services/sql_service.py` & `estimenergy-2.0.6/estimenergy/services/sql_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.5/pyproject.toml` & `estimenergy-2.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 name = "estimenergy"
 description = "Estimate Energy Consumption"
 authors = ["Lennard Beers <l.beers@outlook.de>"]
 repository = "https://github.com/EuleMitKeule/EstimEnergy"
 readme = "README.md"
 packages = [{include = "estimenergy"}]
 license = "MIT"
-version = "2.0.5"
+version = "2.0.6"
 
 [tool.poetry.scripts]
 api = "estimenergy.main:start"
 drop = "estimenergy.db:drop_db"
 generate-openapi = "estimenergy.main:generate_openapi"
 
 [tool.poe.tasks]
```

### Comparing `estimenergy-2.0.5/PKG-INFO` & `estimenergy-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estimenergy
-Version: 2.0.5
+Version: 2.0.6
 Summary: Estimate Energy Consumption
 Home-page: https://github.com/EuleMitKeule/EstimEnergy
 License: MIT
 Author: Lennard Beers
 Author-email: l.beers@outlook.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


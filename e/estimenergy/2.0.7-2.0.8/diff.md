# Comparing `tmp/estimenergy-2.0.7.tar.gz` & `tmp/estimenergy-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estimenergy-2.0.7.tar", max compression
+gzip compressed data, was "estimenergy-2.0.8.tar", max compression
```

## Comparing `estimenergy-2.0.7.tar` & `estimenergy-2.0.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1089 2023-04-29 00:55:26.552125 estimenergy-2.0.7/LICENSE
--rw-r--r--   0        0        0     4481 2023-04-29 00:55:26.552125 estimenergy-2.0.7/README.md
--rw-r--r--   0        0        0        0 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/__init__.py
--rw-r--r--   0        0        0       38 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/client/__init__.py
--rw-r--r--   0        0        0      639 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/client/client.py
--rw-r--r--   0        0        0      451 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/config.py
--rw-r--r--   0        0        0     6030 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/const.py
--rw-r--r--   0        0        0      665 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/db.py
--rw-r--r--   0        0        0      133 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/devices/__init__.py
--rw-r--r--   0        0        0     3140 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/devices/base_device.py
--rw-r--r--   0        0        0       99 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/devices/device_error.py
--rw-r--r--   0        0        0     4048 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/devices/device_registry.py
--rw-r--r--   0        0        0     6226 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/devices/glow_device.py
--rw-r--r--   0        0        0      540 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/helpers.py
--rw-r--r--   0        0        0      318 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/influx.py
--rw-r--r--   0        0        0      613 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/log.py
--rw-r--r--   0        0        0     2088 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/main.py
--rw-r--r--   0        0        0       94 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/models/config/__init__.py
--rw-r--r--   0        0        0     1500 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/models/config/config.py
--rw-r--r--   0        0        0       86 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/models/config/dev_config.py
--rw-r--r--   0        0        0      138 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/models/config/influx_config.py
--rw-r--r--   0        0        0      208 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/models/config/logging_config.py
--rw-r--r--   0        0        0      279 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/models/config/networking_config.py
--rw-r--r--   0        0        0      186 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/models/config/sql_config.py
--rw-r--r--   0        0        0      896 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/models/day.py
--rw-r--r--   0        0        0      912 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/models/device_config.py
--rw-r--r--   0        0        0       76 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/models/message.py
--rw-r--r--   0        0        0      874 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/models/month.py
--rw-r--r--   0        0        0      335 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/models/total.py
--rw-r--r--   0        0        0      799 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/models/year.py
--rw-r--r--   0        0        0      479 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/prometheus.py
--rw-r--r--   0        0        0        0 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/routers/__init__.py
--rw-r--r--   0        0        0     4261 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/routers/day_router.py
--rw-r--r--   0        0        0     4293 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/routers/device_router.py
--rw-r--r--   0        0        0     1466 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/routers/month_router.py
--rw-r--r--   0        0        0     1466 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/routers/total_router.py
--rw-r--r--   0        0        0     1436 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/routers/year_router.py
--rw-r--r--   0        0        0        0 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/services/__init__.py
--rw-r--r--   0        0        0     2663 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/services/data_service.py
--rw-r--r--   0        0        0     3098 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/services/influx_service.py
--rw-r--r--   0        0        0     4486 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/services/prediction_service.py
--rw-r--r--   0        0        0     1725 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/services/prometheus_service.py
--rw-r--r--   0        0        0    15611 2023-04-29 00:55:26.556125 estimenergy-2.0.7/estimenergy/services/sql_service.py
--rw-r--r--   0        0        0     2495 2023-04-29 00:56:01.667510 estimenergy-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     5876 1970-01-01 00:00:00.000000 estimenergy-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-29 01:08:25.902430 estimenergy-2.0.8/LICENSE
+-rw-r--r--   0        0        0     4481 2023-04-29 01:08:25.902430 estimenergy-2.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/__init__.py
+-rw-r--r--   0        0        0       38 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/client/__init__.py
+-rw-r--r--   0        0        0      639 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/client/client.py
+-rw-r--r--   0        0        0      451 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/config.py
+-rw-r--r--   0        0        0     6030 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/const.py
+-rw-r--r--   0        0        0      665 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/db.py
+-rw-r--r--   0        0        0      133 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/devices/__init__.py
+-rw-r--r--   0        0        0     3140 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/devices/base_device.py
+-rw-r--r--   0        0        0       99 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/devices/device_error.py
+-rw-r--r--   0        0        0     4048 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/devices/device_registry.py
+-rw-r--r--   0        0        0     6226 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/devices/glow_device.py
+-rw-r--r--   0        0        0      540 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/helpers.py
+-rw-r--r--   0        0        0      318 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/influx.py
+-rw-r--r--   0        0        0      613 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/log.py
+-rw-r--r--   0        0        0     2088 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/main.py
+-rw-r--r--   0        0        0       94 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/models/config/__init__.py
+-rw-r--r--   0        0        0     1500 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/models/config/config.py
+-rw-r--r--   0        0        0       86 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/models/config/dev_config.py
+-rw-r--r--   0        0        0      138 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/models/config/influx_config.py
+-rw-r--r--   0        0        0      208 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/models/config/logging_config.py
+-rw-r--r--   0        0        0      279 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/models/config/networking_config.py
+-rw-r--r--   0        0        0      186 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/models/config/sql_config.py
+-rw-r--r--   0        0        0      896 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/models/day.py
+-rw-r--r--   0        0        0      912 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/models/device_config.py
+-rw-r--r--   0        0        0       76 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/models/message.py
+-rw-r--r--   0        0        0      874 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/models/month.py
+-rw-r--r--   0        0        0      335 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/models/total.py
+-rw-r--r--   0        0        0      799 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/models/year.py
+-rw-r--r--   0        0        0      479 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/prometheus.py
+-rw-r--r--   0        0        0        0 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/routers/__init__.py
+-rw-r--r--   0        0        0     4261 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/routers/day_router.py
+-rw-r--r--   0        0        0     4293 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/routers/device_router.py
+-rw-r--r--   0        0        0     1466 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/routers/month_router.py
+-rw-r--r--   0        0        0     1466 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/routers/total_router.py
+-rw-r--r--   0        0        0     1436 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/routers/year_router.py
+-rw-r--r--   0        0        0        0 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/services/__init__.py
+-rw-r--r--   0        0        0     2663 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/services/data_service.py
+-rw-r--r--   0        0        0     3098 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/services/influx_service.py
+-rw-r--r--   0        0        0     4486 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/services/prediction_service.py
+-rw-r--r--   0        0        0     1725 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/services/prometheus_service.py
+-rw-r--r--   0        0        0    15611 2023-04-29 01:08:25.906430 estimenergy-2.0.8/estimenergy/services/sql_service.py
+-rw-r--r--   0        0        0     2495 2023-04-29 01:09:03.774546 estimenergy-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5876 1970-01-01 00:00:00.000000 estimenergy-2.0.8/PKG-INFO
```

### Comparing `estimenergy-2.0.7/LICENSE` & `estimenergy-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/README.md` & `estimenergy-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/client/client.py` & `estimenergy-2.0.8/estimenergy/client/client.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/const.py` & `estimenergy-2.0.8/estimenergy/const.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/db.py` & `estimenergy-2.0.8/estimenergy/db.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/devices/base_device.py` & `estimenergy-2.0.8/estimenergy/devices/base_device.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/devices/device_registry.py` & `estimenergy-2.0.8/estimenergy/devices/device_registry.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/devices/glow_device.py` & `estimenergy-2.0.8/estimenergy/devices/glow_device.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/helpers.py` & `estimenergy-2.0.8/estimenergy/helpers.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/log.py` & `estimenergy-2.0.8/estimenergy/log.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/main.py` & `estimenergy-2.0.8/estimenergy/main.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/models/config/config.py` & `estimenergy-2.0.8/estimenergy/models/config/config.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/models/day.py` & `estimenergy-2.0.8/estimenergy/models/day.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/models/device_config.py` & `estimenergy-2.0.8/estimenergy/models/device_config.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/models/month.py` & `estimenergy-2.0.8/estimenergy/models/month.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/models/year.py` & `estimenergy-2.0.8/estimenergy/models/year.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/routers/day_router.py` & `estimenergy-2.0.8/estimenergy/routers/day_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/routers/device_router.py` & `estimenergy-2.0.8/estimenergy/routers/device_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/routers/month_router.py` & `estimenergy-2.0.8/estimenergy/routers/month_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/routers/total_router.py` & `estimenergy-2.0.8/estimenergy/routers/total_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/routers/year_router.py` & `estimenergy-2.0.8/estimenergy/routers/year_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/services/data_service.py` & `estimenergy-2.0.8/estimenergy/services/data_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/services/influx_service.py` & `estimenergy-2.0.8/estimenergy/services/influx_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/services/prediction_service.py` & `estimenergy-2.0.8/estimenergy/services/prediction_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/services/prometheus_service.py` & `estimenergy-2.0.8/estimenergy/services/prometheus_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/estimenergy/services/sql_service.py` & `estimenergy-2.0.8/estimenergy/services/sql_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.7/pyproject.toml` & `estimenergy-2.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 name = "estimenergy"
 description = "Estimate Energy Consumption"
 authors = ["Lennard Beers <l.beers@outlook.de>"]
 repository = "https://github.com/EuleMitKeule/EstimEnergy"
 readme = "README.md"
 packages = [{include = "estimenergy"}]
 license = "MIT"
-version = "2.0.7"
+version = "2.0.8"
 
 [tool.poetry.scripts]
 api = "estimenergy.main:start"
 drop = "estimenergy.db:drop_db"
 generate-openapi = "estimenergy.main:generate_openapi"
 
 [tool.poe.tasks]
```

### Comparing `estimenergy-2.0.7/PKG-INFO` & `estimenergy-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estimenergy
-Version: 2.0.7
+Version: 2.0.8
 Summary: Estimate Energy Consumption
 Home-page: https://github.com/EuleMitKeule/EstimEnergy
 License: MIT
 Author: Lennard Beers
 Author-email: l.beers@outlook.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


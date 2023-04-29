# Comparing `tmp/citizenk-0.1.31.tar.gz` & `tmp/citizenk-0.1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.31.tar", max compression
+gzip compressed data, was "citizenk-0.1.32.tar", max compression
```

## Comparing `citizenk-0.1.31.tar` & `citizenk-0.1.32.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.31/citizenk/__init__.py
--rw-r--r--   0        0        0     3788 2023-04-04 18:14:45.297131 citizenk-0.1.31/citizenk/agent.py
--rw-r--r--   0        0        0    18684 2023-04-29 14:30:59.870468 citizenk-0.1.31/citizenk/citizenk.py
--rw-r--r--   0        0        0    20873 2023-04-29 14:46:47.292021 citizenk-0.1.31/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.31/citizenk/murmur2.py
--rw-r--r--   0        0        0     4827 2023-04-29 14:29:54.086213 citizenk-0.1.31/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.31/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-04-29 14:47:59.914650 citizenk-0.1.31/pyproject.toml
--rw-r--r--   0        0        0      863 2023-04-29 14:48:40.829802 citizenk-0.1.31/setup.py
--rw-r--r--   0        0        0     1076 2023-04-29 14:48:40.830072 citizenk-0.1.31/PKG-INFO
+-rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.32/citizenk/__init__.py
+-rw-r--r--   0        0        0     3788 2023-04-04 18:14:45.297131 citizenk-0.1.32/citizenk/agent.py
+-rw-r--r--   0        0        0    18684 2023-04-29 14:30:59.870468 citizenk-0.1.32/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20883 2023-04-29 15:17:52.325175 citizenk-0.1.32/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.32/citizenk/murmur2.py
+-rw-r--r--   0        0        0     4827 2023-04-29 14:29:54.086213 citizenk-0.1.32/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.32/citizenk/utils.py
+-rw-r--r--   0        0        0     1521 2023-04-29 15:19:32.816599 citizenk-0.1.32/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-04-29 15:19:36.657357 citizenk-0.1.32/setup.py
+-rw-r--r--   0        0        0     1076 2023-04-29 15:19:36.657640 citizenk-0.1.32/PKG-INFO
```

### Comparing `citizenk-0.1.31/citizenk/agent.py` & `citizenk-0.1.32/citizenk/agent.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.31/citizenk/citizenk.py` & `citizenk-0.1.32/citizenk/citizenk.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.31/citizenk/kafka_adapter.py` & `citizenk-0.1.32/citizenk/kafka_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,14 @@
             self.config = {
                 "sasl.mechanism": self.sasl_mechanism,
                 "security.protocol": "SASL_SSL" if config.tls else "SASL_PLAINTEXT",
                 "ssl.ca.location": certifi.where(),
                 "sasl.username": config.sasl_username,
                 "sasl.password": config.sasl_password,
                 "statistics.interval.ms": 15 * 60 * 1000,
-                "partitioner":"murmur2",
                 "error_cb": self._on_kafka_error,
                 "stats_cb": self._on_kafka_stats,
             }
         else:
             raise ValueError("Unsupported sasl_mechanism")
         self.config["bootstrap.servers"] = config.bootstrap_servers
         if config.extra_config is not None:
@@ -97,14 +96,15 @@
                 self.config["enable.auto.commit"] = True
             else:
                 logger.info("Starting consumer without a consumer group")
                 self.config["enable.auto.commit"] = False
                 self.config["group.id"] = "dummy_shouldnt_be_used"
             self.connection = Consumer(self.config)
         elif self.role == KafkaRole.PRODUCER:
+            self.config["partitioner"] = "murmur2"
             self.connection = Producer(self.config)
         else:
             self.connection = AdminClient(self.admin_config)
         metadata = self.connection.list_topics(timeout=10)
         logger.debug("Connected to %s cluster %s", self.role.name, metadata.cluster_id)
 
     def get_all_broker_groups(self) -> List[str]:
```

### Comparing `citizenk-0.1.31/citizenk/murmur2.py` & `citizenk-0.1.32/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.31/citizenk/topic.py` & `citizenk-0.1.32/citizenk/topic.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.31/pyproject.toml` & `citizenk-0.1.32/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.31"
+version = "0.1.32"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
```

### Comparing `citizenk-0.1.31/setup.py` & `citizenk-0.1.32/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.31',
+    'version': '0.1.32',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.31/PKG-INFO` & `citizenk-0.1.32/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.31
+Version: 0.1.32
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```


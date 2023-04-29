# Comparing `tmp/citizenk-0.1.27.tar.gz` & `tmp/citizenk-0.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.27.tar", max compression
+gzip compressed data, was "citizenk-0.1.28.tar", max compression
```

## Comparing `citizenk-0.1.27.tar` & `citizenk-0.1.28.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.27/citizenk/__init__.py
--rw-r--r--   0        0        0     3788 2023-04-04 18:14:45.297131 citizenk-0.1.27/citizenk/agent.py
--rw-r--r--   0        0        0    18378 2023-04-28 17:58:21.332128 citizenk-0.1.27/citizenk/citizenk.py
--rw-r--r--   0        0        0    20783 2023-04-29 08:56:29.722594 citizenk-0.1.27/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.27/citizenk/murmur2.py
--rw-r--r--   0        0        0     4802 2023-04-04 18:14:45.297629 citizenk-0.1.27/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.27/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-04-29 08:56:51.536341 citizenk-0.1.27/pyproject.toml
--rw-r--r--   0        0        0      863 2023-04-29 08:56:56.145997 citizenk-0.1.27/setup.py
--rw-r--r--   0        0        0     1076 2023-04-29 08:56:56.146273 citizenk-0.1.27/PKG-INFO
+-rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.28/citizenk/__init__.py
+-rw-r--r--   0        0        0     3788 2023-04-04 18:14:45.297131 citizenk-0.1.28/citizenk/agent.py
+-rw-r--r--   0        0        0    18378 2023-04-28 17:58:21.332128 citizenk-0.1.28/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20832 2023-04-29 09:40:27.145100 citizenk-0.1.28/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.28/citizenk/murmur2.py
+-rw-r--r--   0        0        0     4802 2023-04-04 18:14:45.297629 citizenk-0.1.28/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.28/citizenk/utils.py
+-rw-r--r--   0        0        0     1521 2023-04-29 09:42:04.999892 citizenk-0.1.28/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-04-29 09:42:10.264538 citizenk-0.1.28/setup.py
+-rw-r--r--   0        0        0     1076 2023-04-29 09:42:10.264798 citizenk-0.1.28/PKG-INFO
```

### Comparing `citizenk-0.1.27/citizenk/agent.py` & `citizenk-0.1.28/citizenk/agent.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.27/citizenk/citizenk.py` & `citizenk-0.1.28/citizenk/citizenk.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.27/citizenk/kafka_adapter.py` & `citizenk-0.1.28/citizenk/kafka_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
             except KafkaException:
                 logger.error("Error while describing group")
         return members
 
     def get_partition_id(self, topic: str, key: Union[str, bytes]) -> int:
         if isinstance(key, str):
-            key = key.encode("utf-8")
+            key = key.encode()
         num_partitions = self.get_partition_count(topic)
         if num_partitions == 0:
             return None
         return murmur2_partition(key, num_partitions)
 
     def get_partition_count(self, topic) -> int:
         """Get list of all topics in the broker"""
@@ -439,15 +439,15 @@
         logger.debug("Finished setting up consumer, and starting consuming")
 
     @staticmethod
     def stringify_key(key):
         if key is None or isinstance(key,str):
             return key
         elif isinstance(key,bytes):
-            return key.decode("utf-8")
+            return key.decode()
         else:
             logger.error("Unexpected key type %s",type(key))
             return str(key)
 
     @staticmethod
     def messages_to_dict(messages: List[Message]) -> List[Dict[str, Any]]:
         try:
@@ -484,14 +484,16 @@
         self,
         topic: str,
         value: Any,
         key: Optional[Any] = None,
         partition: int = -1,
         headers: Optional[Dict[str, bytes]] = None,
     ):
+        if isinstance(key,str):
+            key = key.encode()
         """Produce a message to the given topic"""
         self.topic_stats[topic] += 1
         self.connection.produce(
             topic, value=value, key=key, partition=partition, headers=headers
         )
 
     def _on_kafka_commit(self, err: KafkaError, partitions: List[TopicPartition]):
```

### Comparing `citizenk-0.1.27/citizenk/murmur2.py` & `citizenk-0.1.28/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.27/citizenk/topic.py` & `citizenk-0.1.28/citizenk/topic.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.27/pyproject.toml` & `citizenk-0.1.28/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.27"
+version = "0.1.28"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
```

### Comparing `citizenk-0.1.27/setup.py` & `citizenk-0.1.28/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.27',
+    'version': '0.1.28',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.27/PKG-INFO` & `citizenk-0.1.28/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.27
+Version: 0.1.28
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```


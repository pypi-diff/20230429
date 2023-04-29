# Comparing `tmp/citizenk-0.1.25.tar.gz` & `tmp/citizenk-0.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.25.tar", max compression
+gzip compressed data, was "citizenk-0.1.26.tar", max compression
```

## Comparing `citizenk-0.1.25.tar` & `citizenk-0.1.26.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.25/citizenk/__init__.py
--rw-r--r--   0        0        0     3788 2023-04-04 18:14:45.297131 citizenk-0.1.25/citizenk/agent.py
--rw-r--r--   0        0        0    18378 2023-04-28 17:58:21.332128 citizenk-0.1.25/citizenk/citizenk.py
--rw-r--r--   0        0        0    20636 2023-04-29 08:35:03.908895 citizenk-0.1.25/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.25/citizenk/murmur2.py
--rw-r--r--   0        0        0     4802 2023-04-04 18:14:45.297629 citizenk-0.1.25/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.25/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-04-29 08:35:28.678222 citizenk-0.1.25/pyproject.toml
--rw-r--r--   0        0        0      863 2023-04-29 08:35:34.507911 citizenk-0.1.25/setup.py
--rw-r--r--   0        0        0     1076 2023-04-29 08:35:34.508169 citizenk-0.1.25/PKG-INFO
+-rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.26/citizenk/__init__.py
+-rw-r--r--   0        0        0     3788 2023-04-04 18:14:45.297131 citizenk-0.1.26/citizenk/agent.py
+-rw-r--r--   0        0        0    18378 2023-04-28 17:58:21.332128 citizenk-0.1.26/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20642 2023-04-29 08:43:05.120684 citizenk-0.1.26/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.26/citizenk/murmur2.py
+-rw-r--r--   0        0        0     4802 2023-04-04 18:14:45.297629 citizenk-0.1.26/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.26/citizenk/utils.py
+-rw-r--r--   0        0        0     1521 2023-04-29 08:43:28.424090 citizenk-0.1.26/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-04-29 08:43:35.037829 citizenk-0.1.26/setup.py
+-rw-r--r--   0        0        0     1076 2023-04-29 08:43:35.038087 citizenk-0.1.26/PKG-INFO
```

### Comparing `citizenk-0.1.25/citizenk/agent.py` & `citizenk-0.1.26/citizenk/agent.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.25/citizenk/citizenk.py` & `citizenk-0.1.26/citizenk/citizenk.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.25/citizenk/kafka_adapter.py` & `citizenk-0.1.26/citizenk/kafka_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,15 +436,15 @@
                 self.connection.assign(source_partitions)
         self.consumer_topics = topics
         self.consumer_started = True
         logger.debug("Finished setting up consumer, and starting consuming")
 
     @staticmethod
     def stringify_key(key):
-        if key is None or type(key,str):
+        if key is None or isinstance(key,str):
             return key
         return key().decode("utf-8")
 
     @staticmethod
     def messages_to_dict(messages: List[Message]) -> List[Dict[str, Any]]:
         try:
             return [
```

### Comparing `citizenk-0.1.25/citizenk/murmur2.py` & `citizenk-0.1.26/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.25/citizenk/topic.py` & `citizenk-0.1.26/citizenk/topic.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.25/pyproject.toml` & `citizenk-0.1.26/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.25"
+version = "0.1.26"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
```

### Comparing `citizenk-0.1.25/setup.py` & `citizenk-0.1.26/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.25',
+    'version': '0.1.26',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.25/PKG-INFO` & `citizenk-0.1.26/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.25
+Version: 0.1.26
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```


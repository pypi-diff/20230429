# Comparing `tmp/citizenk-0.1.26.tar.gz` & `tmp/citizenk-0.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.26.tar", max compression
+gzip compressed data, was "citizenk-0.1.27.tar", max compression
```

## Comparing `citizenk-0.1.26.tar` & `citizenk-0.1.27.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.26/citizenk/__init__.py
--rw-r--r--   0        0        0     3788 2023-04-04 18:14:45.297131 citizenk-0.1.26/citizenk/agent.py
--rw-r--r--   0        0        0    18378 2023-04-28 17:58:21.332128 citizenk-0.1.26/citizenk/citizenk.py
--rw-r--r--   0        0        0    20642 2023-04-29 08:43:05.120684 citizenk-0.1.26/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.26/citizenk/murmur2.py
--rw-r--r--   0        0        0     4802 2023-04-04 18:14:45.297629 citizenk-0.1.26/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.26/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-04-29 08:43:28.424090 citizenk-0.1.26/pyproject.toml
--rw-r--r--   0        0        0      863 2023-04-29 08:43:35.037829 citizenk-0.1.26/setup.py
--rw-r--r--   0        0        0     1076 2023-04-29 08:43:35.038087 citizenk-0.1.26/PKG-INFO
+-rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.27/citizenk/__init__.py
+-rw-r--r--   0        0        0     3788 2023-04-04 18:14:45.297131 citizenk-0.1.27/citizenk/agent.py
+-rw-r--r--   0        0        0    18378 2023-04-28 17:58:21.332128 citizenk-0.1.27/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20783 2023-04-29 08:56:29.722594 citizenk-0.1.27/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.27/citizenk/murmur2.py
+-rw-r--r--   0        0        0     4802 2023-04-04 18:14:45.297629 citizenk-0.1.27/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.27/citizenk/utils.py
+-rw-r--r--   0        0        0     1521 2023-04-29 08:56:51.536341 citizenk-0.1.27/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-04-29 08:56:56.145997 citizenk-0.1.27/setup.py
+-rw-r--r--   0        0        0     1076 2023-04-29 08:56:56.146273 citizenk-0.1.27/PKG-INFO
```

### Comparing `citizenk-0.1.26/citizenk/agent.py` & `citizenk-0.1.27/citizenk/agent.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.26/citizenk/citizenk.py` & `citizenk-0.1.27/citizenk/citizenk.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.26/citizenk/kafka_adapter.py` & `citizenk-0.1.27/citizenk/kafka_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -438,15 +438,19 @@
         self.consumer_started = True
         logger.debug("Finished setting up consumer, and starting consuming")
 
     @staticmethod
     def stringify_key(key):
         if key is None or isinstance(key,str):
             return key
-        return key().decode("utf-8")
+        elif isinstance(key,bytes):
+            return key.decode("utf-8")
+        else:
+            logger.error("Unexpected key type %s",type(key))
+            return str(key)
 
     @staticmethod
     def messages_to_dict(messages: List[Message]) -> List[Dict[str, Any]]:
         try:
             return [
                 {
                     "topic": m.topic(),
```

### Comparing `citizenk-0.1.26/citizenk/murmur2.py` & `citizenk-0.1.27/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.26/citizenk/topic.py` & `citizenk-0.1.27/citizenk/topic.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.26/pyproject.toml` & `citizenk-0.1.27/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.26"
+version = "0.1.27"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
```

### Comparing `citizenk-0.1.26/setup.py` & `citizenk-0.1.27/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.26',
+    'version': '0.1.27',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.26/PKG-INFO` & `citizenk-0.1.27/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.26
+Version: 0.1.27
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```


# Comparing `tmp/citizenk-0.1.29.tar.gz` & `tmp/citizenk-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.29.tar", max compression
+gzip compressed data, was "citizenk-0.1.30.tar", max compression
```

## Comparing `citizenk-0.1.29.tar` & `citizenk-0.1.30.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.29/citizenk/__init__.py
--rw-r--r--   0        0        0     3788 2023-04-04 18:14:45.297131 citizenk-0.1.29/citizenk/agent.py
--rw-r--r--   0        0        0    18676 2023-04-29 10:36:35.317877 citizenk-0.1.29/citizenk/citizenk.py
--rw-r--r--   0        0        0    20832 2023-04-29 09:40:27.145100 citizenk-0.1.29/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.29/citizenk/murmur2.py
--rw-r--r--   0        0        0     4802 2023-04-04 18:14:45.297629 citizenk-0.1.29/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.29/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-04-29 10:37:50.419716 citizenk-0.1.29/pyproject.toml
--rw-r--r--   0        0        0      863 2023-04-29 10:37:54.699629 citizenk-0.1.29/setup.py
--rw-r--r--   0        0        0     1076 2023-04-29 10:37:54.699903 citizenk-0.1.29/PKG-INFO
+-rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.30/citizenk/__init__.py
+-rw-r--r--   0        0        0     3788 2023-04-04 18:14:45.297131 citizenk-0.1.30/citizenk/agent.py
+-rw-r--r--   0        0        0    18684 2023-04-29 14:30:59.870468 citizenk-0.1.30/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20832 2023-04-29 09:40:27.145100 citizenk-0.1.30/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.30/citizenk/murmur2.py
+-rw-r--r--   0        0        0     4827 2023-04-29 14:29:54.086213 citizenk-0.1.30/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.30/citizenk/utils.py
+-rw-r--r--   0        0        0     1521 2023-04-29 14:31:52.550934 citizenk-0.1.30/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-04-29 14:31:54.644371 citizenk-0.1.30/setup.py
+-rw-r--r--   0        0        0     1076 2023-04-29 14:31:54.644628 citizenk-0.1.30/PKG-INFO
```

### Comparing `citizenk-0.1.29/citizenk/agent.py` & `citizenk-0.1.30/citizenk/agent.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.29/citizenk/citizenk.py` & `citizenk-0.1.30/citizenk/citizenk.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,16 +300,16 @@
                 await asyncio.sleep(3)
 
     def topic(
             self,
             name: str,
             value_type: BaseModel,
             topic_dir: TopicDir = TopicDir.INPUT,
-            subject_name: str | None = None,
-            partitioner: Callable[[str | bytes], int] = None) -> Topic:
+            subject_name: Optional[str] = None,
+            partitioner: Callable[[Union[str,bytes]], int] = None) -> Topic:
         if name in self.topics:
             raise CitizenKError(f"Topic {name} already exists")
         t = Topic(
             self,
             name=name,
             value_type=value_type,
             topic_dir=topic_dir,
```

### Comparing `citizenk-0.1.29/citizenk/kafka_adapter.py` & `citizenk-0.1.30/citizenk/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.29/citizenk/murmur2.py` & `citizenk-0.1.30/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.29/citizenk/topic.py` & `citizenk-0.1.30/citizenk/topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Callable
+from typing import TYPE_CHECKING, Any, Callable, Optional, Union
 
 from confluent_kafka.schema_registry import Schema, SchemaRegistryClient
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel, ValidationError
 
 from .utils import CitizenKError, annotate_function
 
@@ -31,16 +31,16 @@
 class Topic:
     def __init__(
         self,
         app: CitizenK,
         name: str,
         value_type: BaseModel,
         topic_dir: TopicDir = TopicDir.INPUT,
-        subject_name: str | None = None,
-        partitioner: Callable[[str | bytes], int] = None,
+        subject_name: Optional[str] = None,
+        partitioner: Callable[[Union[str,bytes]], int] = None,
     ):
         self.app = app
         self.name = name
         self.value_type = value_type
         self.topic_dir = topic_dir
         self.subject_name = (
             f"{name}-value".lower() if subject_name is None else subject_name
```

### Comparing `citizenk-0.1.29/pyproject.toml` & `citizenk-0.1.30/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.29"
+version = "0.1.30"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
```

### Comparing `citizenk-0.1.29/setup.py` & `citizenk-0.1.30/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.29',
+    'version': '0.1.30',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.29/PKG-INFO` & `citizenk-0.1.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.29
+Version: 0.1.30
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```


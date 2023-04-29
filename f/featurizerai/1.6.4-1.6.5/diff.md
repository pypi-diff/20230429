# Comparing `tmp/featurizerai-1.6.4.tar.gz` & `tmp/featurizerai-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.6.4.tar", last modified: Fri Apr 28 23:48:29 2023, max compression
+gzip compressed data, was "featurizerai-1.6.5.tar", last modified: Sat Apr 29 16:05:19 2023, max compression
```

## Comparing `featurizerai-1.6.4.tar` & `featurizerai-1.6.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:48:29.633388 featurizerai-1.6.4/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.6.4/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.6.4/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 23:48:29.633459 featurizerai-1.6.4/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.6.4/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 23:48:29.633673 featurizerai-1.6.4/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 23:47:58.000000 featurizerai-1.6.4/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:48:29.629473 featurizerai-1.6.4/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:48:29.631573 featurizerai-1.6.4/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.6.4/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.6.4/src/features/authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.6.4/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.6.4/src/features/custom_schema.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4872 2023-04-28 23:48:14.000000 featurizerai-1.6.4/src/features/materialize.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:48:29.632353 featurizerai-1.6.4/src/features/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.6.4/src/features/tests/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     2766 2023-04-28 14:47:29.000000 featurizerai-1.6.4/src/features/tests/test_materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.6.4/src/features/tests/test_pipeline.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 23:48:29.633275 featurizerai-1.6.4/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 23:48:29.000000 featurizerai-1.6.4/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 23:48:29.000000 featurizerai-1.6.4/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 23:48:29.000000 featurizerai-1.6.4/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 23:48:29.000000 featurizerai-1.6.4/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 23:48:29.000000 featurizerai-1.6.4/src/featurizerai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 16:05:19.911069 featurizerai-1.6.5/
+-rw-rw-rw-   0        0        0     1100 2023-04-29 00:34:12.000000 featurizerai-1.6.5/LICENSE
+-rw-rw-rw-   0        0        0       89 2023-04-29 00:34:12.000000 featurizerai-1.6.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      879 2023-04-29 16:05:19.911069 featurizerai-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-04-29 00:34:12.000000 featurizerai-1.6.5/pyproject.toml
+-rw-rw-rw-   0        0        0      123 2023-04-29 16:05:19.911069 featurizerai-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1378 2023-04-29 16:03:47.000000 featurizerai-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:05:19.864246 featurizerai-1.6.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 16:05:19.879801 featurizerai-1.6.5/src/features/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:34:12.000000 featurizerai-1.6.5/src/features/__init__.py
+-rw-rw-rw-   0        0        0      704 2023-04-29 00:34:12.000000 featurizerai-1.6.5/src/features/authenticate.py
+-rw-rw-rw-   0        0        0     4329 2023-04-29 00:34:12.000000 featurizerai-1.6.5/src/features/create_stream.py
+-rw-rw-rw-   0        0        0      870 2023-04-29 00:34:12.000000 featurizerai-1.6.5/src/features/custom_schema.py
+-rw-rw-rw-   0        0        0     4865 2023-04-29 16:03:39.000000 featurizerai-1.6.5/src/features/materialize.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:05:19.895520 featurizerai-1.6.5/src/features/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:34:12.000000 featurizerai-1.6.5/src/features/tests/__init__.py
+-rw-rw-rw-   0        0        0     2817 2023-04-29 00:34:12.000000 featurizerai-1.6.5/src/features/tests/test_materialize.py
+-rw-rw-rw-   0        0        0     1563 2023-04-29 00:34:12.000000 featurizerai-1.6.5/src/features/tests/test_pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:05:19.911069 featurizerai-1.6.5/src/featurizerai.egg-info/
+-rw-rw-rw-   0        0        0      879 2023-04-29 16:05:19.000000 featurizerai-1.6.5/src/featurizerai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-04-29 16:05:19.000000 featurizerai-1.6.5/src/featurizerai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 16:05:19.000000 featurizerai-1.6.5/src/featurizerai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-29 16:05:19.000000 featurizerai-1.6.5/src/featurizerai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-29 16:05:19.000000 featurizerai-1.6.5/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.6.4/LICENSE` & `featurizerai-1.6.5/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Tom Chen (tomchen.org)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Tom Chen (tomchen.org)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `featurizerai-1.6.4/PKG-INFO` & `featurizerai-1.6.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1
-Name: featurizerai
-Version: 1.6.4
-Summary: Python library for Featurizer AI
-Home-page: https://github.com/burakglobal/featurizerai
-Author: Burak
-Author-email: burakgblobal@gmail.com
-Keywords: featurizer,package
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Provides-Extra: dev
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: featurizerai
+Version: 1.6.5
+Summary: Python library for Featurizer AI
+Home-page: https://github.com/burakglobal/featurizerai
+Author: Burak
+Author-email: burakgblobal@gmail.com
+Keywords: featurizer,package
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Provides-Extra: dev
+License-File: LICENSE
```

### Comparing `featurizerai-1.6.4/setup.py` & `featurizerai-1.6.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.6.4',
+    version='1.6.5',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.6.4/src/features/authenticate.py` & `featurizerai-1.6.5/src/features/authenticate.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import requests
-import base64
-
-class authenticate:
-    def __init__(self, base_url = 'http://0.0.0.0:4000'):
-        self.base_url = base_url
-
-    def authenticate(self, username, password):
-        url = f'{self.base_url}/authenticate'
-        credentials = f'{username}:{password}'.encode('ascii')
-        encoded_credentials = base64.b64encode(credentials).decode('ascii')
-        headers = {'Authorization': f'Basic {encoded_credentials}'}
-        response = requests.post(url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            return data.get('access_token'), data.get('token_type')
-        else:
-            return None, None
+import requests
+import base64
+
+class authenticate:
+    def __init__(self, base_url = 'http://0.0.0.0:4000'):
+        self.base_url = base_url
+
+    def authenticate(self, username, password):
+        url = f'{self.base_url}/authenticate'
+        credentials = f'{username}:{password}'.encode('ascii')
+        encoded_credentials = base64.b64encode(credentials).decode('ascii')
+        headers = {'Authorization': f'Basic {encoded_credentials}'}
+        response = requests.post(url, headers=headers)
+        if response.status_code == 200:
+            data = response.json()
+            return data.get('access_token'), data.get('token_type')
+        else:
+            return None, None
```

### Comparing `featurizerai-1.6.4/src/features/create_stream.py` & `featurizerai-1.6.5/src/features/create_stream.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import json
-import ast
-import logging
-from datetime import datetime
-from http.client import HTTPException
-
-from pymongo import MongoClient
-from pymongo.server_api import ServerApi
-from confluent_kafka import Consumer, KafkaError
-import certifi
-import os
-import threading
-import jwt
-
-class create_stream:
-    def __init__(self, kafka_connection, mongo_connection=None, topicname="", timestamp_attr="timestamp"):
-        self.topicname = topicname
-        self.kafka_connection = kafka_connection
-        self.mongo_connection = mongo_connection
-        self.timestamp_attr = timestamp_attr
-        self._stop_event = threading.Event()
-
-    def is_epoch(self, timestamp):
-        try:
-            datetime.fromtimestamp(int(timestamp))
-            return True
-        except ValueError:
-            return False
-
-    def _run(self, token):
-        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
-        mongo_db = mongo_client[self.mongo_connection['database']]
-        raw_data_collection = mongo_db[self.mongo_connection['rawdata']]
-
-        consumer = Consumer(self.kafka_connection)
-        print(self.topicname)
-        consumer.subscribe([self.topicname])
-
-        while not self._stop_event.is_set():
-            msg = consumer.poll(10.0)
-            print("Poll executed")
-            print(msg)
-            if msg is None:
-                continue
-            if msg.error():
-                print("Consumer error: {}".format(msg.error()))
-            else:
-                message_value = ast.literal_eval(msg.value().decode("utf-8"))
-                print(message_value)
-
-                # New lines added for validation
-                if self.timestamp_attr not in message_value:
-                    print(
-                        f"Error: Message does not contain the required timestamp attribute '{self.timestamp_attr}'. Skipping message.")
-                    continue
-
-                if self.is_epoch(message_value.get(self.timestamp_attr)):
-                    if self.is_epoch(message_value.get(self.timestamp_attr)):
-                        message_value[self.timestamp_attr] = int(message_value[self.timestamp_attr])
-                    else:
-                        message_value[self.timestamp_attr] = datetime.now().timestamp()
-
-                raw_data_collection.insert_one(message_value)
-                print("Message received: {}".format(message_value))
-        consumer.close()
-
-    def start(self, token):
-        # authenicate token
-        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
-        mongo_db = mongo_client[self.mongo_connection['database']]
-        mongo_db_featurizer = mongo_client['featurizer']
-        users_collection = mongo_db_featurizer["users"]
-        SECRET_KEY = "features"  # Change this to your desired secret key
-        TOKEN_EXPIRATION = 3600  # Token expiration in seconds (1 hour)
-
-        try:
-            payload = jwt.decode(token, SECRET_KEY, algorithms=["HS256"])
-            user_id: str = payload.get("user_id")
-            if user_id is None:
-                print("User not found")
-                return ("Invalid token")
-            print(user_id)
-            user = users_collection.find_one({"userid": user_id})
-            if user is None:
-                print("User not found")
-                return ("Invalid token")
-        except Exception as e:
-            print(e)
-            return ("Invalid token")
-
-
-        if not hasattr(self, '_consumer_thread') or not self._consumer_thread.is_alive():
-            self._stop_event.clear()
-            self._consumer_thread = threading.Thread(target=self._run(self))
-            self._consumer_thread.start()
-            print('featurizerai: Started consumer thread.')
-        else:
-            print("Thread is already running. Cannot start it again.")
-
-    def stop(self):
-        if hasattr(self, '_consumer_thread') and self._consumer_thread.is_alive():
-            self._stop_event.set()
-            self._consumer_thread.join()
-            print('featurizerai: Stopped consumer thread.')
-        else:
-            print("Thread is not running. Cannot stop it.")
+import json
+import ast
+import logging
+from datetime import datetime
+from http.client import HTTPException
+
+from pymongo import MongoClient
+from pymongo.server_api import ServerApi
+from confluent_kafka import Consumer, KafkaError
+import certifi
+import os
+import threading
+import jwt
+
+class create_stream:
+    def __init__(self, kafka_connection, mongo_connection=None, topicname="", timestamp_attr="timestamp"):
+        self.topicname = topicname
+        self.kafka_connection = kafka_connection
+        self.mongo_connection = mongo_connection
+        self.timestamp_attr = timestamp_attr
+        self._stop_event = threading.Event()
+
+    def is_epoch(self, timestamp):
+        try:
+            datetime.fromtimestamp(int(timestamp))
+            return True
+        except ValueError:
+            return False
+
+    def _run(self, token):
+        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
+        mongo_db = mongo_client[self.mongo_connection['database']]
+        raw_data_collection = mongo_db[self.mongo_connection['rawdata']]
+
+        consumer = Consumer(self.kafka_connection)
+        print(self.topicname)
+        consumer.subscribe([self.topicname])
+
+        while not self._stop_event.is_set():
+            msg = consumer.poll(10.0)
+            print("Poll executed")
+            print(msg)
+            if msg is None:
+                continue
+            if msg.error():
+                print("Consumer error: {}".format(msg.error()))
+            else:
+                message_value = ast.literal_eval(msg.value().decode("utf-8"))
+                print(message_value)
+
+                # New lines added for validation
+                if self.timestamp_attr not in message_value:
+                    print(
+                        f"Error: Message does not contain the required timestamp attribute '{self.timestamp_attr}'. Skipping message.")
+                    continue
+
+                if self.is_epoch(message_value.get(self.timestamp_attr)):
+                    if self.is_epoch(message_value.get(self.timestamp_attr)):
+                        message_value[self.timestamp_attr] = int(message_value[self.timestamp_attr])
+                    else:
+                        message_value[self.timestamp_attr] = datetime.now().timestamp()
+
+                raw_data_collection.insert_one(message_value)
+                print("Message received: {}".format(message_value))
+        consumer.close()
+
+    def start(self, token):
+        # authenicate token
+        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
+        mongo_db = mongo_client[self.mongo_connection['database']]
+        mongo_db_featurizer = mongo_client['featurizer']
+        users_collection = mongo_db_featurizer["users"]
+        SECRET_KEY = "features"  # Change this to your desired secret key
+        TOKEN_EXPIRATION = 3600  # Token expiration in seconds (1 hour)
+
+        try:
+            payload = jwt.decode(token, SECRET_KEY, algorithms=["HS256"])
+            user_id: str = payload.get("user_id")
+            if user_id is None:
+                print("User not found")
+                return ("Invalid token")
+            print(user_id)
+            user = users_collection.find_one({"userid": user_id})
+            if user is None:
+                print("User not found")
+                return ("Invalid token")
+        except Exception as e:
+            print(e)
+            return ("Invalid token")
+
+
+        if not hasattr(self, '_consumer_thread') or not self._consumer_thread.is_alive():
+            self._stop_event.clear()
+            self._consumer_thread = threading.Thread(target=self._run(self))
+            self._consumer_thread.start()
+            print('featurizerai: Started consumer thread.')
+        else:
+            print("Thread is already running. Cannot start it again.")
+
+    def stop(self):
+        if hasattr(self, '_consumer_thread') and self._consumer_thread.is_alive():
+            self._stop_event.set()
+            self._consumer_thread.join()
+            print('featurizerai: Stopped consumer thread.')
+        else:
+            print("Thread is not running. Cannot stop it.")
```

### Comparing `featurizerai-1.6.4/src/features/custom_schema.py` & `featurizerai-1.6.5/src/features/custom_schema.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from pyspark.sql.types import IntegerType, StringType, StructField, StructType
-class custom_schema:
-    def __init__(self, schema_fields):
-        self.schema = self.generate_schema(schema_fields)
-
-    def generate_schema(self, schema_fields):
-        struct_fields = []
-
-        type_mapping = {
-            "integer": IntegerType,
-            "string": StringType
-        }
-
-        for field in schema_fields:
-            field_name = field.get("name")
-            field_type = field.get("type")
-            field_nullable = field.get("nullable", True)
-
-            if field_name and field_type in type_mapping:
-                struct_field = StructField(
-                    field_name, type_mapping[field_type](), field_nullable
-                )
-                struct_fields.append(struct_field)
-
-        return StructType(struct_fields)
+from pyspark.sql.types import IntegerType, StringType, StructField, StructType
+class custom_schema:
+    def __init__(self, schema_fields):
+        self.schema = self.generate_schema(schema_fields)
+
+    def generate_schema(self, schema_fields):
+        struct_fields = []
+
+        type_mapping = {
+            "integer": IntegerType,
+            "string": StringType
+        }
+
+        for field in schema_fields:
+            field_name = field.get("name")
+            field_type = field.get("type")
+            field_nullable = field.get("nullable", True)
+
+            if field_name and field_type in type_mapping:
+                struct_field = StructField(
+                    field_name, type_mapping[field_type](), field_nullable
+                )
+                struct_fields.append(struct_field)
+
+        return StructType(struct_fields)
```

### Comparing `featurizerai-1.6.4/src/features/materialize.py` & `featurizerai-1.6.5/src/features/materialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.groupby_attr = groupby_attr
         self.token = token
         self.schema = schema
         self.sparksql = sparksql
         self.partition_column = partition_column
 
         self.spark = SparkSession.builder \
-            .appName("IncrementalAggregation") \
+            .appName("Aggregation") \
             .master("local[*]") \
             .getOrCreate()
         self.spark.sparkContext.setLogLevel("ERROR")
 
     def read_data_and_aggregate(self):
 
 
@@ -61,16 +61,16 @@
         raw_data = raw_data_collection.find()
         raw_data_list = [doc for doc in raw_data]
         df = self.spark.createDataFrame(raw_data_list, self.schema)
 
         # Apply partitioning if the partition_column is specified
         if self.partition_column:
             print("Partitioning the DataFrame based on the column: " + self.partition_column)
-            raw_data_collection.create_index(self.partition_column)
-            raw_data_collection.create_index(self.groupby_attr)
+            # raw_data_collection.create_index(self.partition_column)
+            # raw_data_collection.create_index(self.groupby_attr)
             df = df.repartition(col(self.partition_column))
 
         # Filter the DataFrame based on the given device_id
         df = df.filter(col(self.groupby_attr) == self.groupby)
         start_time = self.aggregation_date
         df = df.filter((col(self.groupby_attr) == self.groupby) & (col("timestamp") < start_time.timestamp()))
         df = df.withColumn("timestamp_unix", F.col("timestamp").cast("bigint"))
```

### Comparing `featurizerai-1.6.4/src/features/tests/test_materialize.py` & `featurizerai-1.6.5/src/features/tests/test_materialize.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import features
-from flask import Flask, request, jsonify, json
-from features.materialize import materialize
-from features.custom_schema import custom_schema
-
-schema_fields = [
-    {"name": "timestamp", "type": "integer"},
-    {"name": "name", "type": "string"},
-    {"name": "email", "type": "string"},
-    {"name": "deviceid", "type": "integer"}
-]
-
-custom_schema = custom_schema(schema_fields)
-
-app = Flask(__name__)
-
-@app.route('/materialize', methods=['POST'])
-def aggregate():
-    mongo_connection = {
-        'uri': "mongodb+srv://admin:6lHqq9LqgwDlninK@cluster0.aqtcyq2.mongodb.net/?retryWrites=true&w=majority",
-        'database': 'kafkastream',
-        'rawdata': 'rawdata',
-        'collection': 'sparkaggregate'
-    }
-
-    try:
-        # Define the dynamic Spark SQL queries to be executed
-        sparksql = [
-            "SELECT COUNT(email) AS email_count_last_24_hours, COUNT(name) AS name_count_last_24_hours, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 86400 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
-            "SELECT COUNT(email) AS email_count_last_6_days, COUNT(name) AS name_count_last_6_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 604800 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
-            "SELECT COUNT(email) AS email_count_last_7_days, COUNT(name) AS name_count_last_7_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 604800 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
-            "SELECT COUNT(email) AS email_count_last_15_days, COUNT(name) AS name_count_last_15_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 1296000 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
-            "SELECT COUNT(email) AS email_count_last_45_days, COUNT(name) AS name_count_last_45_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 3.888e+6 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
-        ]
-        json_data = request.get_json()
-        timestamp = json_data.get('timestamp')
-        deviceid = json_data.get('deviceid')
-        token = json_data.get('token')
-
-        materialize_instance = materialize(mongo_connection, timestamp, "deviceid", deviceid, token, custom_schema.schema, sparksql, partition_column="deviceid")
-
-        aggregated_data_str = materialize_instance.read_data_and_aggregate()
-        aggregated_data = json.loads(aggregated_data_str)
-
-        return jsonify(aggregated_data)
-
-    except Exception as e:
-        return jsonify({"Result":"No data found","error": str(e)})
-
-if __name__ == '__main__':
-    app.run(debug=True, port=5001)
+import features
+from flask import Flask, request, jsonify, json
+from features.materialize import materialize
+from features.custom_schema import custom_schema
+
+schema_fields = [
+    {"name": "timestamp", "type": "integer"},
+    {"name": "name", "type": "string"},
+    {"name": "email", "type": "string"},
+    {"name": "deviceid", "type": "integer"}
+]
+
+custom_schema = custom_schema(schema_fields)
+
+app = Flask(__name__)
+
+@app.route('/materialize', methods=['POST'])
+def aggregate():
+    mongo_connection = {
+        'uri': "mongodb+srv://admin:6lHqq9LqgwDlninK@cluster0.aqtcyq2.mongodb.net/?retryWrites=true&w=majority",
+        'database': 'kafkastream',
+        'rawdata': 'rawdata',
+        'collection': 'sparkaggregate'
+    }
+
+    try:
+        # Define the dynamic Spark SQL queries to be executed
+        sparksql = [
+            "SELECT COUNT(email) AS email_count_last_24_hours, COUNT(name) AS name_count_last_24_hours, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 86400 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
+            "SELECT COUNT(email) AS email_count_last_6_days, COUNT(name) AS name_count_last_6_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 604800 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
+            "SELECT COUNT(email) AS email_count_last_7_days, COUNT(name) AS name_count_last_7_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 604800 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
+            "SELECT COUNT(email) AS email_count_last_15_days, COUNT(name) AS name_count_last_15_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 1296000 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
+            "SELECT COUNT(email) AS email_count_last_45_days, COUNT(name) AS name_count_last_45_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 3.888e+6 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
+        ]
+        json_data = request.get_json()
+        timestamp = json_data.get('timestamp')
+        deviceid = json_data.get('deviceid')
+        token = json_data.get('token')
+
+        materialize_instance = materialize(mongo_connection, timestamp, "deviceid", deviceid, token, custom_schema.schema, sparksql, partition_column="deviceid")
+
+        aggregated_data_str = materialize_instance.read_data_and_aggregate()
+        aggregated_data = json.loads(aggregated_data_str)
+
+        return jsonify(aggregated_data)
+
+    except Exception as e:
+        return jsonify({"Result":"No data found","error": str(e)})
+
+if __name__ == '__main__':
+    app.run(debug=True, port=5001)
```

### Comparing `featurizerai-1.6.4/src/features/tests/test_pipeline.py` & `featurizerai-1.6.5/src/features/tests/test_pipeline.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import time
-
-import features
-from features.create_stream import create_stream
-from features.authenticate import authenticate
-
-def authenticate_user():
-    sdk = authenticate()
-    access_token, token_type = sdk.authenticate('burak', 'burak')
-    return access_token
-
-def stream(token):
-    kafka_connection = {
-        "bootstrap.servers": "buraks-air.lan:9092",
-        "group.id": "your-group-id",
-        'enable.auto.commit': True,  # Enable automatic commit of offsets
-        'auto.offset.reset': 'earliest',
-        # Start consuming messages from the beginning of the topic if no offset is stored
-        'session.timeout.ms': 6000,  # Timeout for session management
-    }
-
-    # Optional: Provide custom MongoDB connection settings
-    mongo_connection = {
-        'uri': "mongodb+srv://admin:6lHqq9LqgwDlninK@cluster0.aqtcyq2.mongodb.net/?retryWrites=true&w=majority",
-        'database': 'kafkastream',
-        'rawcollection': 'rawdata',
-        'collection': 'sparkaggregate'
-    }
-
-    # Create a new instance of the create_stream class
-    featurizerai = create_stream(kafka_connection, mongo_connection, "fake-data_test5", "timestamp")
-
-    # Start the Kafka consumer in a separate thread
-    featurizerai.start(token)
-
-    featurizerai.stop()
-
-    # # Run the consumer for 60 seconds
-    # time.sleep(60)
-    #
-    # # Stop the consumer and wait for the thread to finish
-    # featurizerai.stop()
-def main():
-    token = authenticate_user()
-    stream(token)
-
-if __name__ == "__main__":
-    main()
+import time
+
+import features
+from features.create_stream import create_stream
+from features.authenticate import authenticate
+
+def authenticate_user():
+    sdk = authenticate()
+    access_token, token_type = sdk.authenticate('burak', 'burak')
+    return access_token
+
+def stream(token):
+    kafka_connection = {
+        "bootstrap.servers": "buraks-air.lan:9092",
+        "group.id": "your-group-id",
+        'enable.auto.commit': True,  # Enable automatic commit of offsets
+        'auto.offset.reset': 'earliest',
+        # Start consuming messages from the beginning of the topic if no offset is stored
+        'session.timeout.ms': 6000,  # Timeout for session management
+    }
+
+    # Optional: Provide custom MongoDB connection settings
+    mongo_connection = {
+        'uri': "mongodb+srv://admin:6lHqq9LqgwDlninK@cluster0.aqtcyq2.mongodb.net/?retryWrites=true&w=majority",
+        'database': 'kafkastream',
+        'rawcollection': 'rawdata',
+        'collection': 'sparkaggregate'
+    }
+
+    # Create a new instance of the create_stream class
+    featurizerai = create_stream(kafka_connection, mongo_connection, "fake-data_test5", "timestamp")
+
+    # Start the Kafka consumer in a separate thread
+    featurizerai.start(token)
+
+    featurizerai.stop()
+
+    # # Run the consumer for 60 seconds
+    # time.sleep(60)
+    #
+    # # Stop the consumer and wait for the thread to finish
+    # featurizerai.stop()
+def main():
+    token = authenticate_user()
+    stream(token)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `featurizerai-1.6.4/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.6.5/src/featurizerai.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1
-Name: featurizerai
-Version: 1.6.4
-Summary: Python library for Featurizer AI
-Home-page: https://github.com/burakglobal/featurizerai
-Author: Burak
-Author-email: burakgblobal@gmail.com
-Keywords: featurizer,package
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Provides-Extra: dev
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: featurizerai
+Version: 1.6.5
+Summary: Python library for Featurizer AI
+Home-page: https://github.com/burakglobal/featurizerai
+Author: Burak
+Author-email: burakgblobal@gmail.com
+Keywords: featurizer,package
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Provides-Extra: dev
+License-File: LICENSE
```


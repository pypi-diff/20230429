# Comparing `tmp/xapi-python-0.0.3.tar.gz` & `tmp/xapi-python-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xapi-python-0.0.3.tar", last modified: Fri Apr 28 08:36:24 2023, max compression
+gzip compressed data, was "xapi-python-0.1.0.tar", last modified: Sat Apr 29 11:42:03 2023, max compression
```

## Comparing `xapi-python-0.0.3.tar` & `xapi-python-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-28 08:36:24.787298 xapi-python-0.0.3/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1071 2023-04-25 04:51:26.000000 xapi-python-0.0.3/LICENSE
--rw-r--r--   0 pawel     (1000) pawel     (1000)     7880 2023-04-28 08:36:24.787298 xapi-python-0.0.3/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5591 2023-04-26 13:10:27.000000 xapi-python-0.0.3/README.md
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1075 2023-04-28 08:33:22.000000 xapi-python-0.0.3/pyproject.toml
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2023-04-28 08:36:24.787298 xapi-python-0.0.3/setup.cfg
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1011 2023-04-28 08:32:12.000000 xapi-python-0.0.3/setup.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-28 08:36:24.787298 xapi-python-0.0.3/tests/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5636 2023-04-27 06:31:53.000000 xapi-python-0.0.3/tests/test_connect.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     7958 2023-04-26 11:15:10.000000 xapi-python-0.0.3/tests/test_socket.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4014 2023-04-27 05:35:22.000000 xapi-python-0.0.3/tests/test_stream.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1566 2023-04-26 11:04:33.000000 xapi-python-0.0.3/tests/test_xapi.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-28 08:36:24.787298 xapi-python-0.0.3/xapi/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      338 2023-04-28 08:32:24.000000 xapi-python-0.0.3/xapi/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2055 2023-04-28 08:16:16.000000 xapi-python-0.0.3/xapi/connection.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1464 2023-04-24 14:52:49.000000 xapi-python-0.0.3/xapi/enums.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      200 2023-04-24 12:09:22.000000 xapi-python-0.0.3/xapi/exceptions.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     6640 2023-04-28 08:30:55.000000 xapi-python-0.0.3/xapi/socket.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2947 2023-04-26 09:47:15.000000 xapi-python-0.0.3/xapi/stream.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1103 2023-04-28 08:15:26.000000 xapi-python-0.0.3/xapi/xapi.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-28 08:36:24.787298 xapi-python-0.0.3/xapi_python.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     7880 2023-04-28 08:36:24.000000 xapi-python-0.0.3/xapi_python.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      376 2023-04-28 08:36:24.000000 xapi-python-0.0.3/xapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2023-04-28 08:36:24.000000 xapi-python-0.0.3/xapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        5 2023-04-28 08:36:24.000000 xapi-python-0.0.3/xapi_python.egg-info/top_level.txt
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-29 11:42:03.464872 xapi-python-0.1.0/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1071 2023-04-25 04:51:26.000000 xapi-python-0.1.0/LICENSE
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     8099 2023-04-29 11:42:03.464872 xapi-python-0.1.0/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5794 2023-04-29 11:41:41.000000 xapi-python-0.1.0/README.md
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1105 2023-04-29 11:41:41.000000 xapi-python-0.1.0/pyproject.toml
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2023-04-29 11:42:03.464872 xapi-python-0.1.0/setup.cfg
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1027 2023-04-29 11:41:41.000000 xapi-python-0.1.0/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-29 11:42:03.454872 xapi-python-0.1.0/tests/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4687 2023-04-29 11:41:41.000000 xapi-python-0.1.0/tests/test_connect.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     7958 2023-04-26 11:15:10.000000 xapi-python-0.1.0/tests/test_socket.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4014 2023-04-27 05:35:22.000000 xapi-python-0.1.0/tests/test_stream.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1566 2023-04-29 10:20:03.000000 xapi-python-0.1.0/tests/test_xapi.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-29 11:42:03.464872 xapi-python-0.1.0/xapi/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      338 2023-04-29 11:41:41.000000 xapi-python-0.1.0/xapi/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2114 2023-04-29 11:41:41.000000 xapi-python-0.1.0/xapi/connection.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1464 2023-04-24 14:52:49.000000 xapi-python-0.1.0/xapi/enums.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      205 2023-04-29 11:41:41.000000 xapi-python-0.1.0/xapi/exceptions.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     6640 2023-04-29 11:38:37.000000 xapi-python-0.1.0/xapi/socket.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2947 2023-04-29 11:39:31.000000 xapi-python-0.1.0/xapi/stream.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2207 2023-04-29 11:41:41.000000 xapi-python-0.1.0/xapi/xapi.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-29 11:42:03.464872 xapi-python-0.1.0/xapi_python.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     8099 2023-04-29 11:42:03.000000 xapi-python-0.1.0/xapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      376 2023-04-29 11:42:03.000000 xapi-python-0.1.0/xapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2023-04-29 11:42:03.000000 xapi-python-0.1.0/xapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        5 2023-04-29 11:42:03.000000 xapi-python-0.1.0/xapi_python.egg-info/top_level.txt
```

### Comparing `xapi-python-0.0.3/LICENSE` & `xapi-python-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.3/PKG-INFO` & `xapi-python-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xapi-python
-Version: 0.0.3
+Version: 0.1.0
 Summary: The xStation5 API Python library
 Home-page: https://github.com/pawelkn/xapi-python
 Author: Paweł Knioła
 Author-email: Paweł Knioła <pawel.kn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Paweł Knioła
@@ -25,15 +25,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/pawelkn/xapi-python
 Project-URL: Bug Tracker, https://github.com/pawelkn/xapi-python/issues
-Keywords: python,trading,websocket,trading-api,forex,xapi,forex-trading,exchange-api,forex-data,xstation5,xtb,xopenhub,forex-api,xopenhub-api,xtb-api,xstation-api,x-trade-brokers,bfbcapital,xstation
+Keywords: python,python3,bitcoin,trading,websocket,trading-api,forex,xapi,forex-trading,exchange-api,forex-data,xstation,xstation5,xtb,xopenhub,forex-api,xopenhub-api,xtb-api,xstation-api,x-trade-brokers,bfbcapital
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -62,29 +62,29 @@
 
 ```shell
 pip install xapi-python
 ```
 
 ## Usage
 
-To use xAPI, you will need to have an active account with the xStation5 trading platform. Once you have an account, you can use the xStation5 library to connect to the platform and begin trading.
+To use xAPI, you will need to have an active account with the xStation5 trading platform. Once you have an account, you can use the xAPI library to connect to the platform and begin trading.
 
 Here is an example of how to use the xAPI library to connect to the xStation5 platform:
 
 ```python
 import asyncio
 import xapi
 
 # Replace these values with your own credentials
 CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
-    "safe": False
+    "safe": True
 }
 
 async def main():
     try:
         # Create a new xAPI object and connect to the xStation5 platform
         async with await xapi.connect(**CREDENTIALS) as x:
             pass
@@ -109,15 +109,15 @@
 
 # Replace these values with your own credentials
 CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
-    "safe": False
+    "safe": True
 }
 
 async def main():
     while True:
         try:
             async with await xapi.connect(**CREDENTIALS) as x:
                 # Subscribe for the current price of BITCOIN and ETHEREUM
@@ -197,15 +197,15 @@
 
 ```json
 {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
-    "safe": false
+    "safe": true
 }
 ```
 
 Once you have created the _credentials.json_ file, you can run an example using the following command:
 
 ```shell
 python3 examples/get-margin-level.py
@@ -214,7 +214,11 @@
 ## Unit Tests
 
 This will run all of the unit tests in the tests directory:
 
 ```shell
 python3 -m unittest discover tests
 ```
+
+## Buy Me A Coffee! ☕
+
+If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [BuyMeACoffee](https://www.buymeacoffee.com/pawelkn)
```

### Comparing `xapi-python-0.0.3/README.md` & `xapi-python-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 
 ```shell
 pip install xapi-python
 ```
 
 ## Usage
 
-To use xAPI, you will need to have an active account with the xStation5 trading platform. Once you have an account, you can use the xStation5 library to connect to the platform and begin trading.
+To use xAPI, you will need to have an active account with the xStation5 trading platform. Once you have an account, you can use the xAPI library to connect to the platform and begin trading.
 
 Here is an example of how to use the xAPI library to connect to the xStation5 platform:
 
 ```python
 import asyncio
 import xapi
 
 # Replace these values with your own credentials
 CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
-    "safe": False
+    "safe": True
 }
 
 async def main():
     try:
         # Create a new xAPI object and connect to the xStation5 platform
         async with await xapi.connect(**CREDENTIALS) as x:
             pass
@@ -65,15 +65,15 @@
 
 # Replace these values with your own credentials
 CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
-    "safe": False
+    "safe": True
 }
 
 async def main():
     while True:
         try:
             async with await xapi.connect(**CREDENTIALS) as x:
                 # Subscribe for the current price of BITCOIN and ETHEREUM
@@ -153,15 +153,15 @@
 
 ```json
 {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
-    "safe": false
+    "safe": true
 }
 ```
 
 Once you have created the _credentials.json_ file, you can run an example using the following command:
 
 ```shell
 python3 examples/get-margin-level.py
@@ -170,7 +170,11 @@
 ## Unit Tests
 
 This will run all of the unit tests in the tests directory:
 
 ```shell
 python3 -m unittest discover tests
 ```
+
+## Buy Me A Coffee! ☕
+
+If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [BuyMeACoffee](https://www.buymeacoffee.com/pawelkn)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xapi-python-0.0.3/pyproject.toml` & `xapi-python-0.1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 [project]
 name = "xapi-python"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
   { name="Paweł Knioła", email="pawel.kn@gmail.com" },
 ]
 description = "The xStation5 API Python library"
-keywords = ["python", "trading", "websocket", "trading-api", "forex", "xapi", "forex-trading", "exchange-api", "forex-data", "xstation5", "xtb", "xopenhub", "forex-api", "xopenhub-api", "xtb-api", "xstation-api", "x-trade-brokers", "bfbcapital", "xstation"]
+keywords = [
+  "python", "python3", "bitcoin", "trading", "websocket", "trading-api", "forex", "xapi", "forex-trading",
+  "exchange-api", "forex-data", "xstation", "xstation5", "xtb", "xopenhub", "forex-api", "xopenhub-api",
+  "xtb-api", "xstation-api", "x-trade-brokers", "bfbcapital"
+]
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",      #Specify which pyhton versions that you want to support
```

### Comparing `xapi-python-0.0.3/setup.py` & `xapi-python-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 setup(
     name='xapi-python',
     author='Paweł Knioła',
     author_email='pawel.kn@gmail.com',
     description='The xStation5 API Python library',
     long_description=open('README.md', encoding='utf-8').read(),
     license='MIT',
-    keywords='python trading websocket trading-api forex xapi forex-trading exchange-api forex-data xstation5 xtb xopenhub forex-api xopenhub-api xtb-api xstation-api x-trade-brokers bfbcapital xstation',
+    keywords='python python3 bitcoin trading websocket trading-api forex xapi forex-trading exchange-api forex-data xstation xstation5 xtb xopenhub forex-api xopenhub-api xtb-api xstation-api x-trade-brokers bfbcapital',
     url='https://github.com/pawelkn/xapi-python',
     classifiers=[
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12"
     ],
     python_requires='>=3.7',
-    version="0.0.3",
+    version="0.1.0",
     packages=['xapi'],
 )
```

### Comparing `xapi-python-0.0.3/tests/test_connect.py` & `xapi-python-0.1.0/tests/test_connect.py`

 * *Files 13% similar despite different names*

```diff
@@ -81,37 +81,14 @@
         conn._conn = AsyncMock()
         conn._conn.send.side_effect = websockets.exceptions.ConnectionClosed(None, None)
         command = {"command": "test"}
         with self.assertRaises(ConnectionClosed) as cm:
             await conn._request(command)
         self.assertEqual(str(cm.exception), "Connection unexpectedly closed")
 
-    async def test_response_with_connection(self):
-        conn = Connection()
-        conn._conn = AsyncMock()
-        response = {"response": "test"}
-        conn._conn.recv.return_value = json.dumps(response)
-        result = await conn._response()
-        conn._conn.recv.assert_called_once()
-        self.assertEqual(result, response)
-
-    async def test_response_without_connection(self):
-        conn = Connection()
-        with self.assertRaises(ConnectionClosed) as cm:
-            await conn._response()
-        self.assertEqual(str(cm.exception), "Not connected")
-
-    async def test_response_connection_closed(self):
-        conn = Connection()
-        conn._conn = AsyncMock()
-        conn._conn.recv.side_effect = websockets.exceptions.ConnectionClosed(None, None)
-        with self.assertRaises(ConnectionClosed) as cm:
-            await conn._response()
-        self.assertEqual(str(cm.exception), "Connection unexpectedly closed")
-
     async def test_transaction_with_connection(self):
         conn = Connection()
         conn._conn = AsyncMock()
         command = {"command": "test"}
         response = {"response": "test"}
         conn._conn.recv.return_value = json.dumps(response)
         result = await conn._transaction(command)
```

### Comparing `xapi-python-0.0.3/tests/test_socket.py` & `xapi-python-0.1.0/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.3/tests/test_stream.py` & `xapi-python-0.1.0/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.3/tests/test_xapi.py` & `xapi-python-0.1.0/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.3/xapi/enums.py` & `xapi-python-0.1.0/xapi/enums.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.3/xapi/socket.py` & `xapi-python-0.1.0/xapi/socket.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.3/xapi/stream.py` & `xapi-python-0.1.0/xapi/stream.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.3/xapi_python.egg-info/PKG-INFO` & `xapi-python-0.1.0/xapi_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xapi-python
-Version: 0.0.3
+Version: 0.1.0
 Summary: The xStation5 API Python library
 Home-page: https://github.com/pawelkn/xapi-python
 Author: Paweł Knioła
 Author-email: Paweł Knioła <pawel.kn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Paweł Knioła
@@ -25,15 +25,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/pawelkn/xapi-python
 Project-URL: Bug Tracker, https://github.com/pawelkn/xapi-python/issues
-Keywords: python,trading,websocket,trading-api,forex,xapi,forex-trading,exchange-api,forex-data,xstation5,xtb,xopenhub,forex-api,xopenhub-api,xtb-api,xstation-api,x-trade-brokers,bfbcapital,xstation
+Keywords: python,python3,bitcoin,trading,websocket,trading-api,forex,xapi,forex-trading,exchange-api,forex-data,xstation,xstation5,xtb,xopenhub,forex-api,xopenhub-api,xtb-api,xstation-api,x-trade-brokers,bfbcapital
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -62,29 +62,29 @@
 
 ```shell
 pip install xapi-python
 ```
 
 ## Usage
 
-To use xAPI, you will need to have an active account with the xStation5 trading platform. Once you have an account, you can use the xStation5 library to connect to the platform and begin trading.
+To use xAPI, you will need to have an active account with the xStation5 trading platform. Once you have an account, you can use the xAPI library to connect to the platform and begin trading.
 
 Here is an example of how to use the xAPI library to connect to the xStation5 platform:
 
 ```python
 import asyncio
 import xapi
 
 # Replace these values with your own credentials
 CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
-    "safe": False
+    "safe": True
 }
 
 async def main():
     try:
         # Create a new xAPI object and connect to the xStation5 platform
         async with await xapi.connect(**CREDENTIALS) as x:
             pass
@@ -109,15 +109,15 @@
 
 # Replace these values with your own credentials
 CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
-    "safe": False
+    "safe": True
 }
 
 async def main():
     while True:
         try:
             async with await xapi.connect(**CREDENTIALS) as x:
                 # Subscribe for the current price of BITCOIN and ETHEREUM
@@ -197,15 +197,15 @@
 
 ```json
 {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
-    "safe": false
+    "safe": true
 }
 ```
 
 Once you have created the _credentials.json_ file, you can run an example using the following command:
 
 ```shell
 python3 examples/get-margin-level.py
@@ -214,7 +214,11 @@
 ## Unit Tests
 
 This will run all of the unit tests in the tests directory:
 
 ```shell
 python3 -m unittest discover tests
 ```
+
+## Buy Me A Coffee! ☕
+
+If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [BuyMeACoffee](https://www.buymeacoffee.com/pawelkn)
```


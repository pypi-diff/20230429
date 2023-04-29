# Comparing `tmp/eircode-0.0.7.tar.gz` & `tmp/eircode-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eircode-0.0.7.tar", last modified: Sun Feb 27 13:47:25 2022, max compression
+gzip compressed data, was "eircode-0.0.8.tar", last modified: Sun Feb 27 17:42:06 2022, max compression
```

## Comparing `eircode-0.0.7.tar` & `eircode-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 13:47:25.778190 eircode-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-27 13:47:10.000000 eircode-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-02-27 13:47:25.778190 eircode-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-02-27 13:47:10.000000 eircode-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-27 13:47:25.778190 eircode-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-02-27 13:47:10.000000 eircode-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 13:47:25.778190 eircode-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 13:47:25.778190 eircode-0.0.7/src/eircode/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-27 13:47:10.000000 eircode-0.0.7/src/eircode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4764 2022-02-27 13:47:10.000000 eircode-0.0.7/src/eircode/address.py
--rw-r--r--   0 runner    (1001) docker     (121)     7623 2022-02-27 13:47:10.000000 eircode-0.0.7/src/eircode/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-02-27 13:47:10.000000 eircode-0.0.7/src/eircode/eircode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 13:47:25.778190 eircode-0.0.7/src/eircode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-02-27 13:47:25.000000 eircode-0.0.7/src/eircode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-02-27 13:47:25.000000 eircode-0.0.7/src/eircode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-27 13:47:25.000000 eircode-0.0.7/src/eircode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-02-27 13:47:25.000000 eircode-0.0.7/src/eircode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-27 13:47:25.000000 eircode-0.0.7/src/eircode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 13:47:25.778190 eircode-0.0.7/test/
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-02-27 13:47:10.000000 eircode-0.0.7/test/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 17:42:06.280369 eircode-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-27 17:41:48.000000 eircode-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-02-27 17:42:06.280369 eircode-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-02-27 17:41:48.000000 eircode-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-27 17:42:06.280369 eircode-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-02-27 17:41:48.000000 eircode-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 17:42:06.276369 eircode-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 17:42:06.276369 eircode-0.0.8/src/eircode/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-27 17:41:48.000000 eircode-0.0.8/src/eircode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5773 2022-02-27 17:41:48.000000 eircode-0.0.8/src/eircode/address.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7623 2022-02-27 17:41:48.000000 eircode-0.0.8/src/eircode/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-02-27 17:41:48.000000 eircode-0.0.8/src/eircode/eircode.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 17:42:06.280369 eircode-0.0.8/src/eircode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-02-27 17:42:06.000000 eircode-0.0.8/src/eircode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2022-02-27 17:42:06.000000 eircode-0.0.8/src/eircode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-27 17:42:06.000000 eircode-0.0.8/src/eircode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-02-27 17:42:06.000000 eircode-0.0.8/src/eircode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-27 17:42:06.000000 eircode-0.0.8/src/eircode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 17:42:06.280369 eircode-0.0.8/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2022-02-27 17:41:48.000000 eircode-0.0.8/test/test_basic.py
```

### Comparing `eircode-0.0.7/LICENSE` & `eircode-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `eircode-0.0.7/README.md` & `eircode-0.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Eircode
 =======
 
-Tool to get eircodes from an address
+Tool to get eircodes from an address. Optional proxy to avoid rate limiting.
 
 Installation
 ------------
 
 `pip install eircode`
 
 Usage
```

### Comparing `eircode-0.0.7/src/eircode/address.py` & `eircode-0.0.8/src/eircode/address.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from difflib import SequenceMatcher
+import urllib
 
 from cached_property import cached_property
 import requests
+from requests_ip_rotator import ApiGateway
 
 from eircode.eircode import Eircode
 from eircode.constants import (
     IDENTITY_URL_PATH,
     EIRCODE_FINDER_URL_PATH
 )
+from eircode.proxy import Proxy
+
+proxy_cli = Proxy(skip_setup=True)
+
 
 class Addresses():
 
     def __init__(self):
         self._data = []
 
     def append(self, address):
@@ -38,31 +44,58 @@
         self.input_address = address
 
         self.display_name = kwargs.get('display_name', None)
         self.link = kwargs.get('link', None)
         self._eircode = kwargs.get('eircode', None)
 
         if not kwargs.get('skip_set', False):
-            self.set(throw_ex=kwargs.get('throw_ex', False))
-
-    def set(self, throw_ex=True):
-        identity_response = requests.get(IDENTITY_URL_PATH).json()
+            self.set(
+                throw_ex=kwargs.get('throw_ex', False),
+                proxy=kwargs.get('proxy', False)
+            )
+
+    def set(self, throw_ex=True, proxy=False):
+
+        if proxy:
+
+            try:
+                proxy_cli.setup()
+            except:
+                raise Exception('Could not set up proxy cli. Go to here for details: https://github.com/Ge0rg3/requests-ip-rotator')
+
+            identity_response = proxy_cli.get(IDENTITY_URL_PATH).json()
+
+            params = {
+                'key': identity_response['key'],
+                'address': self.input_address,
+                'language': 'en',
+                'geographicAddress': True,
+                'clientVersion': None
+            }
+
+            finder_response = proxy_cli.get(
+                EIRCODE_FINDER_URL_PATH + '?' + urllib.parse.urlencode(params)
+            )
+
+        else:
+            identity_response = requests.get(IDENTITY_URL_PATH).json()
+            params = {
+                'key': identity_response['key'],
+                'address': self.input_address,
+                'language': 'en',
+                'geographicAddress': True,
+                'clientVersion': None
+            }
+
+            finder_response = requests.get(
+                EIRCODE_FINDER_URL_PATH,
+                params=params
+            )
 
-        params = {
-            'key': identity_response['key'],
-            'address': self.input_address,
-            'language': 'en',
-            'geographicAddress': True,
-            'clientVersion': None
-        }
-
-        finder_response = requests.get(
-            EIRCODE_FINDER_URL_PATH,
-            params=params
-        ).json()
+        finder_response = finder_response.json()
 
         if 'postcode' in finder_response:
             self._eircode = finder_response['postcode']
             self.display_name = self.input_address
             return
 
         if finder_response.get('error', {}).get('code', None) == 403:
```

### Comparing `eircode-0.0.7/src/eircode/constants.py` & `eircode-0.0.8/src/eircode/constants.py`

 * *Files identical despite different names*

### Comparing `eircode-0.0.7/src/eircode/eircode.py` & `eircode-0.0.8/src/eircode/eircode.py`

 * *Files identical despite different names*


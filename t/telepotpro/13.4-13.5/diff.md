# Comparing `tmp/telepotpro-13.4.tar.gz` & `tmp/telepotpro-13.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telepotpro-13.4.tar", last modified: Wed Apr 26 20:08:58 2023, max compression
+gzip compressed data, was "telepotpro-13.5.tar", last modified: Sat Apr 29 08:26:14 2023, max compression
```

## Comparing `telepotpro-13.4.tar` & `telepotpro-13.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:08:58.696465 telepotpro-13.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-26 20:08:42.000000 telepotpro-13.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-26 20:08:58.696465 telepotpro-13.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-26 20:08:42.000000 telepotpro-13.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:08:58.696465 telepotpro-13.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-04-26 20:08:42.000000 telepotpro-13.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:08:58.696465 telepotpro-13.4/telepotpro/
--rw-r--r--   0 runner    (1001) docker     (123)    55319 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:08:58.696465 telepotpro-13.4/telepotpro/aio/
--rw-r--r--   0 runner    (1001) docker     (123)    39799 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/aio/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/aio/delegate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/aio/hack.py
--rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/aio/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/aio/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/aio/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/delegate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/hack.py
--rw-r--r--   0 runner    (1001) docker     (123)    41205 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    31684 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/namedtuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:08:58.696465 telepotpro-13.4/telepotpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-26 20:08:58.000000 telepotpro-13.4/telepotpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-26 20:08:58.000000 telepotpro-13.4/telepotpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:08:58.000000 telepotpro-13.4/telepotpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-26 20:08:58.000000 telepotpro-13.4/telepotpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 20:08:58.000000 telepotpro-13.4/telepotpro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:26:14.103238 telepotpro-13.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-29 08:25:58.000000 telepotpro-13.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-29 08:26:14.103238 telepotpro-13.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-29 08:25:58.000000 telepotpro-13.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 08:26:14.103238 telepotpro-13.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-04-29 08:25:58.000000 telepotpro-13.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:26:14.103238 telepotpro-13.5/telepotpro/
+-rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:26:14.103238 telepotpro-13.5/telepotpro/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)    39940 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/aio/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/aio/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/aio/hack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/aio/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/aio/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/aio/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/hack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41205 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31684 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/namedtuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-29 08:25:58.000000 telepotpro-13.5/telepotpro/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:26:14.103238 telepotpro-13.5/telepotpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-29 08:26:14.000000 telepotpro-13.5/telepotpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-29 08:26:14.000000 telepotpro-13.5/telepotpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 08:26:14.000000 telepotpro-13.5/telepotpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-29 08:26:14.000000 telepotpro-13.5/telepotpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 08:26:14.000000 telepotpro-13.5/telepotpro.egg-info/top_level.txt
```

### Comparing `telepotpro-13.4/LICENSE.md` & `telepotpro-13.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/PKG-INFO` & `telepotpro-13.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telepotpro
-Version: 13.4
+Version: 13.5
 Summary: Python framework for Telegram Bot API
 Home-page: https://github.com/pesaventofilippo/telepotpro
 Author: Filippo Pesavento
 Author-email: pesaventofilippo@gmail.com
 License: MIT
 Keywords: telegram bot api python wrapper
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `telepotpro-13.4/README.md` & `telepotpro-13.5/README.md`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/setup.py` & `telepotpro-13.5/setup.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/__init__.py` & `telepotpro-13.5/telepotpro/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Patch urllib3 for sending unicode filename
 from . import hack
 
 from . import exception
 
 
-__version_info__ = (13, 4)
+__version_info__ = (13, 5)
 __version__ = '.'.join(map(str, __version_info__))
 
 
 def flavor(msg):
     """
     Return flavor of message or event.
 
@@ -516,14 +516,18 @@
             files = {file_key: file_value}
             return self._api_request(method, _rectify(params), files, **kwargs)
 
     def getMe(self):
         """ See: https://core.telegram.org/bots/api#getme """
         return self._api_request('getMe')
 
+    def logOut(self):
+        """ See: https://core.telegram.org/bots/api#logout """
+        return self._api_request('logOut')
+
     def sendMessage(self, chat_id, text,
                     parse_mode=None,
                     disable_web_page_preview=None,
                     disable_notification=None,
                     reply_to_message_id=None,
                     reply_markup=None):
         """ See: https://core.telegram.org/bots/api#sendmessage """
```

### Comparing `telepotpro-13.4/telepotpro/aio/__init__.py` & `telepotpro-13.5/telepotpro/aio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,18 @@
             files = {file_key: file_value}
             return await self._api_request(method, _rectify(params), files, **kwargs)
 
     async def getMe(self):
         """ See: https://core.telegram.org/bots/api#getme """
         return await self._api_request('getMe')
 
+    async def logOut(self):
+        """ See: https://core.telegram.org/bots/api#logout """
+        return await self._api_request('logOut')
+
     async def sendMessage(self, chat_id, text,
                           parse_mode=None,
                           disable_web_page_preview=None,
                           disable_notification=None,
                           reply_to_message_id=None,
                           reply_markup=None):
         """ See: https://core.telegram.org/bots/api#sendmessage """
```

### Comparing `telepotpro-13.4/telepotpro/aio/api.py` & `telepotpro-13.5/telepotpro/aio/api.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/aio/delegate.py` & `telepotpro-13.5/telepotpro/aio/delegate.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/aio/hack.py` & `telepotpro-13.5/telepotpro/aio/hack.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/aio/helper.py` & `telepotpro-13.5/telepotpro/aio/helper.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/aio/loop.py` & `telepotpro-13.5/telepotpro/aio/loop.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/aio/routing.py` & `telepotpro-13.5/telepotpro/aio/routing.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/api.py` & `telepotpro-13.5/telepotpro/api.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/delegate.py` & `telepotpro-13.5/telepotpro/delegate.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/exception.py` & `telepotpro-13.5/telepotpro/exception.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/filtering.py` & `telepotpro-13.5/telepotpro/filtering.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/helper.py` & `telepotpro-13.5/telepotpro/helper.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/loop.py` & `telepotpro-13.5/telepotpro/loop.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/namedtuple.py` & `telepotpro-13.5/telepotpro/namedtuple.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/routing.py` & `telepotpro-13.5/telepotpro/routing.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro/text.py` & `telepotpro-13.5/telepotpro/text.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.4/telepotpro.egg-info/PKG-INFO` & `telepotpro-13.5/telepotpro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telepotpro
-Version: 13.4
+Version: 13.5
 Summary: Python framework for Telegram Bot API
 Home-page: https://github.com/pesaventofilippo/telepotpro
 Author: Filippo Pesavento
 Author-email: pesaventofilippo@gmail.com
 License: MIT
 Keywords: telegram bot api python wrapper
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `telepotpro-13.4/telepotpro.egg-info/SOURCES.txt` & `telepotpro-13.5/telepotpro.egg-info/SOURCES.txt`

 * *Files identical despite different names*


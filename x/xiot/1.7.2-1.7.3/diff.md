# Comparing `tmp/xiot-1.7.2.tar.gz` & `tmp/xiot-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xiot-1.7.2.tar", last modified: Sat Apr 15 14:10:55 2023, max compression
+gzip compressed data, was "dist/xiot-1.7.3.tar", last modified: Sat Apr 29 16:50:47 2023, max compression
```

## Comparing `xiot-1.7.2.tar` & `xiot-1.7.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-04-15 14:10:55.000000 xiot-1.7.2/
--rw-r--r--   0 Robin      (501) staff       (20)      242 2023-04-15 14:10:55.000000 xiot-1.7.2/PKG-INFO
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-04-15 14:10:55.000000 xiot-1.7.2/xiot.egg-info/
--rw-r--r--   0 Robin      (501) staff       (20)      242 2023-04-15 14:10:55.000000 xiot-1.7.2/xiot.egg-info/PKG-INFO
--rw-r--r--   0 Robin      (501) staff       (20)      168 2023-04-15 14:10:55.000000 xiot-1.7.2/xiot.egg-info/SOURCES.txt
--rw-r--r--   0 Robin      (501) staff       (20)       23 2023-04-15 14:10:55.000000 xiot-1.7.2/xiot.egg-info/requires.txt
--rw-r--r--   0 Robin      (501) staff       (20)       15 2023-04-15 14:10:55.000000 xiot-1.7.2/xiot.egg-info/top_level.txt
--rw-r--r--   0 Robin      (501) staff       (20)        1 2023-04-15 14:10:55.000000 xiot-1.7.2/xiot.egg-info/dependency_links.txt
--rw-r--r--   0 Robin      (501) staff       (20)     9471 2023-04-15 14:10:31.000000 xiot-1.7.2/xiot.py
--rw-r--r--   0 Robin      (501) staff       (20)      395 2020-02-10 15:11:28.000000 xiot-1.7.2/setup.py
--rw-r--r--   0 Robin      (501) staff       (20)       38 2023-04-15 14:10:55.000000 xiot-1.7.2/setup.cfg
--rw-r--r--   0 Robin      (501) staff       (20)    17265 2023-04-15 06:15:40.000000 xiot-1.7.2/xiotshell.py
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-04-29 16:50:47.000000 xiot-1.7.3/
+-rw-r--r--   0 Robin      (501) staff       (20)      242 2023-04-29 16:50:47.000000 xiot-1.7.3/PKG-INFO
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2023-04-29 16:50:47.000000 xiot-1.7.3/xiot.egg-info/
+-rw-r--r--   0 Robin      (501) staff       (20)      242 2023-04-29 16:50:46.000000 xiot-1.7.3/xiot.egg-info/PKG-INFO
+-rw-r--r--   0 Robin      (501) staff       (20)      168 2023-04-29 16:50:46.000000 xiot-1.7.3/xiot.egg-info/SOURCES.txt
+-rw-r--r--   0 Robin      (501) staff       (20)       23 2023-04-29 16:50:46.000000 xiot-1.7.3/xiot.egg-info/requires.txt
+-rw-r--r--   0 Robin      (501) staff       (20)       15 2023-04-29 16:50:46.000000 xiot-1.7.3/xiot.egg-info/top_level.txt
+-rw-r--r--   0 Robin      (501) staff       (20)        1 2023-04-29 16:50:46.000000 xiot-1.7.3/xiot.egg-info/dependency_links.txt
+-rw-r--r--   0 Robin      (501) staff       (20)     9597 2023-04-29 16:49:50.000000 xiot-1.7.3/xiot.py
+-rw-r--r--   0 Robin      (501) staff       (20)      395 2020-02-10 15:11:28.000000 xiot-1.7.3/setup.py
+-rw-r--r--   0 Robin      (501) staff       (20)       38 2023-04-29 16:50:47.000000 xiot-1.7.3/setup.cfg
+-rw-r--r--   0 Robin      (501) staff       (20)    17265 2023-04-15 06:15:40.000000 xiot-1.7.3/xiotshell.py
```

### Comparing `xiot-1.7.2/xiot.py` & `xiot-1.7.3/xiot.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 '''
 Created on 2018年11月23日
 
 @author: Robin
 '''
 from __future__ import print_function
 
-__version__ = '1.7.2'
+__version__ = '1.7.3'
 
 
 def md5(s):
     import hashlib
     m2 = hashlib.md5()
     m2.update(s.encode("utf8"))
     return m2.hexdigest()
@@ -156,15 +156,20 @@
         #     print('retry')
         self.connected = False
 
     def _on_message(self, client, userdata, msg):
         import json
         # print("_on_message", client, userdata, msg.topic, msg.payload)
         try:
-            self.on_message(msg.topic, json.loads(msg.payload.decode('utf-8')))
+            msgd = json.loads(msg.payload.decode('utf-8'))
+        except:
+            print('not json', msg.topic, msg.payload)
+            return
+        try:
+            self.on_message(msg.topic, msgd)
         except:
             import traceback
             traceback.print_exc()
             print(msg.topic, msg.payload)
 
     def on_message(self, topic, data):
         pass
```

### Comparing `xiot-1.7.2/xiotshell.py` & `xiot-1.7.3/xiotshell.py`

 * *Files identical despite different names*


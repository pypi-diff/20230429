# Comparing `tmp/xia_pusher-0.0.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_pusher-0.1.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 110694 bytes, number of entries: 7
--rw-r--r--  2.0 unx       88 b- defN 23-Mar-02 22:48 xia_pusher/__init__.py
--rw-r--r--  2.0 unx   258560 b- defN 23-Mar-02 23:10 xia_pusher/pusher.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Mar-02 23:10 xia_pusher-0.0.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      689 b- defN 23-Mar-02 23:10 xia_pusher-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Mar-02 23:10 xia_pusher-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Mar-02 23:10 xia_pusher-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      575 b- defN 23-Mar-02 23:10 xia_pusher-0.0.7.dist-info/RECORD
-7 files, 260174 bytes uncompressed, 109668 bytes compressed:  57.8%
+Zip file size: 110137 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       88 b- defN 23-Apr-29 18:03 xia_pusher/__init__.py
+-rw-r--r--  2.0 unx   257536 b- defN 23-Apr-29 18:06 xia_pusher/pusher.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-29 18:06 xia_pusher-0.1.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      689 b- defN 23-Apr-29 18:06 xia_pusher-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-29 18:06 xia_pusher-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-29 18:06 xia_pusher-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      575 b- defN 23-Apr-29 18:06 xia_pusher-0.1.0.dist-info/RECORD
+7 files, 259150 bytes uncompressed, 109111 bytes compressed:  57.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_pusher/__init__.py
 Comment: 
 
 Filename: xia_pusher/pusher.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_pusher-0.0.7.dist-info/LICENSE.txt
+Filename: xia_pusher-0.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_pusher-0.0.7.dist-info/METADATA
+Filename: xia_pusher-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: xia_pusher-0.0.7.dist-info/WHEEL
+Filename: xia_pusher-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: xia_pusher-0.0.7.dist-info/top_level.txt
+Filename: xia_pusher-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_pusher-0.0.7.dist-info/RECORD
+Filename: xia_pusher-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_pusher/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_pusher.pusher import Pusher
 
 __all__ = [
     "Pusher"
 ]
 
-__version__ = "0.0.7"
+__version__ = "0.1.0"
```

## Comparing `xia_pusher-0.0.7.dist-info/METADATA` & `xia_pusher-0.1.0.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-pusher
-Version: 0.0.7
+Version: 0.1.0
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-pusher/0.0.7/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-pusher/0.1.0/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```


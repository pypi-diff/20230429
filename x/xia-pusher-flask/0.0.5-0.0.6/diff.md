# Comparing `tmp/xia_pusher_flask-0.0.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_pusher_flask-0.0.6-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 108597 bytes, number of entries: 7
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-29 10:23 xia_pusher_flask/__init__.py
--rw-r--r--  2.0 unx   253952 b- defN 23-Apr-29 10:41 xia_pusher_flask/api.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-29 10:41 xia_pusher_flask-0.0.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      714 b- defN 23-Apr-29 10:41 xia_pusher_flask-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-29 10:41 xia_pusher_flask-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-29 10:41 xia_pusher_flask-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      614 b- defN 23-Apr-29 10:41 xia_pusher_flask-0.0.5.dist-info/RECORD
-7 files, 255645 bytes uncompressed, 107493 bytes compressed:  58.0%
+Zip file size: 107887 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       97 b- defN 23-Apr-29 18:26 xia_pusher_flask/__init__.py
+-rw-r--r--  2.0 unx   252928 b- defN 23-Apr-29 18:29 xia_pusher_flask/api.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-29 18:29 xia_pusher_flask-0.0.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      714 b- defN 23-Apr-29 18:29 xia_pusher_flask-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-29 18:29 xia_pusher_flask-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-29 18:29 xia_pusher_flask-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      614 b- defN 23-Apr-29 18:29 xia_pusher_flask-0.0.6.dist-info/RECORD
+7 files, 254621 bytes uncompressed, 106783 bytes compressed:  58.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_pusher_flask/__init__.py
 Comment: 
 
 Filename: xia_pusher_flask/api.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_pusher_flask-0.0.5.dist-info/LICENSE.txt
+Filename: xia_pusher_flask-0.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_pusher_flask-0.0.5.dist-info/METADATA
+Filename: xia_pusher_flask-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_pusher_flask-0.0.5.dist-info/WHEEL
+Filename: xia_pusher_flask-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_pusher_flask-0.0.5.dist-info/top_level.txt
+Filename: xia_pusher_flask-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_pusher_flask-0.0.5.dist-info/RECORD
+Filename: xia_pusher_flask-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_pusher_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_pusher_flask.api import PusherApi
 
 __all__ = [
     "PusherApi"
 ]
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

## Comparing `xia_pusher_flask-0.0.5.dist-info/METADATA` & `xia_pusher_flask-0.0.6.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-pusher-flask
-Version: 0.0.5
+Version: 0.0.6
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-pusher-flask/0.0.5/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-pusher-flask/0.0.6/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_pusher_flask-0.0.5.dist-info/RECORD` & `xia_pusher_flask-0.0.6.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_pusher_flask/__init__.py,sha256=qkSXEUiKdToZhED9fOPLQ2xjDiLu8PSTsgjRL_dXPP8,97
-xia_pusher_flask/api.cp39-win_amd64.pyd,sha256=1xrDcAotrMUjFMJ9PATEJ72mMs3Em0lGWrogAnNiBkA,253952
-xia_pusher_flask-0.0.5.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
-xia_pusher_flask-0.0.5.dist-info/METADATA,sha256=zTabXvmxs0-rnKzZNtjuNSdU4myD_G0355QgD1D0R3o,714
-xia_pusher_flask-0.0.5.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_pusher_flask-0.0.5.dist-info/top_level.txt,sha256=bwG9aPiKiGDYuKjuxyCH1xRmPzxRHfspYZ0_OOvaz90,17
-xia_pusher_flask-0.0.5.dist-info/RECORD,,
+xia_pusher_flask/__init__.py,sha256=Gt83I_8R4dwji4RUezDzWfvNfYnoBFDuixQmxterbMo,97
+xia_pusher_flask/api.cp39-win_amd64.pyd,sha256=eMMf596HSWKZ6AE5jzVoEo66IIXMzsmAnyXm52Vgwig,252928
+xia_pusher_flask-0.0.6.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_pusher_flask-0.0.6.dist-info/METADATA,sha256=SbN4oBQ45w1rgl3D-5888ABFtDjrt425kTKWAfZ0GdY,714
+xia_pusher_flask-0.0.6.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_pusher_flask-0.0.6.dist-info/top_level.txt,sha256=bwG9aPiKiGDYuKjuxyCH1xRmPzxRHfspYZ0_OOvaz90,17
+xia_pusher_flask-0.0.6.dist-info/RECORD,,
```


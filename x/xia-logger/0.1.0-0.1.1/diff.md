# Comparing `tmp/xia_logger-0.1.0-cp39-none-win_amd64.whl.zip` & `tmp/xia_logger-0.1.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 146497 bytes, number of entries: 7
--rw-r--r--  2.0 unx      160 b- defN 23-Mar-26 15:27 xia_logger/__init__.py
--rw-r--r--  2.0 unx   381952 b- defN 23-Mar-26 15:30 xia_logger/logger.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Mar-26 15:30 xia_logger-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      726 b- defN 23-Mar-26 15:30 xia_logger-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Mar-26 15:30 xia_logger-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Mar-26 15:30 xia_logger-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      576 b- defN 23-Mar-26 15:30 xia_logger-0.1.0.dist-info/RECORD
-7 files, 383676 bytes uncompressed, 145471 bytes compressed:  62.1%
+Zip file size: 146560 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      160 b- defN 23-Apr-29 16:32 xia_logger/__init__.py
+-rw-r--r--  2.0 unx   381440 b- defN 23-Apr-29 16:35 xia_logger/logger.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-29 16:35 xia_logger-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      726 b- defN 23-Apr-29 16:35 xia_logger-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-29 16:35 xia_logger-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-29 16:35 xia_logger-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      576 b- defN 23-Apr-29 16:35 xia_logger-0.1.1.dist-info/RECORD
+7 files, 383164 bytes uncompressed, 145534 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_logger/__init__.py
 Comment: 
 
 Filename: xia_logger/logger.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_logger-0.1.0.dist-info/LICENSE.txt
+Filename: xia_logger-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_logger-0.1.0.dist-info/METADATA
+Filename: xia_logger-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: xia_logger-0.1.0.dist-info/WHEEL
+Filename: xia_logger-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: xia_logger-0.1.0.dist-info/top_level.txt
+Filename: xia_logger-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_logger-0.1.0.dist-info/RECORD
+Filename: xia_logger-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_logger/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_logger.logger import Logger, HttpLogger, JsonLogger, DataLog
 
 __all__ = [
     "Logger", "HttpLogger", "JsonLogger", "DataLog"
 ]
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## Comparing `xia_logger-0.1.0.dist-info/METADATA` & `xia_logger-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-logger
-Version: 0.1.0
+Version: 0.1.1
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-logger/0.1.0/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-logger/0.1.1/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```


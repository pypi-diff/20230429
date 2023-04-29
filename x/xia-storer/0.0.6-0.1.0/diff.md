# Comparing `tmp/xia_storer-0.0.6-cp39-none-win_amd64.whl.zip` & `tmp/xia_storer-0.1.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 112203 bytes, number of entries: 7
--rw-r--r--  2.0 unx      116 b- defN 23-Feb-14 09:52 xia_storer/__init__.py
--rw-r--r--  2.0 unx   268800 b- defN 23-Feb-14 10:22 xia_storer/storer.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      155 b- defN 23-Feb-14 10:22 xia_storer-0.0.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      623 b- defN 23-Feb-14 10:22 xia_storer-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Feb-14 10:22 xia_storer-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Feb-14 10:22 xia_storer-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      576 b- defN 23-Feb-14 10:22 xia_storer-0.0.6.dist-info/RECORD
-7 files, 270380 bytes uncompressed, 111177 bytes compressed:  58.9%
+Zip file size: 112186 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      116 b- defN 23-Apr-29 16:17 xia_storer/__init__.py
+-rw-r--r--  2.0 unx   268800 b- defN 23-Apr-29 16:20 xia_storer/storer.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-29 16:20 xia_storer-0.1.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      623 b- defN 23-Apr-29 16:20 xia_storer-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-29 16:20 xia_storer-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-29 16:20 xia_storer-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      576 b- defN 23-Apr-29 16:20 xia_storer-0.1.0.dist-info/RECORD
+7 files, 270377 bytes uncompressed, 111160 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_storer/__init__.py
 Comment: 
 
 Filename: xia_storer/storer.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_storer-0.0.6.dist-info/LICENSE.txt
+Filename: xia_storer-0.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_storer-0.0.6.dist-info/METADATA
+Filename: xia_storer-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: xia_storer-0.0.6.dist-info/WHEEL
+Filename: xia_storer-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: xia_storer-0.0.6.dist-info/top_level.txt
+Filename: xia_storer-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_storer-0.0.6.dist-info/RECORD
+Filename: xia_storer-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_storer/__init__.py

```diff
@@ -2,8 +2,8 @@
 
 
 __all__ = [
     'Storer', "FileStorer"
 ]
 
 
-__version__ = "0.0.6"
+__version__ = "0.1.0"
```

## Comparing `xia_storer-0.0.6.dist-info/METADATA` & `xia_storer-0.1.0.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-storer
-Version: 0.0.6
+Version: 0.1.0
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-storer/0.0.6/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-storer/0.1.0/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_storer-0.0.6.dist-info/RECORD` & `xia_storer-0.1.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_storer/__init__.py,sha256=ljmsQ3ObuaX3Z4C0AGHOroY-1qhbih3HRH_yzddhB9U,116
-xia_storer/storer.cp39-win_amd64.pyd,sha256=Dej-ur4iCN4wi5IXqGEn3wiKu8B6QQUH2nvaYEDqCI8,268800
-xia_storer-0.0.6.dist-info/LICENSE.txt,sha256=m5FJNVsGdpkCy739qw5P9fx_HHwOxouu3PxutfTeIa8,155
-xia_storer-0.0.6.dist-info/METADATA,sha256=qC120WhdXinRwGURk8Fq4VA7arUkqKCCioaCWd8pF2E,623
-xia_storer-0.0.6.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_storer-0.0.6.dist-info/top_level.txt,sha256=qVGcZtbSEokZNMgGUQhw9e9FoXdlHNNCf412j7p_i1c,11
-xia_storer-0.0.6.dist-info/RECORD,,
+xia_storer/__init__.py,sha256=2TCDaZLe2bab7hJTZWRiI45YrqNJ4ZGSu4NGYK3XvVA,116
+xia_storer/storer.cp39-win_amd64.pyd,sha256=n2M-_pi8kX4A8pW839vdcEmNfe1FegclWLyETTSlIeE,268800
+xia_storer-0.1.0.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_storer-0.1.0.dist-info/METADATA,sha256=jT8pUnoOYNUv61V7IQqJHrDJdDDbQhhrteXnkSmz9fM,623
+xia_storer-0.1.0.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_storer-0.1.0.dist-info/top_level.txt,sha256=qVGcZtbSEokZNMgGUQhw9e9FoXdlHNNCf412j7p_i1c,11
+xia_storer-0.1.0.dist-info/RECORD,,
```


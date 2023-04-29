# Comparing `tmp/miniagent-0.0.4-py3-none-any.whl.zip` & `tmp/miniagent-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 12482 bytes, number of entries: 18
+Zip file size: 12453 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-29 08:47 miniadmin/__init__.py
 -rw-rw-r--  2.0 unx     2440 b- defN 23-Apr-29 08:47 miniadmin/admin.py
--rw-rw-r--  2.0 unx     2556 b- defN 23-Apr-29 08:47 miniagent/__init__.py
+-rw-rw-r--  2.0 unx     2556 b- defN 23-Apr-29 09:24 miniagent/__init__.py
 -rw-rw-r--  2.0 unx     1958 b- defN 23-Apr-29 08:47 miniagent/adapter.py
 -rw-rw-r--  2.0 unx     3296 b- defN 23-Apr-29 08:47 miniagent/app_config.py
 -rw-rw-r--  2.0 unx     1540 b- defN 23-Apr-29 08:47 miniagent/command_reciever.py
 -rw-rw-r--  2.0 unx      863 b- defN 23-Apr-29 08:47 miniagent/common.py
 -rw-rw-r--  2.0 unx      791 b- defN 23-Apr-29 08:47 miniagent/event_reciever.py
 -rw-rw-r--  2.0 unx     3389 b- defN 23-Apr-29 08:47 miniagent/executer.py
 -rw-rw-r--  2.0 unx      528 b- defN 23-Apr-29 08:47 miniagent/job_reciever.py
 -rw-rw-r--  2.0 unx     2216 b- defN 23-Apr-29 08:47 miniagent/message_reciever.py
 -rw-rw-r--  2.0 unx      275 b- defN 23-Apr-29 08:47 miniagent/models.py
--rw-rw-r--  2.0 unx     1063 b- defN 23-Apr-29 09:11 miniagent-0.0.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2321 b- defN 23-Apr-29 09:11 miniagent-0.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-29 09:11 miniagent-0.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       71 b- defN 23-Apr-29 09:11 miniagent-0.0.4.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       20 b- defN 23-Apr-29 09:11 miniagent-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1442 b- defN 23-Apr-29 09:11 miniagent-0.0.4.dist-info/RECORD
-18 files, 24861 bytes uncompressed, 10126 bytes compressed:  59.3%
+-rw-rw-r--  2.0 unx     1063 b- defN 23-Apr-29 09:25 miniagent-0.0.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2328 b- defN 23-Apr-29 09:25 miniagent-0.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-29 09:25 miniagent-0.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       71 b- defN 23-Apr-29 09:25 miniagent-0.0.5.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       20 b- defN 23-Apr-29 09:25 miniagent-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1442 b- defN 23-Apr-29 09:25 miniagent-0.0.5.dist-info/RECORD
+18 files, 24868 bytes uncompressed, 10097 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: miniagent/message_reciever.py
 Comment: 
 
 Filename: miniagent/models.py
 Comment: 
 
-Filename: miniagent-0.0.4.dist-info/LICENSE
+Filename: miniagent-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: miniagent-0.0.4.dist-info/METADATA
+Filename: miniagent-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: miniagent-0.0.4.dist-info/WHEEL
+Filename: miniagent-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: miniagent-0.0.4.dist-info/entry_points.txt
+Filename: miniagent-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: miniagent-0.0.4.dist-info/top_level.txt
+Filename: miniagent-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: miniagent-0.0.4.dist-info/RECORD
+Filename: miniagent-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## miniagent/__init__.py

```diff
@@ -10,15 +10,15 @@
 from datetime import datetime
 from .app_config import AppConfig
 from .executer import ExecuterCaller
 from .command_reciever import CommandsReciever
 from .event_reciever import Command
 from .message_reciever import MessageReciever
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 
 #Load configuration
 configure = AppConfig(os.getcwd())
 configure.from_pyfile('config.py')
 
 #Set logging
 """
```

## Comparing `miniagent-0.0.4.dist-info/LICENSE` & `miniagent-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `miniagent-0.0.4.dist-info/METADATA` & `miniagent-0.0.5.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: miniagent
-Version: 0.0.4
-Summary: PYPI tutorial package creation written by TeddyNote
+Version: 0.0.5
+Summary: Multi-adaptable and lightweight server framework based on Flask
 Home-page: https://github.com/tanminkwan/local-agent
 Author: tanminkwan
 Author-email: tanminkwan@gmail.com
 License: MIT
 Keywords: flask,sqlalchemy,scheduler
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Miniagent
 
-Miniagent is a multi-adaptable and lightweight application framework based on **Flask**.
+Miniagent is a multi-adaptable and lightweight server framework based on **Flask**.
 
 ## Installing
 
 Install and update using **pip**:
 `$ pip install -U miniagent`
 
 ## Example code download
```

## Comparing `miniagent-0.0.4.dist-info/RECORD` & `miniagent-0.0.5.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 miniadmin/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 miniadmin/admin.py,sha256=MejGCYRC8vHuGFRQ5xaZaVBEpio1FCaFl6xNtSkyD-k,2440
-miniagent/__init__.py,sha256=F7FSOfgHTf8JK06Qs-7ObBsCItYCMgf9Q57y4f9yd0k,2556
+miniagent/__init__.py,sha256=Qih--0DYmeLi3dQb1Qb75lHy7OHogxSeCXqAlbTWnAo,2556
 miniagent/adapter.py,sha256=uR-e9a--WaSlxbXHWFKR2Vgc2ITbInDV2io0Cmr5Wjg,1958
 miniagent/app_config.py,sha256=B-K-5ebnUIekZlrDoLdVttGzewTNjCpu6DDVmKqPB2M,3296
 miniagent/command_reciever.py,sha256=NQZbYEKNHovddJ9duKjZ9SKiV-RzhRavJQIvdgH6Q3I,1540
 miniagent/common.py,sha256=mANId-sgxiLYOva-m63hnNud0Cco-JH6JpXrSv74A5Q,863
 miniagent/event_reciever.py,sha256=DJp0TiN_pJ_BnZLfUM_hKks6QDy_OONV_rAmc6aeN-U,791
 miniagent/executer.py,sha256=y4BEMX7NLKgPARbRbNmPEhPuqlhZzgTvEP3N8nm_wC8,3389
 miniagent/job_reciever.py,sha256=xm0lD99RUkPqD3tUzvI0ZcDFgxAwcXwiGCiJHphP0Kw,528
 miniagent/message_reciever.py,sha256=zSheWN9ZSP1J79CUA-SP99cT5uvuWHvyNo5j8AQcTW0,2216
 miniagent/models.py,sha256=oEWOA0awWmcjo_nm0IVwoY9_FTkssLG6pX-oLYvFnTo,275
-miniagent-0.0.4.dist-info/LICENSE,sha256=nj6HxIMEUT6XKDHjyJYPnIS37d5NKErlNwbV0XbxcsQ,1063
-miniagent-0.0.4.dist-info/METADATA,sha256=ELKo1rAqhikihcyxB9BrX6c3CVllRfusFSj9jqoKVkg,2321
-miniagent-0.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-miniagent-0.0.4.dist-info/entry_points.txt,sha256=v6HAev-cy1ey5C3hnCdS589pljKD1wOW6zURhAq5P6Q,71
-miniagent-0.0.4.dist-info/top_level.txt,sha256=AMyT-pye0DyB9Q8Ow_lGVtXb3COCxNZoS0yIdptLgzU,20
-miniagent-0.0.4.dist-info/RECORD,,
+miniagent-0.0.5.dist-info/LICENSE,sha256=nj6HxIMEUT6XKDHjyJYPnIS37d5NKErlNwbV0XbxcsQ,1063
+miniagent-0.0.5.dist-info/METADATA,sha256=sYTcRapaoZ473C6TJDW84jV89Dx2fWKDHhaeH4TPp1s,2328
+miniagent-0.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+miniagent-0.0.5.dist-info/entry_points.txt,sha256=v6HAev-cy1ey5C3hnCdS589pljKD1wOW6zURhAq5P6Q,71
+miniagent-0.0.5.dist-info/top_level.txt,sha256=AMyT-pye0DyB9Q8Ow_lGVtXb3COCxNZoS0yIdptLgzU,20
+miniagent-0.0.5.dist-info/RECORD,,
```


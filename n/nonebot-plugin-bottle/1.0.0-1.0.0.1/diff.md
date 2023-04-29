# Comparing `tmp/nonebot_plugin_bottle-1.0.0-py3-none-any.whl.zip` & `tmp/nonebot_plugin_bottle-1.0.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 26837 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat    17111 b- defN 23-Apr-29 06:02 nonebot_plugin_bottle/__init__.py
+Zip file size: 26856 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat    17114 b- defN 23-Apr-29 10:07 nonebot_plugin_bottle/__init__.py
 -rw-rw-rw-  2.0 fat      636 b- defN 23-Apr-29 05:06 nonebot_plugin_bottle/config.py
 -rw-rw-rw-  2.0 fat    17498 b- defN 23-Apr-29 05:06 nonebot_plugin_bottle/data_source.py
--rw-rw-rw-  2.0 fat     1426 b- defN 23-Apr-29 05:06 nonebot_plugin_bottle/model.py
--rw-rw-rw-  2.0 fat    35821 b- defN 23-Apr-29 06:06 nonebot_plugin_bottle-1.0.0.dist-info/LICENCE
--rw-rw-rw-  2.0 fat     8238 b- defN 23-Apr-29 06:06 nonebot_plugin_bottle-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 06:06 nonebot_plugin_bottle-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-29 06:06 nonebot_plugin_bottle-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      816 b- defN 23-Apr-29 06:06 nonebot_plugin_bottle-1.0.0.dist-info/RECORD
-9 files, 81660 bytes uncompressed, 25413 bytes compressed:  68.9%
+-rw-rw-rw-  2.0 fat     1426 b- defN 23-Apr-29 10:05 nonebot_plugin_bottle/model.py
+-rw-rw-rw-  2.0 fat    35821 b- defN 23-Apr-29 10:08 nonebot_plugin_bottle-1.0.0.1.dist-info/LICENCE
+-rw-rw-rw-  2.0 fat     8240 b- defN 23-Apr-29 10:08 nonebot_plugin_bottle-1.0.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 10:08 nonebot_plugin_bottle-1.0.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-29 10:08 nonebot_plugin_bottle-1.0.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      826 b- defN 23-Apr-29 10:08 nonebot_plugin_bottle-1.0.0.1.dist-info/RECORD
+9 files, 81675 bytes uncompressed, 25412 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: nonebot_plugin_bottle/data_source.py
 Comment: 
 
 Filename: nonebot_plugin_bottle/model.py
 Comment: 
 
-Filename: nonebot_plugin_bottle-1.0.0.dist-info/LICENCE
+Filename: nonebot_plugin_bottle-1.0.0.1.dist-info/LICENCE
 Comment: 
 
-Filename: nonebot_plugin_bottle-1.0.0.dist-info/METADATA
+Filename: nonebot_plugin_bottle-1.0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: nonebot_plugin_bottle-1.0.0.dist-info/WHEEL
+Filename: nonebot_plugin_bottle-1.0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: nonebot_plugin_bottle-1.0.0.dist-info/top_level.txt
+Filename: nonebot_plugin_bottle-1.0.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: nonebot_plugin_bottle-1.0.0.dist-info/RECORD
+Filename: nonebot_plugin_bottle-1.0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nonebot_plugin_bottle/__init__.py

```diff
@@ -51,15 +51,15 @@
     漂流瓶黑名单 [QQ / 群聊] [QQ号 / 群号]
     漂流瓶详情 [漂流瓶编号]
 """.strip(),
     extra={
         "unique_name": "nonebot_plugin_bottle",
         "example": "扔漂流瓶\n寄漂流瓶\n捡漂流瓶\n评论漂流瓶\n举报漂流瓶\n查看漂流瓶\n删除漂流瓶",
         "author": "Todysheep",
-        "version": "1.0.0,
+        "version": "1.0.0.1",
     },
 )
 
 throw = on_command(
     "扔漂流瓶", aliases=set(["寄漂流瓶", "丢漂流瓶"]), permission=GROUP, priority=100, block=True
 )
 get = on_command("捡漂流瓶", priority=100, block=True)
```

## Comparing `nonebot_plugin_bottle-1.0.0.dist-info/LICENCE` & `nonebot_plugin_bottle-1.0.0.1.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `nonebot_plugin_bottle-1.0.0.dist-info/METADATA` & `nonebot_plugin_bottle-1.0.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bottle
-Version: 1.0.0
+Version: 1.0.0.1
 Summary: Bottle post plugin in Nonebot
 Home-page: https://github.com/Todysheep/nonebot_plugin_bottle
 Author: Todysheep
 Author-email: todysheep@163.com
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```


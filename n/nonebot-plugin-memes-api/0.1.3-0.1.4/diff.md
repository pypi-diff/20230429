# Comparing `tmp/nonebot_plugin_memes_api-0.1.3.tar.gz` & `tmp/nonebot_plugin_memes_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_memes_api-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_memes_api-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_memes_api-0.1.3.tar` & `nonebot_plugin_memes_api-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-04-01 15:23:53.779588 nonebot_plugin_memes_api-0.1.3/LICENSE
--rw-r--r--   0        0        0     3310 2023-04-01 15:23:53.779588 nonebot_plugin_memes_api-0.1.3/README.md
--rw-r--r--   0        0        0    15014 2023-04-01 15:23:53.779588 nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/__init__.py
--rw-r--r--   0        0        0      532 2023-04-01 15:23:53.779588 nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/config.py
--rw-r--r--   0        0        0      152 2023-04-01 15:23:53.779588 nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/data_source/__init__.py
--rw-r--r--   0        0        0     2857 2023-04-01 15:23:53.779588 nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/data_source/image_source.py
--rw-r--r--   0        0        0      375 2023-04-01 15:23:53.779588 nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/data_source/user_id.py
--rw-r--r--   0        0        0     1978 2023-04-01 15:23:53.779588 nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/data_source/user_info.py
--rw-r--r--   0        0        0     7468 2023-04-01 15:23:53.783588 nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/depends.py
--rw-r--r--   0        0        0      967 2023-04-01 15:23:53.783588 nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/exception.py
--rw-r--r--   0        0        0     5047 2023-04-01 15:23:53.783588 nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/manager.py
--rw-r--r--   0        0        0     4999 2023-04-01 15:23:53.783588 nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/request.py
--rw-r--r--   0        0        0     3122 2023-04-01 15:23:53.783588 nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/rule.py
--rw-r--r--   0        0        0     2415 2023-04-01 15:23:53.783588 nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/utils.py
--rw-r--r--   0        0        0      709 2023-04-01 15:23:53.783588 nonebot_plugin_memes_api-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4245 1970-01-01 00:00:00.000000 nonebot_plugin_memes_api-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3310 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/README.md
+-rw-r--r--   0        0        0    15014 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/__init__.py
+-rw-r--r--   0        0        0      532 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/config.py
+-rw-r--r--   0        0        0      152 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/data_source/__init__.py
+-rw-r--r--   0        0        0     2857 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/data_source/image_source.py
+-rw-r--r--   0        0        0      375 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/data_source/user_id.py
+-rw-r--r--   0        0        0     1978 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/data_source/user_info.py
+-rw-r--r--   0        0        0     7468 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/depends.py
+-rw-r--r--   0        0        0      967 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/exception.py
+-rw-r--r--   0        0        0     5047 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/manager.py
+-rw-r--r--   0        0        0     4999 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/request.py
+-rw-r--r--   0        0        0     3135 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/rule.py
+-rw-r--r--   0        0        0     2415 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/utils.py
+-rw-r--r--   0        0        0      709 2023-04-29 06:15:10.975005 nonebot_plugin_memes_api-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4245 1970-01-01 00:00:00.000000 nonebot_plugin_memes_api-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_memes_api-0.1.3/LICENSE` & `nonebot_plugin_memes_api-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.3/README.md` & `nonebot_plugin_memes_api-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/__init__.py` & `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 __plugin_meta__ = PluginMetadata(
     name="表情包制作",
     description="制作各种沙雕表情包",
     usage="发送“表情包制作”查看表情包列表",
     extra={
         "unique_name": "memes_api",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.1.3",
+        "version": "0.1.4",
     },
 )
 
 memes_cache_dir = get_cache_dir("nonebot_plugin_memes_api")
 
 
 PERM_EDIT = GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND | PRIVATE | SUPERUSER
```

### Comparing `nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/config.py` & `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/data_source/image_source.py` & `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/data_source/image_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/data_source/user_info.py` & `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/data_source/user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/depends.py` & `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/depends.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/exception.py` & `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/manager.py` & `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/request.py` & `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/rule.py` & `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             return True
         return False
 
     return Rule(checker)
 
 
 def regex_rule(patterns: List[str]) -> Rule:
-    start = re.escape("|".join(command_start))
+    start = "|".join([re.escape(s) for s in command_start])
     pattern = "|".join([rf"(?:{p})" for p in patterns])
 
     def checker(event: Event, state: T_State) -> bool:
         if not (message := event.get_message()):
             return False
         message_seg: MessageSegment = message[0]
         if not message_seg.is_text():
```

### Comparing `nonebot_plugin_memes_api-0.1.3/nonebot_plugin_memes_api/utils.py` & `nonebot_plugin_memes_api-0.1.4/nonebot_plugin_memes_api/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes_api-0.1.3/pyproject.toml` & `nonebot_plugin_memes_api-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_memes_api"
-version = "0.1.3"
+version = "0.1.4"
 description = "Nonebot2 plugin for making memes"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-memes-api"
 repository = "https://github.com/noneplugin/nonebot-plugin-memes-api"
```

### Comparing `nonebot_plugin_memes_api-0.1.3/PKG-INFO` & `nonebot_plugin_memes_api-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-memes-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: Nonebot2 plugin for making memes
 Home-page: https://github.com/noneplugin/nonebot-plugin-memes-api
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-memes-api Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-memes-api Version: 0.1.4 Summary:
 Nonebot2 plugin for making memes Home-page: https://github.com/noneplugin/
 nonebot-plugin-memes-api License: MIT Author: meetwq Author-email:
 meetwq@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: httpx
```


# Comparing `tmp/nonebot_plugin_memes-0.4.5.tar.gz` & `tmp/nonebot_plugin_memes-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_memes-0.4.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_memes-0.4.6.tar", max compression
```

## Comparing `nonebot_plugin_memes-0.4.5.tar` & `nonebot_plugin_memes-0.4.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-04-01 15:04:23.949057 nonebot_plugin_memes-0.4.5/LICENSE
--rw-r--r--   0        0        0     6164 2023-04-01 15:04:23.949057 nonebot_plugin_memes-0.4.5/README.md
--rw-r--r--   0        0        0    14799 2023-04-01 15:04:23.949057 nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/__init__.py
--rw-r--r--   0        0        0      523 2023-04-01 15:04:23.949057 nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/config.py
--rw-r--r--   0        0        0      152 2023-04-01 15:04:23.949057 nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/data_source/__init__.py
--rw-r--r--   0        0        0     2857 2023-04-01 15:04:23.949057 nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/data_source/image_source.py
--rw-r--r--   0        0        0      375 2023-04-01 15:04:23.949057 nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/data_source/user_id.py
--rw-r--r--   0        0        0     1978 2023-04-01 15:04:23.949057 nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/data_source/user_info.py
--rw-r--r--   0        0        0     7507 2023-04-01 15:04:23.949057 nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/depends.py
--rw-r--r--   0        0        0      155 2023-04-01 15:04:23.949057 nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/exception.py
--rw-r--r--   0        0        0     4858 2023-04-01 15:04:23.949057 nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/manager.py
--rw-r--r--   0        0        0     3122 2023-04-01 15:04:23.949057 nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/rule.py
--rw-r--r--   0        0        0     2561 2023-04-01 15:04:23.949057 nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/utils.py
--rw-r--r--   0        0        0      752 2023-04-01 15:04:23.953057 nonebot_plugin_memes-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     7176 1970-01-01 00:00:00.000000 nonebot_plugin_memes-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/LICENSE
+-rw-r--r--   0        0        0     6459 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/README.md
+-rw-r--r--   0        0        0    14799 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/__init__.py
+-rw-r--r--   0        0        0      523 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/config.py
+-rw-r--r--   0        0        0      152 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/data_source/__init__.py
+-rw-r--r--   0        0        0     2857 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/data_source/image_source.py
+-rw-r--r--   0        0        0      375 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/data_source/user_id.py
+-rw-r--r--   0        0        0     1978 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/data_source/user_info.py
+-rw-r--r--   0        0        0     7507 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/depends.py
+-rw-r--r--   0        0        0      155 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/exception.py
+-rw-r--r--   0        0        0     4858 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/manager.py
+-rw-r--r--   0        0        0     3135 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/rule.py
+-rw-r--r--   0        0        0     2561 2023-04-29 06:11:31.399272 nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/utils.py
+-rw-r--r--   0        0        0      752 2023-04-29 06:11:31.403272 nonebot_plugin_memes-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     7471 1970-01-01 00:00:00.000000 nonebot_plugin_memes-0.4.6/PKG-INFO
```

### Comparing `nonebot_plugin_memes-0.4.5/LICENSE` & `nonebot_plugin_memes-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.5/README.md` & `nonebot_plugin_memes-0.4.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 并按照 [NoneBot 加载插件](https://v2.nonebot.dev/docs/tutorial/plugin/load-plugin) 加载插件
 
 
 #### 字体和资源
 
 插件默认在启动时会检查 [meme-generator](https://github.com/MeetWq/meme-generator) 所需的图片资源
 
-需按照 [meme-generator 字体安装](https://github.com/MeetWq/meme-generator#字体安装) 自行安装字体
+需按照 [meme-generator 字体安装](https://github.com/MeetWq/meme-generator/blob/main/docs/install.md#字体安装) 自行安装字体
 
 <div align="left">
   <img src="https://s2.loli.net/2023/03/10/Y81ACvu2pGLW4Qc.jpg" width="150" />
 </div>
 
 
 ### 配置项
@@ -101,19 +101,26 @@
 
 ### 使用
 
 **以下命令需要加 [NoneBot 命令前缀](https://v2.nonebot.dev/docs/api/config#Config-command_start) (默认为`/`)，可自行添加空字符**
 
 #### 表情列表
 
-发送 “表情包制作” 显示如下图所示的表情列表：
+发送 “表情包制作” 查看表情列表
 
-<div align="left">
-  <img src="https://s2.loli.net/2023/03/10/3BSlTXwCIycWUmK.jpg" width="550" />
-</div>
+> **Note**
+>
+> 插件会缓存生成的表情列表图片以避免重复生成
+>
+> 若因为字体没安装好等原因导致生成的图片不正常，需要删除缓存的图片
+>
+> 缓存路径：
+> - Windows: `C:\Users\<username>\AppData\Local\nonebot2\Cache\nonebot_plugin_memes`
+> - Linux: `~/.cache/nonebot2/nonebot_plugin_memes`
+> - Mac: `~/Library/Caches/nonebot2/nonebot_plugin_memes`
 
 
 #### 表情帮助
 
 - 发送 “表情详情 + 表情名/关键词” 查看 表情详细信息 和 表情预览
 
 示例：
```

#### html2text {}

```diff
@@ -12,16 +12,16 @@
 æä»¶ç«¯ä¸ `meme-generator` åå¼é¨ç½² > > `nonebot-plugin-memes-api` ä¸
 `nonebot-plugin-memes` åè½ä¸åºæ¬ä¸è´ ### å®è£ - ä½¿ç¨ nb-cli ``` nb
 plugin install nonebot_plugin_memes ``` - ä½¿ç¨ pip ``` pip install
 nonebot_plugin_memes ``` å¹¶æç§ [NoneBot å è½½æä»¶](https://
 v2.nonebot.dev/docs/tutorial/plugin/load-plugin) å è½½æä»¶ ####
 å­ä½åèµæº æä»¶é»è®¤å¨å¯å¨æ¶ä¼æ£æ¥ [meme-generator](https://
 github.com/MeetWq/meme-generator) æéçå¾çèµæº éæç§ [meme-
-generator å­ä½å®è£](https://github.com/MeetWq/meme-generator#å­ä½å®è£)
-èªè¡å®è£å­ä½
+generator å­ä½å®è£](https://github.com/MeetWq/meme-generator/blob/main/
+docs/install.md#å­ä½å®è£) èªè¡å®è£å­ä½
 [https://s2.loli.net/2023/03/10/Y81ACvu2pGLW4Qc.jpg]
 ### éç½®é¡¹ > ä»¥ä¸éç½®é¡¹å¯å¨ `.env.*` æä»¶ä¸­è®¾ç½®ï¼å·ä½åè
 [NoneBot éç½®æ¹å¼](https://v2.nonebot.dev/docs/tutorial/
 configuration#%E9%85%8D%E7%BD%AE%E6%96%B9%E5%BC%8F) #### `memes_command_start`
 - ç±»åï¼`List[str]` - é»è®¤ï¼`[]` -
 è¯´æï¼å½ä»¤åç¼ï¼è¥ä¸éç½®åä½¿ç¨ [NoneBot å½ä»¤åç¼](https://
 v2.nonebot.dev/docs/api/config#Config-command_start) ####
@@ -40,18 +40,22 @@
 #### `memes_use_sender_when_no_image` - ç±»åï¼`bool` - é»è®¤ï¼`False` -
 è¯´æï¼å¨è¡¨æéè¦è³å°1å¼ å¾ä¸æ²¡æè¾å¥å¾çæ¶ï¼æ¯å¦ä½¿ç¨åéèçå¤´åï¼è°¨æä½¿ç¨ï¼å®¹æè¯¯è§¦åï¼
 #### `memes_use_default_when_no_text` - ç±»åï¼`bool` - é»è®¤ï¼`False` -
 è¯´æï¼å¨è¡¨æéè¦è³å°1æ®µæå­ä¸æ²¡æè¾å¥æå­æ¶ï¼æ¯å¦ä½¿ç¨é»è®¤æå­ï¼è°¨æä½¿ç¨ï¼å®¹æè¯¯è§¦åï¼
 ### ä½¿ç¨ **ä»¥ä¸å½ä»¤éè¦å  [NoneBot å½ä»¤åç¼](https://
 v2.nonebot.dev/docs/api/config#Config-command_start) (é»è®¤ä¸º`/
 `)ï¼å¯èªè¡æ·»å ç©ºå­ç¬¦** #### è¡¨æåè¡¨ åé âè¡¨æåå¶ä½â
-æ¾ç¤ºå¦ä¸å¾æç¤ºçè¡¨æåè¡¨ï¼
-[https://s2.loli.net/2023/03/10/3BSlTXwCIycWUmK.jpg]
-#### è¡¨æå¸®å© - åé âè¡¨æè¯¦æ + è¡¨æå/å³é®è¯â æ¥ç
-è¡¨æè¯¦ç»ä¿¡æ¯ å è¡¨æé¢è§ ç¤ºä¾ï¼
+æ¥çè¡¨æåè¡¨ > **Note** > >
+æä»¶ä¼ç¼å­çæçè¡¨æåè¡¨å¾çä»¥é¿åéå¤çæ > >
+è¥å ä¸ºå­ä½æ²¡å®è£å¥½ç­åå å¯¼è´çæçå¾çä¸æ­£å¸¸ï¼éè¦å é¤ç¼å­çå¾ç
+> > ç¼å­è·¯å¾ï¼ > - Windows: `C:
+\Users\\AppData\Local\nonebot2\Cache\nonebot_plugin_memes` > - Linux:
+`~/.cache/nonebot2/nonebot_plugin_memes` > - Mac: `~/Library/Caches/nonebot2/
+nonebot_plugin_memes` #### è¡¨æå¸®å© - åé âè¡¨æè¯¦æ + è¡¨æå/
+å³é®è¯â æ¥ç è¡¨æè¯¦ç»ä¿¡æ¯ å è¡¨æé¢è§ ç¤ºä¾ï¼
 [https://s2.loli.net/2023/03/10/1glyUrwELCHMfkT.png]
 #### è¡¨æåå¼å³ ç¾¤ä¸» / ç®¡çå / è¶çº§ç¨æ·
 å¯ä»¥å¯ç¨æç¦ç¨æäºè¡¨æå åé `å¯ç¨è¡¨æ/ç¦ç¨è¡¨æ
 [è¡¨æå/è¡¨æå³é®è¯]`ï¼å¦ï¼`ç¦ç¨è¡¨æ æ¸` è¶çº§ç¨æ·
 å¯ä»¥è®¾ç½®æä¸ªè¡¨æåçç®¡æ§æ¨¡å¼ï¼é»åå/ç½ååï¼ åé
 `å¨å±å¯ç¨è¡¨æ [è¡¨æå/è¡¨æå³é®è¯]`
 å¯å°è¡¨æè®¾ä¸ºé»ååæ¨¡å¼ï¼ åé `å¨å±ç¦ç¨è¡¨æ [è¡¨æå/
```

### Comparing `nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/__init__.py` & `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 __plugin_meta__ = PluginMetadata(
     name="表情包制作",
     description="制作各种沙雕表情包",
     usage="发送“表情包制作”查看表情包列表",
     extra={
         "unique_name": "memes",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.4.5",
+        "version": "0.4.6",
     },
 )
 
 memes_cache_dir = get_cache_dir("nonebot_plugin_memes")
 
 
 PERM_EDIT = GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND | PRIVATE | SUPERUSER
```

### Comparing `nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/config.py` & `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/data_source/image_source.py` & `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/data_source/image_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/data_source/user_info.py` & `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/data_source/user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/depends.py` & `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/depends.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/manager.py` & `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/rule.py` & `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/rule.py`

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

### Comparing `nonebot_plugin_memes-0.4.5/nonebot_plugin_memes/utils.py` & `nonebot_plugin_memes-0.4.6/nonebot_plugin_memes/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_memes-0.4.5/pyproject.toml` & `nonebot_plugin_memes-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_memes"
-version = "0.4.5"
+version = "0.4.6"
 description = "Nonebot2 plugin for making memes"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-memes"
 repository = "https://github.com/noneplugin/nonebot-plugin-memes"
```

### Comparing `nonebot_plugin_memes-0.4.5/PKG-INFO` & `nonebot_plugin_memes-0.4.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-memes
-Version: 0.4.5
+Version: 0.4.6
 Summary: Nonebot2 plugin for making memes
 Home-page: https://github.com/noneplugin/nonebot-plugin-memes
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -73,15 +73,15 @@
 并按照 [NoneBot 加载插件](https://v2.nonebot.dev/docs/tutorial/plugin/load-plugin) 加载插件
 
 
 #### 字体和资源
 
 插件默认在启动时会检查 [meme-generator](https://github.com/MeetWq/meme-generator) 所需的图片资源
 
-需按照 [meme-generator 字体安装](https://github.com/MeetWq/meme-generator#字体安装) 自行安装字体
+需按照 [meme-generator 字体安装](https://github.com/MeetWq/meme-generator/blob/main/docs/install.md#字体安装) 自行安装字体
 
 <div align="left">
   <img src="https://s2.loli.net/2023/03/10/Y81ACvu2pGLW4Qc.jpg" width="150" />
 </div>
 
 
 ### 配置项
@@ -126,19 +126,26 @@
 
 ### 使用
 
 **以下命令需要加 [NoneBot 命令前缀](https://v2.nonebot.dev/docs/api/config#Config-command_start) (默认为`/`)，可自行添加空字符**
 
 #### 表情列表
 
-发送 “表情包制作” 显示如下图所示的表情列表：
+发送 “表情包制作” 查看表情列表
 
-<div align="left">
-  <img src="https://s2.loli.net/2023/03/10/3BSlTXwCIycWUmK.jpg" width="550" />
-</div>
+> **Note**
+>
+> 插件会缓存生成的表情列表图片以避免重复生成
+>
+> 若因为字体没安装好等原因导致生成的图片不正常，需要删除缓存的图片
+>
+> 缓存路径：
+> - Windows: `C:\Users\<username>\AppData\Local\nonebot2\Cache\nonebot_plugin_memes`
+> - Linux: `~/.cache/nonebot2/nonebot_plugin_memes`
+> - Mac: `~/Library/Caches/nonebot2/nonebot_plugin_memes`
 
 
 #### 表情帮助
 
 - 发送 “表情详情 + 表情名/关键词” 查看 表情详细信息 和 表情预览
 
 示例：
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-memes Version: 0.4.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-memes Version: 0.4.6 Summary:
 Nonebot2 plugin for making memes Home-page: https://github.com/noneplugin/
 nonebot-plugin-memes License: MIT Author: meetwq Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-
@@ -26,16 +26,16 @@
 æä»¶ç«¯ä¸ `meme-generator` åå¼é¨ç½² > > `nonebot-plugin-memes-api` ä¸
 `nonebot-plugin-memes` åè½ä¸åºæ¬ä¸è´ ### å®è£ - ä½¿ç¨ nb-cli ``` nb
 plugin install nonebot_plugin_memes ``` - ä½¿ç¨ pip ``` pip install
 nonebot_plugin_memes ``` å¹¶æç§ [NoneBot å è½½æä»¶](https://
 v2.nonebot.dev/docs/tutorial/plugin/load-plugin) å è½½æä»¶ ####
 å­ä½åèµæº æä»¶é»è®¤å¨å¯å¨æ¶ä¼æ£æ¥ [meme-generator](https://
 github.com/MeetWq/meme-generator) æéçå¾çèµæº éæç§ [meme-
-generator å­ä½å®è£](https://github.com/MeetWq/meme-generator#å­ä½å®è£)
-èªè¡å®è£å­ä½
+generator å­ä½å®è£](https://github.com/MeetWq/meme-generator/blob/main/
+docs/install.md#å­ä½å®è£) èªè¡å®è£å­ä½
 [https://s2.loli.net/2023/03/10/Y81ACvu2pGLW4Qc.jpg]
 ### éç½®é¡¹ > ä»¥ä¸éç½®é¡¹å¯å¨ `.env.*` æä»¶ä¸­è®¾ç½®ï¼å·ä½åè
 [NoneBot éç½®æ¹å¼](https://v2.nonebot.dev/docs/tutorial/
 configuration#%E9%85%8D%E7%BD%AE%E6%96%B9%E5%BC%8F) #### `memes_command_start`
 - ç±»åï¼`List[str]` - é»è®¤ï¼`[]` -
 è¯´æï¼å½ä»¤åç¼ï¼è¥ä¸éç½®åä½¿ç¨ [NoneBot å½ä»¤åç¼](https://
 v2.nonebot.dev/docs/api/config#Config-command_start) ####
@@ -54,18 +54,22 @@
 #### `memes_use_sender_when_no_image` - ç±»åï¼`bool` - é»è®¤ï¼`False` -
 è¯´æï¼å¨è¡¨æéè¦è³å°1å¼ å¾ä¸æ²¡æè¾å¥å¾çæ¶ï¼æ¯å¦ä½¿ç¨åéèçå¤´åï¼è°¨æä½¿ç¨ï¼å®¹æè¯¯è§¦åï¼
 #### `memes_use_default_when_no_text` - ç±»åï¼`bool` - é»è®¤ï¼`False` -
 è¯´æï¼å¨è¡¨æéè¦è³å°1æ®µæå­ä¸æ²¡æè¾å¥æå­æ¶ï¼æ¯å¦ä½¿ç¨é»è®¤æå­ï¼è°¨æä½¿ç¨ï¼å®¹æè¯¯è§¦åï¼
 ### ä½¿ç¨ **ä»¥ä¸å½ä»¤éè¦å  [NoneBot å½ä»¤åç¼](https://
 v2.nonebot.dev/docs/api/config#Config-command_start) (é»è®¤ä¸º`/
 `)ï¼å¯èªè¡æ·»å ç©ºå­ç¬¦** #### è¡¨æåè¡¨ åé âè¡¨æåå¶ä½â
-æ¾ç¤ºå¦ä¸å¾æç¤ºçè¡¨æåè¡¨ï¼
-[https://s2.loli.net/2023/03/10/3BSlTXwCIycWUmK.jpg]
-#### è¡¨æå¸®å© - åé âè¡¨æè¯¦æ + è¡¨æå/å³é®è¯â æ¥ç
-è¡¨æè¯¦ç»ä¿¡æ¯ å è¡¨æé¢è§ ç¤ºä¾ï¼
+æ¥çè¡¨æåè¡¨ > **Note** > >
+æä»¶ä¼ç¼å­çæçè¡¨æåè¡¨å¾çä»¥é¿åéå¤çæ > >
+è¥å ä¸ºå­ä½æ²¡å®è£å¥½ç­åå å¯¼è´çæçå¾çä¸æ­£å¸¸ï¼éè¦å é¤ç¼å­çå¾ç
+> > ç¼å­è·¯å¾ï¼ > - Windows: `C:
+\Users\\AppData\Local\nonebot2\Cache\nonebot_plugin_memes` > - Linux:
+`~/.cache/nonebot2/nonebot_plugin_memes` > - Mac: `~/Library/Caches/nonebot2/
+nonebot_plugin_memes` #### è¡¨æå¸®å© - åé âè¡¨æè¯¦æ + è¡¨æå/
+å³é®è¯â æ¥ç è¡¨æè¯¦ç»ä¿¡æ¯ å è¡¨æé¢è§ ç¤ºä¾ï¼
 [https://s2.loli.net/2023/03/10/1glyUrwELCHMfkT.png]
 #### è¡¨æåå¼å³ ç¾¤ä¸» / ç®¡çå / è¶çº§ç¨æ·
 å¯ä»¥å¯ç¨æç¦ç¨æäºè¡¨æå åé `å¯ç¨è¡¨æ/ç¦ç¨è¡¨æ
 [è¡¨æå/è¡¨æå³é®è¯]`ï¼å¦ï¼`ç¦ç¨è¡¨æ æ¸` è¶çº§ç¨æ·
 å¯ä»¥è®¾ç½®æä¸ªè¡¨æåçç®¡æ§æ¨¡å¼ï¼é»åå/ç½ååï¼ åé
 `å¨å±å¯ç¨è¡¨æ [è¡¨æå/è¡¨æå³é®è¯]`
 å¯å°è¡¨æè®¾ä¸ºé»ååæ¨¡å¼ï¼ åé `å¨å±ç¦ç¨è¡¨æ [è¡¨æå/
```


# Comparing `tmp/nonebot-plugin-fuckyou-0.1.2.tar.gz` & `tmp/nonebot-plugin-fuckyou-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-fuckyou-0.1.2.tar", last modified: Sat Apr 22 14:09:31 2023, max compression
+gzip compressed data, was "nonebot-plugin-fuckyou-0.1.3.tar", last modified: Sat Apr 29 16:04:32 2023, max compression
```

## Comparing `nonebot-plugin-fuckyou-0.1.2.tar` & `nonebot-plugin-fuckyou-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-04-22 14:09:22.133566 nonebot-plugin-fuckyou-0.1.2/LICENSE
--rw-r--r--   0        0        0     4237 2023-04-22 14:09:22.133566 nonebot-plugin-fuckyou-0.1.2/README.md
--rw-r--r--   0        0        0      318 2023-04-22 14:09:22.133566 nonebot-plugin-fuckyou-0.1.2/nonebot_plugin_fuckyou/__init__.py
--rw-r--r--   0        0        0     1669 2023-04-22 14:09:22.133566 nonebot-plugin-fuckyou-0.1.2/nonebot_plugin_fuckyou/__main__.py
--rw-r--r--   0        0        0      363 2023-04-22 14:09:22.133566 nonebot-plugin-fuckyou-0.1.2/nonebot_plugin_fuckyou/config.py
--rw-r--r--   0        0        0   221958 2023-04-22 14:09:22.137565 nonebot-plugin-fuckyou-0.1.2/nonebot_plugin_fuckyou/const.py
--rw-r--r--   0        0        0     1121 2023-04-22 14:09:22.137565 nonebot-plugin-fuckyou-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4576 1970-01-01 00:00:00.000000 nonebot-plugin-fuckyou-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-29 16:04:18.239304 nonebot-plugin-fuckyou-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4503 2023-04-29 16:04:18.239304 nonebot-plugin-fuckyou-0.1.3/README.md
+-rw-r--r--   0        0        0      318 2023-04-29 16:04:18.239304 nonebot-plugin-fuckyou-0.1.3/nonebot_plugin_fuckyou/__init__.py
+-rw-r--r--   0        0        0     1851 2023-04-29 16:04:18.239304 nonebot-plugin-fuckyou-0.1.3/nonebot_plugin_fuckyou/__main__.py
+-rw-r--r--   0        0        0      439 2023-04-29 16:04:18.239304 nonebot-plugin-fuckyou-0.1.3/nonebot_plugin_fuckyou/config.py
+-rw-r--r--   0        0        0   221958 2023-04-29 16:04:18.243305 nonebot-plugin-fuckyou-0.1.3/nonebot_plugin_fuckyou/const.py
+-rw-r--r--   0        0        0     1121 2023-04-29 16:04:18.243305 nonebot-plugin-fuckyou-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 nonebot-plugin-fuckyou-0.1.3/PKG-INFO
```

### Comparing `nonebot-plugin-fuckyou-0.1.2/LICENSE` & `nonebot-plugin-fuckyou-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fuckyou-0.1.2/README.md` & `nonebot-plugin-fuckyou-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,24 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-fuckyou
+Version: 0.1.3
+Summary: A NoneBot2 plugin designed for curse users
+License: MIT
+Author-email: student_2333 <lgc2333@126.com>
+Requires-Python: >=3.8,<4.0
+Provides-Extra: dev
+Project-URL: homepage, https://github.com/lgc2333/nonebot-plugin-fuckyou
+Description-Content-Type: text/markdown
+
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
-  <img src="https://media.githubusercontent.com/media/lgc-NB2Dev/readme/main/fuckyou/logo.png" width="180" height="180" alt="NoneBotPluginLogo">
+  <img src="https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/fuckyou/logo.png" width="180" height="180" alt="NoneBotPluginLogo">
 </a>
 
 <p>
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
 </p>
 
 # NoneBot-Plugin-FuckYou
@@ -107,15 +118,17 @@
 
 |         配置项         | 必填 | 默认值  |                          说明                          |
 | :--------------------: | :--: | :-----: | :----------------------------------------------------: |
 |    `FUCKYOU_GENTLE`    |  否  | `True`  |                    是否启用温柔词库                    |
 |   `FUCKYOU_VIOLENT`    |  否  | `False` | **慎用**，是否启用攻击性极强的暴力词库，**后果自负**！ |
 |     `FUCKYOU_TOME`     |  否  | `True`  |             是否只有 @机器人 时才会骂回去              |
 | `FUCKYOU_EXTEND_WORDS` |  否  |  `[]`   |                   要额外添加的触发词                   |
-|    `FUCKYOU_BLOCK`     |  否  | `False`  |                   是否阻断 Matcher                   |
+|    `FUCKYOU_BLOCK`     |  否  | `False` |                    是否阻断 Matcher                    |
+|  `FUCKYOU_BLACKLIST`   |  否  |  `[]`   |            插件忽略的用户列表（字符串列表）            |
+|   `FUCKYOU_BL_TO_WL`   |  否  | `False` |           是否将用户黑名单翻转变为白名单判断           |
 
 ## 🎉 使用
 
 直接 @Bot 对骂即可，插件为关键词检测，触发关键词可以看看 [const.py](./nonebot_plugin_fuckyou/const.py)
 
 理论支持所有 adapter
 
@@ -142,14 +155,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.1.3
+
+- 添加两个配置项
+
 ### 0.1.2
 
 - 添加一个配置项
 
 ### 0.1.1
 
 - 添加几个配置项
+
```

#### html2text {}

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1 Name: nonebot-plugin-fuckyou Version: 0.1.3 Summary: A
+NoneBot2 plugin designed for curse users License: MIT Author-email:
+student_2333
+126.com> Requires-Python: >=3.8,<4.0 Provides-Extra: dev Project-URL: homepage,
+https://github.com/lgc2333/nonebot-plugin-fuckyou Description-Content-Type:
+text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # NoneBot-Plugin-FuckYou _ð ä½ æå ä¸ª ð´ï¼è¿ä¹çï¼ ð_ [license]
                   [pypi] [python] [pypi_download] [wakatime]
 ## ð ä»ç» _10 åéç´§æ¥å¼åçæä»¶ï¼è¯¯_ NoneBot2
 éªäººæä»¶ï¼æ»å»æ§æå¼º æä»¶è¯åºæ¥æºï¼[xiaoye12123/js](https://
 gitee.com/xiaoye12123/js) ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸**
@@ -19,19 +25,22 @@
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
 è¯´æ | | :--------------------: | :--: | :-----: | :-------------------------
 ---------------------------: | | `FUCKYOU_GENTLE` | å¦ | `True` |
 æ¯å¦å¯ç¨æ¸©æè¯åº | | `FUCKYOU_VIOLENT` | å¦ | `False` |
 **æç¨**ï¼æ¯å¦å¯ç¨æ»å»æ§æå¼ºçæ´åè¯åºï¼**åæèªè´**ï¼ |
 | `FUCKYOU_TOME` | å¦ | `True` | æ¯å¦åªæ @æºå¨äºº æ¶æä¼éªåå» |
 | `FUCKYOU_EXTEND_WORDS` | å¦ | `[]` | è¦é¢å¤æ·»å çè§¦åè¯ | |
-`FUCKYOU_BLOCK` | å¦ | `False` | æ¯å¦é»æ­ Matcher | ## ð ä½¿ç¨ ç´æ¥
+`FUCKYOU_BLOCK` | å¦ | `False` | æ¯å¦é»æ­ Matcher | | `FUCKYOU_BLACKLIST`
+| å¦ | `[]` | æä»¶å¿½ç¥çç¨æ·åè¡¨ï¼å­ç¬¦ä¸²åè¡¨ï¼ | |
+`FUCKYOU_BL_TO_WL` | å¦ | `False` |
+æ¯å¦å°ç¨æ·é»ååç¿»è½¬åä¸ºç½ååå¤æ­ | ## ð ä½¿ç¨ ç´æ¥
 @Bot å¯¹éªå³å¯ï¼æä»¶ä¸ºå³é®è¯æ£æµï¼è§¦åå³é®è¯å¯ä»¥çç
 [const.py](./nonebot_plugin_fuckyou/const.py) çè®ºæ¯æææ adapter ##
 ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
 å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [`xiaoye12123/js`](https://gitee.com/xiaoye12123/
 js) - æ»å»æ§æå¼ºçåå¤è¯åºæ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.2 - æ·»å ä¸ä¸ªéç½®é¡¹ ###
-0.1.1 - æ·»å å ä¸ªéç½®é¡¹
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.3 - æ·»å ä¸¤ä¸ªéç½®é¡¹ ###
+0.1.2 - æ·»å ä¸ä¸ªéç½®é¡¹ ### 0.1.1 - æ·»å å ä¸ªéç½®é¡¹
```

### Comparing `nonebot-plugin-fuckyou-0.1.2/nonebot_plugin_fuckyou/__main__.py` & `nonebot-plugin-fuckyou-0.1.3/nonebot_plugin_fuckyou/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,20 @@
 
 
 # nb2 的 on_message 貌似不支持忽略大小写，自己写一个
 def trigger_rule(event: Event):
     if config.fuckyou_tome and (not event.is_tome()):
         return False
 
+    in_blacklist = event.get_user_id() in config.fuckyou_blacklist
+    if config.fuckyou_bl_to_wl:
+        in_blacklist = not in_blacklist
+    if in_blacklist:
+        return False
+
     try:
         msg = event.get_plaintext().lower()
     except:
         return False
 
     return any(w in msg for w in TRIGGER_WORDS)
```

### Comparing `nonebot-plugin-fuckyou-0.1.2/nonebot_plugin_fuckyou/const.py` & `nonebot-plugin-fuckyou-0.1.3/nonebot_plugin_fuckyou/const.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fuckyou-0.1.2/pyproject.toml` & `nonebot-plugin-fuckyou-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-fuckyou"
-version = "0.1.2"
+version = "0.1.3"
 description = "A NoneBot2 plugin designed for curse users"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0-rc.1",
     "pydantic>=1.10.4",
```

### Comparing `nonebot-plugin-fuckyou-0.1.2/PKG-INFO` & `nonebot-plugin-fuckyou-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,13 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-fuckyou
-Version: 0.1.2
-Summary: A NoneBot2 plugin designed for curse users
-License: MIT
-Author-email: student_2333 <lgc2333@126.com>
-Requires-Python: >=3.8,<4.0
-Provides-Extra: dev
-Project-URL: homepage, https://github.com/lgc2333/nonebot-plugin-fuckyou
-Description-Content-Type: text/markdown
-
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
-  <img src="https://media.githubusercontent.com/media/lgc-NB2Dev/readme/main/fuckyou/logo.png" width="180" height="180" alt="NoneBotPluginLogo">
+  <img src="https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/fuckyou/logo.png" width="180" height="180" alt="NoneBotPluginLogo">
 </a>
 
 <p>
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
 </p>
 
 # NoneBot-Plugin-FuckYou
@@ -118,15 +107,17 @@
 
 |         配置项         | 必填 | 默认值  |                          说明                          |
 | :--------------------: | :--: | :-----: | :----------------------------------------------------: |
 |    `FUCKYOU_GENTLE`    |  否  | `True`  |                    是否启用温柔词库                    |
 |   `FUCKYOU_VIOLENT`    |  否  | `False` | **慎用**，是否启用攻击性极强的暴力词库，**后果自负**！ |
 |     `FUCKYOU_TOME`     |  否  | `True`  |             是否只有 @机器人 时才会骂回去              |
 | `FUCKYOU_EXTEND_WORDS` |  否  |  `[]`   |                   要额外添加的触发词                   |
-|    `FUCKYOU_BLOCK`     |  否  | `False`  |                   是否阻断 Matcher                   |
+|    `FUCKYOU_BLOCK`     |  否  | `False` |                    是否阻断 Matcher                    |
+|  `FUCKYOU_BLACKLIST`   |  否  |  `[]`   |            插件忽略的用户列表（字符串列表）            |
+|   `FUCKYOU_BL_TO_WL`   |  否  | `False` |           是否将用户黑名单翻转变为白名单判断           |
 
 ## 🎉 使用
 
 直接 @Bot 对骂即可，插件为关键词检测，触发关键词可以看看 [const.py](./nonebot_plugin_fuckyou/const.py)
 
 理论支持所有 adapter
 
@@ -153,15 +144,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.1.3
+
+- 添加两个配置项
+
 ### 0.1.2
 
 - 添加一个配置项
 
 ### 0.1.1
 
 - 添加几个配置项
-
```

#### html2text {}

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-fuckyou Version: 0.1.2 Summary: A
-NoneBot2 plugin designed for curse users License: MIT Author-email:
-student_2333
-126.com> Requires-Python: >=3.8,<4.0 Provides-Extra: dev Project-URL: homepage,
-https://github.com/lgc2333/nonebot-plugin-fuckyou Description-Content-Type:
-text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # NoneBot-Plugin-FuckYou _ð ä½ æå ä¸ª ð´ï¼è¿ä¹çï¼ ð_ [license]
                   [pypi] [python] [pypi_download] [wakatime]
 ## ð ä»ç» _10 åéç´§æ¥å¼åçæä»¶ï¼è¯¯_ NoneBot2
 éªäººæä»¶ï¼æ»å»æ§æå¼º æä»¶è¯åºæ¥æºï¼[xiaoye12123/js](https://
 gitee.com/xiaoye12123/js) ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸**
@@ -25,19 +19,22 @@
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
 è¯´æ | | :--------------------: | :--: | :-----: | :-------------------------
 ---------------------------: | | `FUCKYOU_GENTLE` | å¦ | `True` |
 æ¯å¦å¯ç¨æ¸©æè¯åº | | `FUCKYOU_VIOLENT` | å¦ | `False` |
 **æç¨**ï¼æ¯å¦å¯ç¨æ»å»æ§æå¼ºçæ´åè¯åºï¼**åæèªè´**ï¼ |
 | `FUCKYOU_TOME` | å¦ | `True` | æ¯å¦åªæ @æºå¨äºº æ¶æä¼éªåå» |
 | `FUCKYOU_EXTEND_WORDS` | å¦ | `[]` | è¦é¢å¤æ·»å çè§¦åè¯ | |
-`FUCKYOU_BLOCK` | å¦ | `False` | æ¯å¦é»æ­ Matcher | ## ð ä½¿ç¨ ç´æ¥
+`FUCKYOU_BLOCK` | å¦ | `False` | æ¯å¦é»æ­ Matcher | | `FUCKYOU_BLACKLIST`
+| å¦ | `[]` | æä»¶å¿½ç¥çç¨æ·åè¡¨ï¼å­ç¬¦ä¸²åè¡¨ï¼ | |
+`FUCKYOU_BL_TO_WL` | å¦ | `False` |
+æ¯å¦å°ç¨æ·é»ååç¿»è½¬åä¸ºç½ååå¤æ­ | ## ð ä½¿ç¨ ç´æ¥
 @Bot å¯¹éªå³å¯ï¼æä»¶ä¸ºå³é®è¯æ£æµï¼è§¦åå³é®è¯å¯ä»¥çç
 [const.py](./nonebot_plugin_fuckyou/const.py) çè®ºæ¯æææ adapter ##
 ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
 å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [`xiaoye12123/js`](https://gitee.com/xiaoye12123/
 js) - æ»å»æ§æå¼ºçåå¤è¯åºæ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.2 - æ·»å ä¸ä¸ªéç½®é¡¹ ###
-0.1.1 - æ·»å å ä¸ªéç½®é¡¹
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.3 - æ·»å ä¸¤ä¸ªéç½®é¡¹ ###
+0.1.2 - æ·»å ä¸ä¸ªéç½®é¡¹ ### 0.1.1 - æ·»å å ä¸ªéç½®é¡¹
```


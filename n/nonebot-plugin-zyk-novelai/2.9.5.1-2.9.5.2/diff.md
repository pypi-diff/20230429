# Comparing `tmp/nonebot_plugin_zyk_novelai-2.9.5.1.tar.gz` & `tmp/nonebot_plugin_zyk_novelai-2.9.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_zyk_novelai-2.9.5.1.tar", last modified: Wed Jan 18 07:49:46 2023, max compression
+gzip compressed data, was "nonebot_plugin_zyk_novelai-2.9.5.2.tar", last modified: Sat Apr 29 18:29:34 2023, max compression
```

## Comparing `nonebot_plugin_zyk_novelai-2.9.5.1.tar` & `nonebot_plugin_zyk_novelai-2.9.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-01-18 07:49:46.613884 nonebot_plugin_zyk_novelai-2.9.5.1/
--rw-rw-rw-   0        0        0     1083 2022-11-19 09:58:08.000000 nonebot_plugin_zyk_novelai-2.9.5.1/LICENSE
--rw-rw-rw-   0        0        0      322 2023-01-18 07:49:46.613884 nonebot_plugin_zyk_novelai-2.9.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     6683 2023-01-05 00:49:42.000000 nonebot_plugin_zyk_novelai-2.9.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-18 07:49:46.588951 nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai/
--rw-rw-rw-   0        0        0    13157 2023-01-18 07:48:45.000000 nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai/__init__.py
--rw-rw-rw-   0        0        0     1652 2023-01-02 07:55:24.000000 nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai/config.py
-drwxrwxrwx   0        0        0        0 2023-01-18 07:49:46.611890 nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai/resource/
--rw-rw-rw-   0        0        0  1589248 2022-11-24 14:24:48.000000 nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai/resource/novelai_tags.db
--rw-rw-rw-   0        0        0     4487 2023-01-02 07:42:54.000000 nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai/work.py
-drwxrwxrwx   0        0        0        0 2023-01-18 07:49:46.604909 nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai.egg-info/
--rw-rw-rw-   0        0        0      322 2023-01-18 07:49:46.000000 nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2023-01-18 07:49:46.000000 nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-18 07:49:46.000000 nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-01-18 07:49:46.000000 nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-01-18 07:49:46.000000 nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-18 07:49:46.613884 nonebot_plugin_zyk_novelai-2.9.5.1/setup.cfg
--rw-rw-rw-   0        0        0      595 2023-01-18 07:48:45.000000 nonebot_plugin_zyk_novelai-2.9.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 18:29:34.327677 nonebot_plugin_zyk_novelai-2.9.5.2/
+-rw-rw-rw-   0        0        0     1083 2023-04-20 14:30:38.000000 nonebot_plugin_zyk_novelai-2.9.5.2/LICENSE
+-rw-rw-rw-   0        0        0      347 2023-04-29 18:29:34.326676 nonebot_plugin_zyk_novelai-2.9.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6843 2023-04-20 14:30:38.000000 nonebot_plugin_zyk_novelai-2.9.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 18:29:34.307675 nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai/
+-rw-rw-rw-   0        0        0    11789 2023-04-29 18:26:04.000000 nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai/__init__.py
+-rw-rw-rw-   0        0        0     1652 2023-04-29 18:26:19.000000 nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai/config.py
+drwxrwxrwx   0        0        0        0 2023-04-29 18:29:34.319676 nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai/resource/
+-rw-rw-rw-   0        0        0  1589248 2023-04-20 14:30:38.000000 nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai/resource/novelai_tags.db
+-rw-rw-rw-   0        0        0     3091 2023-04-29 18:26:40.000000 nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai/work.py
+drwxrwxrwx   0        0        0        0 2023-04-29 18:29:34.317676 nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai.egg-info/
+-rw-rw-rw-   0        0        0      347 2023-04-29 18:29:34.000000 nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2023-04-29 18:29:34.000000 nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 18:29:34.000000 nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-04-29 18:29:34.000000 nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-29 18:29:34.000000 nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 18:29:34.327677 nonebot_plugin_zyk_novelai-2.9.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      595 2023-04-20 14:42:28.000000 nonebot_plugin_zyk_novelai-2.9.5.2/setup.py
```

### Comparing `nonebot_plugin_zyk_novelai-2.9.5.1/LICENSE` & `nonebot_plugin_zyk_novelai-2.9.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zyk_novelai-2.9.5.1/README.md` & `nonebot_plugin_zyk_novelai-2.9.5.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # :memo: nonebot_plugin_zyk_novelai
 
+[![Security Status](https://www.murphysec.com/badge/ZYKsslm/nonebot_plugin_zyk_novelai.svg)](https://www.murphysec.com/p/ZYKsslm/nonebot_plugin_zyk_novelai)
+
 *本插件基于Naifu端配置制作*
 
 *:page_facing_up: 使用本插件前请仔细阅读README文档*
 
 ## :sparkles: 新版本一览
 ### :pushpin: version 2.9.5
 >都更新了哪些内容？
```

### Comparing `nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai/__init__.py` & `nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from nonebot.adapters.onebot.v11 import MessageEvent, MessageSegment, GROUP, PRIVATE_FRIEND, Bot, Message
 from nonebot import on_regex, on_command
 from nonebot.params import CommandArg, RegexGroup, RegexDict
 from nonebot.permission import SUPERUSER
 from nonebot.log import logger
 from nonebot.exception import ActionFailed
 
-from .work import get_data, AsyncDownloadFile, random_prompt, search_tags, set_size
+from .work import get_data, AsyncDownloadFile, random_prompt, search_tags
 from .config import *
 from base64 import b64encode, b64decode
 from asyncio import sleep
 from re import findall, S
 from colorama import init, Fore
 
 __version__ = "2.9.5.1"
 
 # 构造响应器
 check_state = on_command(cmd="check state", permission=SUPERUSER, priority=5, block=True)
 set_url = on_regex(pattern=r'set_url:(?P<url>.*/)', permission=SUPERUSER, priority=5, block=True)
 search_tag = on_command(cmd="补魔", aliases={"召唤魔咒", "搜索魔咒"}, permission=SUPERUSER, priority=5, block=True)
-pattern = r'^(?P<mode>ai绘图|AI绘图|ai作图|AI作图)( scale=(?P<scale>\d+))?( steps=(?P<steps>\d+))?( size=(?P<size>\d+x\d+))?( seed=(?P<seed>\d+))?( prompt=(?P<prompt>.+))?'
+pattern = r'^(?P<mode>ai绘图|AI绘图|ai作图|AI作图)( scale=(?P<scale>\d+))?( steps=(?P<steps>\d+))?( size=(?P<size>\d+x\d+))?( seed=(?P<seed>\d+))?( prompt="(?P<prompt>.+?)")?( uc="(?P<uc>.+?)")?'
 process_img = on_regex(pattern=pattern, permission=GROUP | PRIVATE_FRIEND, priority=10, block=True)
-img2img_pattern = r'^(img2img|以图生图).*?url=(?P<url>.*);.*?\](.*?strength=(?P<strength>\d\.\d))?(.*?noise=(?P<noise>\d\.\d))?(.*?scale=(?P<scale>\d+))?(.*?size=(?P<size>\d+x\d+))?(.*?seed=(?P<seed>\d+))?(.*?prompt=(?P<prompt>.+))?'
+img2img_pattern = r'^(img2img|以图生图).*?url=(?P<url>.*);.*?\](.*?strength=(?P<strength>\d\.\d))?(.*?noise=(?P<noise>\d\.\d))?(.*?scale=(?P<scale>\d+))?(.*?size=(?P<size>\d+x\d+))?(.*?seed=(?P<seed>\d+))?(.*?prompt="(?P<prompt>.+)")?(.*?uc="(?P<uc>.+)")?'
 img2img = on_regex(pattern=img2img_pattern, flags=S, permission=GROUP | PRIVATE_FRIEND, priority=10, block=True)
 
 # 获取后端URL
 try:
     post_url = get_driver().config.novelai_post_url
 except AttributeError:
     post_url = ""
@@ -99,67 +99,46 @@
 
     # 生图参数
     seed = regex["seed"]
     scale = regex["scale"]
     steps = regex["steps"]
     size = regex["size"]
     prompt = regex["prompt"]
-    uc = "lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry"
+    uc = regex["uc"]
 
     if seed is None:
         seed = randint(0, pow(2, 32))
     if scale is None:
         scale = 12
     if steps is None:
         steps = 28
     if size is None:
         size = "512x768"
-
-    # 这一段写得很乱，prompt和uc合起来了，要再分一次
+    if uc is None:
+        uc = "lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry"
     if prompt is None:
         if_randomP = True
-        num = randint(0, 1000)
+        num = randint(0, 50)
         prompt = random_prompt(num)
-        try:
-            uc = findall(r'uc=(?P<uc>.+)', str(event.get_plaintext()))[0]
-        except IndexError:
-            pass
     else:
-        # 获取随机prompt
         if "RandomP" in prompt:
             if_randomP = True
-            try:
-                num = findall(r'RandomP (?P<num>\d+)', prompt)[0]
-            except IndexError:
-                switch = True
-                await process_img.finish("请输入随机tag条数！", at_sender=True)
-            else:
-                prompt = random_prompt(num)
+            num = findall(r'RandomP (\d+)', prompt)[0]
+            prompt = random_prompt(num)
         else:
             if_randomP = False
 
-        try:
-            uc = findall(r'uc=(?P<uc>.+)', str(event.get_plaintext()))[0]
-        except IndexError:
-            pass
-        else:
-            if if_randomP is False:
-                prompt = findall(r'(?P<prompt>.+) uc', prompt)[0]
-
     # 处理图片尺寸
-    try:
-        size = size.split("x")
-    except AttributeError:
-        size = [512, 512]
+    size = size.split("x")
     size = [int(size[0]), int(size[1])]
     if size[0] > 1024 or size[1] > 1024:
         switch = True
         await process_img.finish("图片尺寸过大，请重新输入！", at_sender=True)
 
-    # 获取用户名
+    # 获取当前用户名
     name = (await bot.get_stranger_info(user_id=int(id_)))["nickname"]
 
     await process_img.send("正在生成图片，请稍等...", at_sender=True)
     logger.info(
         Fore.LIGHTYELLOW_EX +
         f"\n开始生成{name}的图片："
         f"\nscale={scale}"
@@ -186,15 +165,15 @@
         logger.error(Fore.LIGHTRED_EX + f"后端请求失败：{data[1]}")
         await process_img.finish("生成失败！", at_sender=True)
 
     logger.success(Fore.LIGHTGREEN_EX + f"{name}的图片生成成功！")
 
     # 把base64字符串转成bytes
     image = b64decode(data[1])
-    msg = f"\n{prompt}" + MessageSegment.image(image) if if_randomP == True else MessageSegment.image(image)
+    msg = f"\n{prompt}" + MessageSegment.image(image) if if_randomP else MessageSegment.image(image)
     switch = True
 
     try:
         msg_id = (await process_img.send(msg, at_sender=True))["message_id"]
     except ActionFailed:
         logger.warning(Fore.LIGHTYELLOW_EX + f"{nickname}可能被风控，请稍后再试！")
         await search_tag.finish(f"{nickname}可能被风控，请稍后再试！", at_sender=True)
@@ -228,15 +207,15 @@
     img_url = regex["url"]
     strength = regex["strength"]
     noise = regex["noise"]
     seed = regex["seed"]
     scale = regex["scale"]
     size = regex["size"]
     prompt = regex["prompt"]
-    uc = "lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry"
+    uc = regex["uc"]
 
     if strength is None:
         strength = 0.7
     else:
         if float(strength) > 0.99:
             switch = True
             await img2img.finish("strength过大！（不能超过0.99）", at_sender=True)
@@ -251,48 +230,30 @@
     if seed is None:
         seed = randint(0, pow(2, 32))
     if scale is None:
         scale = 12
 
     if prompt is None:
         if_randomP = True
-        num = randint(0, 1000)
+        num = randint(0, 50)
         prompt = random_prompt(num)
-        try:
-            uc = findall(r'uc=(?P<uc>.+)', str(event.get_plaintext()))[0]
-        except IndexError:
-            pass
     else:
-        # 获取随机prompt
         if "RandomP" in prompt:
             if_randomP = True
-            try:
-                num = findall(r'RandomP (?P<num>\d+)', prompt)[0]
-            except IndexError:
-                switch = True
-                await process_img.finish("请输入随机tag条数！", at_sender=True)
-            else:
-                prompt = random_prompt(num)
+            num = findall(r'RandomP (\d+)', prompt)[0]
+            prompt = random_prompt(num)
         else:
             if_randomP = False
-
-        try:
-            uc = findall(r'uc=(?P<uc>.+)', str(event.get_plaintext()))[0]
-        except IndexError:
-            pass
-        else:
-            if if_randomP is False:
-                prompt = findall(r'(?P<prompt>.+) uc', prompt)[0]
+        
+    if uc is None:
+        uc = "lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry"
 
     if size is not None:
         # 处理图片尺寸
-        try:
-            size = size.split("x")
-        except AttributeError:
-            size = [512, 512]
+        size = size.split("x")
         size = [int(size[0]), int(size[1])]
         if size[0] > 1024 or size[1] > 1024:
             switch = True
             await img2img.finish("图片尺寸过大，请重新输入！", at_sender=True)
 
     switch = False
     name = (await bot.get_stranger_info(user_id=int(id_)))["nickname"]
@@ -305,15 +266,15 @@
         switch = True
         logger.error(Fore.LIGHTRED_EX + f"{name}发送的图片获取失败：{img_data[1]}")
         await img2img.finish("图片获取失败！", at_sender=True)
 
     logger.success(Fore.LIGHTGREEN_EX + f"{name}发送的图片获取成功！")
 
     if size is None:
-        size = set_size(image=img_data[1])
+        size = [512, 768]
 
     await img2img.send("正在生成图片，请稍等...", at_sender=True)
 
     # 先把bytes转成base64，再用utf-8编码
     img = b64encode(img_data[1]).decode("utf-8")
     mode = "以图生图"
     switch = False
@@ -349,15 +310,15 @@
         switch = True
         logger.error(Fore.LIGHTRED_EX + f"后端请求失败：{data[1]}")
         await img2img.finish(f"生成失败：{data[1]}", at_sender=True)
 
     logger.success(Fore.LIGHTGREEN_EX + f"{name}的图片生成成功！")
 
     image = b64decode(data[1])
-    msg = f"\n{prompt}" + MessageSegment.image(image) if if_randomP == True else MessageSegment.image(image)
+    msg = f"\n{prompt}" + MessageSegment.image(image) if if_randomP else MessageSegment.image(image)
     switch = True
 
     try:
         msg_id = (await img2img.send(msg, at_sender=True))["message_id"]
     except ActionFailed:
         logger.warning(Fore.LIGHTYELLOW_EX + f"{nickname}可能被风控，请稍后再试！")
         await search_tag.finish(f"{nickname}可能被风控，请稍后再试！", at_sender=True)
```

### Comparing `nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai/config.py` & `nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zyk_novelai-2.9.5.1/nonebot_plugin_zyk_novelai/resource/novelai_tags.db` & `nonebot_plugin_zyk_novelai-2.9.5.2/nonebot_plugin_zyk_novelai/resource/novelai_tags.db`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zyk_novelai-2.9.5.1/setup.py` & `nonebot_plugin_zyk_novelai-2.9.5.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="nonebot_plugin_zyk_novelai",
-    version="2.9.5.1",
+    version="2.9.5.2",
     packages=find_packages(),
     author="ZSSLM",
     author_email="3119964735@qq.com",
     long_description="This is a simple plugin that is to send your image made by your NovelAI for nonebot2",
     url="https://github.com/ZYKsslm/nonebot_plugin_zyk_novelai",
     license="MIT License",
     install_requires=["fake_useragent", "httpx", "colorama", "Pillow", "nonebot2", "nonebot_adapter_onebot"],
```


# Comparing `tmp/nonebot_plugin_zyk_music-0.1.7.tar.gz` & `tmp/nonebot_plugin_zyk_music-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_zyk_music-0.1.7.tar", last modified: Thu Apr 27 18:12:52 2023, max compression
+gzip compressed data, was "nonebot_plugin_zyk_music-0.1.7.1.tar", last modified: Sat Apr 29 19:19:09 2023, max compression
```

## Comparing `nonebot_plugin_zyk_music-0.1.7.tar` & `nonebot_plugin_zyk_music-0.1.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 18:12:52.398796 nonebot_plugin_zyk_music-0.1.7/
--rw-rw-rw-   0        0        0     1083 2023-04-20 14:29:23.000000 nonebot_plugin_zyk_music-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      310 2023-04-27 18:12:52.397796 nonebot_plugin_zyk_music-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2439 2023-04-20 14:29:23.000000 nonebot_plugin_zyk_music-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 18:12:52.385796 nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music/
--rw-rw-rw-   0        0        0   441964 2023-04-20 14:29:23.000000 nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music/User-Agent.json
--rw-rw-rw-   0        0        0     5805 2023-04-27 18:06:07.000000 nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music/__init__.py
--rw-rw-rw-   0        0        0      713 2023-04-27 18:06:18.000000 nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music/config.py
-drwxrwxrwx   0        0        0        0 2023-04-27 18:12:52.396796 nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music/music/
--rw-rw-rw-   0        0        0       45 2023-04-20 14:29:23.000000 nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music/music/music.txt
--rw-rw-rw-   0        0        0    13240 2023-04-27 18:06:38.000000 nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music/work.py
-drwxrwxrwx   0        0        0        0 2023-04-27 18:12:52.394796 nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-27 18:12:52.000000 nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-04-27 18:12:52.000000 nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 18:12:52.000000 nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-27 18:12:52.000000 nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-27 18:12:52.000000 nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 18:12:52.399797 nonebot_plugin_zyk_music-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      556 2023-04-27 18:05:58.000000 nonebot_plugin_zyk_music-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 19:19:09.662856 nonebot_plugin_zyk_music-0.1.7.1/
+-rw-rw-rw-   0        0        0     1083 2023-04-29 19:17:38.000000 nonebot_plugin_zyk_music-0.1.7.1/LICENSE
+-rw-rw-rw-   0        0        0      312 2023-04-29 19:19:09.660856 nonebot_plugin_zyk_music-0.1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2133 2023-04-29 19:17:38.000000 nonebot_plugin_zyk_music-0.1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 19:19:09.636855 nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music/
+-rw-rw-rw-   0        0        0   441964 2023-04-29 19:17:38.000000 nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music/User-Agent.json
+-rw-rw-rw-   0        0        0     5805 2023-04-29 19:17:38.000000 nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-04-29 19:17:38.000000 nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music/config.py
+drwxrwxrwx   0        0        0        0 2023-04-29 19:19:09.657856 nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music/music/
+-rw-rw-rw-   0        0        0       45 2023-04-29 19:17:38.000000 nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music/music/music.txt
+-rw-rw-rw-   0        0        0    13083 2023-04-29 19:18:06.000000 nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music/work.py
+drwxrwxrwx   0        0        0        0 2023-04-29 19:19:09.653855 nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music.egg-info/
+-rw-rw-rw-   0        0        0      312 2023-04-29 19:19:09.000000 nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-04-29 19:19:09.000000 nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 19:19:09.000000 nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-29 19:19:09.000000 nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 19:19:09.000000 nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 19:19:09.663856 nonebot_plugin_zyk_music-0.1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-04-29 19:18:30.000000 nonebot_plugin_zyk_music-0.1.7.1/setup.py
```

### Comparing `nonebot_plugin_zyk_music-0.1.7/LICENSE` & `nonebot_plugin_zyk_music-0.1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zyk_music-0.1.7/README.md` & `nonebot_plugin_zyk_music-0.1.7.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # :memo: nonebot_plugin_zyk_music
 
 **本插件是我另一个项目改的，有兴趣的话可以去看看[BlackStone_Music_GUI](https://github.com/ZYKsslm/BlackStone_Music_GUI)**
 
 *:page_facing_up: 使用本插件前请仔细阅读README*
 
 ## :sparkles: 新版本一览
-### :pushpin: version 0.1.6
+### :pushpin: version 0.1.7
 >都更新了哪些内容？
-1. 修复了在默认文件保存路径下找不到文件的BUG
-2. 增加导入歌单功能，目前只支持qq音乐的歌单，可直接从歌单点歌
+1. 删去酷我音乐接口
+2. 全面更新代码，更换接口
 
 
 ## :cd: 安装方式
 - #### 使用pip
 ```
 pip install nonebot_plugin_zyk_music
 ```
@@ -21,15 +21,14 @@
 nb plugin install nonebot_plugin_zyk_music
 ```
 
 ## :wrench: env配置
 
 |        Name         |      Example       | Type |        Usage         | Required |
 |:-------------------:|:------------------:|:----:|:--------------------:|:--------:|
-|  music_proxy_port   |       10809        | int  |    本地代理端口，若有代理则需要    |    No    |
 |     music_path      | path/to/your/music | str  | 音乐保存路径，默认保存在music目录下 |    No    |
 |   music_del_file    |       False        | bool |  是否删除下载的文件，默认为True   |    No    |
 | music_retry_songnum |         50         | int  |    歌单发送失败时重新发送的条数    |    No    |
 
 
 ## :bulb: 如何交互
 
@@ -40,15 +39,14 @@
 ![impt_songlist](impt_songlist.gif)
 
 ## :label: 指令
 ### 支持的平台
 - [x] QQ音乐
 - [x] 网易云音乐
 - [x] 酷狗音乐
-- [x] 酷我音乐
 - [x] 咪咕音乐
 
 
 ### QQ点歌
 ```
 qq | QQ点歌 name
 
@@ -68,22 +66,14 @@
 ```
 酷狗 | kg点歌 name
 
 eg：
     kg点歌 stay
 ```
 
-### 酷我点歌
-```
-酷我 | kw点歌 name
-
-eg：
-    kw点歌 stay
-```
-
 ### 网易云点歌
 ```
 网易云 | 网易 | wy点歌 name
 
 eg：
     wy点歌 stay
 ```
```

### Comparing `nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music/User-Agent.json` & `nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music/User-Agent.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music/__init__.py` & `nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music/config.py` & `nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_zyk_music-0.1.7/nonebot_plugin_zyk_music/work.py` & `nonebot_plugin_zyk_music-0.1.7.1/nonebot_plugin_zyk_music/work.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     song = set_name(music_info["song"])
     singer = set_name(music_info["singer"])
     try:
         music = music_info["url"]
     except KeyError:
         return False
 
-    async with AsyncClient(headers="MQQBrowser/26 Mozilla/5.0 (Linux; U; Android 2.3.7; zh-cn; MB200 Build/GRJ22; CyanogenMod-7) AppleWebKit/533.1 (KHTML, like Gecko) Version/4.0 Mobile Safari/533.1", follow_redirects=True, timeout=None) as client:
+    async with AsyncClient(headers=headers, follow_redirects=True, timeout=None) as client:
         resp = await client.get(url=music)
         content = resp.content
 
     kind = guess(content)
     if kind is None:
         return False
```

### Comparing `nonebot_plugin_zyk_music-0.1.7/setup.py` & `nonebot_plugin_zyk_music-0.1.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="nonebot_plugin_zyk_music",
-    version="0.1.7",
+    version="0.1.7.1",
     packages=find_packages(),
     author="ZSSLM",
     author_email="3119964735@qq.com",
     long_description="This is a simple plugin for nonebot2 to pick up music",
     url="https://github.com/ZYKsslm/nonebot_plugin_zyk_music",
     license="MIT License",
     install_requires=["httpx", "colorama", "filetype", "nonebot2", "nonebot_adapter_onebot"],
```


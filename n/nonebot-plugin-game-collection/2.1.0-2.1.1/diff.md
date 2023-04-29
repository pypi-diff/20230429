# Comparing `tmp/nonebot_plugin_game_collection-2.1.0.tar.gz` & `tmp/nonebot_plugin_game_collection-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.1.0.tar", last modified: Fri Apr  7 09:56:11 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.1.1.tar", last modified: Sat Apr 29 02:34:20 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.1.0.tar` & `nonebot_plugin_game_collection-2.1.1.tar`

### file list

```diff
@@ -1,54 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 09:56:11.638506 nonebot_plugin_game_collection-2.1.0/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.0/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-04-07 09:56:11.635503 nonebot_plugin_game_collection-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 09:56:11.589964 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/
-drwxrwxrwx   0        0        0        0 2023-04-07 09:56:11.599472 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/.vs/
--rw-rw-rw-   0        0        0       37 2023-03-04 09:10:52.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/.vs/ProjectSettings.json
--rw-rw-rw-   0        0        0      150 2023-03-04 11:54:34.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/.vs/VSWorkspaceState.json
--rw-rw-rw-   0        0        0    17615 2023-03-04 07:33:31.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0    41084 2023-03-04 07:28:59.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:56:11.606478 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15272 2023-02-28 15:49:25.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6237 2023-02-28 15:49:25.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     4999 2023-02-28 16:14:15.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     8962 2023-02-28 15:50:53.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    10909 2023-03-04 07:38:48.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    20122 2023-03-04 11:07:21.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    13072 2023-03-04 08:07:35.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    28660 2023-03-04 11:53:52.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3129 2023-03-04 11:53:52.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/config.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:56:11.609481 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/data/
--rw-rw-rw-   0        0        0      525 2023-02-24 19:49:14.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/data/api.py
--rw-rw-rw-   0        0        0     5589 2023-03-02 18:02:43.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/data/data.py
--rw-rw-rw-   0        0        0      102 2023-02-24 19:49:02.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/data/run.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:56:11.612984 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/
--rw-rw-rw-   0        0        0      171 2023-02-25 14:16:58.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/element_library.json
-drwxrwxrwx   0        0        0        0 2023-04-07 09:56:11.629498 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5335 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4372 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1692 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      861 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2616 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1208 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22088 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4569 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0      975 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2199 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    11276 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     4976 2023-03-04 08:08:51.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-04-07 09:56:11.630999 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2347 2023-03-04 05:27:28.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:56:11.634502 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1321 2023-02-25 14:16:58.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0     7133 2023-02-27 17:39:47.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1619 2023-02-28 15:47:33.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:56:11.596970 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-04-07 09:56:11.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2151 2023-04-07 09:56:11.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 09:56:11.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-07 09:56:11.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-04-07 09:56:11.000000 nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 09:56:11.638506 nonebot_plugin_game_collection-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-07 09:56:02.000000 nonebot_plugin_game_collection-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:34:20.004921 nonebot_plugin_game_collection-2.1.1/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-04-29 02:34:20.003419 nonebot_plugin_game_collection-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 02:34:19.929856 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    17615 2023-03-04 07:33:31.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0    41084 2023-03-04 07:28:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:34:19.949873 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15272 2023-02-28 15:49:25.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6237 2023-02-28 15:49:25.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     4999 2023-02-28 16:14:15.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     8962 2023-02-28 15:50:53.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    10909 2023-03-04 07:38:48.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    20122 2023-03-04 11:07:21.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    13072 2023-03-04 08:07:35.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    28653 2023-04-29 02:11:48.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3129 2023-03-04 11:53:52.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/config.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:34:19.956879 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/data/
+-rw-rw-rw-   0        0        0      525 2023-02-24 19:49:14.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/data/api.py
+-rw-rw-rw-   0        0        0     5589 2023-03-02 18:02:43.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/data/data.py
+-rw-rw-rw-   0        0        0      102 2023-02-24 19:49:02.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/data/run.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:34:19.962384 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/
+-rw-rw-rw-   0        0        0      171 2023-02-25 14:16:58.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/element_library.json
+drwxrwxrwx   0        0        0        0 2023-04-29 02:34:19.983402 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5335 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4372 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1692 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      861 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2616 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1208 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22088 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4569 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0      975 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2199 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12610 2023-04-29 02:31:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     4976 2023-03-04 08:08:51.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-04-29 02:34:19.986905 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2347 2023-03-04 05:27:28.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:34:20.001417 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1321 2023-02-25 14:16:58.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0     7133 2023-02-27 17:39:47.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1619 2023-02-28 15:47:33.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:34:19.942367 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-04-29 02:34:19.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2038 2023-04-29 02:34:19.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 02:34:19.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-04-29 02:34:19.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-04-29 02:34:19.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 02:34:20.004921 nonebot_plugin_game_collection-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-29 02:34:15.000000 nonebot_plugin_game_collection-2.1.1/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.1.0/LICENSE` & `nonebot_plugin_game_collection-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/README.md` & `nonebot_plugin_game_collection-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Account.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Market.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Prop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -785,15 +785,15 @@
 
 @freeze.got("code")
 
 async def _(bot:Bot, event:MessageEvent, matcher:Matcher, code :Message = Arg()):
     at,confirm = matcher.get_arg("freeze")
     if confirm == str(code):
         target = await Manager.locate_user_at(bot, event, at)
-        msg = Account.freeze(event, target[0])
+        msg = Account.freeze(target[0])
         await freeze.finish(msg)
     else:
         await freeze.finish("【冻结】已取消。")
 
 # 清理无效账户
 delist = on_command("清理无效账户", rule = to_me(), permission = SUPERUSER, priority = 20, block = True)
```

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/data/api.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/data/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/data/data.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/data/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8235294117647058%*

 * *Differences: {'insert': "[(0, OrderedDict([('func', '管理员指令'), ('trigger_method', ''), ('trigger_condition', "*

 * *           "'无'), ('brief_des', '获取金币'), ('detail_des', '获取金币 数量：\\n获取金币\\n获取道具 道具名 "*

 * *           "数量：\\n每次重置后可领取一次。刷新每日：\\n刷新每日签到，补贴，金币转移上限，所有人时效道具的剩余时间-1\\n保存数据：\\n在关bot前需要保存数据，不然会回档到上次自动保存的时间点\\n数据备份：\\n备份游戏数据文件\\n清除对决：\\n删除正在进行的游戏')])), "*

 * *           "(4, OrderedDict([('func', '设置背景图片'), ('trigger_method', '设置背景图片[图片] "*

 * *           "设置背景图片(回复一张图片，删掉at)'), ('trigger_condition', '需要有特定道具'), ('brief_des', "*

 * *       […]*

```diff
@@ -1,10 +1,17 @@
 [
     {
         "brief_des": "\u83b7\u53d6\u91d1\u5e01",
+        "detail_des": "\u83b7\u53d6\u91d1\u5e01 \u6570\u91cf\uff1a\n\u83b7\u53d6\u91d1\u5e01\n\u83b7\u53d6\u9053\u5177 \u9053\u5177\u540d \u6570\u91cf\uff1a\n\u6bcf\u6b21\u91cd\u7f6e\u540e\u53ef\u9886\u53d6\u4e00\u6b21\u3002\u5237\u65b0\u6bcf\u65e5\uff1a\n\u5237\u65b0\u6bcf\u65e5\u7b7e\u5230\uff0c\u8865\u8d34\uff0c\u91d1\u5e01\u8f6c\u79fb\u4e0a\u9650\uff0c\u6240\u6709\u4eba\u65f6\u6548\u9053\u5177\u7684\u5269\u4f59\u65f6\u95f4-1\n\u4fdd\u5b58\u6570\u636e\uff1a\n\u5728\u5173bot\u524d\u9700\u8981\u4fdd\u5b58\u6570\u636e\uff0c\u4e0d\u7136\u4f1a\u56de\u6863\u5230\u4e0a\u6b21\u81ea\u52a8\u4fdd\u5b58\u7684\u65f6\u95f4\u70b9\n\u6570\u636e\u5907\u4efd\uff1a\n\u5907\u4efd\u6e38\u620f\u6570\u636e\u6587\u4ef6\n\u6e05\u9664\u5bf9\u51b3\uff1a\n\u5220\u9664\u6b63\u5728\u8fdb\u884c\u7684\u6e38\u620f",
+        "func": "\u7ba1\u7406\u5458\u6307\u4ee4",
+        "trigger_condition": "\u65e0",
+        "trigger_method": ""
+    },
+    {
+        "brief_des": "\u83b7\u53d6\u91d1\u5e01",
         "detail_des": "\u91d1\u5e01\u7b7e\u5230\uff1a\n\u73a9\u5bb6\u6bcf\u65e5\u53ef\u7b7e\u5230\u4e00\u6b21\uff0c\u6bcf\u65e50\u70b9\u5237\u65b0\u3002\n\u91cd\u7f6e\u7b7e\u5230\uff1a\n\u6bcf\u6b21\u91cd\u7f6e\u540e\u53ef\u9886\u53d6\u4e00\u6b21\u3002",
         "func": "\u83b7\u53d6\u91d1\u5e01",
         "trigger_condition": "\u65e0",
         "trigger_method": "1.\u91d1\u5e01\u7b7e\u5230 2.\u91cd\u7f6e\u7b7e\u5230"
     },
     {
         "brief_des": "\u6e05\u7a7a\u524d\u5341\u540d\u7684\u91d1\u5e01\u3002",
@@ -17,14 +24,28 @@
         "brief_des": "\u67e5\u770b\u4e2a\u4eba\u8d26\u6237\u8d44\u6599",
         "detail_des": "\u6211\u7684\u91d1\u5e01\uff1a\n\u67e5\u770b\u81ea\u5df1\u7684\u91d1\u5e01\u6570\u91cf\n\u6211\u7684\u4ed3\u5e93\uff1a\n\u67e5\u770b\u81ea\u5df1\u83b7\u5f97\u7684\u7684\u9053\u5177\n\u6211\u7684\u8d44\u6599\u5361\uff1a\n\u67e5\u770b\u4e2a\u4eba\u8d26\u6237\u8be6\u7ec6\u8d44\u6599\n\u6211\u7684\u8d44\u4ea7\uff1a\n\u67e5\u770b\u81ea\u5df1\u7684\u5168\u5c40\u8d44\u4ea7\u5206\u5e03",
         "func": "\u4e2a\u4eba\u8d26\u6237",
         "trigger_condition": "\u65e0",
         "trigger_method": "1.\u6211\u7684\u91d1\u5e01 2.\u6211\u7684\u4ed3\u5e93 3.\u6211\u7684\u8d44\u6599\u5361"
     },
     {
+        "brief_des": "\u8bbe\u7f6e\u6211\u7684\u8d44\u6599\u5361\u663e\u793a\u7684\u80cc\u666f\u56fe\u7247",
+        "detail_des": "",
+        "func": "\u8bbe\u7f6e\u80cc\u666f\u56fe\u7247",
+        "trigger_condition": "\u9700\u8981\u6709\u7279\u5b9a\u9053\u5177",
+        "trigger_method": "\u8bbe\u7f6e\u80cc\u666f\u56fe\u7247[\u56fe\u7247] \u8bbe\u7f6e\u80cc\u666f\u56fe\u7247(\u56de\u590d\u4e00\u5f20\u56fe\u7247\uff0c\u5220\u6389at)"
+    },
+    {
+        "brief_des": "\u5c06\u8d44\u6599\u5361\u663e\u793a\u7684\u80cc\u666f\u56fe\u7247\u8bbe\u7f6e\u4e3a\u9ed8\u8ba4",
+        "detail_des": "",
+        "func": "\u5220\u9664\u80cc\u666f\u56fe\u7247",
+        "trigger_condition": "",
+        "trigger_method": ""
+    },
+    {
         "brief_des": "\u7ed9at\u7684\u7528\u6237\u53d1\u91d1\u5e01",
         "detail_des": "",
         "func": "\u53d1\u7ea2\u5305",
         "trigger_condition": "\u65e0",
         "trigger_method": "\u53d1\u7ea2\u5305 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
     },
     {
@@ -66,14 +87,28 @@
         "brief_des": "\u79c1\u804a\u6307\u4ee4\u5173\u8054\u5230\u7fa4\u3002",
         "detail_des": "\u4f60\u53ef\u4ee5\u5728\u79c1\u804a\u5b8c\u6210\u4ee5\u4e0b\u64cd\u4f5c\uff1a\n\u7b7e\u5230\n\u62bd\u5361\n\u67e5\u770b\u4e2a\u4eba\u8d26\u6237\uff1a\n\u67e5\u770b\u6392\u884c\n\u8d2d\u4e70\u6216\u7ed3\u7b97\u80a1\u7968",
         "func": "\u8fde\u63a5\u8d26\u6237",
         "trigger_condition": "\u65e0",
         "trigger_method": "1.\u7fa4\u5185\uff1a@bot\u5173\u8054\u8d26\u6237 2.\u79c1\u804a\uff1a\u5173\u8054\u8d26\u6237\n"
     },
     {
+        "brief_des": "",
+        "detail_des": "",
+        "func": "\u5bf9\u5c40\u5904\u7406",
+        "trigger_condition": "\u8d85\u65f6\u7ed3\u7b97\u9700\u8981\u5bf9\u5c40\u5b58\u5728\u8d85\u8fc760s",
+        "trigger_method": "\u63a5\u53d7\u6311\u6218 \u62d2\u7edd\u6311\u6218 \u8ba4\u8f93 \u8d85\u65f6\u7ed3\u7b97"
+    },
+    {
+        "brief_des": "\u53d1\u8d77\u968f\u673a\u5bf9\u6218",
+        "detail_des": "\u968f\u673a\u6e38\u620f\uff0c\u5982\u4e0d\u6307\u5b9a\u91d1\u989d\u5c31\u662f\u968f\u673a\u91d1\u989d",
+        "func": "\u968f\u673a\u5bf9\u6218",
+        "trigger_condition": "\u9700\u8981\u7279\u5b9a\u9053\u5177",
+        "trigger_method": "\u968f\u673a\u5bf9\u6218 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
+    },
+    {
         "brief_des": "\u53d1\u8d77\u4fc4\u7f57\u65af\u8f6e\u76d8",
         "detail_des": "\u901a\u8fc7 \u88c5\u5f39 \u6765\u5bf9\u5176\u4ed6\u4eba\u53d1\u8d77\u51b3\u6597\n\u4e0d@\u5219\u6240\u6709\u7fa4\u53cb\u90fd\u53ef\u63a5\u53d7\n\u8f6e\u6d41\u5f00\u67aa\uff0c\u76f4\u5230\u8fd0\u6c14\u4e0d\u597d\u7684\u4eba\u5148\u53bb\u4e16\u3002\n\u3010\u7279\u6b8a\u6280\u80fd\u3011\uff1a\u5f00\u67aa0\n\n\u3010\u5f00\u59cb\u6e38\u620f\u3011\n\u88c5\u5f39 \u3010\u5b50\u5f39\u6570\u3011 \u3010\u91d1\u989d\u3011 \u3010at\u3011\uff08\u4e3a\u7a7a\u5219\u6240\u6709\u7fa4\u53cb\u90fd\u53ef\u63a5\u53d7\uff09\n\u3010\u56de\u5e94\u3011\n\u63a5\u53d7\u6311\u6218/\u62d2\u7edd\u6311\u6218\n\u3010\u56de\u5408\u4e2d\u3011\n\u5f00\u67aa/\u5494/\u562d/\u5623 [\u5b50\u5f39\u6570]\uff08\u9ed8\u8ba41)\uff08\u8f6e\u6d41\u5f00\u67aa\uff09\n\u3010\u7ed3\u7b97\u3011\n\u7ed3\u7b97 \uff08\u5f53\u67d0\u4e00\u65b960\u79d2\u672a\u5f00\u67aa\uff0c\u53ef\u4f7f\u7528\u8be5\u547d\u4ee4\u7ed3\u675f\u5bf9\u51b3\u5e76\u80dc\u5229\uff09",
         "func": "\u4fc4\u7f57\u65af\u8f6e\u76d8",
         "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u4e00\u500d\u8d4c\u6ce8\u4e0a\u9650",
         "trigger_method": "\u88c5\u5f39 \u3010\u5b50\u5f39\u6570\u3011 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
     },
     {
@@ -87,14 +122,21 @@
         "brief_des": "\u53d1\u8d77\u6251\u514b\u5bf9\u6218",
         "detail_des": "\u901a\u8fc7 \u6251\u514b\u5bf9\u6218 \u6765\u5bf9\u5176\u4ed6\u4eba\u5bf9\u6218\n\u6253\u51fa\u81ea\u5df1\u7684\u624b\u724c\n\u5f53\u5bf9\u65b9\u7684\u8840\u91cf\u5c0f\u4e8e1\u6216\u8005\u5728\u81ea\u5df1\u56de\u5408\u51fa\u724c\u524d\u8840\u91cf>40\u5373\u53ef\u83b7\u80dc\n\u724c\u5e93\u4e00\u517152\u5f20\u724c\uff0c\u5f53\u724c\u5e93\u6ca1\u6709\u724c\u4e86\u5c31\u4ee5\u76ee\u524d\u8840\u91cf\u7ed3\u7b97\uff0c\u7ed3\u675f\u6e38\u620f\u3002\n\n\u5148\u624b\u521d\u59cb\u70b9\u6570\uff1aHP 20 SP 0 DEF 0\n\u540e\u624b\u521d\u59cb\u70b9\u6570\uff1aHP 25 SP 2 DEF 0\n\u6bcf\u56de\u5408\u62bd\u4e09\u5f20\u724c\uff0c\u6253\u51fa\u5176\u4e2d\u7684\u4e00\u5f20\u4f5c\u4e3a\u884c\u52a8\u724c\uff0c\u5f03\u6389\u5269\u4f59\u624b\u724c\u3002\n\uff08\u7279\u522b\u6ce8\u610f\uff1a\u9632\u5fa1\u724c\u4f5c\u4e3a\u884c\u52a8\u724c\u662f\u653b\u51fb\uff09\n\u4e4b\u540e\u5bf9\u65b9\u6447\u4e00\u4e2a20\u9762\u9ab0\u5b50\uff0c\n\u5982\u679c\u70b9\u6570\u5c0f\u4e8e\u5bf9\u65b9SP\u5219\u4ece\u724c\u5e93\u7ffb\u51fa\u4e00\u5f20\u724c\u4f5c\u4e3a\u6280\u80fd\u724c\u6253\u51fa\u3002\n\u6309\u7167\u6280\u80fd\u724c\u70b9\u6570\u6263\u9664\u5bf9\u65b9SP\u70b9\u3002\n\n<ft size=30 color=black>\u9ed1\u6843</ft>\n\u63cf\u8ff0\uff1a\u9632\u5fa1\n\u884c\u52a8\u724c\u6548\u679c\uff1a\u6253\u51fa\u653b\u51fb\n\u6280\u80fd\u724c\u6548\u679c\uff1a\u589e\u52a0DEF\n<ft size=30 color=red>\u7ea2\u6843</ft>\n\u63cf\u8ff0\uff1a\u751f\u547d\n\u884c\u52a8\u724c\u6548\u679c\uff1a\u6062\u590dHP\n\u6280\u80fd\u724c\u6548\u679c\uff1a\u6062\u590dHP\n<ft size=30 color=black>\u6885\u82b1</ft>\n\u63cf\u8ff0\uff1a\u6280\u80fd\n\u884c\u52a8\u724c\u6548\u679c\uff1a\u4e3b\u52a8\u6280\u80fd\n\u6280\u80fd\u724c\u6548\u679c\uff1a\u589e\u52a0SP\n<ft size=30 color=red>\u65b9\u7247</ft>\n\u63cf\u8ff0\uff1a\u653b\u51fb\u884c\u52a8\u724c\u6548\u679c\uff1a\u6253\u51fa\u653b\u51fb\n\u6280\u80fd\u724c\u6548\u679c\uff1a\u6253\u51fa\u53cd\u51fb\n\n\u4e3b\u52a8\u6280\u80fd\uff1a\n\u6447\u4e00\u4e2a20\u9762\u9ab0\u5b50\n\u5982\u679c\u70b9\u6570\u5c0f\u4e8e\u81ea\u8eabSP\u5219\u628a\u5269\u4f59\u4e24\u5f20\u624b\u724c\u4f5c\u4e3a\u6280\u80fd\u724c\u5168\u90e8\u6253\u51fa\n\u6309\u7167\u6280\u80fd\u724c\u70b9\u6570\u6263\u9664\u81ea\u8eabSP\u70b9ACE\u6280\u80fd\uff1a\n\u6447\u4e00\u4e2a6\u9762\u9ab0\u5b50\n\u628a\u6253\u51fa\u7684ACE\u724c\u70b9\u66ff\u6362\u6210\u6447\u51fa\u7684\u70b9\u6570\n\u518d\u628a\u4e09\u5f20\u624b\u724c\u5168\u90e8\u4f5c\u4e3a\u6280\u80fd\u724c\u6253\u51fa\n\u6309\u7167\u6280\u80fd\u724c\u70b9\u6570\u6263\u9664\u81ea\u8eabSP\u70b9\n\n\u3010\u5f00\u59cb\u6e38\u620f\u3011\n\u6251\u514b\u5bf9\u6218 \u3010\u91d1\u989d\u3011 \u3010at\u3011\uff08\u4e3a\u7a7a\u5219\u6240\u6709\u7fa4\u53cb\u90fd\u53ef\u63a5\u53d7\uff09\n\u3010\u56de\u5e94\u3011\n\u63a5\u53d7\u6311\u6218/\u62d2\u7edd\u6311\u6218\n\u3010\u56de\u5408\u4e2d\u3011\n\u51fa\u724c 1/2/3\uff08\u8f6e\u6d41\u51fa\u724c\uff09\n\u3010\u7ed3\u7b97\u3011\n\u7ed3\u7b97\uff08\u5f53\u67d0\u4e00\u65b960\u79d2\u6ca1\u6709\u56de\u5e94\uff0c\u4ee5\u76ee\u524d\u8840\u91cf\u7ed3\u7b97\uff09",
         "func": "\u6251\u514b\u5bf9\u6218",
         "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u4e00\u500d\u8d4c\u6ce8\u4e0a\u9650",
         "trigger_method": "\u6251\u514b\u5bf9\u6218 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
     },
     {
+        "brief_des": "\u53d1\u8d77\u731c\u6570\u5b57",
+        "detail_des": "\u901a\u8fc7 \u731c\u6570\u5b57 \u6765\u5bf9\u5176\u4ed6\u4eba\u5bf9\u6218\uff0c\u8f6e\u6d41\u731c\u6570\u5b57\uff0c\u731c\u4e2d\u6570\u5b57\u5373\u53ef\u83b7\u80dc\u3002\u6bcf\u8f6e\u8d4c\u6ce8\u90fd\u4f1a\u589e\u957f\u4e00\u500d",
+        "func": "\u731c\u6570\u5b57",
+        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u6bcf\u8f6e\u4e00\u500d\u8d4c\u6ce8\u4e0a\u9650",
+        "trigger_method": "\u731c\u6570\u5b57 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
+    },
+    {
         "brief_des": "\u521b\u5efa\u8d5b\u9a6c\u5c0f\u6e38\u620f",
         "detail_des": "\u6d41\u7a0b\uff1a\n\u8d5b\u9a6c\u521b\u5efa\uff1a\u7b2c\u4e00\u4f4d\u73a9\u5bb6\u53d1\u8d77\u6d3b\u52a8 \u2192\n\u8d5b\u9a6c\u52a0\u5165 \u3010\u4f60\u7684\u9a6c\u513f\u540d\u79f0\u3011\uff1a\u73a9\u5bb6\u53c2\u8d5b \u2192\n\u8d5b\u9a6c\u5f00\u59cb\uff1a\u6e38\u620f\u8fdb\u884c \u2192\n\u8fdb\u884c\u4e2d \u2192\n\u7ed3\u7b97\n\n\u5f53\u9047\u5230\u9519\u8bef\u6216\u5176\u4ed6\u60c5\u51b5\u53ef\u4f7f\u7528\u8d5b\u9a6c\u91cd\u7f6e\u6765\u91cd\u7f6e\u9a6c\u573a\u3002",
         "func": "\u8d5b\u9a6c\u5c0f\u6e38\u620f",
         "trigger_condition": "\u65e0",
         "trigger_method": "\u8d5b\u9a6c\u521b\u5efa"
     },
     {
```

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/utils/chart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.0/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 nonebot_plugin_game_collection/__init__.py
 nonebot_plugin_game_collection/config.py
 nonebot_plugin_game_collection.egg-info/PKG-INFO
 nonebot_plugin_game_collection.egg-info/SOURCES.txt
 nonebot_plugin_game_collection.egg-info/dependency_links.txt
 nonebot_plugin_game_collection.egg-info/requires.txt
 nonebot_plugin_game_collection.egg-info/top_level.txt
-nonebot_plugin_game_collection/.vs/ProjectSettings.json
-nonebot_plugin_game_collection/.vs/VSWorkspaceState.json
 nonebot_plugin_game_collection/HorseRace/events_main.py
 nonebot_plugin_game_collection/HorseRace/horse.py
 nonebot_plugin_game_collection/HorseRace/race_group.py
 nonebot_plugin_game_collection/HorseRace/start.py
 nonebot_plugin_game_collection/data/api.py
 nonebot_plugin_game_collection/data/data.py
 nonebot_plugin_game_collection/data/run.py
```

### Comparing `nonebot_plugin_game_collection-2.1.0/setup.py` & `nonebot_plugin_game_collection-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.1.0',
+version='2.1.1',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```


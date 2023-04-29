# Comparing `tmp/nonebot_plugin_game_collection-2.1.1.tar.gz` & `tmp/nonebot_plugin_game_collection-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.1.1.tar", last modified: Sat Apr 29 02:34:20 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.1.3.tar", last modified: Sat Apr 29 02:55:17 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.1.1.tar` & `nonebot_plugin_game_collection-2.1.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 02:34:20.004921 nonebot_plugin_game_collection-2.1.1/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.1/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-04-29 02:34:20.003419 nonebot_plugin_game_collection-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 02:34:19.929856 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    17615 2023-03-04 07:33:31.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0    41084 2023-03-04 07:28:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-04-29 02:34:19.949873 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15272 2023-02-28 15:49:25.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6237 2023-02-28 15:49:25.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     4999 2023-02-28 16:14:15.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     8962 2023-02-28 15:50:53.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    10909 2023-03-04 07:38:48.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    20122 2023-03-04 11:07:21.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    13072 2023-03-04 08:07:35.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    28653 2023-04-29 02:11:48.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3129 2023-03-04 11:53:52.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/config.py
-drwxrwxrwx   0        0        0        0 2023-04-29 02:34:19.956879 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/data/
--rw-rw-rw-   0        0        0      525 2023-02-24 19:49:14.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/data/api.py
--rw-rw-rw-   0        0        0     5589 2023-03-02 18:02:43.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/data/data.py
--rw-rw-rw-   0        0        0      102 2023-02-24 19:49:02.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/data/run.py
-drwxrwxrwx   0        0        0        0 2023-04-29 02:34:19.962384 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/
--rw-rw-rw-   0        0        0      171 2023-02-25 14:16:58.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/element_library.json
-drwxrwxrwx   0        0        0        0 2023-04-29 02:34:19.983402 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5335 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4372 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1692 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      861 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2616 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1208 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22088 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4569 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0      975 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2199 2023-02-25 14:16:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12610 2023-04-29 02:31:59.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     4976 2023-03-04 08:08:51.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-04-29 02:34:19.986905 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2347 2023-03-04 05:27:28.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-04-29 02:34:20.001417 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1321 2023-02-25 14:16:58.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0     7133 2023-02-27 17:39:47.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1619 2023-02-28 15:47:33.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-29 02:34:19.942367 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-04-29 02:34:19.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2038 2023-04-29 02:34:19.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 02:34:19.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-29 02:34:19.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-04-29 02:34:19.000000 nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 02:34:20.004921 nonebot_plugin_game_collection-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-29 02:34:15.000000 nonebot_plugin_game_collection-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.878164 nonebot_plugin_game_collection-2.1.3/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-04-29 02:55:17.877663 nonebot_plugin_game_collection-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.822116 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    17451 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0    41103 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.838130 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    11367 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    20097 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    13471 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    28768 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/config.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.843634 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/data/
+-rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/data/api.py
+-rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/data/data.py
+-rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/data/run.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.848639 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/
+-rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/element_library.json
+drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.868156 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12610 2023-04-29 02:52:46.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     4949 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.871157 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.876163 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0     7133 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.831624 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-04-29 02:55:17.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2038 2023-04-29 02:55:17.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 02:55:17.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-04-29 02:55:17.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-04-29 02:55:17.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 02:55:17.878164 nonebot_plugin_game_collection-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-29 02:55:13.000000 nonebot_plugin_game_collection-2.1.3/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.1.1/LICENSE` & `nonebot_plugin_game_collection-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.1/README.md` & `nonebot_plugin_game_collection-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Account.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,14 @@
     else:
         account = group_account
 
     account.props.setdefault(prop_code,0)
     account.props[prop_code] += count
     return f"你获得了{count}个【{prop_name}】！"
 
-
-
 def sign(event:MessageEvent) -> str:
     """
     签到
     """
     user,group_account = Manager.locate_user(event)
     if not group_account:
         return "私聊未关联账户，请发送【关联账户】关联群内账户。"
@@ -440,35 +438,32 @@
         delist_group = login_groups - groups
 
         log = ""
         # 处理与不存在的群相关的群账户
         for user_id in user_data:
             user = user_data[user_id]
             group_accounts = user.group_accounts
-            delist_group_accounts = set(group_accounts.keys()) & delist_group
-            for group_id in group_accounts:
+            accountset = set(group_accounts.keys())
+            delist_group_accounts = accountset & delist_group
+            for group_id in accountset:
                 group_account = group_accounts[group_id]
-                # 删除不存在的群账户
                 if group_id in delist_group_accounts:
+                    # 删除不存在的群账户
                     log += f'删除群账户：{user_id} - {group_id}\n'
                     del group_account
-                # 删除不存在的股票
                 else:
-                    for stock, count in group_account.stocks.items():
-                        if stock in delist_group:
-                            log += f'删除股票：{user_id} - {group_id} - {group_data[group_id].company.company_name} {count}'
-                            del group_account.stocks[stock]
+                    # 删除不存在的股票
+                    group_account.stocks = {stock:count for stock, count in group_account.stocks.items() if stock not in delist_group_accounts}
         # 删除不存在的群
         for group_id in delist_group:
             log += f'删除群：{group_id}\n'
             del group_data[group_id]
 
         # 已注册且存在的群
-        live_group = set(group_data.keys())
-        for group_id in live_group:
+        for group_id in list(group_data.keys()):
             users = await bot.get_group_member_list(group_id = group_id, no_cache = True)
             if users:
                 users = set(x["user_id"] for x in users)
             else:
                 continue
             # 删除已注册但不存在的用户
             namelist = group_data[group_id].namelist
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Game.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
     for x in race.player:
         uid = x.playeruid
         if uid in user_data:
             user = user_data[uid]
             user.gold += session.gold
             user.group_accounts[group_id].gold += session.gold
 
-    del race
+    del current_games[group_id]
     return "赛马场已重置。"
 
 
 """+++++++++++++++++
 ——————————
      其他小游戏
 ——————————
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-﻿from typing import List
-import random
-import math
-
-from .horse import horse
-from .events_main import event_main
-
-from ..config import setting_track_length, event_rate
-
-class race_group():
-    def __init__(self):
-        """
-        初始化
-        """
-        self.player:List[horse] = []
-        self.round = 0
-        self.start = 0 # start指示器：0为马儿进场未开始，1为开始，2为暂停（测试用）
-        self.race_only_keys = []
-
-    def add_player(self, horsename = "the_horse", uid = 0, id = "the_player",location = 0, round = 0):
-        """
-        增加赛马位
-        """
-        self.player.append(horse(horsename, uid, id, location, round))
-
-    def query_of_player(self):
-        """
-        赛马位数量查看
-        """
-        return len(self.player)
-
-    def is_player_in(self, uid):
-        """
-        查找有无玩家
-        """
-        for i in range(0, len(self.player)):
-            if self.player[i].playeruid == uid:
-                return True
-        return False
-
-    def round_add(self):
-        """
-        回合开始，回合数+1
-        """
-        self.round += 1
-        for i in range(0, len(self.player)):
-            self.player[i].round = self.round
-            self.player[i].location_add_move = 0
-
-    def del_buff_overtime(self):
-        """
-        所有马儿移除多余buff
-        """
-        for i in range(0, len(self.player)):
-            self.player[i].del_buff_overtime(self.round)
-
-    def fullname(self):
-        """
-        所有马儿buff+名称计算
-        """
-        for i in range(0, len(self.player)):
-            self.player[i].fullname()
-
-    def move(self):
-        """
-        所有马儿移动，移动计算已包含死亡/离开/止步判定
-        """
-        for i in range(0, len(self.player)):
-            self.player[i].location_move()
-
-    def display(self):
-        """
-        所有马儿数据显示（须先移动)
-        """
-        display = ""
-        for i in range(0, len(self.player)):
-            display += self.player[i].display()
-        return display
-
-    def is_die_all(self) -> bool:
-        """
-        所有马儿是否死亡/离开
-        """
-        for i in range(0, len(self.player)):
-            if ( self.player[i].is_die() == False ) and ( self.player[i].is_away() == False ):
-                return False
-        return True
-
-    def is_win_all(self):
-        """
-        所有马儿是否到终点
-        """
-        win_name = []
-        for i in range(0, len(self.player)):
-            if self.player[i].location >= setting_track_length:
-                win_name.append([self.player[i].player,self.player[i].playeruid])
-
-        return win_name
-
-    def event_start(self, events_list):
-        """
-        事件触发
-        """
-        event_display = f""
-        # 延时事件触发：
-        for i in range(0, len(self.player)):
-            if len(self.player[i].delay_events) > 0:
-                for j in range(len(self.player[i].delay_events)-1, -1, -1):
-                    if self.player[i].delay_events[j][0] == self.round:
-                        display_0 = event_main(self, i, self.player[i].delay_events[j][1], 1) + "\n"
-                        if display_0 != "\n":
-                            event_display += display_0
-                        del self.player[i].delay_events[j]
-        # buff随机事件触发
-        for i in range(0, len(self.player)):
-            for j in range(0, len(self.player[i].buff)):
-                if self.player[i].buff[j][5] != []:
-                    event_in_buff = self.player[i].buff[j][5]
-                    event_in_buff_num = len(event_in_buff)
-                    event_in_buff_rate = random.randint(0, event_in_buff[event_in_buff_num - 1][0])
-                    for k in range(0, event_in_buff_num):
-                        if event_in_buff_rate <= event_in_buff[k][0]:
-                            event_in_buff_x = event_in_buff[k][1]
-                            break
-                    display_0 = event_main(self, i, event_in_buff_x, 1) + "\n"
-                    if display_0 != "\n":
-                        event_display += display_0
-                        # 随机事件判定：
-        events_num = len(events_list)
-        for i in range(0, len(self.player)):
-            event_id = random.randint(0, math.ceil(1000 * events_num / event_rate) - 1)
-            if event_id < events_num:
-                event = events_list[event_id]
-                display_0 = event_main(self, i, event) + "\n"
-                if display_0 != "\n":
-                    event_display += display_0
-        return event_display
-
-    def is_race_only_key_in(self, key):
-        """
-        事件唯一码查询
-        """
-        try:
-            self.race_only_keys.index(key)
-            return True
-        except ValueError:
-            return False
-
-    def add_race_only_key(self, key):
-        """
-        事件唯一码增加
-        """
+﻿from typing import List
+import random
+import math
+
+from .horse import horse
+from .events_main import event_main
+
+from ..config import setting_track_length, event_rate
+
+class race_group():
+    def __init__(self):
+        """
+        初始化
+        """
+        self.player:List[horse] = []
+        self.round = 0
+        self.start = 0 # start指示器：0为马儿进场未开始，1为开始，2为暂停（测试用）
+        self.race_only_keys = []
+
+    def add_player(self, horsename = "the_horse", uid = 0, id = "the_player",location = 0, round = 0):
+        """
+        增加赛马位
+        """
+        self.player.append(horse(horsename, uid, id, location, round))
+
+    def query_of_player(self):
+        """
+        赛马位数量查看
+        """
+        return len(self.player)
+
+    def is_player_in(self, uid):
+        """
+        查找有无玩家
+        """
+        for i in range(0, len(self.player)):
+            if self.player[i].playeruid == uid:
+                return True
+        return False
+
+    def round_add(self):
+        """
+        回合开始，回合数+1
+        """
+        self.round += 1
+        for i in range(0, len(self.player)):
+            self.player[i].round = self.round
+            self.player[i].location_add_move = 0
+
+    def del_buff_overtime(self):
+        """
+        所有马儿移除多余buff
+        """
+        for i in range(0, len(self.player)):
+            self.player[i].del_buff_overtime(self.round)
+
+    def fullname(self):
+        """
+        所有马儿buff+名称计算
+        """
+        for i in range(0, len(self.player)):
+            self.player[i].fullname()
+
+    def move(self):
+        """
+        所有马儿移动，移动计算已包含死亡/离开/止步判定
+        """
+        for i in range(0, len(self.player)):
+            self.player[i].location_move()
+
+    def display(self):
+        """
+        所有马儿数据显示（须先移动)
+        """
+        display = ""
+        for i in range(0, len(self.player)):
+            display += self.player[i].display()
+        return display
+
+    def is_die_all(self) -> bool:
+        """
+        所有马儿是否死亡/离开
+        """
+        for i in range(0, len(self.player)):
+            if ( self.player[i].is_die() == False ) and ( self.player[i].is_away() == False ):
+                return False
+        return True
+
+    def is_win_all(self):
+        """
+        所有马儿是否到终点
+        """
+        win_name = []
+        for i in range(0, len(self.player)):
+            if self.player[i].location >= setting_track_length:
+                win_name.append([self.player[i].player,self.player[i].playeruid])
+
+        return win_name
+
+    def event_start(self, events_list):
+        """
+        事件触发
+        """
+        event_display = f""
+        # 延时事件触发：
+        for i in range(0, len(self.player)):
+            if len(self.player[i].delay_events) > 0:
+                for j in range(len(self.player[i].delay_events)-1, -1, -1):
+                    if self.player[i].delay_events[j][0] == self.round:
+                        display_0 = event_main(self, i, self.player[i].delay_events[j][1], 1) + "\n"
+                        if display_0 != "\n":
+                            event_display += display_0
+                        del self.player[i].delay_events[j]
+        # buff随机事件触发
+        for i in range(0, len(self.player)):
+            for j in range(0, len(self.player[i].buff)):
+                if self.player[i].buff[j][5] != []:
+                    event_in_buff = self.player[i].buff[j][5]
+                    event_in_buff_num = len(event_in_buff)
+                    event_in_buff_rate = random.randint(0, event_in_buff[event_in_buff_num - 1][0])
+                    for k in range(0, event_in_buff_num):
+                        if event_in_buff_rate <= event_in_buff[k][0]:
+                            event_in_buff_x = event_in_buff[k][1]
+                            break
+                    display_0 = event_main(self, i, event_in_buff_x, 1) + "\n"
+                    if display_0 != "\n":
+                        event_display += display_0
+                        # 随机事件判定：
+        events_num = len(events_list)
+        for i in range(0, len(self.player)):
+            event_id = random.randint(0, math.ceil(1000 * events_num / event_rate) - 1)
+            if event_id < events_num:
+                event = events_list[event_id]
+                display_0 = event_main(self, i, event) + "\n"
+                if display_0 != "\n":
+                    event_display += display_0
+        return event_display
+
+    def is_race_only_key_in(self, key):
+        """
+        事件唯一码查询
+        """
+        try:
+            self.race_only_keys.index(key)
+            return True
+        except ValueError:
+            return False
+
+    def add_race_only_key(self, key):
+        """
+        事件唯一码增加
+        """
         self.race_only_keys.append(key)
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-﻿from pathlib import Path
-from nonebot.log import logger
-try:
-    import ujson as json
-except ModuleNotFoundError:
-    import json
-from ..data.data import resourcefile
-
-
-def load_dlcs():
-    events_list = []
-    files = Path(resourcefile / "horserace").iterdir()
-    for x in files:
-        log = f"加载事件文件：{x.name}......"
-        try:
-            with open(x, "r", encoding="utf-8") as f:
-                events = deal_events(json.load(f))
-                events_list.extend(events)
-            logger.info(log + "成功!")
-        except Exception as e:
-            logger.info(log + "失败：" + e)
-    return events_list
-
-def deal_events(events):
-    events_out = []
-    for i in range(0,len(events)):
-        event_i = deal(events[i])
-        if event_i != {}:
-            events_out.append(event_i)
-    return events_out
-
-def deal(event):
-    event_out = {}
-    # 读取事件限定值
-    try:
-        event_out["race_only"] = event["race_only"]
-        event_out["race_only_exist"] = 1
-    except KeyError:
-        event_out["race_only_exist"] = 0
-    # 读取 event_name 无则未知事件
-    try:
-        event_out["event_name"] = event["event_name"]
-    except KeyError:
-        event_out["event_name"] = "未知事件"
-    # 读取 describe 事件描述，无描述则空
-    try:
-        event_out["describe"] = event["describe"]
-    except KeyError:
-        event_out["describe"] = f""
-    # 读取 target 目标，无则销毁事件
-    try:
-        event_out["target"] = event["target"]
-    except KeyError:
-        return {}
-    # 判定target_is_buff
-    try:
-        event_out["target_is_buff"] = event["target_is_buff"]
-    except KeyError:
-        event_out["target_is_buff"] = f""
-    # 判定target_no_buff
-    try:
-        event_out["target_no_buff"] = event["target_no_buff"]
-    except KeyError:
-        event_out["target_no_buff"] = f""
-    # ===============以下为一次性事件===============
-    # 复活事件：为1则目标复活
-    try:
-        event_out["live"] = event["live"]
-    except KeyError:
-        event_out["live"] = 0
-    # 位移事件：目标立即进行相当于参数值的位移
-    try:
-        event_out["move"] = event["move"]
-    except KeyError:
-        event_out["move"] = 0
-    # 随机位置事件：有值则让目标移动到指定位置
-    try:
-        event_out["track_to_location"] = event["track_to_location"]
-        event_out["track_to_location_exist"] = 1
-    except KeyError:
-        event_out["track_to_location_exist"] = 0
-    # 随机位置事件：为1则让目标随机位置（位置范围为可设定值，见setting.py）
-    try:
-        event_out["track_random_location"] = event["track_random_location"]
-    except KeyError:
-        event_out["track_random_location"] = 0
-    # buff持续时间调整事件：目标所有buff增加/减少回合数
-    try:
-        event_out["buff_time_add"] = event["buff_time_add"]
-    except KeyError:
-        event_out["buff_time_add"] = 0
-    # 删除buff事件：下回合删除目标含特定buff_tag的所有buff
-    try:
-        event_out["del_buff"] = event["del_buff"]
-    except KeyError:
-        event_out["del_buff"] = f""
-    # 换位事件：值为1则与目标更换位置 （仅target为1,6时生效）
-    try:
-        event_out["track_exchange_location"] = event["track_exchange_location"]
-    except KeyError:
-        event_out["track_exchange_location"] = 0
-    # 一次性随机事件
-    try:
-        event_out["random_event_once"] = event["random_event_once"]
-        if event_out["random_event_once"] != []:
-            for i in range(0, len(event_out["random_event_once"])):
-                event_out["random_event_once"][i][1] = deal(event_out["random_event_once"][i][1])
-    except KeyError:
-        event_out["random_event_once"] = []
-    # ===============以下为永久事件===============
-    # buff_tag，死亡：为1则目标死亡，此参数生成的buff默认持续999回合
-    # buff_tag：die的自定义名称，不填为“死亡”
-    try:
-        event_out["die"] = event["die"]
-    except KeyError:
-        event_out["die"] = 0
-    try:
-        event_out["die_name"] = event["die_name"]
-    except KeyError:
-        event_out["die_name"] = "死亡"
-    # buff_tag，离开：为1则目标离开，此参数生成的buff默认持续999回合
-    # buff_tag：away的自定义名称，不填为“离开”
-    try:
-        event_out["away"] = event["away"]
-    except KeyError:
-        event_out["away"] = 0
-    try:
-        event_out["away_name"] = event["away_name"]
-    except KeyError:
-        event_out["away_name"] = "离开"
-    # ==============================连锁事件预留位置，暂时没做
-
-    # ===============以下为buff事件===============
-    # "rounds": 0,                #buff持续回合数
-    # "name": "xxx",              #buff名称，turn值>0时为必要值
-    # "move_max": 0,              #该buff提供马儿每回合位移值区间的最大值（move_max若小于move_min，则move_max以move_min值为准）
-    # "move_min": 0,              #该buff提供马儿每回合位移值区间的最小值
-    # "locate_lock": 0,           #buff_tag，止步：若为1则目标无法移动
-    # "vertigo": 0,               #buff_tag，眩晕：若为1则目标无法移动，且不主动执行事件（暂定）
-    # "hiding": 0,                #buff_tag，隐身：不显示目标移动距离及位置
-    # "other_buff": ["buff1", "buff2", ....]
-    #                            #自定义buff_tag，仅标识用buff_tag填写处，也可以填入常规buff_tag并正常生效
-    # "random_event": [[概率值1, {事件}], [概率值2, {事件}], ......],
-    # 此为持续性随机事件，以buff形式存在，部分详见文末
-    try:
-        event_out["rounds"] = event["rounds"]
-    except KeyError:
-        event_out["rounds"] = 0
-    try:
-        event_out["name"] = event["name"]
-    except KeyError:
-        event_out["name"] = "未命名buff"
-    try:
-        event_out["move_max"] = event["move_max"]
-    except KeyError:
-        event_out["move_max"] = 0
-    try:
-        event_out["move_min"] = event["move_min"]
-    except KeyError:
-        event_out["move_min"] = 0
-    if event_out["move_max"] < event_out["move_min"]:
-        event_out["move_max"] = event_out["move_min"]
-    try:
-        event_out["locate_lock"] = event["locate_lock"]
-    except KeyError:
-        event_out["locate_lock"] = 0
-    try:
-        event_out["vertigo"] = event["vertigo"]
-    except KeyError:
-        event_out["vertigo"] = 0
-    try:
-        event_out["hiding"] = event["hiding"]
-    except KeyError:
-        event_out["hiding"] = 0
-    try:
-        event_out["other_buff"] = event["other_buff"]
-    except KeyError:
-        event_out["other_buff"] = []
-    try:
-        event_out["random_event"] = event["random_event"]
-        if event_out["random_event"] != []:
-            for i in range(0, len(event_out["random_event"])):
-                event_out["random_event"][i][1] = deal(event_out["random_event"][i][1])
-    except KeyError:
-        event_out["random_event"] = []
-    # ===============以下为延迟事件===============
-    # 延迟事件（以当前事件的targets为发起人的事件）：前者为多少回合后，需>1
-    try:
-        delay_event = event["delay_event"]
-        if event_out["delay_event"] != []:
-            event_out["delay_event"][1] = deal(event_out["delay_event"][1])
-    except KeyError:
-        event_out["delay_event"] = []
-    # 延迟事件（以当前事件发起人为发起人的事件）：前者为多少回合后，需>1
-    try:
-        event_out["delay_event_self"] = event["delay_event_self"]
-        if event_out["delay_event_self"] != []:
-            event_out["delay_event_self"][1] = deal(event_out["delay_event_self"][1])
-    except KeyError:
-        event_out["delay_event_self"] = []
-    # ===============以下同步事件===============
-    # 同步事件（以当前事件的targets为发起人的事件），执行此事件后立马执行该事件
-    try:
-        event_out["another_event"] = event["another_event"]
-        event_out["another_event"] = deal(event_out["another_event"])
-    except KeyError:
-        event_out["another_event"] = {}
-    # 同步事件（以当前事件发起人为发起人的事件），执行此事件后立马执行该事件
-    try:
-        event_out["another_event_self"] = event["another_event_self"]
-        event_out["another_event_self"] = deal(event_out["another_event_self"])
-    except KeyError:
-        event_out["another_event_self"] = {}
-    # ==========永久事件2，换赛道/加马==========
-    # 增加一匹马事件
-    try:
-        event_out["add_horse"] = event["add_horse"]
-    except KeyError:
-        event_out["add_horse"] = {}
-    # 替换一匹马事件
-    try:
-        event_out["replace_horse"] = event["replace_horse"]
-    except KeyError:
-        event_out["replace_horse"] = {}
-    return event_out
+﻿from pathlib import Path
+from nonebot.log import logger
+try:
+    import ujson as json
+except ModuleNotFoundError:
+    import json
+from ..data.data import resourcefile
+
+
+def load_dlcs():
+    events_list = []
+    files = Path(resourcefile / "horserace").iterdir()
+    for x in files:
+        log = f"加载事件文件：{x.name}......"
+        try:
+            with open(x, "r", encoding="utf-8") as f:
+                events = deal_events(json.load(f))
+                events_list.extend(events)
+            logger.info(log + "成功!")
+        except Exception as e:
+            logger.info(log + "失败：" + e)
+    return events_list
+
+def deal_events(events):
+    events_out = []
+    for i in range(0,len(events)):
+        event_i = deal(events[i])
+        if event_i != {}:
+            events_out.append(event_i)
+    return events_out
+
+def deal(event):
+    event_out = {}
+    # 读取事件限定值
+    try:
+        event_out["race_only"] = event["race_only"]
+        event_out["race_only_exist"] = 1
+    except KeyError:
+        event_out["race_only_exist"] = 0
+    # 读取 event_name 无则未知事件
+    try:
+        event_out["event_name"] = event["event_name"]
+    except KeyError:
+        event_out["event_name"] = "未知事件"
+    # 读取 describe 事件描述，无描述则空
+    try:
+        event_out["describe"] = event["describe"]
+    except KeyError:
+        event_out["describe"] = f""
+    # 读取 target 目标，无则销毁事件
+    try:
+        event_out["target"] = event["target"]
+    except KeyError:
+        return {}
+    # 判定target_is_buff
+    try:
+        event_out["target_is_buff"] = event["target_is_buff"]
+    except KeyError:
+        event_out["target_is_buff"] = f""
+    # 判定target_no_buff
+    try:
+        event_out["target_no_buff"] = event["target_no_buff"]
+    except KeyError:
+        event_out["target_no_buff"] = f""
+    # ===============以下为一次性事件===============
+    # 复活事件：为1则目标复活
+    try:
+        event_out["live"] = event["live"]
+    except KeyError:
+        event_out["live"] = 0
+    # 位移事件：目标立即进行相当于参数值的位移
+    try:
+        event_out["move"] = event["move"]
+    except KeyError:
+        event_out["move"] = 0
+    # 随机位置事件：有值则让目标移动到指定位置
+    try:
+        event_out["track_to_location"] = event["track_to_location"]
+        event_out["track_to_location_exist"] = 1
+    except KeyError:
+        event_out["track_to_location_exist"] = 0
+    # 随机位置事件：为1则让目标随机位置（位置范围为可设定值，见setting.py）
+    try:
+        event_out["track_random_location"] = event["track_random_location"]
+    except KeyError:
+        event_out["track_random_location"] = 0
+    # buff持续时间调整事件：目标所有buff增加/减少回合数
+    try:
+        event_out["buff_time_add"] = event["buff_time_add"]
+    except KeyError:
+        event_out["buff_time_add"] = 0
+    # 删除buff事件：下回合删除目标含特定buff_tag的所有buff
+    try:
+        event_out["del_buff"] = event["del_buff"]
+    except KeyError:
+        event_out["del_buff"] = f""
+    # 换位事件：值为1则与目标更换位置 （仅target为1,6时生效）
+    try:
+        event_out["track_exchange_location"] = event["track_exchange_location"]
+    except KeyError:
+        event_out["track_exchange_location"] = 0
+    # 一次性随机事件
+    try:
+        event_out["random_event_once"] = event["random_event_once"]
+        if event_out["random_event_once"] != []:
+            for i in range(0, len(event_out["random_event_once"])):
+                event_out["random_event_once"][i][1] = deal(event_out["random_event_once"][i][1])
+    except KeyError:
+        event_out["random_event_once"] = []
+    # ===============以下为永久事件===============
+    # buff_tag，死亡：为1则目标死亡，此参数生成的buff默认持续999回合
+    # buff_tag：die的自定义名称，不填为“死亡”
+    try:
+        event_out["die"] = event["die"]
+    except KeyError:
+        event_out["die"] = 0
+    try:
+        event_out["die_name"] = event["die_name"]
+    except KeyError:
+        event_out["die_name"] = "死亡"
+    # buff_tag，离开：为1则目标离开，此参数生成的buff默认持续999回合
+    # buff_tag：away的自定义名称，不填为“离开”
+    try:
+        event_out["away"] = event["away"]
+    except KeyError:
+        event_out["away"] = 0
+    try:
+        event_out["away_name"] = event["away_name"]
+    except KeyError:
+        event_out["away_name"] = "离开"
+    # ==============================连锁事件预留位置，暂时没做
+
+    # ===============以下为buff事件===============
+    # "rounds": 0,                #buff持续回合数
+    # "name": "xxx",              #buff名称，turn值>0时为必要值
+    # "move_max": 0,              #该buff提供马儿每回合位移值区间的最大值（move_max若小于move_min，则move_max以move_min值为准）
+    # "move_min": 0,              #该buff提供马儿每回合位移值区间的最小值
+    # "locate_lock": 0,           #buff_tag，止步：若为1则目标无法移动
+    # "vertigo": 0,               #buff_tag，眩晕：若为1则目标无法移动，且不主动执行事件（暂定）
+    # "hiding": 0,                #buff_tag，隐身：不显示目标移动距离及位置
+    # "other_buff": ["buff1", "buff2", ....]
+    #                            #自定义buff_tag，仅标识用buff_tag填写处，也可以填入常规buff_tag并正常生效
+    # "random_event": [[概率值1, {事件}], [概率值2, {事件}], ......],
+    # 此为持续性随机事件，以buff形式存在，部分详见文末
+    try:
+        event_out["rounds"] = event["rounds"]
+    except KeyError:
+        event_out["rounds"] = 0
+    try:
+        event_out["name"] = event["name"]
+    except KeyError:
+        event_out["name"] = "未命名buff"
+    try:
+        event_out["move_max"] = event["move_max"]
+    except KeyError:
+        event_out["move_max"] = 0
+    try:
+        event_out["move_min"] = event["move_min"]
+    except KeyError:
+        event_out["move_min"] = 0
+    if event_out["move_max"] < event_out["move_min"]:
+        event_out["move_max"] = event_out["move_min"]
+    try:
+        event_out["locate_lock"] = event["locate_lock"]
+    except KeyError:
+        event_out["locate_lock"] = 0
+    try:
+        event_out["vertigo"] = event["vertigo"]
+    except KeyError:
+        event_out["vertigo"] = 0
+    try:
+        event_out["hiding"] = event["hiding"]
+    except KeyError:
+        event_out["hiding"] = 0
+    try:
+        event_out["other_buff"] = event["other_buff"]
+    except KeyError:
+        event_out["other_buff"] = []
+    try:
+        event_out["random_event"] = event["random_event"]
+        if event_out["random_event"] != []:
+            for i in range(0, len(event_out["random_event"])):
+                event_out["random_event"][i][1] = deal(event_out["random_event"][i][1])
+    except KeyError:
+        event_out["random_event"] = []
+    # ===============以下为延迟事件===============
+    # 延迟事件（以当前事件的targets为发起人的事件）：前者为多少回合后，需>1
+    try:
+        delay_event = event["delay_event"]
+        if event_out["delay_event"] != []:
+            event_out["delay_event"][1] = deal(event_out["delay_event"][1])
+    except KeyError:
+        event_out["delay_event"] = []
+    # 延迟事件（以当前事件发起人为发起人的事件）：前者为多少回合后，需>1
+    try:
+        event_out["delay_event_self"] = event["delay_event_self"]
+        if event_out["delay_event_self"] != []:
+            event_out["delay_event_self"][1] = deal(event_out["delay_event_self"][1])
+    except KeyError:
+        event_out["delay_event_self"] = []
+    # ===============以下同步事件===============
+    # 同步事件（以当前事件的targets为发起人的事件），执行此事件后立马执行该事件
+    try:
+        event_out["another_event"] = event["another_event"]
+        event_out["another_event"] = deal(event_out["another_event"])
+    except KeyError:
+        event_out["another_event"] = {}
+    # 同步事件（以当前事件发起人为发起人的事件），执行此事件后立马执行该事件
+    try:
+        event_out["another_event_self"] = event["another_event_self"]
+        event_out["another_event_self"] = deal(event_out["another_event_self"])
+    except KeyError:
+        event_out["another_event_self"] = {}
+    # ==========永久事件2，换赛道/加马==========
+    # 增加一匹马事件
+    try:
+        event_out["add_horse"] = event["add_horse"]
+    except KeyError:
+        event_out["add_horse"] = {}
+    # 替换一匹马事件
+    try:
+        event_out["replace_horse"] = event["replace_horse"]
+    except KeyError:
+        event_out["replace_horse"] = {}
+    return event_out
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             return "图片下载失败"
         else:
             with open(BG_image / f"{str(event.user_id)}.png", 'wb') as f:
                 f.write(bytes_image)
             return "图片下载成功"
 
 async def del_BG_image(event:MessageEvent):
-    Path.unlink(BG_image / str(event.user_id),True)
+    Path.unlink(BG_image / f"{str(event.user_id)}.png", True)
     return "背景图片删除成功！"
 
 def Achieve_list(locate:Tuple[UserDict,GroupAccount]):
     """
     成就列表
     """
     user,group_account = locate
@@ -261,42 +261,47 @@
     return gini_coef(rank)
 
 def Newday():
     """
     刷新每日
     """
     log = ""
-
     group_check = {k:set() for k in group_data}
-
     global company_index
     update_company_index(company_index)
     company_ids = company_index.values()
     stock_check = {k:0 for k in company_ids}
-
     # 检查user_data
     for user_id in user_data:
         user = user_data[user_id]
         user.transfer_limit = 0
         props = user.props
         props = {k:v-1 if k[2] == '0' else v for k, v in props.items()}
         user.props = {k:v for k, v in props.items() if v > 0}
         group_accounts = user.group_accounts
         gold = 0
-        for group_id in group_accounts:
-            group_check[group_id].add(user_id)
-            group_account = group_accounts[group_id]
-            group_account.is_sign = False
-            gold += group_account.gold
-            props = group_account.props
-            props = {k:v-1 if k[2] == '0' else v for k, v in props.items()}
-            group_account.props = {k:v for k, v in props.items() if v > 0}
-            stocks = group_account.stocks
-            for company_id in stocks:
-                stock_check[company_id] += stocks[company_id]
+        for group_id in list(group_accounts.keys()):
+            if group_id not in group_check:
+                log += f"{user.nickname} 群账户{group_id}无效，已删除。\n"
+                del group_accounts[group_id]
+            else:
+                group_check[group_id].add(user_id)
+                group_account = group_accounts[group_id]
+                group_account.is_sign = False
+                gold += group_account.gold
+                props = group_account.props
+                props = {k:v-1 if k[2] == '0' else v for k, v in props.items()}
+                group_account.props = {k:v for k, v in props.items() if v > 0}
+                stocks = group_account.stocks
+                for company_id in list(stocks.keys()):
+                    if company_id in stock_check:
+                        stock_check[company_id] += stocks[company_id]
+                    else:
+                        log += f"{user.nickname} 群账户{group_id}内股票{company_id}回收异常，数据已修正。\n"
+                        del stocks[company_id]
         if user.gold != gold:
             log += f"{user.nickname} 金币总数异常。记录值：{user.gold} 实测值：{gold} 数据已修正。\n"
             user.gold = gold
 
     # 检查group_data
     for group_id in group_data:
         group = group_data[group_id]
@@ -315,13 +320,9 @@
                 log += (
                     f"{company.company_name} 股票数量异常。\n"
                     f"记录值：{company.stock}\n"
                     f"实测值：{company.issuance - stock_check[group_id]}\n"
                     "数据已修正。\n"
                     )
                 company.stock = company.issuance - stock_check[group_id]
-
-    del group_check
-    del company_ids
-    del stock_check
     data.save()
     return log[:-1] if log else "数据一切正常！"
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Market.py`

 * *Files 0% similar despite different names*

```diff
@@ -553,15 +553,15 @@
 
 def update():
     """
     刷新市场
     """
     log = ""
 
-    company_ids = list(set([company_index[x] for x in company_index]))
+    company_ids = set(company_index.values())
     for company_id in company_ids:
         company = group_data[company_id].company
         company_update(company)
         log += f"{company.company_name} 更新成功！\n"
 
     for user_id in user_data:
         group_accounts = user_data[user_id].group_accounts
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Prop.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     MessageSegment
     )
 import random
 
 from .utils.utils import get_message_at
 from .utils.chart import bbcode_to_png
 from .data.data import props_library, props_index, element_library
-from .config import sign_gold, revolt_gold,max_bet_gold, gacha_gold
+from .config import bot_name, sign_gold, revolt_gold,max_bet_gold, gacha_gold
 
 from .Manager import data
 from . import Manager
 
 user_data = data.user
 group_data = data.group
 
@@ -88,14 +88,15 @@
         prop_info = props_library.get(prop_code,{"name":prop_code, "color":"black","rare":1,"intro":"未知","des":"未知"})
         color = prop_info['color']
         name = prop_info['name']
         rare = prop_info['rare']
         msg += (f"[align=left][color={color}]【{name}】{rare*'☆'}[/align]\n"
                 f"[align=right]{n}{quant}[/color][/align][/size]\n"
                 f"[align=left][color=gray]——————————————[/color][/align]\n")
+        user.props = {k:10 if k[2] == '0' and v > 10 else v for k, v in user.props.items()}
         group_account.props = {k:v if v < 10 else 10 for k,v in group_account.props.items()}
     return MessageSegment.image(bbcode_to_png(msg[:-1]))
 
 class Prop(str):
     def use(self, event:MessageEvent, count:int):
         """
         使用道具
@@ -211,15 +212,15 @@
         props["42101"] -= 1
         if props["42101"] < 1:
             del props["42101"]
 
         target_user = user_data[at]
         target_group_account = target_user.group_accounts[group_id]
         N = random.randint(0,50)
-        if N < 20:
+        if N < 30:
             gold = int(group_account.gold * N / 1000)
             user.gold -= gold
             group_account.gold -= gold
             target_user.gold += gold
             target_group_account.gold += gold
             info = f"调查没有发现问题。你赔偿了对方{gold}枚金币"
         else:
@@ -304,40 +305,43 @@
         if not group_account:
             return "私聊未关联账户，请发送【关联账户】关联群内账户。"
         props = group_account.props
         if props.get("52102",0) < 1:
             return "数量不足"
 
         gold = group_account.gold
-
-        if count == 2:
+        if count == 1 or count == 2:
+            gold = int(gold/2)
+        if count == 2 or count == 4:
             if props.get("62101",0) > 1:
                 props["62101"] -= 1
                 if props["62101"] < 1:
                     del props["62101"]
             else:
                 return "钻石数量不足"
         else:
-            gold = gold if gold < (50 * max_bet_gold) else (50 * max_bet_gold)
+            gold = gold if gold < (limit := 50 * max_bet_gold) else limit
 
         props["52102"] -= 1
         if props["52102"] < 1:
             del props["52102"]
 
-
         if random.randint(0,1) == 1:
             user.gold += gold
             group_account.gold += gold
-            st = "获得"
+            return f"你获得了{gold}金币"
         else:
-            gold = int(gold/2)
             user.gold -= gold
             group_account.gold -= gold
-            st = "失去"
-        return f"你{st}了{gold}金币"
+            if gold > group_account.gold:
+                user.props.setdefault("53101",0)
+                user.props["53101"] += 1
+                return f"你失去了{gold}金币。\n{bot_name}送你1个『{props_library['53101']['name']}』，祝你好运~"
+            else:
+                return f"你失去了{gold}金币。"
 
     @classmethod
     def use_53101(cls, event:MessageEvent, count:int) -> str:
         """
         使用道具：随机红包
         """
         user,group_account = Manager.locate_user(event)
@@ -347,17 +351,15 @@
         if props.get("53101",0) < count:
             return "数量不足"
 
         props["53101"] -= count
         if props["53101"] < 1:
             del props["53101"]
 
-        gold = 0
-        for i in range(count):
-            gold += random.randint(sign_gold[0], revolt_gold[1])
+        gold = random.randint(sign_gold[0] * count, revolt_gold[1] * count)
 
         user.gold += gold
         group_account.gold += gold
         return f"你获得了{gold}金币。祝你好运~"
 
 def use_prop(event:MessageEvent, prop_name:str, count:int):
     if prop_code := props_index.get(prop_name):
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
     current_games[event.group_id].info["race_group"].start = 2
 
 # GameClear
 GameClear = on_command(
     "GameClear",
     aliases = {"清除游戏", "清除对局", "清除对决"},
     rule = lambda event:isinstance(event,GroupMessageEvent) and event.group_id in current_games,
+    permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
     priority = 20,
     block = True
     )
 
 @GameClear.handle()
 async def _(event:GroupMessageEvent):
     global current_games
@@ -246,15 +247,15 @@
 async def _(bot:Bot, event:GroupMessageEvent, arg:Message = CommandArg()):
     if not (msg := arg.extract_plain_text().strip().split()):
         return
     if len(msg) == 1:
         msg = msg[0]
         if not msg.isdigit():
             return
-        if (msg := int(msg)) < 7:
+        if 0 < (msg := int(msg)) < 7:
             bullet_num = msg
             gold = bet_gold
         else:
             bullet_num = 1
             gold = int(msg)
     else:
         if not (msg[0].isdigit() and msg[1].isdigit()):
@@ -491,15 +492,15 @@
 
 # 我的金币
 my_gold = on_command("我的金币", priority = 20, block = True)
 
 @my_gold.handle()
 async def _(event:MessageEvent):
     msg = Account.my_gold(event)
-    await my_gold.finish(msg)
+    await my_gold.finish(msg, at_sender = True)
 
 # 我的资料卡
 my_info = on_command("我的信息", aliases = {"我的资料"}, priority = 20, block = True)
 
 @my_info.handle()
 async def _(event:MessageEvent):
     msg = await Account.my_info(event)
@@ -515,23 +516,23 @@
 
 # 设置背景图片
 add_BG_image = on_command("设置背景图片", aliases = {"add_BG"}, priority = 20, block = True)
 
 @add_BG_image.handle()
 async def _(event:MessageEvent):
     msg = await Manager.add_BG_image(event)
-    await add_BG_image.finish(msg)
+    await add_BG_image.finish(msg, at_sender = True)
 
 # 删除背景图片
 del_BG_image = on_command("删除背景图片", aliases = {"del_BG"}, priority = 20, block = True)
 
 @del_BG_image.handle()
 async def _(event:MessageEvent):
     msg = await Manager.del_BG_image(event)
-    await del_BG_image.finish(msg)
+    await del_BG_image.finish(msg, at_sender = True)
 
 # 查看排行榜
 russian_rank = on_regex(
     r"^(总金币|总资产|金币|资产|财富|胜率|胜场|败场|路灯)(排行|榜)",
     permission = GROUP,
     priority = 20,
     block = True
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/data/api.py` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/data/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/data/data.py` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/data/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 20% similar despite different names*

```diff
@@ -1,274 +1,285 @@
-00000000: 5b0a 7b0a 2264 6573 6372 6962 6522 3a22  [.{."describe":"
-00000010: 3c30 3ee6 83b3 e8b5 b7e6 9da5 e4bb 8ae5  <0>.............
-00000020: a4a9 e698 afe7 96af e78b 82e6 989f e69c  ................
-00000030: 9fe5 9b9b efbc 8ce4 bb96 e9a3 9ee4 b880  ................
-00000040: e888 ace7 9a84 e6b6 a6e5 9091 e59c bae5  ................
-00000050: a496 efbc 88e6 97a0 e6b3 95e7 a7bb e58a  ................
-00000060: a8e4 b8a4 e59b 9ee5 9088 efbc 8922 2c0a  .............",.
-00000070: 2274 6172 6765 7422 3a30 2c0a 2274 7572  "target":0,."tur
-00000080: 6e22 3a32 2c0a 226e 616d 6522 3a22 6361  n":2,."name":"ca
-00000090: 7272 7922 2c0a 226c 6f63 6174 655f 6c6f  rry",."locate_lo
-000000a0: 636b 223a 310a 7d2c 0a7b 0a22 6465 7363  ck":1.},.{."desc
-000000b0: 7269 6265 223a 223c 303e e4b8 80e4 b88d  ribe":"<0>......
-000000c0: e795 99e7 a59e e8b8 a9e5 88b0 e4ba 86e9  ................
-000000d0: a699 e895 89e7 9aae efbc 8ce9 878d e987  ................
-000000e0: 8de7 9a84 e691 94e4 ba86 e4b8 80e8 b7a4  ................
-000000f0: efbc 88e6 97a0 e6b3 95e7 a7bb e58a a8e4  ................
-00000100: b880 e59b 9ee5 9088 efbc 8922 2c0a 2274  ...........",."t
-00000110: 6172 6765 7422 3a30 2c0a 2272 6f75 6e64  arget":0,."round
-00000120: 7322 3a31 2c20 200a 226e 616d 6522 3a22  s":1,  ."name":"
-00000130: e699 95e7 9ca9 222c 0a22 6c6f 6361 7465  ......",."locate
-00000140: 5f6c 6f63 6b22 3a31 0a7d 2c0a 7b0a 2264  _lock":1.},.{."d
-00000150: 6573 6372 6962 6522 3a22 3c30 3ee8 a789  escribe":"<0>...
-00000160: e986 92e4 ba86 e586 99e8 bdae e79c bcef  ................
-00000170: bc8c e5bc bae5 88b6 e4b8 8e3c 313e e4ba  ...........<1>..
-00000180: a4e6 8da2 e4ba 86e4 b880 e6ac a1e4 bd8d  ................
-00000190: e7bd ae22 2c0a 2274 6172 6765 7422 3a31  ...",."target":1
-000001a0: 2c0a 2274 7261 636b 5f65 7863 6861 6e67  ,."track_exchang
-000001b0: 655f 6c6f 6361 7469 6f6e 223a 310a 7d2c  e_location":1.},
-000001c0: 0a7b 0a20 2264 6573 6372 6962 6522 3a22  .{. "describe":"
-000001d0: 3c30 3ee6 8e8f e587 bae4 ba86 e4b8 80e6  <0>.............
-000001e0: 8a8a 5052 47ef bc8c e79e 84e5 8786 e4ba  ..PRG...........
-000001f0: 863c 313e e79a 84e5 b181 e882 a1ef bc8c  .<1>............
-00000200: e4b8 80e5 8f91 e585 a5e9 ad82 efbc 813c  ...............<
-00000210: 313e e8a6 81e5 af84 e4ba 86ef bc81 222c  1>............",
-00000220: 0a20 2274 6172 6765 7422 3a31 2c0a 2022  . "target":1,. "
-00000230: 6469 6522 3a31 2c0a 2022 6469 655f 6e61  die":1,. "die_na
-00000240: 6d65 223a 22e6 adbb e4ba a122 0a7d 2c0a  me":"......".},.
-00000250: 7b0a 2022 6465 7363 7269 6265 223a 223c  {. "describe":"<
-00000260: 303e e68e 8fe5 87ba e4ba 86e4 ba86 e7a5  0>..............
-00000270: 96e4 bca0 e79a 84e7 a59e e599 a8ef bc9a  ................
-00000280: e5a4 8de6 b4bb e794 b2ef bc81 e4bd 86e6  ................
-00000290: 98af e4bb 96e8 849a e6bb 91e4 ba86 e4b8  ................
-000002a0: 80e4 b88b e7bb 993c 313e e5a5 97e4 b88a  .......<1>......
-000002b0: e4ba 86ef bc81 222c 0a20 2274 6172 6765  ......",. "targe
-000002c0: 7422 3a31 2c0a 2022 6c69 7665 223a 310a  t":1,. "live":1.
-000002d0: 7d2c 0a7b 0a20 2264 6573 6372 6962 6522  },.{. "describe"
-000002e0: 3a22 3c30 3ee8 b8a9 e588 b0e4 ba86 e9a6  :"<0>...........
-000002f0: 99e8 9589 e79a aeef bc8c e4bd 86e6 98af  ................
-00000300: e4bb 96e6 98af e4b8 80e5 8faa e5ad a6e8  ................
-00000310: bf87 e88a ade8 95be e79a 84e9 a9ac efbc  ................
-00000320: 81ef bc88 e589 8de8 bf9b 312d 32ef bc89  ..........1-2...
-00000330: 222c 0a20 2274 6172 6765 7422 3a30 2c0a  ",. "target":0,.
-00000340: 2022 726f 756e 6473 223a 312c 2020 0a20   "rounds":1,  . 
-00000350: 226e 616d 6522 3a22 e586 b2e5 88ba 222c  "name":"......",
-00000360: 0a20 226d 6f76 655f 6d61 7822 3a32 2c0a  . "move_max":2,.
-00000370: 2022 6d6f 7665 5f6d 696e 223a 310a 7d2c   "move_min":1.},
-00000380: 0a7b 0a20 2264 6573 6372 6962 6522 3a22  .{. "describe":"
-00000390: 3c30 3ee4 b88d e5b0 8fe5 bf83 e8b8 a9e5  <0>.............
-000003a0: 88b0 e4ba 86e9 ad94 e6b3 95e9 98b5 2e2e  ................
-000003b0: 2e2e 2e2e 2ee8 bf99 e4b8 9ce8 a5bf e698  ................
-000003c0: afe8 b081 e694 bee5 9ca8 e8b5 9be5 9cba  ................
-000003d0: e4b8 8ae7 9a84 efbc 9fef bc88 e99a 8fe6  ................
-000003e0: 9cba e7a7 bbe5 8aa8 efbc 8922 2c0a 2022  ...........",. "
-000003f0: 7461 7267 6574 223a 302c 0a20 2274 7261  target":0,. "tra
-00000400: 636b 5f72 616e 646f 6d5f 6c6f 6361 7469  ck_random_locati
-00000410: 6f6e 223a 300a 7d2c 0a7b 0a20 2264 6573  on":0.},.{. "des
-00000420: 6372 6962 6522 3a22 3c30 3ee6 8993 e587  cribe":"<0>.....
-00000430: bae4 ba86 e4ba 94e8 b0b7 e4b8 b0e7 99bb  ................
-00000440: efbc 81e6 8980 e69c 89e9 a9ac e589 8de8  ................
-00000450: bf9b 312d 3322 2c0a 2022 7461 7267 6574  ..1-3",. "target
-00000460: 223a 322c 0a20 2274 7572 6e22 3a31 2c0a  ":2,. "turn":1,.
-00000470: 2022 6e61 6d65 223a 22e4 ba94 e8b0 b7e4   "name":".......
-00000480: b8b0 e799 bb22 2c0a 2022 6d6f 7665 5f6d  .....",. "move_m
-00000490: 6178 223a 332c 0a20 226d 6f76 655f 6d69  ax":3,. "move_mi
-000004a0: 6e22 3a31 0a7d 2c0a 7b0a 2022 6465 7363  n":1.},.{. "desc
-000004b0: 7269 6265 223a 223c 303e e689 93e5 87ba  ribe":"<0>......
-000004c0: e4ba 86e4 b887 e7ae ade9 bd90 e58f 91ef  ................
-000004d0: bc81 e999 a43c 303e e4bb a5e5 a496 e689  .....<0>........
-000004e0: 80e6 9c89 e9a9 ace5 8092 e980 8031 2d33  .............1-3
-000004f0: 222c 0a20 2274 6172 6765 7422 3a33 2c0a  ",. "target":3,.
-00000500: 2022 726f 756e 6473 223a 312c 0a20 226e   "rounds":1,. "n
-00000510: 616d 6522 3a22 e4b8 87e7 aead e9bd 90e5  ame":"..........
-00000520: 8f91 222c 0a20 226d 6f76 655f 6d61 7822  ..",. "move_max"
-00000530: 3a33 2c0a 2022 6d6f 7665 5f6d 696e 223a  :3,. "move_min":
-00000540: 310a 7d2c 0a7b 0a20 2264 6573 6372 6962  1.},.{. "describ
-00000550: 6522 3a22 3c30 3ee6 8993 e587 bae4 ba86  e":"<0>.........
-00000560: e58d 97e8 9bae e585 a5e4 beb5 efbc 81e9  ................
-00000570: 99a4 3c30 3ee4 bba5 e5a4 96e6 8980 e69c  ..<0>...........
-00000580: 89e9 a9ac e580 92e9 8080 3222 2c0a 2022  ..........2",. "
-00000590: 7461 7267 6574 223a 332c 0a20 2274 7572  target":3,. "tur
-000005a0: 6e22 3a31 2c0a 2022 6d6f 7665 223a 2d32  n":1,. "move":-2
-000005b0: 2c0a 2022 6e61 6d65 223a 22e5 8d97 e89b  ,. "name":".....
-000005c0: aee5 85a5 e4be b522 0a7d 2c0a 7b0a 2022  .......".},.{. "
-000005d0: 6465 7363 7269 6265 223a 22e8 b59b e59c  describe":".....
-000005e0: bae4 b88a e7aa 81e7 84b6 e593 8de8 b5b7  ................
-000005f0: e4ba 86e9 a9ac e584 bfe8 b7b3 efbc 81e9  ................
-00000600: 99a4 3c30 3ee4 bba5 e5a4 96e6 8980 e69c  ..<0>...........
-00000610: 89e9 a9ac e584 bfe9 83bd e6b2 89e6 b5b8  ................
-00000620: e59c a8e9 9fb3 e4b9 90e4 b8ad efbc 8ce6  ................
-00000630: 97a0 e6b3 95e7 a7bb e58a a8e4 b880 e59b  ................
-00000640: 9ee5 9088 222c 0a20 2274 6172 6765 7422  ....",. "target"
-00000650: 3a33 2c0a 2022 726f 756e 6473 223a 312c  :3,. "rounds":1,
-00000660: 2020 0a20 226e 616d 6522 3a22 e6b2 89e8    . "name":"....
-00000670: bfb7 222c 0a20 226c 6f63 6174 655f 6c6f  ..",. "locate_lo
-00000680: 636b 223a 310a 7d2c 0a7b 0a20 2264 6573  ck":1.},.{. "des
-00000690: 6372 6962 6522 3a22 e8b5 9be5 9cba e4b8  cribe":"........
-000006a0: 8ae7 aa81 e784 b6e5 938d e8b5 b7e4 ba86  ................
-000006b0: e5b8 8ce6 9c9b e4b9 8be8 8ab1 efbc 813c  ...............<
-000006c0: 313e e590 ace5 88b0 e4b9 8be5 908e e6b3  1>..............
-000006d0: aae6 b581 e6bb a1e9 9da2 efbc 81e4 bb96  ................
-000006e0: e4b8 8be5 ae9a e586 b3e5 bf83 e8a6 81e7  ................
-000006f0: bba7 e689 bfe5 9ba2 e995 bfe7 9a84 e684  ................
-00000700: 8fe5 bf97 efbc 8ce5 9091 e7bb 88e7 82b9  ................
-00000710: e9a3 9ee5 a594 e880 8ce5 8ebb efbc 81ef  ................
-00000720: bc88 e589 8de8 bf9b 33ef bc89 222c 0a20  ........3...",. 
-00000730: 2274 6172 6765 7422 3a31 2c0a 2022 6d6f  "target":1,. "mo
-00000740: 7665 223a 332c 0a20 226e 616d 6522 3a22  ve":3,. "name":"
-00000750: e4b8 8de8 a681 e581 9ce4 b88b e69d a5e5  ................
-00000760: 958a 220a 7d2c 0a7b 0a20 2264 6573 6372  ..".},.{. "descr
-00000770: 6962 6522 3a22 3c30 3ee5 8f91 e78e b0e7  ibe":"<0>.......
-00000780: 9c9f e5af bbe9 85b1 e59c a8e8 a782 e4bc  ................
-00000790: 97e5 b8ad e987 8ce4 b8ba e4bb 96e5 8aa0  ................
-000007a0: e6b2 b9ef bc81 3c30 3ee5 bc80 e5bf 83e7  ......<0>.......
-000007b0: 9a84 e69c 9de7 bb88 e782 b9e9 a39e e5a5  ................
-000007c0: 94e8 bf87 e58e bbef bc81 efbc 88e5 898d  ................
-000007d0: e8bf 9b32 efbc 8922 2c0a 2022 7461 7267  ...2...",. "targ
-000007e0: 6574 223a 302c 0a20 2272 6f75 6e64 7322  et":0,. "rounds"
-000007f0: 3a31 2c20 200a 2022 6d6f 7665 223a 320a  :1,  . "move":2.
-00000800: 7d2c 0a7b 0a20 2264 6573 6372 6962 6522  },.{. "describe"
-00000810: 3a22 3c30 3ee7 aa81 e784 b6e8 829a e5ad  :"<0>...........
-00000820: 90e4 b880 e998 b5e5 89a7 e797 9bef bc81  ................
-00000830: e4bb 96e7 8c9b e59c b0e6 83b3 e8b5 b7e6  ................
-00000840: 9da5 e698 a8e5 a4a9 e699 9ae4 b88a e590  ................
-00000850: 83e7 9a84 e7ba a2e4 bc9e e4bc 9ee8 b28c  ................
-00000860: e4bc bce6 9c89 e997 aee9 a298 efbc 81e5  ................
-00000870: 8faf e683 9ce5 b7b2 e7bb 8fe5 a4aa e8bf  ................
-00000880: 9fe4 ba86 e380 8222 2c0a 2022 7461 7267  .......",. "targ
-00000890: 6574 223a 302c 0a20 2264 6965 223a 312c  et":0,. "die":1,
-000008a0: 0a20 2264 6965 5f6e 616d 6522 3a22 e9a3  . "die_name":"..
-000008b0: 9fe7 89a9 e4b8 ade6 af92 220a 7d2c 0a7b  ..........".},.{
-000008c0: 0a20 2264 6573 6372 6962 6522 3a22 3c30  . "describe":"<0
-000008d0: 3ee6 8e8f e587 bae4 ba86 e6ba 9ce5 86b0  >...............
-000008e0: e99e 8bef bc8c e79c 8be6 9da5 e4bb 96e6  ................
-000008f0: 98af e69c 89e5 a487 e880 8ce6 9da5 efbc  ................
-00000900: 81ef bc88 e4b8 89e5 9b9e e590 88e6 af8f  ................
-00000910: e59b 9ee5 9088 e4bd 8de7 a7bb 312d 33ef  ............1-3.
-00000920: bc89 222c 0a20 2274 6172 6765 7422 3a30  ..",. "target":0
-00000930: 2c0a 2022 726f 756e 6473 223a 332c 2020  ,. "rounds":3,  
-00000940: 0a20 226e 616d 6522 3a22 e6ba 9ce5 86b0  . "name":"......
-00000950: 222c 0a20 226d 6f76 655f 6d61 7822 3a33  ",. "move_max":3
-00000960: 2c0a 2022 6d6f 7665 5f6d 696e 223a 310a  ,. "move_min":1.
-00000970: 7d2c 0a7b 0a20 2264 6573 6372 6962 6522  },.{. "describe"
-00000980: 3a22 3c30 3ee4 bb8e e5b8 bde5 ad90 e987  :"<0>...........
-00000990: 8ce6 8e8f e587 bae4 ba86 e998 94e5 8991  ................
-000009a0: e59c b0e9 9bb7 e5b9 b6e4 b8a2 e588 b0e4  ................
-000009b0: ba86 e8b5 9be9 8193 e4b8 8aef bc81 3c31  ..............<1
-000009c0: 3ee4 b880 e4b8 8de7 9599 e7a5 9ee8 b8a9  >...............
-000009d0: e4ba 86e4 b88a e58e bbef bc81 222c 0a20  ............",. 
-000009e0: 2274 6172 6765 7422 3a31 2c0a 2022 6469  "target":1,. "di
-000009f0: 6522 3a31 2c0a 2022 6469 655f 6e61 6d65  e":1,. "die_name
-00000a00: 223a 22e6 adbb e4ba a122 0a7d 2c0a 7b0a  ":"......".},.{.
-00000a10: 2022 6465 7363 7269 6265 223a 22e8 b59b   "describe":"...
-00000a20: e59c bae4 b88a e7aa 81e7 84b6 e593 8de8  ................
-00000a30: b5b7 e4ba 86e5 b18a e381 8be3 81aa e381  ................
-00000a40: 84e6 818b efbc 81e6 8980 e69c 89e9 a9ac  ................
-00000a50: e584 bfe5 90ac e588 b0e4 b98b e590 8ee9  ................
-00000a60: 83bd e683 b3e8 b5b7 e4ba 86e8 87aa e5b7  ................
-00000a70: b1e7 9a84 e5be 80e4 ba8b efbc 8ce8 baba  ................
-00000a80: e59c a8e8 b59b e59c bae4 b88a e593 ade4  ................
-00000a90: ba86 e8b5 b7e6 9da5 efbc 88e6 97a0 e6b3  ................
-00000aa0: 95e7 a7bb e58a a8e4 b880 e59b 9ee5 9088  ................
-00000ab0: efbc 8922 2c0a 2022 7461 7267 6574 223a  ...",. "target":
-00000ac0: 322c 0a20 2272 6f75 6e64 7322 3a31 2c20  2,. "rounds":1, 
-00000ad0: 200a 2022 6e61 6d65 223a 22e5 b18a e4b8   . "name":".....
-00000ae0: 8de5 88b0 222c 0a20 226c 6f63 6174 655f  ....",. "locate_
-00000af0: 6c6f 636b 223a 310a 7d2c 0a7b 0a20 2264  lock":1.},.{. "d
-00000b00: 6573 6372 6962 6522 3a22 3c30 3ee8 8491  escribe":"<0>...
-00000b10: e6b5 b7e4 b8ad e7aa 81e7 84b6 e997 aae8  ................
-00000b20: bf87 e4b8 80e5 8fa5 e592 92e8 afad efbc  ................
-00000b30: 8ce4 bb96 e4b8 8be6 848f e8af 86e7 9a84  ................
-00000b40: e8af bbe5 87ba e69d a5e4 b98b e590 8ee5  ................
-00000b50: 8f91 e78e b0e8 bf99 e5b1 85e7 84b6 e987  ................
-00000b60: 8ae6 94be e4ba 86e5 a4a7 e5a4 8de6 b4bb  ................
-00000b70: e69c afef bc81 efbc 88e5 85a8 e4bd 93e5  ................
-00000b80: a48d e6b4 bbef bc89 222c 0a20 2274 6172  ........",. "tar
-00000b90: 6765 7422 3a32 2c0a 2022 6c69 7665 223a  get":2,. "live":
-00000ba0: 310a 7d2c 0a7b 0a20 2264 6573 6372 6962  1.},.{. "describ
-00000bb0: 6522 3a22 3c30 3ee8 beb9 e8b7 91e8 beb9  e":"<0>.........
-00000bc0: e8b7 b3e8 b5b7 e4ba 86e9 92a2 e7ae a1e8  ................
-00000bd0: 889e efbc 813c 313e e8a2 abe9 ad85 e683  .....<1>........
-00000be0: 91e4 ba86 efbc 81ef bc88 e4ba 8ce5 9b9e  ................
-00000bf0: e590 88e4 b88d e883 bde7 a7bb e58a a8ef  ................
-00000c00: bc89 222c 0a20 2274 6172 6765 7422 3a31  ..",. "target":1
-00000c10: 2c0a 2022 726f 756e 6473 223a 312c 2020  ,. "rounds":1,  
-00000c20: 0a20 226e 616d 6522 3a22 e9ad 85e6 8391  . "name":"......
-00000c30: 222c 0a20 226c 6f63 6174 655f 6c6f 636b  ",. "locate_lock
-00000c40: 223a 310a 7d2c 0a7b 0a20 2264 6573 6372  ":1.},.{. "descr
-00000c50: 6962 6522 3a22 3c30 3ee9 878a e694 bee7  ibe":"<0>.......
-00000c60: a7bd e59c 9fe8 bdac e794 9fe7 9a84 e980  ................
-00000c70: 94e4 b8ad e689 93e4 ba86 e4b8 80e4 b8aa  ................
-00000c80: e596 b7e5 9a8f efbc 81e5 afbc e887 b4e5  ................
-00000c90: a48d e6b4 bbe7 9a84 e79b aee6 a087 e58f  ................
-00000ca0: 98e6 8890 e4ba 863c 313e efbc 8122 2c0a  .......<1>...",.
-00000cb0: 2022 7461 7267 6574 223a 312c 0a20 226c   "target":1,. "l
-00000cc0: 6976 6522 3a31 0a7d 2c0a 7b0a 2022 6465  ive":1.},.{. "de
-00000cd0: 7363 7269 6265 223a 223c 303e e7aa 81e7  scribe":"<0>....
-00000ce0: 84b6 e68e 8fe5 87ba e4ba 86e6 bb91 e69d  ................
-00000cf0: bfef bc81 2e2e 2e2e 2e2e 2e2e 2e2e e8bf  ................
-00000d00: 99e4 b89c e8a5 bfe6 98af e680 8ee4 b988  ................
-00000d10: e585 81e8 aeb8 e5b8 a6e5 85a5 e8b5 9be5  ................
-00000d20: 9cba e79a 843f 3f3f efbc 88e4 b889 e59b  .....???........
-00000d30: 9ee5 9088 e586 85e6 af8f e59b 9ee5 9088  ................
-00000d40: e4bd 8de7 a7bb 322d 34ef bc89 222c 0a20  ......2-4...",. 
-00000d50: 2274 6172 6765 7422 3a30 2c0a 2022 726f  "target":0,. "ro
-00000d60: 756e 6473 223a 332c 2020 0a20 226e 616d  unds":3,  . "nam
-00000d70: 6522 3a22 e6bb 91e6 9dbf 222c 0a20 226d  e":"......",. "m
-00000d80: 6f76 655f 6d61 7822 3a34 2c0a 2022 6d6f  ove_max":4,. "mo
-00000d90: 7665 5f6d 696e 223a 320a 7d2c 0a7b 0a20  ve_min":2.},.{. 
-00000da0: 2264 6573 6372 6962 6522 3a22 3c30 3ee7  "describe":"<0>.
-00000db0: aa81 e784 b6e5 8f91 e78e b0e8 baab e4b8  ................
-00000dc0: 8ae7 9a84 e680 80e8 a1a8 e581 9ce8 bdac  ................
-00000dd0: e4ba 86ef bc8c e4bb 96e8 a2ab e590 93e5  ................
-00000de0: be97 e987 8de9 878d e79a 84e6 9194 e4ba  ................
-00000df0: 86e4 b880 e8b7 a422 2c0a 2022 7461 7267  .......",. "targ
-00000e00: 6574 223a 302c 0a20 2264 6965 223a 312c  et":0,. "die":1,
-00000e10: 0a20 2264 6965 5f6e 616d 6522 3a22 e6ad  . "die_name":"..
-00000e20: bbe4 baa1 220a 7d2c 0a7b 0a20 2264 6573  ....".},.{. "des
-00000e30: 6372 6962 6522 3a22 3c30 3ee7 aa81 e784  cribe":"<0>.....
-00000e40: b6e9 81ad e58f 97e5 88b0 e4ba 86e4 ba8c  ................
-00000e50: e590 91e7 ae94 e689 93e5 87bb efbc 81e5  ................
-00000e60: 9ba0 e4b8 bae4 bb96 e6af abe6 97a0 e998  ................
-00000e70: b2e5 a487 e689 80e4 bba5 e79b b4e6 8ea5  ................
-00000e80: e5af 84e4 ba86 efbc 8122 2c0a 2022 7461  .........",. "ta
-00000e90: 7267 6574 223a 302c 0a20 2264 6965 223a  rget":0,. "die":
-00000ea0: 312c 0a20 2264 6965 5f6e 616d 6522 3a22  1,. "die_name":"
-00000eb0: e999 8de7 bbb4 e689 93e5 87bb 220a 7d2c  ............".},
-00000ec0: 0a7b 0a20 2264 6573 6372 6962 6522 3a22  .{. "describe":"
-00000ed0: e8b5 9be5 9cba e4b8 8ae7 aa81 e784 b6e4  ................
-00000ee0: b88b e8b5 b7e4 ba86 e99b b7e9 98b5 e99b  ................
-00000ef0: a8ef bc81 3c31 3ee5 be88 e4b8 8de5 b9b8  ....<1>.........
-00000f00: e79a 84e8 a2ab e99b b7e5 87bb e4b8 ade4  ................
-00000f10: ba86 efbc 81ef bc88 e9ba bbe7 97b9 e4b8  ................
-00000f20: a4e5 9b9e e590 88ef bc89 222c 0a20 2274  ..........",. "t
-00000f30: 6172 6765 7422 3a34 2c0a 2022 726f 756e  arget":4,. "roun
-00000f40: 6473 223a 322c 0a20 226e 616d 6522 3a22  ds":2,. "name":"
-00000f50: e9ba bbe7 97b9 222c 0a20 226c 6f63 6174  ......",. "locat
-00000f60: 655f 6c6f 636b 223a 310a 7d2c 0a7b 0a20  e_lock":1.},.{. 
-00000f70: 2264 6573 6372 6962 6522 3a22 3c31 3ee8  "describe":"<1>.
-00000f80: b8a9 e588 b0e4 ba86 e4b8 80e6 9e9a e992  ................
-00000f90: 89e5 ad90 efbc 81e4 bb96 e797 9be7 9a84  ................
-00000fa0: e8ba bae5 9ca8 e59c b0e4 b88a e79b b4e6  ................
-00000fb0: 8993 e6bb 9aef bc81 efbc 88e6 9a82 e581  ................
-00000fc0: 9ce4 b880 e59b 9ee5 9088 efbc 8922 2c0a  .............",.
-00000fd0: 2022 7461 7267 6574 223a 342c 0a20 2272   "target":4,. "r
-00000fe0: 6f75 6e64 7322 3a31 2c0a 2022 6e61 6d65  ounds":1,. "name
-00000ff0: 223a 22e7 96bc e797 9b22 2c0a 2022 6c6f  ":"......",. "lo
-00001000: 6361 7465 5f6c 6f63 6b22 3a31 0a7d 2c0a  cate_lock":1.},.
-00001010: 7b0a 2022 6465 7363 7269 6265 223a 22e5  {. "describe":".
-00001020: a4a9 e4b8 8ae7 aa81 e784 b6e6 8e89 e4b8  ................
-00001030: 8be6 9da5 e4b8 80e9 a297 e999 a8e7 9fb3  ................
-00001040: efbc 813c 313e e8a2 abe7 a0b8 e6ad bbe4  ...<1>..........
-00001050: ba86 efbc 8122 2c0a 2022 7461 7267 6574  .....",. "target
-00001060: 223a 342c 0a20 2264 6965 223a 312c 0a20  ":4,. "die":1,. 
-00001070: 2264 6965 5f6e 616d 6522 3a22 e7a0 b8e6  "die_name":"....
-00001080: 8981 220a 7d2c 0a7b 0a20 2264 6573 6372  ..".},.{. "descr
-00001090: 6962 6522 3a22 e59c bae5 a496 e7aa 81e7  ibe":"..........
-000010a0: 84b6 e9a3 9ee8 bf9b e69d a5e4 b880 e4b8  ................
-000010b0: aae6 a392 e790 83ef bc81 e7b2 bee5 8786  ................
-000010c0: e79a 84e7 a0b8 e588 b0e4 ba86 3c31 3ee7  ............<1>.
-000010d0: 9a84 e884 b8e4 b88a efbc 8122 2c0a 2022  ...........",. "
-000010e0: 7461 7267 6574 223a 342c 0a20 2264 6965  target":4,. "die
-000010f0: 223a 312c 0a20 2264 6965 5f6e 616d 6522  ":1,. "die_name"
-00001100: 3a22 e9a3 9ee6 9da5 e6a8 aae7 a5b8 220a  :"............".
-00001110: 7d0a 5d0a                                }.].
+00000000: 5b0d 0a7b 0d0a 2264 6573 6372 6962 6522  [..{.."describe"
+00000010: 3a22 3c30 3ee6 83b3 e8b5 b7e6 9da5 e4bb  :"<0>...........
+00000020: 8ae5 a4a9 e698 afe7 96af e78b 82e6 989f  ................
+00000030: e69c 9fe5 9b9b efbc 8ce4 bb96 e9a3 9ee4  ................
+00000040: b880 e888 ace7 9a84 e6b6 a6e5 9091 e59c  ................
+00000050: bae5 a496 efbc 88e6 97a0 e6b3 95e7 a7bb  ................
+00000060: e58a a8e4 b8a4 e59b 9ee5 9088 efbc 8922  ..............."
+00000070: 2c0d 0a22 7461 7267 6574 223a 302c 0d0a  ,.."target":0,..
+00000080: 2274 7572 6e22 3a32 2c0d 0a22 6e61 6d65  "turn":2,.."name
+00000090: 223a 2263 6172 7279 222c 0d0a 226c 6f63  ":"carry",.."loc
+000000a0: 6174 655f 6c6f 636b 223a 310d 0a7d 2c0d  ate_lock":1..},.
+000000b0: 0a7b 0d0a 2264 6573 6372 6962 6522 3a22  .{.."describe":"
+000000c0: 3c30 3ee4 b880 e4b8 8de7 9599 e7a5 9ee8  <0>.............
+000000d0: b8a9 e588 b0e4 ba86 e9a6 99e8 9589 e79a  ................
+000000e0: aeef bc8c e987 8de9 878d e79a 84e6 9194  ................
+000000f0: e4ba 86e4 b880 e8b7 a4ef bc88 e697 a0e6  ................
+00000100: b395 e7a7 bbe5 8aa8 e4b8 80e5 9b9e e590  ................
+00000110: 88ef bc89 222c 0d0a 2274 6172 6765 7422  ....",.."target"
+00000120: 3a30 2c0d 0a22 726f 756e 6473 223a 312c  :0,.."rounds":1,
+00000130: 2020 0d0a 226e 616d 6522 3a22 e699 95e7    .."name":"....
+00000140: 9ca9 222c 0d0a 226c 6f63 6174 655f 6c6f  ..",.."locate_lo
+00000150: 636b 223a 310d 0a7d 2c0d 0a7b 0d0a 2264  ck":1..},..{.."d
+00000160: 6573 6372 6962 6522 3a22 3c30 3ee8 a789  escribe":"<0>...
+00000170: e986 92e4 ba86 e586 99e8 bdae e79c bcef  ................
+00000180: bc8c e5bc bae5 88b6 e4b8 8e3c 313e e4ba  ...........<1>..
+00000190: a4e6 8da2 e4ba 86e4 b880 e6ac a1e4 bd8d  ................
+000001a0: e7bd ae22 2c0d 0a22 7461 7267 6574 223a  ...",.."target":
+000001b0: 312c 0d0a 2274 7261 636b 5f65 7863 6861  1,.."track_excha
+000001c0: 6e67 655f 6c6f 6361 7469 6f6e 223a 310d  nge_location":1.
+000001d0: 0a7d 2c0d 0a7b 0d0a 2022 6465 7363 7269  .},..{.. "descri
+000001e0: 6265 223a 223c 303e e68e 8fe5 87ba e4ba  be":"<0>........
+000001f0: 86e4 b880 e68a 8a50 5247 efbc 8ce7 9e84  .......PRG......
+00000200: e587 86e4 ba86 3c31 3ee7 9a84 e5b1 81e8  ......<1>.......
+00000210: 82a1 efbc 8ce4 b880 e58f 91e5 85a5 e9ad  ................
+00000220: 82ef bc81 3c31 3ee8 a681 e5af 84e4 ba86  ....<1>.........
+00000230: efbc 8122 2c0d 0a20 2274 6172 6765 7422  ...",.. "target"
+00000240: 3a31 2c0d 0a20 2264 6965 223a 312c 0d0a  :1,.. "die":1,..
+00000250: 2022 6469 655f 6e61 6d65 223a 22e6 adbb   "die_name":"...
+00000260: e4ba a122 0d0a 7d2c 0d0a 7b0d 0a20 2264  ..."..},..{.. "d
+00000270: 6573 6372 6962 6522 3a22 3c30 3ee6 8e8f  escribe":"<0>...
+00000280: e587 bae4 ba86 e4ba 86e7 a596 e4bc a0e7  ................
+00000290: 9a84 e7a5 9ee5 99a8 efbc 9ae5 a48d e6b4  ................
+000002a0: bbe7 94b2 efbc 81e4 bd86 e698 afe4 bb96  ................
+000002b0: e884 9ae6 bb91 e4ba 86e4 b880 e4b8 8be7  ................
+000002c0: bb99 3c31 3ee5 a597 e4b8 8ae4 ba86 efbc  ..<1>...........
+000002d0: 8122 2c0d 0a20 2274 6172 6765 7422 3a31  .",.. "target":1
+000002e0: 2c0d 0a20 226c 6976 6522 3a31 0d0a 7d2c  ,.. "live":1..},
+000002f0: 0d0a 7b0d 0a20 2264 6573 6372 6962 6522  ..{.. "describe"
+00000300: 3a22 3c30 3ee8 b8a9 e588 b0e4 ba86 e9a6  :"<0>...........
+00000310: 99e8 9589 e79a aeef bc8c e4bd 86e6 98af  ................
+00000320: e4bb 96e6 98af e4b8 80e5 8faa e5ad a6e8  ................
+00000330: bf87 e88a ade8 95be e79a 84e9 a9ac efbc  ................
+00000340: 81ef bc88 e589 8de8 bf9b 312d 32ef bc89  ..........1-2...
+00000350: 222c 0d0a 2022 7461 7267 6574 223a 302c  ",.. "target":0,
+00000360: 0d0a 2022 726f 756e 6473 223a 312c 2020  .. "rounds":1,  
+00000370: 0d0a 2022 6e61 6d65 223a 22e5 86b2 e588  .. "name":".....
+00000380: ba22 2c0d 0a20 226d 6f76 655f 6d61 7822  .",.. "move_max"
+00000390: 3a32 2c0d 0a20 226d 6f76 655f 6d69 6e22  :2,.. "move_min"
+000003a0: 3a31 0d0a 7d2c 0d0a 7b0d 0a20 2264 6573  :1..},..{.. "des
+000003b0: 6372 6962 6522 3a22 3c30 3ee4 b88d e5b0  cribe":"<0>.....
+000003c0: 8fe5 bf83 e8b8 a9e5 88b0 e4ba 86e9 ad94  ................
+000003d0: e6b3 95e9 98b5 2e2e 2e2e 2e2e 2ee8 bf99  ................
+000003e0: e4b8 9ce8 a5bf e698 afe8 b081 e694 bee5  ................
+000003f0: 9ca8 e8b5 9be5 9cba e4b8 8ae7 9a84 efbc  ................
+00000400: 9fef bc88 e99a 8fe6 9cba e7a7 bbe5 8aa8  ................
+00000410: efbc 8922 2c0d 0a20 2274 6172 6765 7422  ...",.. "target"
+00000420: 3a30 2c0d 0a20 2274 7261 636b 5f72 616e  :0,.. "track_ran
+00000430: 646f 6d5f 6c6f 6361 7469 6f6e 223a 300d  dom_location":0.
+00000440: 0a7d 2c0d 0a7b 0d0a 2022 6465 7363 7269  .},..{.. "descri
+00000450: 6265 223a 223c 303e e689 93e5 87ba e4ba  be":"<0>........
+00000460: 86e4 ba94 e8b0 b7e4 b8b0 e799 bbef bc81  ................
+00000470: e689 80e6 9c89 e9a9 ace5 898d e8bf 9b31  ...............1
+00000480: 2d33 222c 0d0a 2022 7461 7267 6574 223a  -3",.. "target":
+00000490: 322c 0d0a 2022 7475 726e 223a 312c 0d0a  2,.. "turn":1,..
+000004a0: 2022 6e61 6d65 223a 22e4 ba94 e8b0 b7e4   "name":".......
+000004b0: b8b0 e799 bb22 2c0d 0a20 226d 6f76 655f  .....",.. "move_
+000004c0: 6d61 7822 3a33 2c0d 0a20 226d 6f76 655f  max":3,.. "move_
+000004d0: 6d69 6e22 3a31 0d0a 7d2c 0d0a 7b0d 0a20  min":1..},..{.. 
+000004e0: 2264 6573 6372 6962 6522 3a22 3c30 3ee6  "describe":"<0>.
+000004f0: 8993 e587 bae4 ba86 e4b8 87e7 aead e9bd  ................
+00000500: 90e5 8f91 efbc 81e9 99a4 3c30 3ee4 bba5  ..........<0>...
+00000510: e5a4 96e6 8980 e69c 89e9 a9ac e580 92e9  ................
+00000520: 8080 312d 3322 2c0d 0a20 2274 6172 6765  ..1-3",.. "targe
+00000530: 7422 3a33 2c0d 0a20 2272 6f75 6e64 7322  t":3,.. "rounds"
+00000540: 3a31 2c0d 0a20 226e 616d 6522 3a22 e4b8  :1,.. "name":"..
+00000550: 87e7 aead e9bd 90e5 8f91 222c 0d0a 2022  ..........",.. "
+00000560: 6d6f 7665 5f6d 6178 223a 332c 0d0a 2022  move_max":3,.. "
+00000570: 6d6f 7665 5f6d 696e 223a 310d 0a7d 2c0d  move_min":1..},.
+00000580: 0a7b 0d0a 2022 6465 7363 7269 6265 223a  .{.. "describe":
+00000590: 223c 303e e689 93e5 87ba e4ba 86e5 8d97  "<0>............
+000005a0: e89b aee5 85a5 e4be b5ef bc81 e999 a43c  ...............<
+000005b0: 303e e4bb a5e5 a496 e689 80e6 9c89 e9a9  0>..............
+000005c0: ace5 8092 e980 8032 222c 0d0a 2022 7461  .......2",.. "ta
+000005d0: 7267 6574 223a 332c 0d0a 2022 7475 726e  rget":3,.. "turn
+000005e0: 223a 312c 0d0a 2022 6d6f 7665 223a 2d32  ":1,.. "move":-2
+000005f0: 2c0d 0a20 226e 616d 6522 3a22 e58d 97e8  ,.. "name":"....
+00000600: 9bae e585 a5e4 beb5 220d 0a7d 2c0d 0a7b  ........"..},..{
+00000610: 0d0a 2022 6465 7363 7269 6265 223a 22e8  .. "describe":".
+00000620: b59b e59c bae4 b88a e7aa 81e7 84b6 e593  ................
+00000630: 8de8 b5b7 e4ba 86e9 a9ac e584 bfe8 b7b3  ................
+00000640: efbc 81e9 99a4 3c30 3ee4 bba5 e5a4 96e6  ......<0>.......
+00000650: 8980 e69c 89e9 a9ac e584 bfe9 83bd e6b2  ................
+00000660: 89e6 b5b8 e59c a8e9 9fb3 e4b9 90e4 b8ad  ................
+00000670: efbc 8ce6 97a0 e6b3 95e7 a7bb e58a a8e4  ................
+00000680: b880 e59b 9ee5 9088 222c 0d0a 2022 7461  ........",.. "ta
+00000690: 7267 6574 223a 332c 0d0a 2022 726f 756e  rget":3,.. "roun
+000006a0: 6473 223a 312c 2020 0d0a 2022 6e61 6d65  ds":1,  .. "name
+000006b0: 223a 22e6 b289 e8bf b722 2c0d 0a20 226c  ":"......",.. "l
+000006c0: 6f63 6174 655f 6c6f 636b 223a 310d 0a7d  ocate_lock":1..}
+000006d0: 2c0d 0a7b 0d0a 2022 6465 7363 7269 6265  ,..{.. "describe
+000006e0: 223a 22e8 b59b e59c bae4 b88a e7aa 81e7  ":".............
+000006f0: 84b6 e593 8de8 b5b7 e4ba 86e5 b88c e69c  ................
+00000700: 9be4 b98b e88a b1ef bc81 3c31 3ee5 90ac  ..........<1>...
+00000710: e588 b0e4 b98b e590 8ee6 b3aa e6b5 81e6  ................
+00000720: bba1 e99d a2ef bc81 e4bb 96e4 b88b e5ae  ................
+00000730: 9ae5 86b3 e5bf 83e8 a681 e7bb a7e6 89bf  ................
+00000740: e59b a2e9 95bf e79a 84e6 848f e5bf 97ef  ................
+00000750: bc8c e590 91e7 bb88 e782 b9e9 a39e e5a5  ................
+00000760: 94e8 808c e58e bbef bc81 efbc 88e5 898d  ................
+00000770: e8bf 9b33 efbc 8922 2c0d 0a20 2274 6172  ...3...",.. "tar
+00000780: 6765 7422 3a31 2c0d 0a20 226d 6f76 6522  get":1,.. "move"
+00000790: 3a33 2c0d 0a20 226e 616d 6522 3a22 e4b8  :3,.. "name":"..
+000007a0: 8de8 a681 e581 9ce4 b88b e69d a5e5 958a  ................
+000007b0: 220d 0a7d 2c0d 0a7b 0d0a 2022 6465 7363  "..},..{.. "desc
+000007c0: 7269 6265 223a 223c 303e e58f 91e7 8eb0  ribe":"<0>......
+000007d0: e79c 9fe5 afbb e985 b1e5 9ca8 e8a7 82e4  ................
+000007e0: bc97 e5b8 ade9 878c e4b8 bae4 bb96 e58a  ................
+000007f0: a0e6 b2b9 efbc 813c 303e e5bc 80e5 bf83  .......<0>......
+00000800: e79a 84e6 9c9d e7bb 88e7 82b9 e9a3 9ee5  ................
+00000810: a594 e8bf 87e5 8ebb efbc 81ef bc88 e589  ................
+00000820: 8de8 bf9b 32ef bc89 222c 0d0a 2022 7461  ....2...",.. "ta
+00000830: 7267 6574 223a 302c 0d0a 2022 726f 756e  rget":0,.. "roun
+00000840: 6473 223a 312c 2020 0d0a 2022 6d6f 7665  ds":1,  .. "move
+00000850: 223a 320d 0a7d 2c0d 0a7b 0d0a 2022 6465  ":2..},..{.. "de
+00000860: 7363 7269 6265 223a 223c 303e e7aa 81e7  scribe":"<0>....
+00000870: 84b6 e882 9ae5 ad90 e4b8 80e9 98b5 e589  ................
+00000880: a7e7 979b efbc 81e4 bb96 e78c 9be5 9cb0  ................
+00000890: e683 b3e8 b5b7 e69d a5e6 98a8 e5a4 a9e6  ................
+000008a0: 999a e4b8 8ae5 9083 e79a 84e7 baa2 e4bc  ................
+000008b0: 9ee4 bc9e e8b2 8ce4 bcbc e69c 89e9 97ae  ................
+000008c0: e9a2 98ef bc81 e58f afe6 839c e5b7 b2e7  ................
+000008d0: bb8f e5a4 aae8 bf9f e4ba 86e3 8082 222c  ..............",
+000008e0: 0d0a 2022 7461 7267 6574 223a 302c 0d0a  .. "target":0,..
+000008f0: 2022 6469 6522 3a31 2c0d 0a20 2264 6965   "die":1,.. "die
+00000900: 5f6e 616d 6522 3a22 e9a3 9fe7 89a9 e4b8  _name":"........
+00000910: ade6 af92 220d 0a7d 2c0d 0a7b 0d0a 2022  ...."..},..{.. "
+00000920: 6465 7363 7269 6265 223a 223c 303e e68e  describe":"<0>..
+00000930: 8fe5 87ba e4ba 86e6 ba9c e586 b0e9 9e8b  ................
+00000940: efbc 8ce7 9c8b e69d a5e4 bb96 e698 afe6  ................
+00000950: 9c89 e5a4 87e8 808c e69d a5ef bc81 efbc  ................
+00000960: 88e4 b889 e59b 9ee5 9088 e6af 8fe5 9b9e  ................
+00000970: e590 88e4 bd8d e7a7 bb31 2d33 efbc 8922  .........1-3..."
+00000980: 2c0d 0a20 2274 6172 6765 7422 3a30 2c0d  ,.. "target":0,.
+00000990: 0a20 2272 6f75 6e64 7322 3a33 2c20 200d  . "rounds":3,  .
+000009a0: 0a20 226e 616d 6522 3a22 e6ba 9ce5 86b0  . "name":"......
+000009b0: 222c 0d0a 2022 6d6f 7665 5f6d 6178 223a  ",.. "move_max":
+000009c0: 332c 0d0a 2022 6d6f 7665 5f6d 696e 223a  3,.. "move_min":
+000009d0: 310d 0a7d 2c0d 0a7b 0d0a 2022 6465 7363  1..},..{.. "desc
+000009e0: 7269 6265 223a 223c 303e e4bb 8ee5 b8bd  ribe":"<0>......
+000009f0: e5ad 90e9 878c e68e 8fe5 87ba e4ba 86e9  ................
+00000a00: 9894 e589 91e5 9cb0 e99b b7e5 b9b6 e4b8  ................
+00000a10: a2e5 88b0 e4ba 86e8 b59b e981 93e4 b88a  ................
+00000a20: efbc 813c 313e e4b8 80e4 b88d e795 99e7  ...<1>..........
+00000a30: a59e e8b8 a9e4 ba86 e4b8 8ae5 8ebb efbc  ................
+00000a40: 8122 2c0d 0a20 2274 6172 6765 7422 3a31  .",.. "target":1
+00000a50: 2c0d 0a20 2264 6965 223a 312c 0d0a 2022  ,.. "die":1,.. "
+00000a60: 6469 655f 6e61 6d65 223a 22e6 adbb e4ba  die_name":".....
+00000a70: a122 0d0a 7d2c 0d0a 7b0d 0a20 2264 6573  ."..},..{.. "des
+00000a80: 6372 6962 6522 3a22 e8b5 9be5 9cba e4b8  cribe":"........
+00000a90: 8ae7 aa81 e784 b6e5 938d e8b5 b7e4 ba86  ................
+00000aa0: e5b1 8ae3 818b e381 aae3 8184 e681 8bef  ................
+00000ab0: bc81 e689 80e6 9c89 e9a9 ace5 84bf e590  ................
+00000ac0: ace5 88b0 e4b9 8be5 908e e983 bde6 83b3  ................
+00000ad0: e8b5 b7e4 ba86 e887 aae5 b7b1 e79a 84e5  ................
+00000ae0: be80 e4ba 8bef bc8c e8ba bae5 9ca8 e8b5  ................
+00000af0: 9be5 9cba e4b8 8ae5 93ad e4ba 86e8 b5b7  ................
+00000b00: e69d a5ef bc88 e697 a0e6 b395 e7a7 bbe5  ................
+00000b10: 8aa8 e4b8 80e5 9b9e e590 88ef bc89 222c  ..............",
+00000b20: 0d0a 2022 7461 7267 6574 223a 322c 0d0a  .. "target":2,..
+00000b30: 2022 726f 756e 6473 223a 312c 2020 0d0a   "rounds":1,  ..
+00000b40: 2022 6e61 6d65 223a 22e5 b18a e4b8 8de5   "name":".......
+00000b50: 88b0 222c 0d0a 2022 6c6f 6361 7465 5f6c  ..",.. "locate_l
+00000b60: 6f63 6b22 3a31 0d0a 7d2c 0d0a 7b0d 0a20  ock":1..},..{.. 
+00000b70: 2264 6573 6372 6962 6522 3a22 3c30 3ee8  "describe":"<0>.
+00000b80: 8491 e6b5 b7e4 b8ad e7aa 81e7 84b6 e997  ................
+00000b90: aae8 bf87 e4b8 80e5 8fa5 e592 92e8 afad  ................
+00000ba0: efbc 8ce4 bb96 e4b8 8be6 848f e8af 86e7  ................
+00000bb0: 9a84 e8af bbe5 87ba e69d a5e4 b98b e590  ................
+00000bc0: 8ee5 8f91 e78e b0e8 bf99 e5b1 85e7 84b6  ................
+00000bd0: e987 8ae6 94be e4ba 86e5 a4a7 e5a4 8de6  ................
+00000be0: b4bb e69c afef bc81 efbc 88e5 85a8 e4bd  ................
+00000bf0: 93e5 a48d e6b4 bbef bc89 222c 0d0a 2022  ..........",.. "
+00000c00: 7461 7267 6574 223a 322c 0d0a 2022 6c69  target":2,.. "li
+00000c10: 7665 223a 310d 0a7d 2c0d 0a7b 0d0a 2022  ve":1..},..{.. "
+00000c20: 6465 7363 7269 6265 223a 223c 303e e8be  describe":"<0>..
+00000c30: b9e8 b791 e8be b9e8 b7b3 e8b5 b7e4 ba86  ................
+00000c40: e992 a2e7 aea1 e888 9eef bc81 3c31 3ee8  ............<1>.
+00000c50: a2ab e9ad 85e6 8391 e4ba 86ef bc81 efbc  ................
+00000c60: 88e4 ba8c e59b 9ee5 9088 e4b8 8de8 83bd  ................
+00000c70: e7a7 bbe5 8aa8 efbc 8922 2c0d 0a20 2274  .........",.. "t
+00000c80: 6172 6765 7422 3a31 2c0d 0a20 2272 6f75  arget":1,.. "rou
+00000c90: 6e64 7322 3a31 2c20 200d 0a20 226e 616d  nds":1,  .. "nam
+00000ca0: 6522 3a22 e9ad 85e6 8391 222c 0d0a 2022  e":"......",.. "
+00000cb0: 6c6f 6361 7465 5f6c 6f63 6b22 3a31 0d0a  locate_lock":1..
+00000cc0: 7d2c 0d0a 7b0d 0a20 2264 6573 6372 6962  },..{.. "describ
+00000cd0: 6522 3a22 3c30 3ee9 878a e694 bee7 a7bd  e":"<0>.........
+00000ce0: e59c 9fe8 bdac e794 9fe7 9a84 e980 94e4  ................
+00000cf0: b8ad e689 93e4 ba86 e4b8 80e4 b8aa e596  ................
+00000d00: b7e5 9a8f efbc 81e5 afbc e887 b4e5 a48d  ................
+00000d10: e6b4 bbe7 9a84 e79b aee6 a087 e58f 98e6  ................
+00000d20: 8890 e4ba 863c 313e efbc 8122 2c0d 0a20  .....<1>...",.. 
+00000d30: 2274 6172 6765 7422 3a31 2c0d 0a20 226c  "target":1,.. "l
+00000d40: 6976 6522 3a31 0d0a 7d2c 0d0a 7b0d 0a20  ive":1..},..{.. 
+00000d50: 2264 6573 6372 6962 6522 3a22 3c30 3ee7  "describe":"<0>.
+00000d60: aa81 e784 b6e6 8e8f e587 bae4 ba86 e6bb  ................
+00000d70: 91e6 9dbf efbc 812e 2e2e 2e2e 2e2e 2e2e  ................
+00000d80: 2ee8 bf99 e4b8 9ce8 a5bf e698 afe6 808e  ................
+00000d90: e4b9 88e5 8581 e8ae b8e5 b8a6 e585 a5e8  ................
+00000da0: b59b e59c bae7 9a84 3f3f 3fef bc88 e4b8  ........???.....
+00000db0: 89e5 9b9e e590 88e5 8685 e6af 8fe5 9b9e  ................
+00000dc0: e590 88e4 bd8d e7a7 bb32 2d34 efbc 8922  .........2-4..."
+00000dd0: 2c0d 0a20 2274 6172 6765 7422 3a30 2c0d  ,.. "target":0,.
+00000de0: 0a20 2272 6f75 6e64 7322 3a33 2c20 200d  . "rounds":3,  .
+00000df0: 0a20 226e 616d 6522 3a22 e6bb 91e6 9dbf  . "name":"......
+00000e00: 222c 0d0a 2022 6d6f 7665 5f6d 6178 223a  ",.. "move_max":
+00000e10: 342c 0d0a 2022 6d6f 7665 5f6d 696e 223a  4,.. "move_min":
+00000e20: 320d 0a7d 2c0d 0a7b 0d0a 2022 6465 7363  2..},..{.. "desc
+00000e30: 7269 6265 223a 223c 303e e7aa 81e7 84b6  ribe":"<0>......
+00000e40: e58f 91e7 8eb0 e8ba abe4 b88a e79a 84e6  ................
+00000e50: 8080 e8a1 a8e5 819c e8bd ace4 ba86 efbc  ................
+00000e60: 8ce4 bb96 e8a2 abe5 9093 e5be 97e9 878d  ................
+00000e70: e987 8de7 9a84 e691 94e4 ba86 e4b8 80e8  ................
+00000e80: b7a4 222c 0d0a 2022 7461 7267 6574 223a  ..",.. "target":
+00000e90: 302c 0d0a 2022 6469 6522 3a31 2c0d 0a20  0,.. "die":1,.. 
+00000ea0: 2264 6965 5f6e 616d 6522 3a22 e6ad bbe4  "die_name":"....
+00000eb0: baa1 220d 0a7d 2c0d 0a7b 0d0a 2022 6465  .."..},..{.. "de
+00000ec0: 7363 7269 6265 223a 223c 303e e7aa 81e7  scribe":"<0>....
+00000ed0: 84b6 e981 ade5 8f97 e588 b0e4 ba86 e4ba  ................
+00000ee0: 8ce5 9091 e7ae 94e6 8993 e587 bbef bc81  ................
+00000ef0: e59b a0e4 b8ba e4bb 96e6 afab e697 a0e9  ................
+00000f00: 98b2 e5a4 87e6 8980 e4bb a5e7 9bb4 e68e  ................
+00000f10: a5e5 af84 e4ba 86ef bc81 222c 0d0a 2022  ..........",.. "
+00000f20: 7461 7267 6574 223a 302c 0d0a 2022 6469  target":0,.. "di
+00000f30: 6522 3a31 2c0d 0a20 2264 6965 5f6e 616d  e":1,.. "die_nam
+00000f40: 6522 3a22 e999 8de7 bbb4 e689 93e5 87bb  e":"............
+00000f50: 220d 0a7d 2c0d 0a7b 0d0a 2022 6465 7363  "..},..{.. "desc
+00000f60: 7269 6265 223a 22e8 b59b e59c bae4 b88a  ribe":".........
+00000f70: e7aa 81e7 84b6 e4b8 8be8 b5b7 e4ba 86e9  ................
+00000f80: 9bb7 e998 b5e9 9ba8 efbc 813c 313e e5be  ...........<1>..
+00000f90: 88e4 b88d e5b9 b8e7 9a84 e8a2 abe9 9bb7  ................
+00000fa0: e587 bbe4 b8ad e4ba 86ef bc81 efbc 88e9  ................
+00000fb0: babb e797 b9e4 b8a4 e59b 9ee5 9088 efbc  ................
+00000fc0: 8922 2c0d 0a20 2274 6172 6765 7422 3a34  .",.. "target":4
+00000fd0: 2c0d 0a20 2272 6f75 6e64 7322 3a32 2c0d  ,.. "rounds":2,.
+00000fe0: 0a20 226e 616d 6522 3a22 e9ba bbe7 97b9  . "name":"......
+00000ff0: 222c 0d0a 2022 6c6f 6361 7465 5f6c 6f63  ",.. "locate_loc
+00001000: 6b22 3a31 0d0a 7d2c 0d0a 7b0d 0a20 2264  k":1..},..{.. "d
+00001010: 6573 6372 6962 6522 3a22 3c31 3ee8 b8a9  escribe":"<1>...
+00001020: e588 b0e4 ba86 e4b8 80e6 9e9a e992 89e5  ................
+00001030: ad90 efbc 81e4 bb96 e797 9be7 9a84 e8ba  ................
+00001040: bae5 9ca8 e59c b0e4 b88a e79b b4e6 8993  ................
+00001050: e6bb 9aef bc81 efbc 88e6 9a82 e581 9ce4  ................
+00001060: b880 e59b 9ee5 9088 efbc 8922 2c0d 0a20  ...........",.. 
+00001070: 2274 6172 6765 7422 3a34 2c0d 0a20 2272  "target":4,.. "r
+00001080: 6f75 6e64 7322 3a31 2c0d 0a20 226e 616d  ounds":1,.. "nam
+00001090: 6522 3a22 e796 bce7 979b 222c 0d0a 2022  e":"......",.. "
+000010a0: 6c6f 6361 7465 5f6c 6f63 6b22 3a31 0d0a  locate_lock":1..
+000010b0: 7d2c 0d0a 7b0d 0a20 2264 6573 6372 6962  },..{.. "describ
+000010c0: 6522 3a22 e5a4 a9e4 b88a e7aa 81e7 84b6  e":"............
+000010d0: e68e 89e4 b88b e69d a5e4 b880 e9a2 97e9  ................
+000010e0: 99a8 e79f b3ef bc81 3c31 3ee8 a2ab e7a0  ........<1>.....
+000010f0: b8e6 adbb e4ba 86ef bc81 222c 0d0a 2022  ..........",.. "
+00001100: 7461 7267 6574 223a 342c 0d0a 2022 6469  target":4,.. "di
+00001110: 6522 3a31 2c0d 0a20 2264 6965 5f6e 616d  e":1,.. "die_nam
+00001120: 6522 3a22 e7a0 b8e6 8981 220d 0a7d 2c0d  e":"......"..},.
+00001130: 0a7b 0d0a 2022 6465 7363 7269 6265 223a  .{.. "describe":
+00001140: 22e5 9cba e5a4 96e7 aa81 e784 b6e9 a39e  "...............
+00001150: e8bf 9be6 9da5 e4b8 80e4 b8aa e6a3 92e7  ................
+00001160: 9083 efbc 81e7 b2be e587 86e7 9a84 e7a0  ................
+00001170: b8e5 88b0 e4ba 863c 313e e79a 84e8 84b8  .......<1>......
+00001180: e4b8 8aef bc81 222c 0d0a 2022 7461 7267  ......",.. "targ
+00001190: 6574 223a 342c 0d0a 2022 6469 6522 3a31  et":4,.. "die":1
+000011a0: 2c0d 0a20 2264 6965 5f6e 616d 6522 3a22  ,.. "die_name":"
+000011b0: e9a3 9ee6 9da5 e6a8 aae7 a5b8 220d 0a7d  ............"..}
+000011c0: 0d0a 5d0d 0a                             ..]..
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 27% similar despite different names*

```diff
@@ -1,106 +1,110 @@
-00000000: 5b0a 7b0a 2022 6576 656e 745f 6e61 6d65  [.{. "event_name
-00000010: 223a 22e5 858b e88b 8fe9 b281 e4ba 8be4  ":".............
-00000020: bbb6 3122 2c0a 2022 6465 7363 7269 6265  ..1",. "describe
-00000030: 223a 223c 303e e7aa 81e7 84b6 e684 9fe8  ":"<0>..........
-00000040: a789 e8a7 82e4 bc97 e5b8 ade4 b8ad e69c  ................
-00000050: 89e4 b880 e58f 8ce7 9cbc e79d 9be5 9ca8  ................
-00000060: e79b afe7 9d80 e4bb 9622 2c0a 2022 7461  .........",. "ta
-00000070: 7267 6574 223a 300a 7d2c 0a7b 0a20 2265  rget":0.},.{. "e
-00000080: 7665 6e74 5f6e 616d 6522 3a22 e585 8be8  vent_name":"....
-00000090: 8b8f e9b2 81e4 ba8b e4bb b632 222c 0a20  ...........2",. 
-000000a0: 2264 6573 6372 6962 6522 3a22 3c30 3ee6  "describe":"<0>.
-000000b0: 849f e8a7 89e8 baab e8be b9e8 b28c e4bc  ................
-000000c0: bce9 99a4 e4ba 86e8 b59b e9a9 ace4 bba5  ................
-000000d0: e5a4 96e8 bf98 e69c 89e4 b880 e4ba 9be5  ................
-000000e0: 85b6 e5ae 83e4 b89c e8a5 bf22 2c0a 2022  ...........",. "
-000000f0: 7461 7267 6574 223a 300a 7d2c 0a7b 0a20  target":0.},.{. 
-00000100: 2265 7665 6e74 5f6e 616d 6522 3a22 e585  "event_name":"..
-00000110: 8be8 8b8f e9b2 81e4 ba8b e4bb b633 222c  .............3",
-00000120: 0a20 2264 6573 6372 6962 6522 3a22 3c30  . "describe":"<0
-00000130: 3ee4 b88d e79b b8e4 bfa1 e4b8 96e7 958c  >...............
-00000140: e4b8 8ae6 9c89 e4bb 80e4 b988 e5a5 87e6  ................
-00000150: 80aa e79a 84e4 b89c e8a5 bf22 2c0a 2022  ...........",. "
-00000160: 7461 7267 6574 223a 300a 7d2c 0a7b 0a20  target":0.},.{. 
-00000170: 2265 7665 6e74 5f6e 616d 6522 3a22 e585  "event_name":"..
-00000180: 8be8 8b8f e9b2 81e4 ba8b e4bb b634 222c  .............4",
-00000190: 0a20 2264 6573 6372 6962 6522 3a22 3c30  . "describe":"<0
-000001a0: 3ee6 849f e8a7 89e4 bb8a e5a4 a9e5 a4aa  >...............
-000001b0: e998 b3e5 8589 e79a 84e9 a29c e889 b2e6  ................
-000001c0: 9c89 e4ba 9be4 b88d e5af b9ef bc8c e4bc  ................
-000001d0: bce4 b98e e6af 94e5 b9b3 e5b8 b8e6 9a97  ................
-000001e0: e4ba 86e8 aeb8 e5a4 9a22 2c0a 2022 7461  .........",. "ta
-000001f0: 7267 6574 223a 300a 7d2c 0a7b 0a20 2265  rget":0.},.{. "e
-00000200: 7665 6e74 5f6e 616d 6522 3a22 e585 8be8  vent_name":"....
-00000210: 8b8f e9b2 81e4 ba8b e4bb b635 222c 0a20  ...........5",. 
-00000220: 2264 6573 6372 6962 6522 3a22 3c30 3ee6  "describe":"<0>.
-00000230: 849f e8a7 89e6 9c89 e4bb 80e4 b988 e280  ................
-00000240: 9ce4 b89c e8a5 bfe2 809d e59c a8e6 8e90  ................
-00000250: e79d 80e8 87aa e5b7 b1e7 9a84 e596 89e5  ................
-00000260: 9299 222c 0a20 2274 6172 6765 7422 3a30  ..",. "target":0
-00000270: 2c0a 2022 726f 756e 6473 223a 312c 0a20  ,. "rounds":1,. 
-00000280: 226e 616d 6522 3a22 e7bc bae6 b0a7 222c  "name":"......",
-00000290: 0a20 226c 6f63 6174 655f 6c6f 636b 223a  . "locate_lock":
-000002a0: 310a 7d2c 0a7b 0a20 2265 7665 6e74 5f6e  1.},.{. "event_n
-000002b0: 616d 6522 3a22 e585 8be8 8b8f e9b2 81e4  ame":"..........
-000002c0: ba8b e4bb b636 222c 0a20 2264 6573 6372  .....6",. "descr
-000002d0: 6962 6522 3a22 3c30 3ee7 aa81 e784 b6e6  ibe":"<0>.......
-000002e0: 849f e8a7 89e4 b880 e998 b5e6 af9b e9aa  ................
-000002f0: a8e6 829a e784 b6ef bc8c e683 85e4 b88d  ................
-00000300: e887 aae7 a681 e79a 84e5 908e e980 80e4  ................
-00000310: ba86 e4b8 a4e6 ada5 222c 0a20 2274 6172  ........",. "tar
-00000320: 6765 7422 3a30 2c0a 2022 6d6f 7665 223a  get":0,. "move":
-00000330: 2d32 0a7d 2c0a 7b0a 2022 6576 656e 745f  -2.},.{. "event_
-00000340: 6e61 6d65 223a 22e5 858b e88b 8fe9 b281  name":".........
-00000350: e4ba 8be4 bbb6 3722 2c0a 2022 6465 7363  ......7",. "desc
-00000360: 7269 6265 223a 223c 303e e58f 91e7 8eb0  ribe":"<0>......
-00000370: e7bb 88e7 82b9 e589 8de5 a5bd e583 8fe6  ................
-00000380: 9c89 e4b8 80e4 b8aa e6a8 a1e7 b38a e79a  ................
-00000390: 84e8 baab e5bd b1e7 ab99 e59c a8e9 82a3  ................
-000003a0: efbc 8ce4 bd86 e4bb 96e7 9c8b e4b8 8de6  ................
-000003b0: b885 e982 a3e2 809c e4b8 9ce8 a5bf e280  ................
-000003c0: 9de5 88b0 e5ba 95e6 98af e4bb 80e4 b988  ................
-000003d0: 222c 0a20 2274 6172 6765 7422 3a30 0a7d  ",. "target":0.}
-000003e0: 2c0a 7b0a 2022 6576 656e 745f 6e61 6d65  ,.{. "event_name
-000003f0: 223a 22e5 858b e88b 8fe9 b281 e4ba 8be4  ":".............
-00000400: bbb6 3822 2c0a 2022 6465 7363 7269 6265  ..8",. "describe
-00000410: 223a 223c 303e e684 9fe8 a789 e8bf 99e4  ":"<0>..........
-00000420: b8aa e4b8 96e7 958c e4bc bce4 b98e e58f  ................
-00000430: 91e7 949f e4ba 86e4 bb80 e4b9 88e5 8f98  ................
-00000440: e58c 9622 2c0a 2022 7461 7267 6574 223a  ...",. "target":
-00000450: 300a 7d2c 0a7b 0a22 6576 656e 745f 6e61  0.},.{."event_na
-00000460: 6d65 223a 22e5 858b e88b 8fe9 b281 e4ba  me":"...........
-00000470: 8be4 bbb6 3922 2c0a 2264 6573 6372 6962  ....9",."describ
-00000480: 6522 3a22 3c30 3ee5 8f91 e78e b0e8 87aa  e":"<0>.........
-00000490: e5b7 b1e7 9a84 e5af b9e6 898b e5a5 bde5  ................
-000004a0: 838f e5b9 b6e4 b88d e698 afe2 809c e8b5  ................
-000004b0: 9be9 a9ac e280 9d22 2c0a 2274 6172 6765  .......",."targe
-000004c0: 7422 3a30 0a7d 2c0a 7b0a 2022 6576 656e  t":0.},.{. "even
-000004d0: 745f 6e61 6d65 223a 22e5 858b e88b 8fe9  t_name":".......
-000004e0: b281 e4ba 8be4 bbb6 3130 222c 0a20 2264  ........10",. "d
-000004f0: 6573 6372 6962 6522 3a22 3c30 3ee5 8f91  escribe":"<0>...
-00000500: e78e b0e5 898d e696 b9e7 ab99 e79d 80e4  ................
-00000510: b880 e4b8 aae2 9693 e296 93e2 9693 e296  ................
-00000520: 93e2 9693 e296 93e2 9693 e296 93e2 9693  ................
-00000530: e296 93e2 9693 e296 93e2 80a6 e280 a626  ...............&
-00000540: 2a25 2b2d 2aef bc8c e4bd a0e8 af95 e59b  *%+-*...........
-00000550: bee9 8083 e8b7 91ef bc8c e58f afe6 98af  ................
-00000560: e8bf 98e6 98af e8a2 abe2 809c e4bb 96e5  ................
-00000570: 8f91 e78e b0e4 ba86 e280 9def bc8c e298  ................
-00000580: 85e2 9886 e286 91e2 978e c2a4 e298 85e2  ................
-00000590: 9886 e297 8ee2 8691 c2a4 e298 85e2 9886  ................
-000005a0: e297 8ec2 a4e2 978e e286 91c2 a4e2 9885  ................
-000005b0: e298 86e2 8691 222c 0a20 2274 6172 6765  ......",. "targe
-000005c0: 7422 3a30 2c0a 2022 6177 6179 223a 312c  t":0,. "away":1,
-000005d0: 0a20 2261 7761 795f 6e61 6d65 223a 223f  . "away_name":"?
-000005e0: 3f3f 220a 7d2c 0a7b 0a20 2265 7665 6e74  ??".},.{. "event
-000005f0: 5f6e 616d 6522 3a22 e585 8be8 8b8f e9b2  _name":"........
-00000600: 81e4 ba8b e4bb b631 3122 2c0a 2022 6465  .......11",. "de
-00000610: 7363 7269 6265 223a 223c 303e e6b6 88e5  scribe":"<0>....
-00000620: a4b1 e59c a8e4 ba86 e8b5 9be5 9cba e4b8  ................
-00000630: 8aef bc8c e6b2 a1e6 9c89 e4ba bae7 9fa5  ................
-00000640: e981 93e8 bf99 e59c bae6 af94 e8b5 9be4  ................
-00000650: b8ad e58f 91e7 949f e4ba 86e4 bb80 e4b9  ................
-00000660: 88e3 8082 222c 0a20 2274 6172 6765 7422  ....",. "target"
-00000670: 3a30 2c0a 2022 6469 6522 3a31 2c0a 2022  :0,. "die":1,. "
-00000680: 6469 655f 6e61 6d65 223a 22c2 a4e2 9885  die_name":".....
-00000690: e298 86e2 8691 220a 7d0a 5d0a            ......".}.].
+00000000: 5b0d 0a7b 0d0a 2022 6576 656e 745f 6e61  [..{.. "event_na
+00000010: 6d65 223a 22e5 858b e88b 8fe9 b281 e4ba  me":"...........
+00000020: 8be4 bbb6 3122 2c0d 0a20 2264 6573 6372  ....1",.. "descr
+00000030: 6962 6522 3a22 3c30 3ee7 aa81 e784 b6e6  ibe":"<0>.......
+00000040: 849f e8a7 89e8 a782 e4bc 97e5 b8ad e4b8  ................
+00000050: ade6 9c89 e4b8 80e5 8f8c e79c bce7 9d9b  ................
+00000060: e59c a8e7 9baf e79d 80e4 bb96 222c 0d0a  ............",..
+00000070: 2022 7461 7267 6574 223a 300d 0a7d 2c0d   "target":0..},.
+00000080: 0a7b 0d0a 2022 6576 656e 745f 6e61 6d65  .{.. "event_name
+00000090: 223a 22e5 858b e88b 8fe9 b281 e4ba 8be4  ":".............
+000000a0: bbb6 3222 2c0d 0a20 2264 6573 6372 6962  ..2",.. "describ
+000000b0: 6522 3a22 3c30 3ee6 849f e8a7 89e8 baab  e":"<0>.........
+000000c0: e8be b9e8 b28c e4bc bce9 99a4 e4ba 86e8  ................
+000000d0: b59b e9a9 ace4 bba5 e5a4 96e8 bf98 e69c  ................
+000000e0: 89e4 b880 e4ba 9be5 85b6 e5ae 83e4 b89c  ................
+000000f0: e8a5 bf22 2c0d 0a20 2274 6172 6765 7422  ...",.. "target"
+00000100: 3a30 0d0a 7d2c 0d0a 7b0d 0a20 2265 7665  :0..},..{.. "eve
+00000110: 6e74 5f6e 616d 6522 3a22 e585 8be8 8b8f  nt_name":"......
+00000120: e9b2 81e4 ba8b e4bb b633 222c 0d0a 2022  .........3",.. "
+00000130: 6465 7363 7269 6265 223a 223c 303e e4b8  describe":"<0>..
+00000140: 8de7 9bb8 e4bf a1e4 b896 e795 8ce4 b88a  ................
+00000150: e69c 89e4 bb80 e4b9 88e5 a587 e680 aae7  ................
+00000160: 9a84 e4b8 9ce8 a5bf 222c 0d0a 2022 7461  ........",.. "ta
+00000170: 7267 6574 223a 300d 0a7d 2c0d 0a7b 0d0a  rget":0..},..{..
+00000180: 2022 6576 656e 745f 6e61 6d65 223a 22e5   "event_name":".
+00000190: 858b e88b 8fe9 b281 e4ba 8be4 bbb6 3422  ..............4"
+000001a0: 2c0d 0a20 2264 6573 6372 6962 6522 3a22  ,.. "describe":"
+000001b0: 3c30 3ee6 849f e8a7 89e4 bb8a e5a4 a9e5  <0>.............
+000001c0: a4aa e998 b3e5 8589 e79a 84e9 a29c e889  ................
+000001d0: b2e6 9c89 e4ba 9be4 b88d e5af b9ef bc8c  ................
+000001e0: e4bc bce4 b98e e6af 94e5 b9b3 e5b8 b8e6  ................
+000001f0: 9a97 e4ba 86e8 aeb8 e5a4 9a22 2c0d 0a20  ...........",.. 
+00000200: 2274 6172 6765 7422 3a30 0d0a 7d2c 0d0a  "target":0..},..
+00000210: 7b0d 0a20 2265 7665 6e74 5f6e 616d 6522  {.. "event_name"
+00000220: 3a22 e585 8be8 8b8f e9b2 81e4 ba8b e4bb  :"..............
+00000230: b635 222c 0d0a 2022 6465 7363 7269 6265  .5",.. "describe
+00000240: 223a 223c 303e e684 9fe8 a789 e69c 89e4  ":"<0>..........
+00000250: bb80 e4b9 88e2 809c e4b8 9ce8 a5bf e280  ................
+00000260: 9de5 9ca8 e68e 90e7 9d80 e887 aae5 b7b1  ................
+00000270: e79a 84e5 9689 e592 9922 2c0d 0a20 2274  .........",.. "t
+00000280: 6172 6765 7422 3a30 2c0d 0a20 2272 6f75  arget":0,.. "rou
+00000290: 6e64 7322 3a31 2c0d 0a20 226e 616d 6522  nds":1,.. "name"
+000002a0: 3a22 e7bc bae6 b0a7 222c 0d0a 2022 6c6f  :"......",.. "lo
+000002b0: 6361 7465 5f6c 6f63 6b22 3a31 0d0a 7d2c  cate_lock":1..},
+000002c0: 0d0a 7b0d 0a20 2265 7665 6e74 5f6e 616d  ..{.. "event_nam
+000002d0: 6522 3a22 e585 8be8 8b8f e9b2 81e4 ba8b  e":"............
+000002e0: e4bb b636 222c 0d0a 2022 6465 7363 7269  ...6",.. "descri
+000002f0: 6265 223a 223c 303e e7aa 81e7 84b6 e684  be":"<0>........
+00000300: 9fe8 a789 e4b8 80e9 98b5 e6af 9be9 aaa8  ................
+00000310: e682 9ae7 84b6 efbc 8ce6 8385 e4b8 8de8  ................
+00000320: 87aa e7a6 81e7 9a84 e590 8ee9 8080 e4ba  ................
+00000330: 86e4 b8a4 e6ad a522 2c0d 0a20 2274 6172  .......",.. "tar
+00000340: 6765 7422 3a30 2c0d 0a20 226d 6f76 6522  get":0,.. "move"
+00000350: 3a2d 320d 0a7d 2c0d 0a7b 0d0a 2022 6576  :-2..},..{.. "ev
+00000360: 656e 745f 6e61 6d65 223a 22e5 858b e88b  ent_name":".....
+00000370: 8fe9 b281 e4ba 8be4 bbb6 3722 2c0d 0a20  ..........7",.. 
+00000380: 2264 6573 6372 6962 6522 3a22 3c30 3ee5  "describe":"<0>.
+00000390: 8f91 e78e b0e7 bb88 e782 b9e5 898d e5a5  ................
+000003a0: bde5 838f e69c 89e4 b880 e4b8 aae6 a8a1  ................
+000003b0: e7b3 8ae7 9a84 e8ba abe5 bdb1 e7ab 99e5  ................
+000003c0: 9ca8 e982 a3ef bc8c e4bd 86e4 bb96 e79c  ................
+000003d0: 8be4 b88d e6b8 85e9 82a3 e280 9ce4 b89c  ................
+000003e0: e8a5 bfe2 809d e588 b0e5 ba95 e698 afe4  ................
+000003f0: bb80 e4b9 8822 2c0d 0a20 2274 6172 6765  .....",.. "targe
+00000400: 7422 3a30 0d0a 7d2c 0d0a 7b0d 0a20 2265  t":0..},..{.. "e
+00000410: 7665 6e74 5f6e 616d 6522 3a22 e585 8be8  vent_name":"....
+00000420: 8b8f e9b2 81e4 ba8b e4bb b638 222c 0d0a  ...........8",..
+00000430: 2022 6465 7363 7269 6265 223a 223c 303e   "describe":"<0>
+00000440: e684 9fe8 a789 e8bf 99e4 b8aa e4b8 96e7  ................
+00000450: 958c e4bc bce4 b98e e58f 91e7 949f e4ba  ................
+00000460: 86e4 bb80 e4b9 88e5 8f98 e58c 9622 2c0d  .............",.
+00000470: 0a20 2274 6172 6765 7422 3a30 0d0a 7d2c  . "target":0..},
+00000480: 0d0a 7b0d 0a22 6576 656e 745f 6e61 6d65  ..{.."event_name
+00000490: 223a 22e5 858b e88b 8fe9 b281 e4ba 8be4  ":".............
+000004a0: bbb6 3922 2c0d 0a22 6465 7363 7269 6265  ..9",.."describe
+000004b0: 223a 223c 303e e58f 91e7 8eb0 e887 aae5  ":"<0>..........
+000004c0: b7b1 e79a 84e5 afb9 e689 8be5 a5bd e583  ................
+000004d0: 8fe5 b9b6 e4b8 8de6 98af e280 9ce8 b59b  ................
+000004e0: e9a9 ace2 809d 222c 0d0a 2274 6172 6765  ......",.."targe
+000004f0: 7422 3a30 0d0a 7d2c 0d0a 7b0d 0a20 2265  t":0..},..{.. "e
+00000500: 7665 6e74 5f6e 616d 6522 3a22 e585 8be8  vent_name":"....
+00000510: 8b8f e9b2 81e4 ba8b e4bb b631 3022 2c0d  ...........10",.
+00000520: 0a20 2264 6573 6372 6962 6522 3a22 3c30  . "describe":"<0
+00000530: 3ee5 8f91 e78e b0e5 898d e696 b9e7 ab99  >...............
+00000540: e79d 80e4 b880 e4b8 aae2 9693 e296 93e2  ................
+00000550: 9693 e296 93e2 9693 e296 93e2 9693 e296  ................
+00000560: 93e2 9693 e296 93e2 9693 e296 93e2 80a6  ................
+00000570: e280 a626 2a25 2b2d 2aef bc8c e4bd a0e8  ...&*%+-*.......
+00000580: af95 e59b bee9 8083 e8b7 91ef bc8c e58f  ................
+00000590: afe6 98af e8bf 98e6 98af e8a2 abe2 809c  ................
+000005a0: e4bb 96e5 8f91 e78e b0e4 ba86 e280 9def  ................
+000005b0: bc8c e298 85e2 9886 e286 91e2 978e c2a4  ................
+000005c0: e298 85e2 9886 e297 8ee2 8691 c2a4 e298  ................
+000005d0: 85e2 9886 e297 8ec2 a4e2 978e e286 91c2  ................
+000005e0: a4e2 9885 e298 86e2 8691 222c 0d0a 2022  ..........",.. "
+000005f0: 7461 7267 6574 223a 302c 0d0a 2022 6177  target":0,.. "aw
+00000600: 6179 223a 312c 0d0a 2022 6177 6179 5f6e  ay":1,.. "away_n
+00000610: 616d 6522 3a22 3f3f 3f22 0d0a 7d2c 0d0a  ame":"???"..},..
+00000620: 7b0d 0a20 2265 7665 6e74 5f6e 616d 6522  {.. "event_name"
+00000630: 3a22 e585 8be8 8b8f e9b2 81e4 ba8b e4bb  :"..............
+00000640: b631 3122 2c0d 0a20 2264 6573 6372 6962  .11",.. "describ
+00000650: 6522 3a22 3c30 3ee6 b688 e5a4 b1e5 9ca8  e":"<0>.........
+00000660: e4ba 86e8 b59b e59c bae4 b88a efbc 8ce6  ................
+00000670: b2a1 e69c 89e4 baba e79f a5e9 8193 e8bf  ................
+00000680: 99e5 9cba e6af 94e8 b59b e4b8 ade5 8f91  ................
+00000690: e794 9fe4 ba86 e4bb 80e4 b988 e380 8222  ..............."
+000006a0: 2c0d 0a20 2274 6172 6765 7422 3a30 2c0d  ,.. "target":0,.
+000006b0: 0a20 2264 6965 223a 312c 0d0a 2022 6469  . "die":1,.. "di
+000006c0: 655f 6e61 6d65 223a 22c2 a4e2 9885 e298  e_name":".......
+000006d0: 86e2 8691 220d 0a7d 0d0a 5d0d 0a         ...."..}..]..
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 24% similar despite different names*

```diff
@@ -1,286 +1,297 @@
-00000000: 5b0a 2020 7b0a 2020 2020 2265 7665 6e74  [.  {.    "event
-00000010: 5f6e 616d 6522 3a22 e8b6 85e7 a8b3 e5ae  _name":"........
-00000020: 9ae8 8a9c e6b9 965f e589 8de8 bf9b 3422  ......._......4"
-00000030: 2c0a 2020 2020 2274 6172 6765 7422 3a30  ,.    "target":0
-00000040: 2c0a 2020 2020 2264 6573 6372 6962 6522  ,.    "describe"
-00000050: 3a22 3c30 3ee5 be97 e588 b0e4 ba86 e8b6  :"<0>...........
-00000060: 85e7 a8b3 e5ae 9ae8 8a9c e6b9 96ef bc8c  ................
-00000070: e5bf abe9 809f e9a2 9de5 a496 e589 8de8  ................
-00000080: bf9b e4ba 8633 e6a0 bc22 2c0a 2020 2020  .....3...",.    
-00000090: 226d 6f76 6522 3a34 0a20 207d 2c0a 2020  "move":4.  },.  
-000000a0: 7b0a 2020 2020 2265 7665 6e74 5f6e 616d  {.    "event_nam
-000000b0: 6522 3a22 e4b8 8de7 a8b3 e5ae 9ae8 8a9c  e":"............
-000000c0: e6b9 965f e589 8de8 bf9b 2d34 7e34 222c  ..._......-4~4",
-000000d0: 0a20 2020 2022 7461 7267 6574 223a 302c  .    "target":0,
-000000e0: 0a20 2020 2022 6465 7363 7269 6265 223a  .    "describe":
-000000f0: 223c 303e e5be 97e5 88b0 e4ba 86e4 b88d  "<0>............
-00000100: e7a8 b3e5 ae9a e88a 9ce6 b996 e58a 9be9  ................
-00000110: 878f 2c22 2c0a 2020 2020 2272 616e 646f  ..,",.    "rando
-00000120: 6d5f 6576 656e 745f 6f6e 6365 223a 5b5b  m_event_once":[[
-00000130: 3130 2c20 7b0a 2020 2020 2020 2020 2020  10, {.          
-00000140: 2265 7665 6e74 5f6e 616d 6522 3a22 e4b8  "event_name":"..
-00000150: 8de7 a8b3 e5ae 9ae8 8a9c e6b9 965f e589  ............._..
-00000160: 8de8 bf9b 2d34 222c 0a20 2020 2020 2020  ....-4",.       
-00000170: 2020 2022 7461 7267 6574 223a 302c 0a20     "target":0,. 
-00000180: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00000190: 6265 223a 22e5 908e e980 80e4 ba86 34e6  be":".........4.
-000001a0: a0bc 222c 0a20 2020 2020 2020 2020 2022  ..",.          "
-000001b0: 6d6f 7665 223a 2d34 0a20 2020 2020 2020  move":-4.       
-000001c0: 207d 0a20 2020 2020 205d 2c0a 2020 2020   }.      ],.    
-000001d0: 2020 2020 2020 5b32 302c 207b 0a20 2020        [20, {.   
-000001e0: 2020 2020 2020 2022 6576 656e 745f 6e61         "event_na
-000001f0: 6d65 223a 22e4 b88d e7a8 b3e5 ae9a e88a  me":"...........
-00000200: 9ce6 b996 5fe5 898d e8bf 9b2d 3322 2c0a  ...._......-3",.
-00000210: 2020 2020 2020 2020 2020 2274 6172 6765            "targe
-00000220: 7422 3a30 2c0a 2020 2020 2020 2020 2020  t":0,.          
-00000230: 2264 6573 6372 6962 6522 3a22 e590 8ee9  "describe":"....
-00000240: 8080 e4ba 8633 e6a0 bc22 2c0a 2020 2020  .....3...",.    
-00000250: 2020 2020 2020 226d 6f76 6522 3a2d 330a        "move":-3.
-00000260: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000270: 5d2c 0a20 2020 2020 2020 2020 205b 3330  ],.          [30
-00000280: 2c20 7b0a 2020 2020 2020 2020 2020 2265  , {.          "e
-00000290: 7665 6e74 5f6e 616d 6522 3a22 e4b8 8de7  vent_name":"....
-000002a0: a8b3 e5ae 9ae8 8a9c e6b9 965f e589 8de8  ..........._....
-000002b0: bf9b 2d32 222c 0a20 2020 2020 2020 2020  ..-2",.         
-000002c0: 2022 7461 7267 6574 223a 302c 0a20 2020   "target":0,.   
-000002d0: 2020 2020 2020 2022 6465 7363 7269 6265         "describe
-000002e0: 223a 22e5 908e e980 80e4 ba86 32e6 a0bc  ":".........2...
-000002f0: 222c 0a20 2020 2020 2020 2020 2022 6d6f  ",.          "mo
-00000300: 7665 223a 2d32 0a20 2020 2020 2020 207d  ve":-2.        }
-00000310: 0a20 2020 2020 205d 2c0a 2020 2020 2020  .      ],.      
-00000320: 2020 2020 5b34 302c 207b 0a20 2020 2020      [40, {.     
-00000330: 2020 2020 2022 6576 656e 745f 6e61 6d65       "event_name
-00000340: 223a 22e4 b88d e7a8 b3e5 ae9a e88a 9ce6  ":".............
-00000350: b996 5fe5 898d e8bf 9b2d 3122 2c0a 2020  .._......-1",.  
-00000360: 2020 2020 2020 2020 2274 6172 6765 7422          "target"
-00000370: 3a30 2c0a 2020 2020 2020 2020 2020 2264  :0,.          "d
-00000380: 6573 6372 6962 6522 3a22 e590 8ee9 8080  escribe":"......
-00000390: e4ba 8631 e6a0 bc22 2c0a 2020 2020 2020  ...1...",.      
-000003a0: 2020 2020 226d 6f76 6522 3a2d 310a 2020      "move":-1.  
-000003b0: 2020 2020 2020 7d0a 2020 2020 2020 5d2c        }.      ],
-000003c0: 0a20 2020 2020 2020 2020 205b 3530 2c20  .          [50, 
-000003d0: 7b0a 2020 2020 2020 2020 2020 2265 7665  {.          "eve
-000003e0: 6e74 5f6e 616d 6522 3a22 e4b8 8de7 a8b3  nt_name":"......
-000003f0: e5ae 9ae8 8a9c e6b9 965f e589 8de8 bf9b  ........._......
-00000400: 3122 2c0a 2020 2020 2020 2020 2020 2274  1",.          "t
-00000410: 6172 6765 7422 3a30 2c0a 2020 2020 2020  arget":0,.      
-00000420: 2020 2020 2264 6573 6372 6962 6522 3a22      "describe":"
-00000430: e589 8de8 bf9b e4ba 8631 e6a0 bc22 2c0a  .........1...",.
-00000440: 2020 2020 2020 2020 2020 226d 6f76 6522            "move"
-00000450: 3a31 0a20 2020 2020 2020 207d 0a20 2020  :1.        }.   
-00000460: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
-00000470: 5b36 302c 207b 0a20 2020 2020 2020 2020  [60, {.         
-00000480: 2022 6576 656e 745f 6e61 6d65 223a 22e4   "event_name":".
-00000490: b88d e7a8 b3e5 ae9a e88a 9ce6 b996 5fe5  .............._.
-000004a0: 898d e8bf 9b32 222c 0a20 2020 2020 2020  .....2",.       
-000004b0: 2020 2022 7461 7267 6574 223a 302c 0a20     "target":0,. 
-000004c0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-000004d0: 6265 223a 22e5 898d e8bf 9be4 ba86 32e6  be":".........2.
-000004e0: a0bc 222c 0a20 2020 2020 2020 2020 2022  ..",.          "
-000004f0: 6d6f 7665 223a 320a 2020 2020 2020 2020  move":2.        
-00000500: 7d0a 2020 2020 2020 5d2c 0a20 2020 2020  }.      ],.     
-00000510: 2020 2020 205b 3730 2c20 7b0a 2020 2020       [70, {.    
-00000520: 2020 2020 2020 2265 7665 6e74 5f6e 616d        "event_nam
-00000530: 6522 3a22 e4b8 8de7 a8b3 e5ae 9ae8 8a9c  e":"............
-00000540: e6b9 965f e589 8de8 bf9b 3322 2c0a 2020  ..._......3",.  
-00000550: 2020 2020 2020 2020 2274 6172 6765 7422          "target"
-00000560: 3a30 2c0a 2020 2020 2020 2020 2020 2264  :0,.          "d
-00000570: 6573 6372 6962 6522 3a22 e589 8de8 bf9b  escribe":"......
-00000580: e4ba 8633 e6a0 bc22 2c0a 2020 2020 2020  ...3...",.      
-00000590: 2020 2020 226d 6f76 6522 3a33 0a20 2020      "move":3.   
-000005a0: 2020 2020 207d 0a20 2020 2020 205d 2c0a       }.      ],.
-000005b0: 2020 2020 2020 2020 2020 5b38 302c 207b            [80, {
-000005c0: 0a20 2020 2020 2020 2020 2022 6576 656e  .          "even
-000005d0: 745f 6e61 6d65 223a 22e4 b88d e7a8 b3e5  t_name":".......
-000005e0: ae9a e88a 9ce6 b996 5fe5 898d e8bf 9b34  ........_......4
-000005f0: 222c 0a20 2020 2020 2020 2020 2022 7461  ",.          "ta
-00000600: 7267 6574 223a 302c 0a20 2020 2020 2020  rget":0,.       
-00000610: 2020 2022 6465 7363 7269 6265 223a 22e5     "describe":".
-00000620: 898d e8bf 9be4 ba86 34e6 a0bc 222c 0a20  ........4...",. 
-00000630: 2020 2020 2020 2020 2022 6d6f 7665 223a           "move":
-00000640: 340a 2020 2020 2020 2020 7d0a 2020 2020  4.        }.    
-00000650: 2020 5d0a 2020 2020 5d0a 2020 7d2c 0a20    ].    ].  },. 
-00000660: 207b 0a20 2020 2022 6576 656e 745f 6e61   {.    "event_na
-00000670: 6d65 223a 22e9 bb91 e69a 97e8 8a9c e6b9  me":"...........
-00000680: 96e5 8a9b e987 8f22 2c0a 2020 2020 2274  .......",.    "t
-00000690: 6172 6765 7422 3a31 2c0a 2020 2020 2264  arget":1,.    "d
-000006a0: 6573 6372 6962 6522 3a22 3c30 3ee5 be97  escribe":"<0>...
-000006b0: e588 b0e4 ba86 e8b6 85e7 a8b3 e5ae 9ae8  ................
-000006c0: 8a9c e6b9 96e5 8a9b e987 8fef bc8c e69d  ................
-000006d0: 80e6 adbb e4ba 863c 313e 222c 0a20 2020  .......<1>",.   
-000006e0: 2022 6469 6522 3a31 2c0a 2020 2020 2264   "die":1,.    "d
-000006f0: 6965 5f6e 616d 6522 3a22 e88a 9ce6 b996  ie_name":"......
-00000700: e4be b5e8 9a80 220a 2020 7d2c 0a20 207b  ......".  },.  {
-00000710: 0a20 2020 2022 6576 656e 745f 6e61 6d65  .    "event_name
-00000720: 223a 22e9 9499 e8af afe7 9a84 e88a 9ce6  ":".............
-00000730: b996 e58a 9be9 878f 222c 0a20 2020 2022  ........",.    "
-00000740: 7461 7267 6574 223a 302c 0a20 2020 2022  target":0,.    "
-00000750: 6465 7363 7269 6265 223a 223c 303e e5be  describe":"<0>..
-00000760: 97e5 88b0 e4ba 86e9 9499 e8af afe7 9a84  ................
-00000770: e88a 9ce6 b996 e58a 9be9 878f efbc 8ce6  ................
-00000780: 9d80 e6ad bbe4 ba86 e887 aae5 b7b1 222c  ..............",
-00000790: 0a20 2020 2022 6469 6522 3a31 2c0a 2020  .    "die":1,.  
-000007a0: 2020 2264 6965 5f6e 616d 6522 3a22 e88a    "die_name":"..
-000007b0: 9ce6 b996 e4be b5e8 9a80 220a 2020 7d2c  ..........".  },
-000007c0: 0a20 207b 0a20 2020 2022 6576 656e 745f  .  {.    "event_
-000007d0: 6e61 6d65 223a 22e8 87b3 e5b0 8ae8 8a9c  name":".........
-000007e0: e6b9 96e5 8a9b e987 8f22 2c0a 2020 2020  .........",.    
-000007f0: 2274 6172 6765 7422 3a30 2c0a 2020 2020  "target":0,.    
-00000800: 2264 6573 6372 6962 6522 3a22 3c30 3ee5  "describe":"<0>.
-00000810: be97 e588 b0e4 ba86 e987 91e5 8589 e997  ................
-00000820: aae9 97aa e887 b3e5 b08a e88a 9ce6 b996  ................
-00000830: e58a 9be9 878f efbc 8c22 2c0a 2020 2020  .........",.    
-00000840: 2272 616e 646f 6d5f 6576 656e 745f 6f6e  "random_event_on
-00000850: 6365 223a 5b5b 3230 2c20 7b0a 2020 2020  ce":[[20, {.    
-00000860: 2020 2020 2265 7665 6e74 5f6e 616d 6522      "event_name"
-00000870: 3a22 e887 b3e5 b08a e88a 9ce6 b996 e58a  :"..............
-00000880: 9be9 878f 2de7 bb88 e782 b922 2c0a 2020  ....-......",.  
-00000890: 2020 2020 2020 2274 6172 6765 7422 3a32        "target":2
-000008a0: 2c0a 2020 2020 2020 2020 2264 6573 6372  ,.        "descr
-000008b0: 6962 6522 3a22 e8ae a9e6 8980 e69c 89e9  ibe":"..........
-000008c0: 8089 e689 8be9 83bd e588 b0e8 bebe e4ba  ................
-000008d0: 86e7 bb88 e782 b922 2c0a 2020 2020 2020  .......",.      
-000008e0: 2020 2274 7261 636b 5f72 616e 646f 6d5f    "track_random_
-000008f0: 6c6f 6361 7469 6f6e 223a 3130 300a 2020  location":100.  
-00000900: 2020 2020 2020 7d0a 2020 2020 2020 5d2c        }.      ],
-00000910: 0a20 2020 2020 205b 3130 302c 207b 0a20  .      [100, {. 
-00000920: 2020 2020 2020 2022 6576 656e 745f 6e61         "event_na
-00000930: 6d65 223a 22e8 87b3 e5b0 8ae8 8a9c e6b9  me":"...........
-00000940: 96e5 8a9b e987 8f2d e697 a0e4 ba8b e58f  .......-........
-00000950: 91e7 949f 222c 0a20 2020 2020 2020 2022  ....",.        "
-00000960: 7461 7267 6574 223a 302c 0a20 2020 2020  target":0,.     
-00000970: 2020 2022 6465 7363 7269 6265 223a 22e4     "describe":".
-00000980: bd86 e5a5 bde5 838f e6b2 a1e6 9c89 e595  ................
-00000990: a5e7 94a8 220a 2020 2020 2020 2020 7d0a  ....".        }.
-000009a0: 2020 2020 2020 5d0a 2020 2020 5d0a 2020        ].    ].  
-000009b0: 7d2c 0a20 207b 0a20 2020 2022 6576 656e  },.  {.    "even
-000009c0: 745f 6e61 6d65 223a 22e8 bdbb e987 8fe8  t_name":".......
-000009d0: 8a9c e6b9 96e5 8a9b e987 8f22 2c0a 2020  ...........",.  
-000009e0: 2020 2274 6172 6765 7422 3a30 2c0a 2020    "target":0,.  
-000009f0: 2020 2264 6573 6372 6962 6522 3a22 3c30    "describe":"<0
-00000a00: 3ee5 be97 e588 b0e4 ba86 e8bd bbe9 878f  >...............
-00000a10: e88a 9ce6 b996 e58a 9be9 878f efbc 8ce8  ................
-00000a20: aea9 e887 aae5 b7b1 e9a2 9de5 a496 e589  ................
-00000a30: 8de8 bf9b 31e6 a0bc 222c 0a20 2020 2022  ....1...",.    "
-00000a40: 6d6f 7665 223a 310a 2020 7d2c 0a20 207b  move":1.  },.  {
-00000a50: 0a20 2020 2022 6576 656e 745f 6e61 6d65  .    "event_name
-00000a60: 223a 22e8 8a9c e6b9 96e6 b395 e69d 96c2  ":".............
-00000a70: b7e5 a48d e88b 8f22 2c0a 2020 2020 2274  .......",.    "t
-00000a80: 6172 6765 7422 3a32 2c0a 2020 2020 2264  arget":2,.    "d
-00000a90: 6573 6372 6962 6522 3a22 3c30 3ee5 be97  escribe":"<0>...
-00000aa0: e588 b0e4 ba86 3ce8 8a9c e6b9 96e6 b395  ......<.........
-00000ab0: e69d 96c2 b7e5 a48d e88b 8f3e efbc 8ce5  ...........>....
-00000ac0: a48d e88b 8fe4 ba86 e689 80e6 9c89 e79a  ................
-00000ad0: 84e9 8089 e689 8b21 222c 0a20 2020 2022  .......!",.    "
-00000ae0: 6c69 7665 223a 310a 2020 7d2c 0a20 207b  live":1.  },.  {
-00000af0: 0a20 2020 2022 6576 656e 745f 6e61 6d65  .    "event_name
-00000b00: 223a 22e8 8a9c e6b9 96e6 b395 e69d 96c2  ":".............
-00000b10: b7e5 a4a9 e590 af31 222c 0a20 2020 2022  .......1",.    "
-00000b20: 7461 7267 6574 223a 302c 0a20 2020 2022  target":0,.    "
-00000b30: 6465 7363 7269 6265 223a 223c 303e e5be  describe":"<0>..
-00000b40: 97e5 88b0 e4ba 863c e88a 9ce6 b996 e6b3  .......<........
-00000b50: 95e6 9d96 c2b7 e5a4 a9e5 90af 3eef bc8c  ............>...
-00000b60: e693 8de4 bd9c e5a4 b1e8 afaf efbc 8ce6  ................
-00000b70: af81 e781 ade4 ba86 e887 aae5 b7b1 222c  ..............",
-00000b80: 0a20 2020 2022 6469 6522 3a31 0a20 207d  .    "die":1.  }
-00000b90: 2c0a 2020 7b0a 2020 2020 2265 7665 6e74  ,.  {.    "event
-00000ba0: 5f6e 616d 6522 3a22 e88a 9ce6 b996 e6b3  _name":"........
-00000bb0: 95e6 9d96 c2b7 e5a4 a9e5 90af 3222 2c0a  ............2",.
-00000bc0: 2020 2020 2274 6172 6765 7422 3a33 2c0a      "target":3,.
-00000bd0: 2020 2020 2264 6573 6372 6962 6522 3a22      "describe":"
-00000be0: 3c30 3ee5 be97 e588 b0e4 ba86 3ce8 8a9c  <0>.........<...
-00000bf0: e6b9 96e6 b395 e69d 96c2 b7e5 a4a9 e590  ................
-00000c00: af3e efbc 8ce5 b09d e8af 95e6 af81 e781  .>..............
-00000c10: ade6 8980 e69c 89e7 9a84 e980 89e6 898b  ................
-00000c20: efbc 8ce4 bd86 e587 86e6 989f e5ae 9ee5  ................
-00000c30: 9ca8 e5a4 aae5 b7ae e4ba 8622 2c0a 2020  ...........",.  
-00000c40: 2020 2272 616e 646f 6d5f 6576 656e 745f    "random_event_
-00000c50: 6f6e 6365 223a 5b5b 3330 2c20 7b0a 2020  once":[[30, {.  
-00000c60: 2020 2020 2020 2265 7665 6e74 5f6e 616d        "event_nam
-00000c70: 6522 3a22 e88a 9ce6 b996 e6b3 95e6 9d96  e":"............
-00000c80: c2b7 e5a4 a9e5 90af 322d e591 bde4 b8ad  ........2-......
-00000c90: 222c 0a20 2020 2020 2020 2022 6465 7363  ",.        "desc
-00000ca0: 7269 6265 223a 22ef bc8c 3c30 3ee8 a2ab  ribe":"...<0>...
-00000cb0: e689 93e4 b8ad e4ba 8622 2c0a 2020 2020  .........",.    
-00000cc0: 2020 2020 2274 6172 6765 7422 3a30 2c0a      "target":0,.
-00000cd0: 2020 2020 2020 2020 2264 6965 223a 310a          "die":1.
-00000ce0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000cf0: 5d2c 0a20 2020 2020 205b 3130 302c 207b  ],.      [100, {
-00000d00: 0a20 2020 2020 2020 2020 2022 6576 656e  .          "even
-00000d10: 745f 6e61 6d65 223a 22e8 8a9c e6b9 96e6  t_name":".......
-00000d20: b395 e69d 96c2 b7e5 a4a9 e590 af32 2de6  .............2-.
-00000d30: 9caa e591 bde4 b8ad 222c 0a20 2020 2020  ........",.     
-00000d40: 2020 2020 2022 6465 7363 7269 6265 223a       "describe":
-00000d50: 2222 2c0a 2020 2020 2020 2020 2020 2274  "",.          "t
-00000d60: 6172 6765 7422 3a30 0a20 2020 2020 2020  arget":0.       
-00000d70: 207d 0a20 2020 2020 205d 0a20 2020 205d   }.      ].    ]
-00000d80: 0a20 207d 2c0a 2020 7b0a 2020 2020 2265  .  },.  {.    "e
-00000d90: 7665 6e74 5f6e 616d 6522 3a22 e88a 9ce6  vent_name":"....
-00000da0: b996 e6b3 95e6 9d96 c2b7 e5a4 a9e5 90af  ................
-00000db0: 3322 2c0a 2020 2020 2274 6172 6765 7422  3",.    "target"
-00000dc0: 3a30 2c0a 2020 2020 2264 6573 6372 6962  :0,.    "describ
-00000dd0: 6522 3a22 3c30 3ee5 be97 e588 b0e4 ba86  e":"<0>.........
-00000de0: 3ce8 8a9c e6b9 96e6 b395 e69d 96c2 b7e5  <...............
-00000df0: a4a9 e590 af3e efbc 8ce8 b5b7 e4ba 86e6  .....>..........
-00000e00: 9d80 e5bf 83ef bc8c e4bd 86e6 98af e5b9  ................
-00000e10: b6e4 b88d e4bc 9ae6 938d e4bd 9c22 0a20  .............". 
-00000e20: 207d 2c0a 2020 7b0a 2020 2020 2265 7665   },.  {.    "eve
-00000e30: 6e74 5f6e 616d 6522 3a22 e88a 9ce6 b996  nt_name":"......
-00000e40: e6b3 95e6 9d96 c2b7 e69c aae6 9da5 222c  ..............",
-00000e50: 0a20 2020 2022 7461 7267 6574 223a 322c  .    "target":2,
-00000e60: 0a20 2020 2022 6465 7363 7269 6265 223a  .    "describe":
-00000e70: 223c 303e e5be 97e5 88b0 e4ba 863c e88a  "<0>.........<..
-00000e80: 9ce6 b996 e6b3 95e6 9d96 c2b7 e69c aae6  ................
-00000e90: 9da5 3eef bc8c e581 9ce6 ada2 e4ba 86e6  ..>.............
-00000ea0: 8980 e69c 89e9 8089 e689 8be7 9a84 e697  ................
-00000eb0: b6e9 97b4 2122 2c0a 2020 2020 2272 6f75  ....!",.    "rou
-00000ec0: 6e64 7322 3a31 2c0a 2020 2020 226e 616d  nds":1,.    "nam
-00000ed0: 6522 3a22 e697 b6e5 819c 222c 0a20 2020  e":"......",.   
-00000ee0: 2022 6c6f 6361 7465 5f6c 6f63 6b22 3a31   "locate_lock":1
-00000ef0: 0a20 207d 2c0a 2020 2020 7b0a 2020 2020  .  },.    {.    
-00000f00: 2265 7665 6e74 5f6e 616d 6522 3a22 e99a  "event_name":"..
-00000f10: 90e7 a798 e88a 9ce6 b996 e58a 9be9 878f  ................
-00000f20: 222c 0a20 2020 2022 7461 7267 6574 223a  ",.    "target":
-00000f30: 302c 0a20 2020 2022 6465 7363 7269 6265  0,.    "describe
-00000f40: 223a 223c 303e e5be 97e5 88b0 e4ba 86e9  ":"<0>..........
-00000f50: 9a90 e7a7 98e8 8a9c e6b9 96e5 8a9b e987  ................
-00000f60: 8fef bc8c 222c 0a20 2020 2022 7261 6e64  ....",.    "rand
-00000f70: 6f6d 5f65 7665 6e74 5f6f 6e63 6522 3a5b  om_event_once":[
-00000f80: 5b37 302c 207b 0a20 2020 2020 2020 2022  [70, {.        "
-00000f90: 6576 656e 745f 6e61 6d65 223a 22e9 9a90  event_name":"...
-00000fa0: e7a7 98e8 8a9c e6b9 96e5 8a9b e987 8f2d  ...............-
-00000fb0: e99a 90e8 baab 222c 0a20 2020 2020 2020  ......",.       
-00000fc0: 2022 6465 7363 7269 6265 223a 22e8 8eb7   "describe":"...
-00000fd0: e5be 97e4 ba86 e4ba 8ce5 9b9e e590 88e7  ................
-00000fe0: 9a84 3ce9 9a90 e8ba ab3e e78a b6e6 8081  ..<......>......
-00000ff0: 222c 0a20 2020 2020 2020 2022 7461 7267  ",.        "targ
-00001000: 6574 223a 302c 0a20 2020 2020 2020 2022  et":0,.        "
-00001010: 6e61 6d65 223a 22e9 9a90 e8ba ab22 2c0a  name":"......",.
-00001020: 2020 2020 2020 2020 2272 6f75 6e64 223a          "round":
-00001030: 322c 0a20 2020 2020 2020 2022 6869 6469  2,.        "hidi
-00001040: 6e67 223a 310a 2020 2020 2020 2020 7d0a  ng":1.        }.
-00001050: 2020 2020 2020 5d2c 0a20 2020 2020 205b        ],.      [
-00001060: 3130 302c 207b 0a20 2020 2020 2020 2020  100, {.         
-00001070: 2022 6576 656e 745f 6e61 6d65 223a 22e9   "event_name":".
-00001080: 9a90 e7a7 98e8 8a9c e6b9 96e5 8a9b e987  ................
-00001090: 8f2d e697 a0e4 ba8b e58f 91e7 949f 222c  .-............",
-000010a0: 0a20 2020 2020 2020 2020 2022 6465 7363  .          "desc
-000010b0: 7269 6265 223a 22e4 bd86 e698 afe5 a5bd  ribe":".........
-000010c0: e583 8fe8 a2ab e5a5 87e6 80aa e79a 84e5  ................
-000010d0: 8a9b e987 8fe9 98bb e6ad a2e4 ba86 222c  ..............",
-000010e0: 0a20 2020 2020 2020 2020 2022 7461 7267  .          "targ
-000010f0: 6574 223a 300a 2020 2020 2020 2020 7d0a  et":0.        }.
-00001100: 2020 2020 2020 5d0a 2020 2020 5d0a 2020        ].    ].  
-00001110: 7d2c 0a20 207b 0a20 2022 6576 656e 745f  },.  {.  "event_
-00001120: 6e61 6d65 223a 22e8 8a9c e6b9 96e6 b395  name":".........
-00001130: e69d 96c2 b7e9 9a90 e8ba ab22 2c0a 2020  ...........",.  
-00001140: 2274 6172 6765 7422 3a32 2c0a 2020 2264  "target":2,.  "d
-00001150: 6573 6372 6962 6522 3a22 3c30 3ee5 be97  escribe":"<0>...
-00001160: e588 b0e4 ba86 e88a 9ce6 b996 e6b3 95e6  ................
-00001170: 9d96 efbc 8ce8 aea9 e689 80e6 9c89 e980  ................
-00001180: 89e6 898b e99a 90e8 baab e4ba 8628 31e5  .............(1.
-00001190: 9b9e e590 88ef bc89 222c 0a20 2022 6c69  ........",.  "li
-000011a0: 7665 223a 312c 0a20 2022 6e61 6d65 223a  ve":1,.  "name":
-000011b0: 22e9 9a90 e8ba ab22 2c0a 2020 2272 6f75  "......",.  "rou
-000011c0: 6e64 223a 312c 0a20 2022 6869 6469 6e67  nd":1,.  "hiding
-000011d0: 223a 310a 2020 7d0a 5d                   ":1.  }.]
+00000000: 5b0d 0a20 207b 0d0a 2020 2020 2265 7665  [..  {..    "eve
+00000010: 6e74 5f6e 616d 6522 3a22 e8b6 85e7 a8b3  nt_name":"......
+00000020: e5ae 9ae8 8a9c e6b9 965f e589 8de8 bf9b  ........._......
+00000030: 3422 2c0d 0a20 2020 2022 7461 7267 6574  4",..    "target
+00000040: 223a 302c 0d0a 2020 2020 2264 6573 6372  ":0,..    "descr
+00000050: 6962 6522 3a22 3c30 3ee5 be97 e588 b0e4  ibe":"<0>.......
+00000060: ba86 e8b6 85e7 a8b3 e5ae 9ae8 8a9c e6b9  ................
+00000070: 96ef bc8c e5bf abe9 809f e9a2 9de5 a496  ................
+00000080: e589 8de8 bf9b e4ba 8633 e6a0 bc22 2c0d  .........3...",.
+00000090: 0a20 2020 2022 6d6f 7665 223a 340d 0a20  .    "move":4.. 
+000000a0: 207d 2c0d 0a20 207b 0d0a 2020 2020 2265   },..  {..    "e
+000000b0: 7665 6e74 5f6e 616d 6522 3a22 e4b8 8de7  vent_name":"....
+000000c0: a8b3 e5ae 9ae8 8a9c e6b9 965f e589 8de8  ..........._....
+000000d0: bf9b 2d34 7e34 222c 0d0a 2020 2020 2274  ..-4~4",..    "t
+000000e0: 6172 6765 7422 3a30 2c0d 0a20 2020 2022  arget":0,..    "
+000000f0: 6465 7363 7269 6265 223a 223c 303e e5be  describe":"<0>..
+00000100: 97e5 88b0 e4ba 86e4 b88d e7a8 b3e5 ae9a  ................
+00000110: e88a 9ce6 b996 e58a 9be9 878f 2c22 2c0d  ............,",.
+00000120: 0a20 2020 2022 7261 6e64 6f6d 5f65 7665  .    "random_eve
+00000130: 6e74 5f6f 6e63 6522 3a5b 5b31 302c 207b  nt_once":[[10, {
+00000140: 0d0a 2020 2020 2020 2020 2020 2265 7665  ..          "eve
+00000150: 6e74 5f6e 616d 6522 3a22 e4b8 8de7 a8b3  nt_name":"......
+00000160: e5ae 9ae8 8a9c e6b9 965f e589 8de8 bf9b  ........._......
+00000170: 2d34 222c 0d0a 2020 2020 2020 2020 2020  -4",..          
+00000180: 2274 6172 6765 7422 3a30 2c0d 0a20 2020  "target":0,..   
+00000190: 2020 2020 2020 2022 6465 7363 7269 6265         "describe
+000001a0: 223a 22e5 908e e980 80e4 ba86 34e6 a0bc  ":".........4...
+000001b0: 222c 0d0a 2020 2020 2020 2020 2020 226d  ",..          "m
+000001c0: 6f76 6522 3a2d 340d 0a20 2020 2020 2020  ove":-4..       
+000001d0: 207d 0d0a 2020 2020 2020 5d2c 0d0a 2020   }..      ],..  
+000001e0: 2020 2020 2020 2020 5b32 302c 207b 0d0a          [20, {..
+000001f0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00000200: 5f6e 616d 6522 3a22 e4b8 8de7 a8b3 e5ae  _name":"........
+00000210: 9ae8 8a9c e6b9 965f e589 8de8 bf9b 2d33  ......._......-3
+00000220: 222c 0d0a 2020 2020 2020 2020 2020 2274  ",..          "t
+00000230: 6172 6765 7422 3a30 2c0d 0a20 2020 2020  arget":0,..     
+00000240: 2020 2020 2022 6465 7363 7269 6265 223a       "describe":
+00000250: 22e5 908e e980 80e4 ba86 33e6 a0bc 222c  ".........3...",
+00000260: 0d0a 2020 2020 2020 2020 2020 226d 6f76  ..          "mov
+00000270: 6522 3a2d 330d 0a20 2020 2020 2020 207d  e":-3..        }
+00000280: 0d0a 2020 2020 2020 5d2c 0d0a 2020 2020  ..      ],..    
+00000290: 2020 2020 2020 5b33 302c 207b 0d0a 2020        [30, {..  
+000002a0: 2020 2020 2020 2020 2265 7665 6e74 5f6e          "event_n
+000002b0: 616d 6522 3a22 e4b8 8de7 a8b3 e5ae 9ae8  ame":"..........
+000002c0: 8a9c e6b9 965f e589 8de8 bf9b 2d32 222c  ....._......-2",
+000002d0: 0d0a 2020 2020 2020 2020 2020 2274 6172  ..          "tar
+000002e0: 6765 7422 3a30 2c0d 0a20 2020 2020 2020  get":0,..       
+000002f0: 2020 2022 6465 7363 7269 6265 223a 22e5     "describe":".
+00000300: 908e e980 80e4 ba86 32e6 a0bc 222c 0d0a  ........2...",..
+00000310: 2020 2020 2020 2020 2020 226d 6f76 6522            "move"
+00000320: 3a2d 320d 0a20 2020 2020 2020 207d 0d0a  :-2..        }..
+00000330: 2020 2020 2020 5d2c 0d0a 2020 2020 2020        ],..      
+00000340: 2020 2020 5b34 302c 207b 0d0a 2020 2020      [40, {..    
+00000350: 2020 2020 2020 2265 7665 6e74 5f6e 616d        "event_nam
+00000360: 6522 3a22 e4b8 8de7 a8b3 e5ae 9ae8 8a9c  e":"............
+00000370: e6b9 965f e589 8de8 bf9b 2d31 222c 0d0a  ..._......-1",..
+00000380: 2020 2020 2020 2020 2020 2274 6172 6765            "targe
+00000390: 7422 3a30 2c0d 0a20 2020 2020 2020 2020  t":0,..         
+000003a0: 2022 6465 7363 7269 6265 223a 22e5 908e   "describe":"...
+000003b0: e980 80e4 ba86 31e6 a0bc 222c 0d0a 2020  ......1...",..  
+000003c0: 2020 2020 2020 2020 226d 6f76 6522 3a2d          "move":-
+000003d0: 310d 0a20 2020 2020 2020 207d 0d0a 2020  1..        }..  
+000003e0: 2020 2020 5d2c 0d0a 2020 2020 2020 2020      ],..        
+000003f0: 2020 5b35 302c 207b 0d0a 2020 2020 2020    [50, {..      
+00000400: 2020 2020 2265 7665 6e74 5f6e 616d 6522      "event_name"
+00000410: 3a22 e4b8 8de7 a8b3 e5ae 9ae8 8a9c e6b9  :"..............
+00000420: 965f e589 8de8 bf9b 3122 2c0d 0a20 2020  ._......1",..   
+00000430: 2020 2020 2020 2022 7461 7267 6574 223a         "target":
+00000440: 302c 0d0a 2020 2020 2020 2020 2020 2264  0,..          "d
+00000450: 6573 6372 6962 6522 3a22 e589 8de8 bf9b  escribe":"......
+00000460: e4ba 8631 e6a0 bc22 2c0d 0a20 2020 2020  ...1...",..     
+00000470: 2020 2020 2022 6d6f 7665 223a 310d 0a20       "move":1.. 
+00000480: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+00000490: 5d2c 0d0a 2020 2020 2020 2020 2020 5b36  ],..          [6
+000004a0: 302c 207b 0d0a 2020 2020 2020 2020 2020  0, {..          
+000004b0: 2265 7665 6e74 5f6e 616d 6522 3a22 e4b8  "event_name":"..
+000004c0: 8de7 a8b3 e5ae 9ae8 8a9c e6b9 965f e589  ............._..
+000004d0: 8de8 bf9b 3222 2c0d 0a20 2020 2020 2020  ....2",..       
+000004e0: 2020 2022 7461 7267 6574 223a 302c 0d0a     "target":0,..
+000004f0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00000500: 6962 6522 3a22 e589 8de8 bf9b e4ba 8632  ibe":".........2
+00000510: e6a0 bc22 2c0d 0a20 2020 2020 2020 2020  ...",..         
+00000520: 2022 6d6f 7665 223a 320d 0a20 2020 2020   "move":2..     
+00000530: 2020 207d 0d0a 2020 2020 2020 5d2c 0d0a     }..      ],..
+00000540: 2020 2020 2020 2020 2020 5b37 302c 207b            [70, {
+00000550: 0d0a 2020 2020 2020 2020 2020 2265 7665  ..          "eve
+00000560: 6e74 5f6e 616d 6522 3a22 e4b8 8de7 a8b3  nt_name":"......
+00000570: e5ae 9ae8 8a9c e6b9 965f e589 8de8 bf9b  ........._......
+00000580: 3322 2c0d 0a20 2020 2020 2020 2020 2022  3",..          "
+00000590: 7461 7267 6574 223a 302c 0d0a 2020 2020  target":0,..    
+000005a0: 2020 2020 2020 2264 6573 6372 6962 6522        "describe"
+000005b0: 3a22 e589 8de8 bf9b e4ba 8633 e6a0 bc22  :".........3..."
+000005c0: 2c0d 0a20 2020 2020 2020 2020 2022 6d6f  ,..          "mo
+000005d0: 7665 223a 330d 0a20 2020 2020 2020 207d  ve":3..        }
+000005e0: 0d0a 2020 2020 2020 5d2c 0d0a 2020 2020  ..      ],..    
+000005f0: 2020 2020 2020 5b38 302c 207b 0d0a 2020        [80, {..  
+00000600: 2020 2020 2020 2020 2265 7665 6e74 5f6e          "event_n
+00000610: 616d 6522 3a22 e4b8 8de7 a8b3 e5ae 9ae8  ame":"..........
+00000620: 8a9c e6b9 965f e589 8de8 bf9b 3422 2c0d  ....._......4",.
+00000630: 0a20 2020 2020 2020 2020 2022 7461 7267  .          "targ
+00000640: 6574 223a 302c 0d0a 2020 2020 2020 2020  et":0,..        
+00000650: 2020 2264 6573 6372 6962 6522 3a22 e589    "describe":"..
+00000660: 8de8 bf9b e4ba 8634 e6a0 bc22 2c0d 0a20  .......4...",.. 
+00000670: 2020 2020 2020 2020 2022 6d6f 7665 223a           "move":
+00000680: 340d 0a20 2020 2020 2020 207d 0d0a 2020  4..        }..  
+00000690: 2020 2020 5d0d 0a20 2020 205d 0d0a 2020      ]..    ]..  
+000006a0: 7d2c 0d0a 2020 7b0d 0a20 2020 2022 6576  },..  {..    "ev
+000006b0: 656e 745f 6e61 6d65 223a 22e9 bb91 e69a  ent_name":".....
+000006c0: 97e8 8a9c e6b9 96e5 8a9b e987 8f22 2c0d  .............",.
+000006d0: 0a20 2020 2022 7461 7267 6574 223a 312c  .    "target":1,
+000006e0: 0d0a 2020 2020 2264 6573 6372 6962 6522  ..    "describe"
+000006f0: 3a22 3c30 3ee5 be97 e588 b0e4 ba86 e8b6  :"<0>...........
+00000700: 85e7 a8b3 e5ae 9ae8 8a9c e6b9 96e5 8a9b  ................
+00000710: e987 8fef bc8c e69d 80e6 adbb e4ba 863c  ...............<
+00000720: 313e 222c 0d0a 2020 2020 2264 6965 223a  1>",..    "die":
+00000730: 312c 0d0a 2020 2020 2264 6965 5f6e 616d  1,..    "die_nam
+00000740: 6522 3a22 e88a 9ce6 b996 e4be b5e8 9a80  e":"............
+00000750: 220d 0a20 207d 2c0d 0a20 207b 0d0a 2020  "..  },..  {..  
+00000760: 2020 2265 7665 6e74 5f6e 616d 6522 3a22    "event_name":"
+00000770: e994 99e8 afaf e79a 84e8 8a9c e6b9 96e5  ................
+00000780: 8a9b e987 8f22 2c0d 0a20 2020 2022 7461  .....",..    "ta
+00000790: 7267 6574 223a 302c 0d0a 2020 2020 2264  rget":0,..    "d
+000007a0: 6573 6372 6962 6522 3a22 3c30 3ee5 be97  escribe":"<0>...
+000007b0: e588 b0e4 ba86 e994 99e8 afaf e79a 84e8  ................
+000007c0: 8a9c e6b9 96e5 8a9b e987 8fef bc8c e69d  ................
+000007d0: 80e6 adbb e4ba 86e8 87aa e5b7 b122 2c0d  .............",.
+000007e0: 0a20 2020 2022 6469 6522 3a31 2c0d 0a20  .    "die":1,.. 
+000007f0: 2020 2022 6469 655f 6e61 6d65 223a 22e8     "die_name":".
+00000800: 8a9c e6b9 96e4 beb5 e89a 8022 0d0a 2020  ..........."..  
+00000810: 7d2c 0d0a 2020 7b0d 0a20 2020 2022 6576  },..  {..    "ev
+00000820: 656e 745f 6e61 6d65 223a 22e8 87b3 e5b0  ent_name":".....
+00000830: 8ae8 8a9c e6b9 96e5 8a9b e987 8f22 2c0d  .............",.
+00000840: 0a20 2020 2022 7461 7267 6574 223a 302c  .    "target":0,
+00000850: 0d0a 2020 2020 2264 6573 6372 6962 6522  ..    "describe"
+00000860: 3a22 3c30 3ee5 be97 e588 b0e4 ba86 e987  :"<0>...........
+00000870: 91e5 8589 e997 aae9 97aa e887 b3e5 b08a  ................
+00000880: e88a 9ce6 b996 e58a 9be9 878f efbc 8c22  ..............."
+00000890: 2c0d 0a20 2020 2022 7261 6e64 6f6d 5f65  ,..    "random_e
+000008a0: 7665 6e74 5f6f 6e63 6522 3a5b 5b32 302c  vent_once":[[20,
+000008b0: 207b 0d0a 2020 2020 2020 2020 2265 7665   {..        "eve
+000008c0: 6e74 5f6e 616d 6522 3a22 e887 b3e5 b08a  nt_name":"......
+000008d0: e88a 9ce6 b996 e58a 9be9 878f 2de7 bb88  ............-...
+000008e0: e782 b922 2c0d 0a20 2020 2020 2020 2022  ...",..        "
+000008f0: 7461 7267 6574 223a 322c 0d0a 2020 2020  target":2,..    
+00000900: 2020 2020 2264 6573 6372 6962 6522 3a22      "describe":"
+00000910: e8ae a9e6 8980 e69c 89e9 8089 e689 8be9  ................
+00000920: 83bd e588 b0e8 bebe e4ba 86e7 bb88 e782  ................
+00000930: b922 2c0d 0a20 2020 2020 2020 2022 7472  .",..        "tr
+00000940: 6163 6b5f 7261 6e64 6f6d 5f6c 6f63 6174  ack_random_locat
+00000950: 696f 6e22 3a31 3030 0d0a 2020 2020 2020  ion":100..      
+00000960: 2020 7d0d 0a20 2020 2020 205d 2c0d 0a20    }..      ],.. 
+00000970: 2020 2020 205b 3130 302c 207b 0d0a 2020       [100, {..  
+00000980: 2020 2020 2020 2265 7665 6e74 5f6e 616d        "event_nam
+00000990: 6522 3a22 e887 b3e5 b08a e88a 9ce6 b996  e":"............
+000009a0: e58a 9be9 878f 2de6 97a0 e4ba 8be5 8f91  ......-.........
+000009b0: e794 9f22 2c0d 0a20 2020 2020 2020 2022  ...",..        "
+000009c0: 7461 7267 6574 223a 302c 0d0a 2020 2020  target":0,..    
+000009d0: 2020 2020 2264 6573 6372 6962 6522 3a22      "describe":"
+000009e0: e4bd 86e5 a5bd e583 8fe6 b2a1 e69c 89e5  ................
+000009f0: 95a5 e794 a822 0d0a 2020 2020 2020 2020  ....."..        
+00000a00: 7d0d 0a20 2020 2020 205d 0d0a 2020 2020  }..      ]..    
+00000a10: 5d0d 0a20 207d 2c0d 0a20 207b 0d0a 2020  ]..  },..  {..  
+00000a20: 2020 2265 7665 6e74 5f6e 616d 6522 3a22    "event_name":"
+00000a30: e8bd bbe9 878f e88a 9ce6 b996 e58a 9be9  ................
+00000a40: 878f 222c 0d0a 2020 2020 2274 6172 6765  ..",..    "targe
+00000a50: 7422 3a30 2c0d 0a20 2020 2022 6465 7363  t":0,..    "desc
+00000a60: 7269 6265 223a 223c 303e e5be 97e5 88b0  ribe":"<0>......
+00000a70: e4ba 86e8 bdbb e987 8fe8 8a9c e6b9 96e5  ................
+00000a80: 8a9b e987 8fef bc8c e8ae a9e8 87aa e5b7  ................
+00000a90: b1e9 a29d e5a4 96e5 898d e8bf 9b31 e6a0  .............1..
+00000aa0: bc22 2c0d 0a20 2020 2022 6d6f 7665 223a  .",..    "move":
+00000ab0: 310d 0a20 207d 2c0d 0a20 207b 0d0a 2020  1..  },..  {..  
+00000ac0: 2020 2265 7665 6e74 5f6e 616d 6522 3a22    "event_name":"
+00000ad0: e88a 9ce6 b996 e6b3 95e6 9d96 c2b7 e5a4  ................
+00000ae0: 8de8 8b8f 222c 0d0a 2020 2020 2274 6172  ....",..    "tar
+00000af0: 6765 7422 3a32 2c0d 0a20 2020 2022 6465  get":2,..    "de
+00000b00: 7363 7269 6265 223a 223c 303e e5be 97e5  scribe":"<0>....
+00000b10: 88b0 e4ba 863c e88a 9ce6 b996 e6b3 95e6  .....<..........
+00000b20: 9d96 c2b7 e5a4 8de8 8b8f 3eef bc8c e5a4  ..........>.....
+00000b30: 8de8 8b8f e4ba 86e6 8980 e69c 89e7 9a84  ................
+00000b40: e980 89e6 898b 2122 2c0d 0a20 2020 2022  ......!",..    "
+00000b50: 6c69 7665 223a 310d 0a20 207d 2c0d 0a20  live":1..  },.. 
+00000b60: 207b 0d0a 2020 2020 2265 7665 6e74 5f6e   {..    "event_n
+00000b70: 616d 6522 3a22 e88a 9ce6 b996 e6b3 95e6  ame":"..........
+00000b80: 9d96 c2b7 e5a4 a9e5 90af 3122 2c0d 0a20  ..........1",.. 
+00000b90: 2020 2022 7461 7267 6574 223a 302c 0d0a     "target":0,..
+00000ba0: 2020 2020 2264 6573 6372 6962 6522 3a22      "describe":"
+00000bb0: 3c30 3ee5 be97 e588 b0e4 ba86 3ce8 8a9c  <0>.........<...
+00000bc0: e6b9 96e6 b395 e69d 96c2 b7e5 a4a9 e590  ................
+00000bd0: af3e efbc 8ce6 938d e4bd 9ce5 a4b1 e8af  .>..............
+00000be0: afef bc8c e6af 81e7 81ad e4ba 86e8 87aa  ................
+00000bf0: e5b7 b122 2c0d 0a20 2020 2022 6469 6522  ...",..    "die"
+00000c00: 3a31 0d0a 2020 7d2c 0d0a 2020 7b0d 0a20  :1..  },..  {.. 
+00000c10: 2020 2022 6576 656e 745f 6e61 6d65 223a     "event_name":
+00000c20: 22e8 8a9c e6b9 96e6 b395 e69d 96c2 b7e5  "...............
+00000c30: a4a9 e590 af32 222c 0d0a 2020 2020 2274  .....2",..    "t
+00000c40: 6172 6765 7422 3a33 2c0d 0a20 2020 2022  arget":3,..    "
+00000c50: 6465 7363 7269 6265 223a 223c 303e e5be  describe":"<0>..
+00000c60: 97e5 88b0 e4ba 863c e88a 9ce6 b996 e6b3  .......<........
+00000c70: 95e6 9d96 c2b7 e5a4 a9e5 90af 3eef bc8c  ............>...
+00000c80: e5b0 9de8 af95 e6af 81e7 81ad e689 80e6  ................
+00000c90: 9c89 e79a 84e9 8089 e689 8bef bc8c e4bd  ................
+00000ca0: 86e5 8786 e698 9fe5 ae9e e59c a8e5 a4aa  ................
+00000cb0: e5b7 aee4 ba86 222c 0d0a 2020 2020 2272  ......",..    "r
+00000cc0: 616e 646f 6d5f 6576 656e 745f 6f6e 6365  andom_event_once
+00000cd0: 223a 5b5b 3330 2c20 7b0d 0a20 2020 2020  ":[[30, {..     
+00000ce0: 2020 2022 6576 656e 745f 6e61 6d65 223a     "event_name":
+00000cf0: 22e8 8a9c e6b9 96e6 b395 e69d 96c2 b7e5  "...............
+00000d00: a4a9 e590 af32 2de5 91bd e4b8 ad22 2c0d  .....2-......",.
+00000d10: 0a20 2020 2020 2020 2022 6465 7363 7269  .        "descri
+00000d20: 6265 223a 22ef bc8c 3c30 3ee8 a2ab e689  be":"...<0>.....
+00000d30: 93e4 b8ad e4ba 8622 2c0d 0a20 2020 2020  .......",..     
+00000d40: 2020 2022 7461 7267 6574 223a 302c 0d0a     "target":0,..
+00000d50: 2020 2020 2020 2020 2264 6965 223a 310d          "die":1.
+00000d60: 0a20 2020 2020 2020 207d 0d0a 2020 2020  .        }..    
+00000d70: 2020 5d2c 0d0a 2020 2020 2020 5b31 3030    ],..      [100
+00000d80: 2c20 7b0d 0a20 2020 2020 2020 2020 2022  , {..          "
+00000d90: 6576 656e 745f 6e61 6d65 223a 22e8 8a9c  event_name":"...
+00000da0: e6b9 96e6 b395 e69d 96c2 b7e5 a4a9 e590  ................
+00000db0: af32 2de6 9caa e591 bde4 b8ad 222c 0d0a  .2-.........",..
+00000dc0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00000dd0: 6962 6522 3a22 222c 0d0a 2020 2020 2020  ibe":"",..      
+00000de0: 2020 2020 2274 6172 6765 7422 3a30 0d0a      "target":0..
+00000df0: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
+00000e00: 205d 0d0a 2020 2020 5d0d 0a20 207d 2c0d   ]..    ]..  },.
+00000e10: 0a20 207b 0d0a 2020 2020 2265 7665 6e74  .  {..    "event
+00000e20: 5f6e 616d 6522 3a22 e88a 9ce6 b996 e6b3  _name":"........
+00000e30: 95e6 9d96 c2b7 e5a4 a9e5 90af 3322 2c0d  ............3",.
+00000e40: 0a20 2020 2022 7461 7267 6574 223a 302c  .    "target":0,
+00000e50: 0d0a 2020 2020 2264 6573 6372 6962 6522  ..    "describe"
+00000e60: 3a22 3c30 3ee5 be97 e588 b0e4 ba86 3ce8  :"<0>.........<.
+00000e70: 8a9c e6b9 96e6 b395 e69d 96c2 b7e5 a4a9  ................
+00000e80: e590 af3e efbc 8ce8 b5b7 e4ba 86e6 9d80  ...>............
+00000e90: e5bf 83ef bc8c e4bd 86e6 98af e5b9 b6e4  ................
+00000ea0: b88d e4bc 9ae6 938d e4bd 9c22 0d0a 2020  ..........."..  
+00000eb0: 7d2c 0d0a 2020 7b0d 0a20 2020 2022 6576  },..  {..    "ev
+00000ec0: 656e 745f 6e61 6d65 223a 22e8 8a9c e6b9  ent_name":".....
+00000ed0: 96e6 b395 e69d 96c2 b7e6 9caa e69d a522  ..............."
+00000ee0: 2c0d 0a20 2020 2022 7461 7267 6574 223a  ,..    "target":
+00000ef0: 322c 0d0a 2020 2020 2264 6573 6372 6962  2,..    "describ
+00000f00: 6522 3a22 3c30 3ee5 be97 e588 b0e4 ba86  e":"<0>.........
+00000f10: 3ce8 8a9c e6b9 96e6 b395 e69d 96c2 b7e6  <...............
+00000f20: 9caa e69d a53e efbc 8ce5 819c e6ad a2e4  .....>..........
+00000f30: ba86 e689 80e6 9c89 e980 89e6 898b e79a  ................
+00000f40: 84e6 97b6 e997 b421 222c 0d0a 2020 2020  .......!",..    
+00000f50: 2272 6f75 6e64 7322 3a31 2c0d 0a20 2020  "rounds":1,..   
+00000f60: 2022 6e61 6d65 223a 22e6 97b6 e581 9c22   "name":"......"
+00000f70: 2c0d 0a20 2020 2022 6c6f 6361 7465 5f6c  ,..    "locate_l
+00000f80: 6f63 6b22 3a31 0d0a 2020 7d2c 0d0a 2020  ock":1..  },..  
+00000f90: 2020 7b0d 0a20 2020 2022 6576 656e 745f    {..    "event_
+00000fa0: 6e61 6d65 223a 22e9 9a90 e7a7 98e8 8a9c  name":".........
+00000fb0: e6b9 96e5 8a9b e987 8f22 2c0d 0a20 2020  .........",..   
+00000fc0: 2022 7461 7267 6574 223a 302c 0d0a 2020   "target":0,..  
+00000fd0: 2020 2264 6573 6372 6962 6522 3a22 3c30    "describe":"<0
+00000fe0: 3ee5 be97 e588 b0e4 ba86 e99a 90e7 a798  >...............
+00000ff0: e88a 9ce6 b996 e58a 9be9 878f efbc 8c22  ..............."
+00001000: 2c0d 0a20 2020 2022 7261 6e64 6f6d 5f65  ,..    "random_e
+00001010: 7665 6e74 5f6f 6e63 6522 3a5b 5b37 302c  vent_once":[[70,
+00001020: 207b 0d0a 2020 2020 2020 2020 2265 7665   {..        "eve
+00001030: 6e74 5f6e 616d 6522 3a22 e99a 90e7 a798  nt_name":"......
+00001040: e88a 9ce6 b996 e58a 9be9 878f 2de9 9a90  ............-...
+00001050: e8ba ab22 2c0d 0a20 2020 2020 2020 2022  ...",..        "
+00001060: 6465 7363 7269 6265 223a 22e8 8eb7 e5be  describe":".....
+00001070: 97e4 ba86 e4ba 8ce5 9b9e e590 88e7 9a84  ................
+00001080: 3ce9 9a90 e8ba ab3e e78a b6e6 8081 222c  <......>......",
+00001090: 0d0a 2020 2020 2020 2020 2274 6172 6765  ..        "targe
+000010a0: 7422 3a30 2c0d 0a20 2020 2020 2020 2022  t":0,..        "
+000010b0: 6e61 6d65 223a 22e9 9a90 e8ba ab22 2c0d  name":"......",.
+000010c0: 0a20 2020 2020 2020 2022 726f 756e 6422  .        "round"
+000010d0: 3a32 2c0d 0a20 2020 2020 2020 2022 6869  :2,..        "hi
+000010e0: 6469 6e67 223a 310d 0a20 2020 2020 2020  ding":1..       
+000010f0: 207d 0d0a 2020 2020 2020 5d2c 0d0a 2020   }..      ],..  
+00001100: 2020 2020 5b31 3030 2c20 7b0d 0a20 2020      [100, {..   
+00001110: 2020 2020 2020 2022 6576 656e 745f 6e61         "event_na
+00001120: 6d65 223a 22e9 9a90 e7a7 98e8 8a9c e6b9  me":"...........
+00001130: 96e5 8a9b e987 8f2d e697 a0e4 ba8b e58f  .......-........
+00001140: 91e7 949f 222c 0d0a 2020 2020 2020 2020  ....",..        
+00001150: 2020 2264 6573 6372 6962 6522 3a22 e4bd    "describe":"..
+00001160: 86e6 98af e5a5 bde5 838f e8a2 abe5 a587  ................
+00001170: e680 aae7 9a84 e58a 9be9 878f e998 bbe6  ................
+00001180: ada2 e4ba 8622 2c0d 0a20 2020 2020 2020  .....",..       
+00001190: 2020 2022 7461 7267 6574 223a 300d 0a20     "target":0.. 
+000011a0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+000011b0: 5d0d 0a20 2020 205d 0d0a 2020 7d2c 0d0a  ]..    ]..  },..
+000011c0: 2020 7b0d 0a20 2022 6576 656e 745f 6e61    {..  "event_na
+000011d0: 6d65 223a 22e8 8a9c e6b9 96e6 b395 e69d  me":"...........
+000011e0: 96c2 b7e9 9a90 e8ba ab22 2c0d 0a20 2022  .........",..  "
+000011f0: 7461 7267 6574 223a 322c 0d0a 2020 2264  target":2,..  "d
+00001200: 6573 6372 6962 6522 3a22 3c30 3ee5 be97  escribe":"<0>...
+00001210: e588 b0e4 ba86 e88a 9ce6 b996 e6b3 95e6  ................
+00001220: 9d96 efbc 8ce8 aea9 e689 80e6 9c89 e980  ................
+00001230: 89e6 898b e99a 90e8 baab e4ba 8628 31e5  .............(1.
+00001240: 9b9e e590 88ef bc89 222c 0d0a 2020 226c  ........",..  "l
+00001250: 6976 6522 3a31 2c0d 0a20 2022 6e61 6d65  ive":1,..  "name
+00001260: 223a 22e9 9a90 e8ba ab22 2c0d 0a20 2022  ":"......",..  "
+00001270: 726f 756e 6422 3a31 2c0d 0a20 2022 6869  round":1,..  "hi
+00001280: 6469 6e67 223a 310d 0a20 207d 0d0a 5d    ding":1..  }..]
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,64 @@
-00000000: 5b0a 2020 7b0a 2020 2265 7665 6e74 5f6e  [.  {.  "event_n
-00000010: 616d 6522 3a22 e588 b7e6 96b0 e980 89e6  ame":"..........
-00000020: 898b e695 b0e6 8dae 3122 2c0a 2020 2274  ........1",.  "t
-00000030: 6172 6765 7422 3a30 2c0a 2020 2264 6573  arget":0,.  "des
-00000040: 6372 6962 6522 3a22 e8b5 abe5 b094 e99a  cribe":"........
-00000050: 8fe6 898b e4b8 80e7 82b9 efbc 8ce7 94a8  ................
-00000060: e7a5 9ee7 a798 e58a 9be9 878f e58a a0e5  ................
-00000070: bfab e4ba 863c 303e e79a 8442 7566 6673  .....<0>...Buffs
-00000080: e980 9fe5 baa6 efbc 8ce6 8980 e69c 89e7  ................
-00000090: 9a84 e695 88e6 9e9c e68c 81e7 bbad e697  ................
-000000a0: b6e9 97b4 2d31 222c 0a20 2022 6275 6666  ....-1",.  "buff
-000000b0: 5f74 696d 655f 6164 6422 3a2d 310a 2020  _time_add":-1.  
-000000c0: 7d2c 0a20 207b 0a20 2022 6576 656e 745f  },.  {.  "event_
-000000d0: 6e61 6d65 223a 22e5 88b7 e696 b0e9 8089  name":".........
-000000e0: e689 8be6 95b0 e68d ae32 222c 0a20 2022  .........2",.  "
-000000f0: 7461 7267 6574 223a 322c 0a20 2022 6465  target":2,.  "de
-00000100: 7363 7269 6265 223a 22e8 b5ab e5b0 94e9  scribe":".......
-00000110: 9a8f e689 8be4 b880 e782 b9ef bc8c e794  ................
-00000120: a8e7 a59e e7a7 98e5 8a9b e987 8fe5 8aa0  ................
-00000130: e5bf abe4 ba86 3c30 3ee7 9a84 4275 6666  ......<0>...Buff
-00000140: 73e9 809f e5ba a6ef bc8c e689 80e6 9c89  s...............
-00000150: e79a 84e6 9588 e69e 9ce6 8c81 e7bb ade6  ................
-00000160: 97b6 e997 b42d 3122 2c0a 2020 2262 7566  .....-1",.  "buf
-00000170: 665f 7469 6d65 5f61 6464 223a 2d31 0a20  f_time_add":-1. 
-00000180: 207d 2c0a 2020 7b0a 2020 2265 7665 6e74   },.  {.  "event
-00000190: 5f6e 616d 6522 3a22 e8b5 8be4 ba88 e980  _name":"........
-000001a0: 89e6 898b e79c a9e6 9995 4275 6666 222c  ..........Buff",
-000001b0: 0a20 2022 7461 7267 6574 223a 302c 0a20  .  "target":0,. 
-000001c0: 2022 6465 7363 7269 6265 223a 22e8 b5ab   "describe":"...
-000001d0: e5b0 94e6 89be e4b8 8de5 88b0 e794 b7e6  ................
-000001e0: 9c8b e58f 8be4 b99f e689 bee4 b88d e588  ................
-000001f0: b0e5 a5b3 e69c 8be5 8f8b efbc 8ce9 9d9e  ................
-00000200: e5b8 b8e7 949f e6b0 94ef bc8c e99a 8fe4  ................
-00000210: bebf e7bb 99e4 ba86 3c30 3ee4 b880 e4b8  ........<0>.....
-00000220: aa33 e59b 9ee5 9088 e79a 84e7 9ca9 e699  .3..............
-00000230: 9542 7566 6622 2c0a 2020 2272 6f75 6e64  .Buff",.  "round
-00000240: 7322 3a33 2c0a 2020 226e 616d 6522 3a22  s":3,.  "name":"
-00000250: e79c a9e6 9995 222c 0a20 2022 7665 7274  ......",.  "vert
-00000260: 6967 6f22 3a31 0a20 207d 2c0a 2020 7b0a  igo":1.  },.  {.
-00000270: 2020 2265 7665 6e74 5f6e 616d 6522 3a22    "event_name":"
-00000280: e688 91e5 b086 21e6 89ad e8bd ace4 b887  ......!.........
-00000290: e8b1 a121 222c 0a20 2022 7461 7267 6574  ...!",.  "target
-000002a0: 223a 322c 0a20 2022 6465 7363 7269 6265  ":2,.  "describe
-000002b0: 223a 22e8 b5ab e5b0 94e5 9ba0 e4b8 bae6  ":".............
-000002c0: 8abd e4b8 8de5 87ba e8af 86e5 ae9d efbc  ................
-000002d0: 8ce6 b094 e684 a4e7 9a84 e5a4 a7e5 968a  ................
-000002e0: efbc 8ce6 8891 e5b0 8621 21e6 89ad e8bd  .........!!.....
-000002f0: ace4 b887 e8b1 a121 2122 2c0a 2020 2274  .......!!",.  "t
-00000300: 7261 636b 5f72 616e 646f 6d5f 6c6f 6361  rack_random_loca
-00000310: 7469 6f6e 223a 310a 2020 7d2c 0a20 207b  tion":1.  },.  {
-00000320: 0a20 2022 6576 656e 745f 6e61 6d65 223a  .  "event_name":
-00000330: 22e6 8891 e5b0 8621 e689 ade8 bdac e4b8  "......!........
-00000340: 87e8 b1a1 2122 2c0a 2020 2274 6172 6765  ....!",.  "targe
-00000350: 7422 3a32 2c0a 2020 2264 6573 6372 6962  t":2,.  "describ
-00000360: 6522 3a22 e8b5 abe5 b094 e68a bde5 87ba  e":"............
-00000370: e4ba 86e8 af86 e5ae 9def bc8c e5bc 80e5  ................
-00000380: bf83 e79a 84e5 a4a7 e596 8aef bc8c e688  ................
-00000390: 91e5 b086 2121 e689 ade8 bdac e4b8 80e5  ....!!..........
-000003a0: 8887 2121 28e6 8980 e69c 89e9 8089 e689  ..!!(...........
-000003b0: 8be5 a48d e6b4 bbef bc89 222c 0a20 2022  ..........",.  "
-000003c0: 6c69 7665 223a 310a 2020 7d0a 5d0a 0a    live":1.  }.]..
+00000000: 5b0d 0a20 207b 0d0a 2020 2265 7665 6e74  [..  {..  "event
+00000010: 5f6e 616d 6522 3a22 e588 b7e6 96b0 e980  _name":"........
+00000020: 89e6 898b e695 b0e6 8dae 3122 2c0d 0a20  ..........1",.. 
+00000030: 2022 7461 7267 6574 223a 302c 0d0a 2020   "target":0,..  
+00000040: 2264 6573 6372 6962 6522 3a22 e8b5 abe5  "describe":"....
+00000050: b094 e99a 8fe6 898b e4b8 80e7 82b9 efbc  ................
+00000060: 8ce7 94a8 e7a5 9ee7 a798 e58a 9be9 878f  ................
+00000070: e58a a0e5 bfab e4ba 863c 303e e79a 8442  .........<0>...B
+00000080: 7566 6673 e980 9fe5 baa6 efbc 8ce6 8980  uffs............
+00000090: e69c 89e7 9a84 e695 88e6 9e9c e68c 81e7  ................
+000000a0: bbad e697 b6e9 97b4 2d31 222c 0d0a 2020  ........-1",..  
+000000b0: 2262 7566 665f 7469 6d65 5f61 6464 223a  "buff_time_add":
+000000c0: 2d31 0d0a 2020 7d2c 0d0a 2020 7b0d 0a20  -1..  },..  {.. 
+000000d0: 2022 6576 656e 745f 6e61 6d65 223a 22e5   "event_name":".
+000000e0: 88b7 e696 b0e9 8089 e689 8be6 95b0 e68d  ................
+000000f0: ae32 222c 0d0a 2020 2274 6172 6765 7422  .2",..  "target"
+00000100: 3a32 2c0d 0a20 2022 6465 7363 7269 6265  :2,..  "describe
+00000110: 223a 22e8 b5ab e5b0 94e9 9a8f e689 8be4  ":".............
+00000120: b880 e782 b9ef bc8c e794 a8e7 a59e e7a7  ................
+00000130: 98e5 8a9b e987 8fe5 8aa0 e5bf abe4 ba86  ................
+00000140: 3c30 3ee7 9a84 4275 6666 73e9 809f e5ba  <0>...Buffs.....
+00000150: a6ef bc8c e689 80e6 9c89 e79a 84e6 9588  ................
+00000160: e69e 9ce6 8c81 e7bb ade6 97b6 e997 b42d  ...............-
+00000170: 3122 2c0d 0a20 2022 6275 6666 5f74 696d  1",..  "buff_tim
+00000180: 655f 6164 6422 3a2d 310d 0a20 207d 2c0d  e_add":-1..  },.
+00000190: 0a20 207b 0d0a 2020 2265 7665 6e74 5f6e  .  {..  "event_n
+000001a0: 616d 6522 3a22 e8b5 8be4 ba88 e980 89e6  ame":"..........
+000001b0: 898b e79c a9e6 9995 4275 6666 222c 0d0a  ........Buff",..
+000001c0: 2020 2274 6172 6765 7422 3a30 2c0d 0a20    "target":0,.. 
+000001d0: 2022 6465 7363 7269 6265 223a 22e8 b5ab   "describe":"...
+000001e0: e5b0 94e6 89be e4b8 8de5 88b0 e794 b7e6  ................
+000001f0: 9c8b e58f 8be4 b99f e689 bee4 b88d e588  ................
+00000200: b0e5 a5b3 e69c 8be5 8f8b efbc 8ce9 9d9e  ................
+00000210: e5b8 b8e7 949f e6b0 94ef bc8c e99a 8fe4  ................
+00000220: bebf e7bb 99e4 ba86 3c30 3ee4 b880 e4b8  ........<0>.....
+00000230: aa33 e59b 9ee5 9088 e79a 84e7 9ca9 e699  .3..............
+00000240: 9542 7566 6622 2c0d 0a20 2022 726f 756e  .Buff",..  "roun
+00000250: 6473 223a 332c 0d0a 2020 226e 616d 6522  ds":3,..  "name"
+00000260: 3a22 e79c a9e6 9995 222c 0d0a 2020 2276  :"......",..  "v
+00000270: 6572 7469 676f 223a 310d 0a20 207d 2c0d  ertigo":1..  },.
+00000280: 0a20 207b 0d0a 2020 2265 7665 6e74 5f6e  .  {..  "event_n
+00000290: 616d 6522 3a22 e688 91e5 b086 21e6 89ad  ame":"......!...
+000002a0: e8bd ace4 b887 e8b1 a121 222c 0d0a 2020  .........!",..  
+000002b0: 2274 6172 6765 7422 3a32 2c0d 0a20 2022  "target":2,..  "
+000002c0: 6465 7363 7269 6265 223a 22e8 b5ab e5b0  describe":".....
+000002d0: 94e5 9ba0 e4b8 bae6 8abd e4b8 8de5 87ba  ................
+000002e0: e8af 86e5 ae9d efbc 8ce6 b094 e684 a4e7  ................
+000002f0: 9a84 e5a4 a7e5 968a efbc 8ce6 8891 e5b0  ................
+00000300: 8621 21e6 89ad e8bd ace4 b887 e8b1 a121  .!!............!
+00000310: 2122 2c0d 0a20 2022 7472 6163 6b5f 7261  !",..  "track_ra
+00000320: 6e64 6f6d 5f6c 6f63 6174 696f 6e22 3a31  ndom_location":1
+00000330: 0d0a 2020 7d2c 0d0a 2020 7b0d 0a20 2022  ..  },..  {..  "
+00000340: 6576 656e 745f 6e61 6d65 223a 22e6 8891  event_name":"...
+00000350: e5b0 8621 e689 ade8 bdac e4b8 87e8 b1a1  ...!............
+00000360: 2122 2c0d 0a20 2022 7461 7267 6574 223a  !",..  "target":
+00000370: 322c 0d0a 2020 2264 6573 6372 6962 6522  2,..  "describe"
+00000380: 3a22 e8b5 abe5 b094 e68a bde5 87ba e4ba  :"..............
+00000390: 86e8 af86 e5ae 9def bc8c e5bc 80e5 bf83  ................
+000003a0: e79a 84e5 a4a7 e596 8aef bc8c e688 91e5  ................
+000003b0: b086 2121 e689 ade8 bdac e4b8 80e5 8887  ..!!............
+000003c0: 2121 28e6 8980 e69c 89e9 8089 e689 8be5  !!(.............
+000003d0: a48d e6b4 bbef bc89 222c 0d0a 2020 226c  ........",..  "l
+000003e0: 6976 6522 3a31 0d0a 2020 7d0d 0a5d 0d0a  ive":1..  }..]..
+000003f0: 0d0a                                     ..
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 23% similar despite different names*

```diff
@@ -1,138 +1,141 @@
-00000000: 5b0a 2020 7b0a 2020 2020 2265 7665 6e74  [.  {.    "event
-00000010: 5f6e 616d 6522 3a22 e8b5 9be9 a9ac e59c  _name":"........
-00000020: bae4 ba8b e4bb b6e7 b0bf 3122 2c0a 2020  ..........1",.  
-00000030: 2020 2274 6172 6765 7422 3a30 2c0a 2020    "target":0,.  
-00000040: 2020 2264 6573 6372 6962 6522 3a22 5be8    "describe":"[.
-00000050: b59b e9a9 ace5 9cba e680 aae8 b088 5d3c  ..............]<
-00000060: 303e e79c 8be5 88b0 e4ba 86e8 b59b e9a9  0>..............
-00000070: ace5 9cba e79a 84e6 898b e586 8cef bc9a  ................
-00000080: 322e e8af b7e4 b88d e8a6 81e6 90ba e5b8  2...............
-00000090: a6e9 a39f e789 a9ef bc8c e5b0 a4e5 85b6  ................
-000000a0: e698 afe4 baba e7b1 bbe7 9a84 e9a3 9fe7  ................
-000000b0: 89a9 e68a 95e5 9682 e4bc 91e6 81af e58c  ................
-000000c0: bae4 b8ad e79a 84e9 a9ac e584 bfe3 8082  ................
-000000d0: 220a 7d2c 0a20 207b 0a20 2020 2022 6576  ".},.  {.    "ev
-000000e0: 656e 745f 6e61 6d65 223a 22e8 b59b e9a9  ent_name":".....
-000000f0: ace5 9cba e4ba 8be4 bbb6 e7b0 bf32 222c  .............2",
-00000100: 0a20 2020 2022 7461 7267 6574 223a 302c  .    "target":0,
-00000110: 0a20 2020 2022 6465 7363 7269 6265 223a  .    "describe":
-00000120: 225b e8b5 9be9 a9ac e59c bae6 80aa e8b0  "[..............
-00000130: 885d 3c30 3ee7 9c8b e588 b0e4 ba86 e8b5  .]<0>...........
-00000140: 9be9 a9ac e59c bae7 9a84 e689 8be5 868c  ................
-00000150: efbc 9a33 2ee5 a682 e69e 9ce4 bda0 e79c  ...3............
-00000160: 8be5 88b0 e9a9 ace5 84bf e592 8ce4 bda0  ................
-00000170: e5af b9e8 a786 efbc 8ce8 afb7 e7ab 8be5  ................
-00000180: 88bb e8bd ace7 a7bb e8a7 86e7 babf 220a  ..............".
-00000190: 7d2c 0a20 2020 207b 0a20 2020 2022 6576  },.    {.    "ev
-000001a0: 656e 745f 6e61 6d65 223a 22e8 b59b e9a9  ent_name":".....
-000001b0: ace5 9cba e4ba 8be4 bbb6 e7b0 bf33 222c  .............3",
-000001c0: 0a20 2020 2022 7461 7267 6574 223a 302c  .    "target":0,
-000001d0: 0a20 2020 2022 6465 7363 7269 6265 223a  .    "describe":
-000001e0: 225b e8b5 9be9 a9ac e59c bae6 80aa e8b0  "[..............
-000001f0: 885d 3c30 3ee7 9c8b e588 b0e4 ba86 e8b5  .]<0>...........
-00000200: 9be9 a9ac e59c bae7 9a84 e689 8be5 868c  ................
-00000210: efbc 9a37 2ee5 9ca8 e8b5 9be9 a9ac e591  ...7............
-00000220: a8e8 beb9 e5b0 8fe9 93ba e4b8 adef bc8c  ................
-00000230: e688 91e4 bbac e4b8 8de4 bc9a e68f 90e4  ................
-00000240: be9b e4b8 94e4 bdbf e794 a8e5 908d e4b8  ................
-00000250: bae9 8791 e5b8 81e7 9a84 e5b0 8fe7 a1ac  ................
-00000260: e5b8 81ef bc8c e5a6 82e6 9e9c e58f 91e7  ................
-00000270: 8eb0 e5b7 a5e4 bd9c e4ba bae5 9198 e8af  ................
-00000280: a2e9 97ae e4bd a0e6 98af e590 a6e8 a681  ................
-00000290: e4bd bfe7 94a8 e987 91e5 b881 e585 91e6  ................
-000002a0: 8da2 e789 a9e5 9381 efbc 8ce8 afb7 e7ab  ................
-000002b0: 8be5 88bb e7a6 bbe5 bc80 e591 a8e8 beb9  ................
-000002c0: e5b0 8fe9 93ba efbc 8ce5 b9b6 e5af bbe6  ................
-000002d0: 89be e999 84e8 bf91 e79a 84e5 b7a5 e4bd  ................
-000002e0: 9ce4 baba e591 98e8 afb4 e698 8ee6 8385  ................
-000002f0: e586 b5e3 8082 220a 0a7d 2c0a 2020 7b0a  ......"..},.  {.
-00000300: 2020 2020 2265 7665 6e74 5f6e 616d 6522      "event_name"
-00000310: 3a22 e8b5 9be9 a9ac e59c bae4 ba8b e4bb  :"..............
-00000320: b6e7 b0bf 3422 2c0a 2020 2020 2274 6172  ....4",.    "tar
-00000330: 6765 7422 3a30 2c0a 2020 2020 2264 6573  get":0,.    "des
-00000340: 6372 6962 6522 3a22 5be8 b59b e9a9 ace5  cribe":"[.......
-00000350: 9cba e680 aae8 b088 5d3c 303e e79c 8be5  ........]<0>....
-00000360: 88b0 e4ba 86e8 b59b e9a9 ace5 9cba e79a  ................
-00000370: 84e6 898b e586 8cef bc9a 382e e8b5 9be9  ..........8.....
-00000380: a9ac e59c bae4 bbbb e4bd 95e4 b880 e4b8  ................
-00000390: aae6 af94 e8b5 9be5 8cba e59f 9fe5 8faa  ................
-000003a0: e4bc 9ae5 9ca8 393a 3030 2d31 313a 3030  ......9:00-11:00
-000003b0: e592 8c31 353a 3030 2d31 373a 3030 e5bc  ...15:00-17:00..
-000003c0: 80e6 94be efbc 8ce5 a682 e69e 9ce5 85b6  ................
-000003d0: e4bb 96e6 97b6 e997 b4e5 b7a5 e4bd 9ce4  ................
-000003e0: baba e591 98e6 8ea8 e88d 90e4 bda0 e589  ................
-000003f0: 8de5 be80 e8a7 82e7 9c8b e6af 94e8 b59b  ................
-00000400: efbc 8ce8 afb7 e4b8 8de8 a681 e78a b9e8  ................
-00000410: b1ab e79b b4e6 8ea5 e68b 92e7 bb9d e5b9  ................
-00000420: b6e8 bf9c e7a6 bbe6 ada4 e5b7 a5e4 bd9c  ................
-00000430: e4ba bae5 9198 e380 8222 0a7d 2c0a 2020  .........".},.  
-00000440: 7b0a 2020 2020 2265 7665 6e74 5f6e 616d  {.    "event_nam
-00000450: 6522 3a22 e8b5 9be9 a9ac e59c bae4 ba8b  e":"............
-00000460: e4bb b6e7 b0bf 3522 2c0a 2020 2020 2274  ......5",.    "t
-00000470: 6172 6765 7422 3a30 2c0a 2020 2020 2264  arget":0,.    "d
-00000480: 6573 6372 6962 6522 3a22 5be8 b59b e9a9  escribe":"[.....
-00000490: ace5 9cba e680 aae8 b088 5d3c 303e e68d  ..........]<0>..
-000004a0: a1e5 88b0 e4ba 86e4 b880 e4b8 aae8 b59b  ................
-000004b0: e9a9 ace5 9cba e689 8be5 868c e4b9 a6e3  ................
-000004c0: 8082 e58f afe4 bba5 e587 ade5 809f e8bf  ................
-000004d0: 99e6 9da1 e6b6 88e6 81af e689 be20 e8b5  ............. ..
-000004e0: abe5 b094 20e9 a286 e58f 9620 3ee8 b59b  .... ...... >...
-000004f0: e9a9 ace5 9cba e680 aae8 b088 e8a7 84e5  ................
-00000500: 8899 e696 87e6 a188 3c22 0a7d 2c0a 2020  ........<".},.  
-00000510: 7b0a 2020 2020 2265 7665 6e74 5f6e 616d  {.    "event_nam
-00000520: 6522 3a22 e8b5 9be9 a9ac e59c bae4 ba8b  e":"............
-00000530: e4bb b6e7 b0bf 3622 2c0a 2020 2020 2274  ......6",.    "t
-00000540: 6172 6765 7422 3a30 2c0a 2020 2020 2264  arget":0,.    "d
-00000550: 6573 6372 6962 6522 3a22 5be8 b59b e9a9  escribe":"[.....
-00000560: ace5 9cba e680 aae8 b088 5d3c 303e e6ad  ..........]<0>..
-00000570: a3e5 9ca8 e4bb 94e7 bb86 e998 85e8 afbb  ................
-00000580: e8b5 9be9 a9ac e59c bae6 898b e586 8cef  ................
-00000590: bc9a 3130 2ee5 a682 e69e 9ce5 8f91 e78e  ..10............
-000005a0: b0e5 91a8 e8be b9e6 9c89 e99b bee9 9cbe  ................
-000005b0: efbc 8ce8 afb7 e68c 89e7 85a7 e59c b0e5  ................
-000005c0: 9bbe e68c 87e7 a4ba e79a 84e8 b7af e5be  ................
-000005d0: 84e7 a6bb e5bc 80e8 b59b e9a9 ace5 9cba  ................
-000005e0: e380 8222 0a7d 2c0a 2020 7b0a 2020 2020  ...".},.  {.    
-000005f0: 2265 7665 6e74 5f6e 616d 6522 3a22 e8b5  "event_name":"..
-00000600: 9be9 a9ac e59c bae4 ba8b e4bb b6e7 b0bf  ................
-00000610: 3722 2c0a 2020 2020 2274 6172 6765 7422  7",.    "target"
-00000620: 3a30 2c0a 2020 2020 2264 6573 6372 6962  :0,.    "describ
-00000630: 6522 3a22 5be5 8aa8 e789 a9e5 9bad e8a7  e":"[...........
-00000640: 84e5 8899 e680 aae8 b088 5d3c 303e e59c  ..........]<0>..
-00000650: a8e8 b59b e9a9 ace5 9cba e79c 8be5 88b0  ................
-00000660: e4ba 86e7 99bd e889 b2e7 9a84 e5a4 a7e8  ................
-00000670: b1a1 e59c a8e6 b8b8 e6b3 b3e3 8082 e5bc  ................
-00000680: 80e5 a78b e680 80e7 9691 e887 aae5 b7b1  ................
-00000690: e698 afe8 b081 efbc 8128 33e5 9b9e e590  .........(3.....
-000006a0: 882d 327e 2b32 2922 2c0a 2020 2020 2272  .-2~+2)",.    "r
-000006b0: 6f75 6e64 7322 3a33 2c0a 2020 2020 226e  ounds":3,.    "n
-000006c0: 616d 6522 3a22 3f22 2c0a 2020 2020 226d  ame":"?",.    "m
-000006d0: 6f76 655f 6d61 7822 3a32 2c0a 2020 2020  ove_max":2,.    
-000006e0: 226d 6f76 655f 6d69 6e22 3a2d 320a 7d2c  "move_min":-2.},
-000006f0: 0a20 207b 0a20 2020 2022 6576 656e 745f  .  {.    "event_
-00000700: 6e61 6d65 223a 22e8 b59b e9a9 ace5 9cba  name":".........
-00000710: e4ba 8be4 bbb6 e7b0 bf38 222c 0a20 2020  .........8",.   
-00000720: 2022 7461 7267 6574 223a 302c 0a20 2020   "target":0,.   
-00000730: 2022 6465 7363 7269 6265 223a 225b e58a   "describe":"[..
-00000740: a8e7 89a9 e59b ade8 a784 e588 99e6 80aa  ................
-00000750: e8b0 885d 3c30 3ee5 9ca8 e8b5 9be9 a9ac  ...]<0>.........
-00000760: e59c bae5 8685 e58f 91e7 8eb0 e4ba 86e6  ................
-00000770: b0b4 e697 8fe9 a686 efbc 8153 616e e580  ...........San..
-00000780: bce7 96af e78b 82e4 b88b e999 8def bc81  ................
-00000790: e79b b4e6 8ea5 e980 80e5 9b9e e8b5 b7e7  ................
-000007a0: 82b9 efbc 8122 2c0a 2020 2020 226d 6f76  .....",.    "mov
-000007b0: 6522 3a2d 3130 300a 2020 7d2c 0a20 207b  e":-100.  },.  {
-000007c0: 0a20 2020 2022 6576 656e 745f 6e61 6d65  .    "event_name
-000007d0: 223a 22e8 b59b e9a9 ace5 9cba e4ba 8be4  ":".............
-000007e0: bbb6 e7b0 bf39 222c 0a20 2020 2022 7461  .....9",.    "ta
-000007f0: 7267 6574 223a 302c 0a20 2020 2022 6465  rget":0,.    "de
-00000800: 7363 7269 6265 223a 225b e58a a8e7 89a9  scribe":"[......
-00000810: e59b ade8 a784 e588 99e6 80aa e8b0 885d  ...............]
-00000820: 3c30 3ee5 9ca8 e8b5 9be9 a9ac e59c bae5  <0>.............
-00000830: 8685 e596 9de4 ba86 e585 94e5 ad90 e8a1  ................
-00000840: 80ef bc8c e590 83e4 ba86 e5b1 b1e7 be8a  ................
-00000850: e882 89e3 8082 e8a7 89e5 be97 e887 aae5  ................
-00000860: b7b1 e7aa 81e7 84b6 e585 85e6 bba1 e4ba  ................
-00000870: 86e5 8a9b e987 8fef bc81 e589 8de8 bf9b  ................
-00000880: 3522 2c0a 2020 2020 226d 6f76 6522 3a35  5",.    "move":5
-00000890: 0a20 207d 0a5d 0a                        .  }.].
+00000000: 5b0d 0a20 207b 0d0a 2020 2020 2265 7665  [..  {..    "eve
+00000010: 6e74 5f6e 616d 6522 3a22 e8b5 9be9 a9ac  nt_name":"......
+00000020: e59c bae4 ba8b e4bb b6e7 b0bf 3122 2c0d  ............1",.
+00000030: 0a20 2020 2022 7461 7267 6574 223a 302c  .    "target":0,
+00000040: 0d0a 2020 2020 2264 6573 6372 6962 6522  ..    "describe"
+00000050: 3a22 5be8 b59b e9a9 ace5 9cba e680 aae8  :"[.............
+00000060: b088 5d3c 303e e79c 8be5 88b0 e4ba 86e8  ..]<0>..........
+00000070: b59b e9a9 ace5 9cba e79a 84e6 898b e586  ................
+00000080: 8cef bc9a 322e e8af b7e4 b88d e8a6 81e6  ....2...........
+00000090: 90ba e5b8 a6e9 a39f e789 a9ef bc8c e5b0  ................
+000000a0: a4e5 85b6 e698 afe4 baba e7b1 bbe7 9a84  ................
+000000b0: e9a3 9fe7 89a9 e68a 95e5 9682 e4bc 91e6  ................
+000000c0: 81af e58c bae4 b8ad e79a 84e9 a9ac e584  ................
+000000d0: bfe3 8082 220d 0a7d 2c0d 0a20 207b 0d0a  ...."..},..  {..
+000000e0: 2020 2020 2265 7665 6e74 5f6e 616d 6522      "event_name"
+000000f0: 3a22 e8b5 9be9 a9ac e59c bae4 ba8b e4bb  :"..............
+00000100: b6e7 b0bf 3222 2c0d 0a20 2020 2022 7461  ....2",..    "ta
+00000110: 7267 6574 223a 302c 0d0a 2020 2020 2264  rget":0,..    "d
+00000120: 6573 6372 6962 6522 3a22 5be8 b59b e9a9  escribe":"[.....
+00000130: ace5 9cba e680 aae8 b088 5d3c 303e e79c  ..........]<0>..
+00000140: 8be5 88b0 e4ba 86e8 b59b e9a9 ace5 9cba  ................
+00000150: e79a 84e6 898b e586 8cef bc9a 332e e5a6  ............3...
+00000160: 82e6 9e9c e4bd a0e7 9c8b e588 b0e9 a9ac  ................
+00000170: e584 bfe5 928c e4bd a0e5 afb9 e8a7 86ef  ................
+00000180: bc8c e8af b7e7 ab8b e588 bbe8 bdac e7a7  ................
+00000190: bbe8 a786 e7ba bf22 0d0a 7d2c 0d0a 2020  ......."..},..  
+000001a0: 2020 7b0d 0a20 2020 2022 6576 656e 745f    {..    "event_
+000001b0: 6e61 6d65 223a 22e8 b59b e9a9 ace5 9cba  name":".........
+000001c0: e4ba 8be4 bbb6 e7b0 bf33 222c 0d0a 2020  .........3",..  
+000001d0: 2020 2274 6172 6765 7422 3a30 2c0d 0a20    "target":0,.. 
+000001e0: 2020 2022 6465 7363 7269 6265 223a 225b     "describe":"[
+000001f0: e8b5 9be9 a9ac e59c bae6 80aa e8b0 885d  ...............]
+00000200: 3c30 3ee7 9c8b e588 b0e4 ba86 e8b5 9be9  <0>.............
+00000210: a9ac e59c bae7 9a84 e689 8be5 868c efbc  ................
+00000220: 9a37 2ee5 9ca8 e8b5 9be9 a9ac e591 a8e8  .7..............
+00000230: beb9 e5b0 8fe9 93ba e4b8 adef bc8c e688  ................
+00000240: 91e4 bbac e4b8 8de4 bc9a e68f 90e4 be9b  ................
+00000250: e4b8 94e4 bdbf e794 a8e5 908d e4b8 bae9  ................
+00000260: 8791 e5b8 81e7 9a84 e5b0 8fe7 a1ac e5b8  ................
+00000270: 81ef bc8c e5a6 82e6 9e9c e58f 91e7 8eb0  ................
+00000280: e5b7 a5e4 bd9c e4ba bae5 9198 e8af a2e9  ................
+00000290: 97ae e4bd a0e6 98af e590 a6e8 a681 e4bd  ................
+000002a0: bfe7 94a8 e987 91e5 b881 e585 91e6 8da2  ................
+000002b0: e789 a9e5 9381 efbc 8ce8 afb7 e7ab 8be5  ................
+000002c0: 88bb e7a6 bbe5 bc80 e591 a8e8 beb9 e5b0  ................
+000002d0: 8fe9 93ba efbc 8ce5 b9b6 e5af bbe6 89be  ................
+000002e0: e999 84e8 bf91 e79a 84e5 b7a5 e4bd 9ce4  ................
+000002f0: baba e591 98e8 afb4 e698 8ee6 8385 e586  ................
+00000300: b5e3 8082 220d 0a0d 0a7d 2c0d 0a20 207b  ...."....},..  {
+00000310: 0d0a 2020 2020 2265 7665 6e74 5f6e 616d  ..    "event_nam
+00000320: 6522 3a22 e8b5 9be9 a9ac e59c bae4 ba8b  e":"............
+00000330: e4bb b6e7 b0bf 3422 2c0d 0a20 2020 2022  ......4",..    "
+00000340: 7461 7267 6574 223a 302c 0d0a 2020 2020  target":0,..    
+00000350: 2264 6573 6372 6962 6522 3a22 5be8 b59b  "describe":"[...
+00000360: e9a9 ace5 9cba e680 aae8 b088 5d3c 303e  ............]<0>
+00000370: e79c 8be5 88b0 e4ba 86e8 b59b e9a9 ace5  ................
+00000380: 9cba e79a 84e6 898b e586 8cef bc9a 382e  ..............8.
+00000390: e8b5 9be9 a9ac e59c bae4 bbbb e4bd 95e4  ................
+000003a0: b880 e4b8 aae6 af94 e8b5 9be5 8cba e59f  ................
+000003b0: 9fe5 8faa e4bc 9ae5 9ca8 393a 3030 2d31  ..........9:00-1
+000003c0: 313a 3030 e592 8c31 353a 3030 2d31 373a  1:00...15:00-17:
+000003d0: 3030 e5bc 80e6 94be efbc 8ce5 a682 e69e  00..............
+000003e0: 9ce5 85b6 e4bb 96e6 97b6 e997 b4e5 b7a5  ................
+000003f0: e4bd 9ce4 baba e591 98e6 8ea8 e88d 90e4  ................
+00000400: bda0 e589 8de5 be80 e8a7 82e7 9c8b e6af  ................
+00000410: 94e8 b59b efbc 8ce8 afb7 e4b8 8de8 a681  ................
+00000420: e78a b9e8 b1ab e79b b4e6 8ea5 e68b 92e7  ................
+00000430: bb9d e5b9 b6e8 bf9c e7a6 bbe6 ada4 e5b7  ................
+00000440: a5e4 bd9c e4ba bae5 9198 e380 8222 0d0a  ............."..
+00000450: 7d2c 0d0a 2020 7b0d 0a20 2020 2022 6576  },..  {..    "ev
+00000460: 656e 745f 6e61 6d65 223a 22e8 b59b e9a9  ent_name":".....
+00000470: ace5 9cba e4ba 8be4 bbb6 e7b0 bf35 222c  .............5",
+00000480: 0d0a 2020 2020 2274 6172 6765 7422 3a30  ..    "target":0
+00000490: 2c0d 0a20 2020 2022 6465 7363 7269 6265  ,..    "describe
+000004a0: 223a 225b e8b5 9be9 a9ac e59c bae6 80aa  ":"[............
+000004b0: e8b0 885d 3c30 3ee6 8da1 e588 b0e4 ba86  ...]<0>.........
+000004c0: e4b8 80e4 b8aa e8b5 9be9 a9ac e59c bae6  ................
+000004d0: 898b e586 8ce4 b9a6 e380 82e5 8faf e4bb  ................
+000004e0: a5e5 87ad e580 9fe8 bf99 e69d a1e6 b688  ................
+000004f0: e681 afe6 89be 20e8 b5ab e5b0 9420 e9a2  ...... ...... ..
+00000500: 86e5 8f96 203e e8b5 9be9 a9ac e59c bae6  .... >..........
+00000510: 80aa e8b0 88e8 a784 e588 99e6 9687 e6a1  ................
+00000520: 883c 220d 0a7d 2c0d 0a20 207b 0d0a 2020  .<"..},..  {..  
+00000530: 2020 2265 7665 6e74 5f6e 616d 6522 3a22    "event_name":"
+00000540: e8b5 9be9 a9ac e59c bae4 ba8b e4bb b6e7  ................
+00000550: b0bf 3622 2c0d 0a20 2020 2022 7461 7267  ..6",..    "targ
+00000560: 6574 223a 302c 0d0a 2020 2020 2264 6573  et":0,..    "des
+00000570: 6372 6962 6522 3a22 5be8 b59b e9a9 ace5  cribe":"[.......
+00000580: 9cba e680 aae8 b088 5d3c 303e e6ad a3e5  ........]<0>....
+00000590: 9ca8 e4bb 94e7 bb86 e998 85e8 afbb e8b5  ................
+000005a0: 9be9 a9ac e59c bae6 898b e586 8cef bc9a  ................
+000005b0: 3130 2ee5 a682 e69e 9ce5 8f91 e78e b0e5  10..............
+000005c0: 91a8 e8be b9e6 9c89 e99b bee9 9cbe efbc  ................
+000005d0: 8ce8 afb7 e68c 89e7 85a7 e59c b0e5 9bbe  ................
+000005e0: e68c 87e7 a4ba e79a 84e8 b7af e5be 84e7  ................
+000005f0: a6bb e5bc 80e8 b59b e9a9 ace5 9cba e380  ................
+00000600: 8222 0d0a 7d2c 0d0a 2020 7b0d 0a20 2020  ."..},..  {..   
+00000610: 2022 6576 656e 745f 6e61 6d65 223a 22e8   "event_name":".
+00000620: b59b e9a9 ace5 9cba e4ba 8be4 bbb6 e7b0  ................
+00000630: bf37 222c 0d0a 2020 2020 2274 6172 6765  .7",..    "targe
+00000640: 7422 3a30 2c0d 0a20 2020 2022 6465 7363  t":0,..    "desc
+00000650: 7269 6265 223a 225b e58a a8e7 89a9 e59b  ribe":"[........
+00000660: ade8 a784 e588 99e6 80aa e8b0 885d 3c30  .............]<0
+00000670: 3ee5 9ca8 e8b5 9be9 a9ac e59c bae7 9c8b  >...............
+00000680: e588 b0e4 ba86 e799 bde8 89b2 e79a 84e5  ................
+00000690: a4a7 e8b1 a1e5 9ca8 e6b8 b8e6 b3b3 e380  ................
+000006a0: 82e5 bc80 e5a7 8be6 8080 e796 91e8 87aa  ................
+000006b0: e5b7 b1e6 98af e8b0 81ef bc81 2833 e59b  ............(3..
+000006c0: 9ee5 9088 2d32 7e2b 3229 222c 0d0a 2020  ....-2~+2)",..  
+000006d0: 2020 2272 6f75 6e64 7322 3a33 2c0d 0a20    "rounds":3,.. 
+000006e0: 2020 2022 6e61 6d65 223a 223f 222c 0d0a     "name":"?",..
+000006f0: 2020 2020 226d 6f76 655f 6d61 7822 3a32      "move_max":2
+00000700: 2c0d 0a20 2020 2022 6d6f 7665 5f6d 696e  ,..    "move_min
+00000710: 223a 2d32 0d0a 7d2c 0d0a 2020 7b0d 0a20  ":-2..},..  {.. 
+00000720: 2020 2022 6576 656e 745f 6e61 6d65 223a     "event_name":
+00000730: 22e8 b59b e9a9 ace5 9cba e4ba 8be4 bbb6  "...............
+00000740: e7b0 bf38 222c 0d0a 2020 2020 2274 6172  ...8",..    "tar
+00000750: 6765 7422 3a30 2c0d 0a20 2020 2022 6465  get":0,..    "de
+00000760: 7363 7269 6265 223a 225b e58a a8e7 89a9  scribe":"[......
+00000770: e59b ade8 a784 e588 99e6 80aa e8b0 885d  ...............]
+00000780: 3c30 3ee5 9ca8 e8b5 9be9 a9ac e59c bae5  <0>.............
+00000790: 8685 e58f 91e7 8eb0 e4ba 86e6 b0b4 e697  ................
+000007a0: 8fe9 a686 efbc 8153 616e e580 bce7 96af  .......San......
+000007b0: e78b 82e4 b88b e999 8def bc81 e79b b4e6  ................
+000007c0: 8ea5 e980 80e5 9b9e e8b5 b7e7 82b9 efbc  ................
+000007d0: 8122 2c0d 0a20 2020 2022 6d6f 7665 223a  .",..    "move":
+000007e0: 2d31 3030 0d0a 2020 7d2c 0d0a 2020 7b0d  -100..  },..  {.
+000007f0: 0a20 2020 2022 6576 656e 745f 6e61 6d65  .    "event_name
+00000800: 223a 22e8 b59b e9a9 ace5 9cba e4ba 8be4  ":".............
+00000810: bbb6 e7b0 bf39 222c 0d0a 2020 2020 2274  .....9",..    "t
+00000820: 6172 6765 7422 3a30 2c0d 0a20 2020 2022  arget":0,..    "
+00000830: 6465 7363 7269 6265 223a 225b e58a a8e7  describe":"[....
+00000840: 89a9 e59b ade8 a784 e588 99e6 80aa e8b0  ................
+00000850: 885d 3c30 3ee5 9ca8 e8b5 9be9 a9ac e59c  .]<0>...........
+00000860: bae5 8685 e596 9de4 ba86 e585 94e5 ad90  ................
+00000870: e8a1 80ef bc8c e590 83e4 ba86 e5b1 b1e7  ................
+00000880: be8a e882 89e3 8082 e8a7 89e5 be97 e887  ................
+00000890: aae5 b7b1 e7aa 81e7 84b6 e585 85e6 bba1  ................
+000008a0: e4ba 86e5 8a9b e987 8fef bc81 e589 8de8  ................
+000008b0: bf9b 3522 2c0d 0a20 2020 2022 6d6f 7665  ..5",..    "move
+000008c0: 223a 350d 0a20 207d 0d0a 5d0d 0a         ":5..  }..]..
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954545454545454%*

 * *Differences: {"'52102'": "{'intro': '有50%的概率获得金币，50%的概率失去金币。\\n上限 Lv.50 金库。', 'des': '带参数2或4使用一颗钻石取消上线。'}"}*

```diff
@@ -123,16 +123,16 @@
         "des": "\u4f7f\u7528\u795e\u79d8\u5929\u5e73\u9700\u8981\u4e00\u70b9\u70b9\u624b\u7eed\u8d39\u3002",
         "intro": "\u4e0e\u968f\u673a\u4e00\u4e2a\u4eba\u5e73\u5206\u91d1\u5e01\u3002",
         "name": "\u795e\u79d8\u5929\u5e73",
         "rare": 5
     },
     "52102": {
         "color": "#FF6600",
-        "des": "\u5c01\u9876Lv.50\u91d1\u5e93\u3002\n\u4f7f\u7528\u53c2\u65702\u53ef\u6d88\u8017\u4e00\u9897\u94bb\u77f3\u89e3\u9664\u5c01\u9876\u3002",
-        "intro": "50%\u7684\u6982\u7387\u4f7f\u4f60\u7684\u91d1\u5e01\u6570\u7ffb\u500d\uff0c\u53e6\u591650%\u7684\u6982\u7387\u4f7f\u4f60\u7684\u91d1\u5e01\u6570\u51cf\u534a\u3002",
+        "des": "\u5e26\u53c2\u65702\u62164\u4f7f\u7528\u4e00\u9897\u94bb\u77f3\u53d6\u6d88\u4e0a\u7ebf\u3002",
+        "intro": "\u670950%\u7684\u6982\u7387\u83b7\u5f97\u91d1\u5e01\uff0c50%\u7684\u6982\u7387\u5931\u53bb\u91d1\u5e01\u3002\n\u4e0a\u9650 Lv.50 \u91d1\u5e93\u3002",
         "name": "\u5e78\u8fd0\u786c\u5e01",
         "rare": 5
     },
     "53101": {
         "color": "#FF3300",
         "des": "\u611f\u8c22\u5404\u4f4d\u73a9\u5bb6\u7684\u652f\u6301\uff01",
         "intro": "\u6253\u5f00\u540e\u53ef\u4ee5\u83b7\u5f97\u3010\u91d1\u5e01\u7b7e\u5230-\u91cd\u7f6e\u7b7e\u5230\u3011\u8303\u56f4\u7684\u968f\u673a\u91d1\u5e01\u3002",
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,21 +55,18 @@
         tight_layout = True,
         style = style,
         figsize = figsize,
         savefig = savefig
         )
 
 if __name__ == "__main__":
-    #russian_path = Path(sys.argv[1])
-    #company_id = sys.argv[2]
-    russian_path = Path("D:\\testbot\\data\\russian")
-    company_id = "546421320"
+    russian_path = Path(sys.argv[1])
+    company_id = sys.argv[2]
     candlestick_cache = russian_path / "candlestick"
     candlestick_cache.mkdir(parents = True, exist_ok = True)
     candlestick = Path(candlestick_cache / f"{company_id}.png")
     if candlestick.exists() and time.time() - candlestick.stat().st_ctime < 600:
-        pass
-        #sys.exit(0)
+        sys.exit(0)
     history_file = russian_path / "market_history.json"
     with open(history_file, "r", encoding="utf8") as f:
         market_history = json.load(f)
     market_candlestick((9.5,3), 12, market_history[company_id], candlestick_cache / f"{company_id}.png")
```

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/utils/chart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.1/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.1/setup.py` & `nonebot_plugin_game_collection-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.1.1',
+version='2.1.3',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```


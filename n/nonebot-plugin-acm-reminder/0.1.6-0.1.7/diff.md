# Comparing `tmp/nonebot-plugin-acm-reminder-0.1.6.tar.gz` & `tmp/nonebot-plugin-acm-reminder-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-acm-reminder-0.1.6.tar", last modified: Thu Apr  6 15:34:14 2023, max compression
+gzip compressed data, was "nonebot-plugin-acm-reminder-0.1.7.tar", last modified: Sat Apr 29 14:08:23 2023, max compression
```

## Comparing `nonebot-plugin-acm-reminder-0.1.6.tar` & `nonebot-plugin-acm-reminder-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1088 2023-01-15 11:05:12.918513 nonebot-plugin-acm-reminder-0.1.6/LICENSE
--rw-r--r--   0        0        0     3028 2023-04-06 15:33:46.324195 nonebot-plugin-acm-reminder-0.1.6/nonebot_plugin_acm_reminder/__init__.py
--rw-r--r--   0        0        0      228 2023-04-06 15:33:46.324195 nonebot-plugin-acm-reminder-0.1.6/nonebot_plugin_acm_reminder/config.py
--rw-r--r--   0        0        0     3579 2023-04-06 15:33:46.324195 nonebot-plugin-acm-reminder-0.1.6/nonebot_plugin_acm_reminder/data_source.py
--rw-r--r--   0        0        0      636 2023-04-06 15:33:46.324195 nonebot-plugin-acm-reminder-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      852 2023-04-06 15:33:46.324195 nonebot-plugin-acm-reminder-0.1.6/README.md
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 nonebot-plugin-acm-reminder-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-01-15 11:05:12.918513 nonebot-plugin-acm-reminder-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3028 2023-04-06 15:33:46.324195 nonebot-plugin-acm-reminder-0.1.7/nonebot_plugin_acm_reminder/__init__.py
+-rw-r--r--   0        0        0      228 2023-04-06 15:33:46.324195 nonebot-plugin-acm-reminder-0.1.7/nonebot_plugin_acm_reminder/config.py
+-rw-r--r--   0        0        0     3706 2023-04-29 14:08:14.618792 nonebot-plugin-acm-reminder-0.1.7/nonebot_plugin_acm_reminder/data_source.py
+-rw-r--r--   0        0        0      636 2023-04-29 14:08:14.618792 nonebot-plugin-acm-reminder-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      852 2023-04-06 15:33:46.324195 nonebot-plugin-acm-reminder-0.1.7/README.md
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 nonebot-plugin-acm-reminder-0.1.7/PKG-INFO
```

### Comparing `nonebot-plugin-acm-reminder-0.1.6/LICENSE` & `nonebot-plugin-acm-reminder-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-acm-reminder-0.1.6/nonebot_plugin_acm_reminder/__init__.py` & `nonebot-plugin-acm-reminder-0.1.7/nonebot_plugin_acm_reminder/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-acm-reminder-0.1.6/nonebot_plugin_acm_reminder/data_source.py` & `nonebot-plugin-acm-reminder-0.1.7/nonebot_plugin_acm_reminder/data_source.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from json import loads
 from time import strptime, mktime
 from html import unescape
-from typing import Literal, Optional, TypedDict, List, Dict
+from typing import Literal, Optional, TypedDict, List
 from httpx import AsyncClient
 from httpx._types import URLTypes, ProxiesTypes
 from bs4 import BeautifulSoup, ResultSet
 
 class ContestType(TypedDict):
     id: int  # 竞赛ID
     name: str  # 竞赛名称
@@ -50,15 +50,18 @@
     contest_list = datatable.find_all("tr")  # type: ignore
     for contest in contest_list:
         cdata = contest.find_all("td")
         if cdata:
             cwriters = [i.string for i in cdata[1].find_all("a")] #获得主办方
             ctime = mktime(strptime(cdata[2].find("span").string, "%b/%d/%Y %H:%M")) #获得开始时间戳
             ctime+=5*60*60
-            clength = strptime(str(cdata[3].string).strip("\n").strip(), "%H:%M")
+            try:
+                clength = strptime(str(cdata[3].string).strip("\n").strip(), "%H:%M")
+            except:
+                clength = strptime(str(cdata[3].string).strip("\n").strip(), "%H:%M:%S")
             contest_data.append({"name": str(cdata[0].string).strip("\n").strip(), 
                                 "writes": cwriters, 
                                 "time": ctime, 
                                 "length": clength.tm_hour * 60 + clength.tm_min, 
                                 "platform": "Codeforces", 
                                 "id": contest.get("data-contestid")})
     return contest_data
```

### Comparing `nonebot-plugin-acm-reminder-0.1.6/pyproject.toml` & `nonebot-plugin-acm-reminder-0.1.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "nonebot_plugin_acm_reminder"
-version = "0.1.6"
+version = "0.1.7"
 description = "A subscribe CodeForces/NowCoder contest info plugin for nonebot2"
 authors = [
     { name = "BigOrangeQWQ", email = "2284086963@qq.com" },
 ]
 dependencies = [
     "BeautifulSoup4>=4.11.2",
     "nonebot2>=2.0.0b5",
```

### Comparing `nonebot-plugin-acm-reminder-0.1.6/README.md` & `nonebot-plugin-acm-reminder-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-acm-reminder-0.1.6/PKG-INFO` & `nonebot-plugin-acm-reminder-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_acm_reminder
-Version: 0.1.6
+Version: 0.1.7
 Summary: A subscribe CodeForces/NowCoder contest info plugin for nonebot2
 License: MIT
 Author-email: BigOrangeQWQ <2284086963@qq.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_acm_reminder Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_acm_reminder Version: 0.1.7 Summary:
 A subscribe CodeForces/NowCoder contest info plugin for nonebot2 License: MIT
 Author-email: BigOrangeQWQ <2284086963@qq.com> Requires-Python: >=3.8
 Description-Content-Type: text/markdown
    # ACMReminder ä¸æ¬¾å¯æ¥è¯¢ä¸è®¢éçå®¢/CFç«èµçæä»¶ [Download]
 ## å®è£ ``` pip install nonebot-plugin-acm-reminder nb plugin install
 nonebot-plugin-acm-reminder ``` ## éç½®é¡¹ *
 æåç«èµåè¡¨çæ´æ°æ¶é´(åé) ``` update_time = 720 ``` ## ç¨æ³
```


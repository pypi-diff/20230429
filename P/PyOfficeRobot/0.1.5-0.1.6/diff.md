# Comparing `tmp/PyOfficeRobot-0.1.5.tar.gz` & `tmp/PyOfficeRobot-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyOfficeRobot-0.1.5.tar", last modified: Wed Apr 26 14:22:46 2023, max compression
+gzip compressed data, was "PyOfficeRobot-0.1.6.tar", last modified: Sat Apr 29 11:49:44 2023, max compression
```

## Comparing `PyOfficeRobot-0.1.5.tar` & `PyOfficeRobot-0.1.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.685162 PyOfficeRobot-0.1.5/
--rw-rw-rw-   0        0        0     1093 2022-09-09 17:29:26.000000 PyOfficeRobot-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     7869 2023-04-26 14:22:46.686158 PyOfficeRobot-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.563447 PyOfficeRobot-0.1.5/PyOfficeRobot/
--rw-rw-rw-   0        0        0      158 2023-04-23 15:01:44.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.635623 PyOfficeRobot-0.1.5/PyOfficeRobot/api/
--rw-rw-rw-   0        0        0        0 2022-09-09 17:57:22.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/api/__init__.py
--rw-rw-rw-   0        0        0     3834 2023-03-19 10:39:04.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/api/chat.py
--rw-rw-rw-   0        0        0     6984 2023-04-17 13:43:21.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/api/file.py
--rw-rw-rw-   0        0        0     9290 2023-04-26 14:07:27.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/api/friend.py
--rw-rw-rw-   0        0        0     1625 2023-04-16 15:41:21.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/api/test.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.640628 PyOfficeRobot-0.1.5/PyOfficeRobot/core/
--rw-rw-rw-   0        0        0    13543 2023-04-18 13:17:17.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/core/WeChatType.py
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.652621 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/
--rw-rw-rw-   0        0        0      117 2023-03-19 07:06:10.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/CONST.py
--rw-rw-rw-   0        0        0        0 2022-09-12 08:16:33.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.658623 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/dec/
--rw-rw-rw-   0        0        0        0 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/dec/__init__.py
--rw-rw-rw-   0        0        0      385 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/dec/act_dec.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.670629 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/decorator_utils/
--rw-rw-rw-   0        0        0        0 2023-01-31 14:24:33.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/decorator_utils/__init__.py
--rw-rw-rw-   0        0        0     2323 2023-03-19 12:08:23.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/decorator_utils/instruction_url.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.605654 PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/
--rw-rw-rw-   0        0        0     7869 2023-04-26 14:22:46.000000 PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      756 2023-04-26 14:22:46.000000 PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 14:22:46.000000 PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-26 14:08:10.000000 PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       52 2023-04-26 14:22:46.000000 PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-26 14:22:46.000000 PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7289 2023-04-02 05:09:27.000000 PyOfficeRobot-0.1.5/README.md
--rw-rw-rw-   0        0        0      807 2023-04-26 14:22:46.689164 PyOfficeRobot-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 PyOfficeRobot-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.683161 PyOfficeRobot-0.1.5/tests/
--rw-rw-rw-   0        0        0      193 2023-02-13 13:41:39.000000 PyOfficeRobot-0.1.5/tests/__init__.py
--rw-rw-rw-   0        0        0       13 2023-04-17 13:43:22.000000 PyOfficeRobot-0.1.5/tests/chat.py
--rw-rw-rw-   0        0        0     1230 2023-04-18 13:15:33.000000 PyOfficeRobot-0.1.5/tests/test_file.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.363536 PyOfficeRobot-0.1.6/
+-rw-rw-rw-   0        0        0     1093 2022-09-09 17:29:26.000000 PyOfficeRobot-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     8068 2023-04-29 11:49:44.363536 PyOfficeRobot-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.302373 PyOfficeRobot-0.1.6/PyOfficeRobot/
+-rw-rw-rw-   0        0        0      195 2023-04-27 13:53:55.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.330943 PyOfficeRobot-0.1.6/PyOfficeRobot/api/
+-rw-rw-rw-   0        0        0        0 2022-09-09 17:57:22.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/api/__init__.py
+-rw-rw-rw-   0        0        0     3834 2023-03-19 10:39:04.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/api/chat.py
+-rw-rw-rw-   0        0        0     6984 2023-04-17 13:43:21.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/api/file.py
+-rw-rw-rw-   0        0        0     9379 2023-04-27 13:42:29.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/api/friend.py
+-rw-rw-rw-   0        0        0      640 2023-04-27 14:44:49.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/api/group.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.334940 PyOfficeRobot-0.1.6/PyOfficeRobot/core/
+-rw-rw-rw-   0        0        0    13556 2023-04-26 14:23:30.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/core/WeChatType.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.338955 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/
+-rw-rw-rw-   0        0        0      117 2023-03-19 07:06:10.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/CONST.py
+-rw-rw-rw-   0        0        0        0 2022-09-12 08:16:33.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.345495 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/dec/
+-rw-rw-rw-   0        0        0        0 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/dec/__init__.py
+-rw-rw-rw-   0        0        0      385 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/dec/act_dec.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.352013 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/decorator_utils/
+-rw-rw-rw-   0        0        0        0 2023-01-31 14:24:33.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/decorator_utils/__init__.py
+-rw-rw-rw-   0        0        0     2413 2023-04-27 13:42:29.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/decorator_utils/instruction_url.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.317888 PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/
+-rw-rw-rw-   0        0        0     8068 2023-04-29 11:49:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      757 2023-04-29 11:49:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:49:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-27 13:31:57.000000 PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       77 2023-04-29 11:49:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-29 11:49:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7488 2023-04-26 16:01:49.000000 PyOfficeRobot-0.1.6/README.md
+-rw-rw-rw-   0        0        0      838 2023-04-29 11:49:44.365540 PyOfficeRobot-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 PyOfficeRobot-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.360013 PyOfficeRobot-0.1.6/tests/
+-rw-rw-rw-   0        0        0      193 2023-02-13 13:41:39.000000 PyOfficeRobot-0.1.6/tests/__init__.py
+-rw-rw-rw-   0        0        0       13 2023-04-17 13:43:22.000000 PyOfficeRobot-0.1.6/tests/chat.py
+-rw-rw-rw-   0        0        0     1230 2023-04-18 13:15:33.000000 PyOfficeRobot-0.1.6/tests/test_file.py
```

### Comparing `PyOfficeRobot-0.1.5/LICENSE` & `PyOfficeRobot-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.5/PKG-INFO` & `PyOfficeRobot-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOfficeRobot
-Version: 0.1.5
+Version: 0.1.6
 Summary: pip install PyOfficeRobot
 Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/README.md
@@ -79,16 +79,16 @@
 | 003-自动发文件 | [点我直达](https://www.bilibili.com/video/BV1te4y1y7Ro)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/003-file.py)     |
 | 004-根据关键词，自动回复 | [点我直达](https://www.bilibili.com/video/BV1fV4y1M7ju)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/004-%E6%A0%B9%E6%8D%AE%E5%85%B3%E9%94%AE%E8%AF%8D%E5%9B%9E%E5%A4%8D.py)     |
 | ⌚005-定时自动发消息 | [点我直达](https://www.bilibili.com/video/BV1m8411b7LZ/)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/06-%E5%AE%9A%E6%97%B6.py)     |
 | 006-自己加功能 | [点我直达](https://www.bilibili.com/video/BV14R4y127h6)     |     |
 | ⭐007-独立使用 | [点我直达](https://www.bilibili.com/video/BV1SY411y7Uh)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot)     |
 | 08-收集群信息 | [点我直达](https://www.bilibili.com/video/BV1eD4y1g7yZ)     |[点我直达](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw)     |
 | 09-发消息如何换行？ | [点我直达](https://www.bilibili.com/video/BV1Xg4y1s79z/)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/08-new_line.py)     |
-| 10-微信 + ChatGPT | [点我直达](http://xhslink.com/zXZAeo)     |[点我直达](https://blog.51cto.com/u_15493782/6131326)     |
-
+| 特别篇-微信 + ChatGPT | [点我直达](http://xhslink.com/zXZAeo)     |[点我直达](https://blog.51cto.com/u_15493782/6131326)     |
+| 10-批量加好友 | [点我直达](https://www.bilibili.com/video/BV1DV4y1o7t2)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py)     |
 > 持续更新中，交流群：[点我加入](http://www.python4office.cn/wechat-group/)
 #### 微信机器人-其它实现方式
 
 
 | 功能说明       | 视频 |代码 |
 | -------------- | -------- |-------- |
 | 机器人.exe | [点我直达](https://www.bilibili.com/video/BV1Q64y1Z7TB/)     |     |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.5 Summary: pip install
+Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.6 Summary: pip install
 PyOfficeRobot Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL:
 Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
 Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/
 README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 PyOfficeRobot Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
@@ -42,17 +42,20 @@
 [ç¹æç´è¾¾](https://www.bilibili.com/video/BV14R4y127h6) | | | â­007-
 ç¬ç«ä½¿ç¨ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1SY411y7Uh) |
 [ç¹æç´è¾¾](https://github.com/CoderWanFeng/PyOfficeRobot) | | 08-
 æ¶éç¾¤ä¿¡æ¯ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1eD4y1g7yZ) |
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw) | | 09-
 åæ¶æ¯å¦ä½æ¢è¡ï¼ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
 BV1Xg4y1s79z/) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/PyOfficeRobot/
-blob/main/demo/08-new_line.py) | | 10-å¾®ä¿¡ + ChatGPT | [ç¹æç´è¾¾](http://
-xhslink.com/zXZAeo) |[ç¹æç´è¾¾](https://blog.51cto.com/u_15493782/6131326)
-| > æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥](http://www.python4office.cn/
+blob/main/demo/08-new_line.py) | | ç¹å«ç¯-å¾®ä¿¡ + ChatGPT | [ç¹æç´è¾¾]
+(http://xhslink.com/zXZAeo) |[ç¹æç´è¾¾](https://blog.51cto.com/u_15493782/
+6131326) | | 10-æ¹éå å¥½å | [ç¹æç´è¾¾](https://www.bilibili.com/
+video/BV1DV4y1o7t2) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/
+PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py) | >
+æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥](http://www.python4office.cn/
 wechat-group/) #### å¾®ä¿¡æºå¨äºº-å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢
 |ä»£ç  | | -------------- | -------- |-------- | | æºå¨äºº.exe |
 [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Q64y1Z7TB/) | | |
 ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Dx4y157qy) |
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-
 24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
 BV11L411L7oi/) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
```

### Comparing `PyOfficeRobot-0.1.5/PyOfficeRobot/api/chat.py` & `PyOfficeRobot-0.1.6/PyOfficeRobot/api/chat.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.5/PyOfficeRobot/api/file.py` & `PyOfficeRobot-0.1.6/PyOfficeRobot/api/file.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.5/PyOfficeRobot/api/friend.py` & `PyOfficeRobot-0.1.6/PyOfficeRobot/api/friend.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 from pywinauto.application import *
 from pywinauto.base_wrapper import *
 from pywinauto.controls.uiawrapper import UIAWrapper
 from pywinauto.keyboard import send_keys
 from pywinauto.uia_element_info import UIAElementInfo
 
+from PyOfficeRobot.lib.decorator_utils.instruction_url import instruction
+
 
 def Carry_TXL(App_Object, Hello_Str, Tel_Number, notes):
     """
     该函数为申请好友验证时的函数胡\n
     :param App_Object: 微信窗口操作对象
     :param Hello_Str: 打招呼的字符串
     :param Tel_Number: 备注名,用于备注该用户的手机号码
@@ -158,15 +160,15 @@
     Button_EXE_Wrapper.click_input()
     sleep(0.5)
     Button_TXL_Wrapper.draw_outline(colour="red", thickness=5)
     Button_TXL_Wrapper.click_input()
     sleep(0.5)
     # </editor-fold>
 
-
+@instruction
 def add(num_notes, msg):
     # <editor-fold desc="代码块 : 获取微信窗口句柄">
     Get_WeChat_Hwnd = lambda: win32gui.FindWindow("WeChatMainWndForPC", "微信")
     WeChat_Hwnd = Get_WeChat_Hwnd()
     # </editor-fold>
 
     # <editor-fold desc="代码块 : 设置窗口状态以及位置">
```

### Comparing `PyOfficeRobot-0.1.5/PyOfficeRobot/core/WeChatType.py` & `PyOfficeRobot-0.1.6/PyOfficeRobot/core/WeChatType.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import os
 import time
 from ctypes import *
 from pathlib import Path
 
 import uiautomation as uia
-import win32clipboard
+import win32clipboard  # pywin32
 import win32clipboard as wc
 import win32con
 import win32gui
 
 PUBLISH_ID = '公众号：程序员晚枫'
 
 COPYDICT = {}
@@ -308,14 +308,15 @@
 
     def test_SendFiles(self, filepath, not_exists='ignore'):
         """向当前聊天窗口发送文件
         not_exists: 如果未找到指定文件，继续或终止程序
         filepath: 要复制文件的绝对路径"""
         if not Path(filepath).exists():
             raise BaseException(f'你指定的文件不存在，请检查filepath后，重新运行：{filepath}')
+
         class DROPFILES(Structure):
             _fields_ = [
                 ("pFiles", c_uint),
                 ("x", c_long),
                 ("y", c_long),
                 ("fNC", c_int),
                 ("fWide", c_bool),
```

### Comparing `PyOfficeRobot-0.1.5/PyOfficeRobot/lib/decorator_utils/instruction_url.py` & `PyOfficeRobot-0.1.6/PyOfficeRobot/lib/decorator_utils/instruction_url.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,38 +4,41 @@
 #############################################
 # File Name: instruction_url.py
 # Mail: 1957875073@qq.com
 # Created Time:  2022-12-17 08:14:34
 # Description: 有关 方法说明 的装饰器
 #############################################
 
+import os
 # 每个文件的具体方法说明
 from functools import wraps
 
-
-import os
-
 from PyOfficeRobot.lib.CONST import SPLIT_LINE
 
 chat_dict = {"chat_by_keywords": "https://www.bilibili.com/video/BV1fV4y1M7ju",
-               "receive_message": "",
-               "send_message": "https://www.bilibili.com/video/BV1Jt4y1j7F1",
-               "send_message_by_time": "https://www.bilibili.com/video/BV1m8411b7LZ",
-               "chat_by_gpt": "https://blog.51cto.com/u_15493782/6131326",
-}
+             "receive_message": "",
+             "send_message": "https://www.bilibili.com/video/BV1Jt4y1j7F1",
+             "send_message_by_time": "https://www.bilibili.com/video/BV1m8411b7LZ",
+             "chat_by_gpt": "https://blog.51cto.com/u_15493782/6131326",
+             }
 file_dict = {
     "send_file": "https://www.bilibili.com/video/BV1te4y1y7Ro",
 
 }
 
+friend_dict = {
+    "add": "https://www.bilibili.com/video/BV1DV4y1o7t2",
+
+}
 
 # 有多少文件需要说明
 instruction_file_dict = {
     "chat.py": chat_dict,
     "file.py": file_dict,
+    "friend.py": friend_dict,
 }
 
 
 def instruction(func):
     @wraps(func)
     def instruction_wrapper(*args, **kwargs):
         func_filename = os.path.basename(func.__code__.co_filename)  # 取出方法所在的文件名
@@ -51,17 +54,15 @@
         return instruction_res
 
     return instruction_wrapper
 
 
 #############################################
 # 以下是本文件的工具模块，用来更新方法和链接
-from inspect import getmembers, isfunction, ismethod, isclass
+from inspect import getmembers, isfunction
 
 
 # 获取模块包含的方法名
 def get_method_name(file):
     for method_name in getmembers(file):
         if isfunction(method_name[1]):
             print(f'"{method_name[0]}":"",')
-
-
```

### Comparing `PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/PKG-INFO` & `PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOfficeRobot
-Version: 0.1.5
+Version: 0.1.6
 Summary: pip install PyOfficeRobot
 Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/README.md
@@ -79,16 +79,16 @@
 | 003-自动发文件 | [点我直达](https://www.bilibili.com/video/BV1te4y1y7Ro)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/003-file.py)     |
 | 004-根据关键词，自动回复 | [点我直达](https://www.bilibili.com/video/BV1fV4y1M7ju)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/004-%E6%A0%B9%E6%8D%AE%E5%85%B3%E9%94%AE%E8%AF%8D%E5%9B%9E%E5%A4%8D.py)     |
 | ⌚005-定时自动发消息 | [点我直达](https://www.bilibili.com/video/BV1m8411b7LZ/)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/06-%E5%AE%9A%E6%97%B6.py)     |
 | 006-自己加功能 | [点我直达](https://www.bilibili.com/video/BV14R4y127h6)     |     |
 | ⭐007-独立使用 | [点我直达](https://www.bilibili.com/video/BV1SY411y7Uh)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot)     |
 | 08-收集群信息 | [点我直达](https://www.bilibili.com/video/BV1eD4y1g7yZ)     |[点我直达](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw)     |
 | 09-发消息如何换行？ | [点我直达](https://www.bilibili.com/video/BV1Xg4y1s79z/)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/08-new_line.py)     |
-| 10-微信 + ChatGPT | [点我直达](http://xhslink.com/zXZAeo)     |[点我直达](https://blog.51cto.com/u_15493782/6131326)     |
-
+| 特别篇-微信 + ChatGPT | [点我直达](http://xhslink.com/zXZAeo)     |[点我直达](https://blog.51cto.com/u_15493782/6131326)     |
+| 10-批量加好友 | [点我直达](https://www.bilibili.com/video/BV1DV4y1o7t2)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py)     |
 > 持续更新中，交流群：[点我加入](http://www.python4office.cn/wechat-group/)
 #### 微信机器人-其它实现方式
 
 
 | 功能说明       | 视频 |代码 |
 | -------------- | -------- |-------- |
 | 机器人.exe | [点我直达](https://www.bilibili.com/video/BV1Q64y1Z7TB/)     |     |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.5 Summary: pip install
+Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.6 Summary: pip install
 PyOfficeRobot Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL:
 Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
 Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/
 README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 PyOfficeRobot Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
@@ -42,17 +42,20 @@
 [ç¹æç´è¾¾](https://www.bilibili.com/video/BV14R4y127h6) | | | â­007-
 ç¬ç«ä½¿ç¨ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1SY411y7Uh) |
 [ç¹æç´è¾¾](https://github.com/CoderWanFeng/PyOfficeRobot) | | 08-
 æ¶éç¾¤ä¿¡æ¯ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1eD4y1g7yZ) |
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw) | | 09-
 åæ¶æ¯å¦ä½æ¢è¡ï¼ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
 BV1Xg4y1s79z/) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/PyOfficeRobot/
-blob/main/demo/08-new_line.py) | | 10-å¾®ä¿¡ + ChatGPT | [ç¹æç´è¾¾](http://
-xhslink.com/zXZAeo) |[ç¹æç´è¾¾](https://blog.51cto.com/u_15493782/6131326)
-| > æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥](http://www.python4office.cn/
+blob/main/demo/08-new_line.py) | | ç¹å«ç¯-å¾®ä¿¡ + ChatGPT | [ç¹æç´è¾¾]
+(http://xhslink.com/zXZAeo) |[ç¹æç´è¾¾](https://blog.51cto.com/u_15493782/
+6131326) | | 10-æ¹éå å¥½å | [ç¹æç´è¾¾](https://www.bilibili.com/
+video/BV1DV4y1o7t2) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/
+PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py) | >
+æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥](http://www.python4office.cn/
 wechat-group/) #### å¾®ä¿¡æºå¨äºº-å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢
 |ä»£ç  | | -------------- | -------- |-------- | | æºå¨äºº.exe |
 [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Q64y1Z7TB/) | | |
 ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Dx4y157qy) |
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-
 24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
 BV11L411L7oi/) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
```

### Comparing `PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/SOURCES.txt` & `PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 PyOfficeRobot.egg-info/not-zip-safe
 PyOfficeRobot.egg-info/requires.txt
 PyOfficeRobot.egg-info/top_level.txt
 PyOfficeRobot/api/__init__.py
 PyOfficeRobot/api/chat.py
 PyOfficeRobot/api/file.py
 PyOfficeRobot/api/friend.py
-PyOfficeRobot/api/test.py
+PyOfficeRobot/api/group.py
 PyOfficeRobot/core/WeChatType.py
 PyOfficeRobot/core/__init__.py
 PyOfficeRobot/lib/CONST.py
 PyOfficeRobot/lib/__init__.py
 PyOfficeRobot/lib/dec/__init__.py
 PyOfficeRobot/lib/dec/act_dec.py
 PyOfficeRobot/lib/decorator_utils/__init__.py
```

### Comparing `PyOfficeRobot-0.1.5/README.md` & `PyOfficeRobot-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 | 003-自动发文件 | [点我直达](https://www.bilibili.com/video/BV1te4y1y7Ro)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/003-file.py)     |
 | 004-根据关键词，自动回复 | [点我直达](https://www.bilibili.com/video/BV1fV4y1M7ju)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/004-%E6%A0%B9%E6%8D%AE%E5%85%B3%E9%94%AE%E8%AF%8D%E5%9B%9E%E5%A4%8D.py)     |
 | ⌚005-定时自动发消息 | [点我直达](https://www.bilibili.com/video/BV1m8411b7LZ/)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/06-%E5%AE%9A%E6%97%B6.py)     |
 | 006-自己加功能 | [点我直达](https://www.bilibili.com/video/BV14R4y127h6)     |     |
 | ⭐007-独立使用 | [点我直达](https://www.bilibili.com/video/BV1SY411y7Uh)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot)     |
 | 08-收集群信息 | [点我直达](https://www.bilibili.com/video/BV1eD4y1g7yZ)     |[点我直达](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw)     |
 | 09-发消息如何换行？ | [点我直达](https://www.bilibili.com/video/BV1Xg4y1s79z/)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/08-new_line.py)     |
-| 10-微信 + ChatGPT | [点我直达](http://xhslink.com/zXZAeo)     |[点我直达](https://blog.51cto.com/u_15493782/6131326)     |
-
+| 特别篇-微信 + ChatGPT | [点我直达](http://xhslink.com/zXZAeo)     |[点我直达](https://blog.51cto.com/u_15493782/6131326)     |
+| 10-批量加好友 | [点我直达](https://www.bilibili.com/video/BV1DV4y1o7t2)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py)     |
 > 持续更新中，交流群：[点我加入](http://www.python4office.cn/wechat-group/)
 #### 微信机器人-其它实现方式
 
 
 | 功能说明       | 视频 |代码 |
 | -------------- | -------- |-------- |
 | 机器人.exe | [点我直达](https://www.bilibili.com/video/BV1Q64y1Z7TB/)     |     |
```

#### html2text {}

```diff
@@ -34,17 +34,20 @@
 [ç¹æç´è¾¾](https://www.bilibili.com/video/BV14R4y127h6) | | | â­007-
 ç¬ç«ä½¿ç¨ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1SY411y7Uh) |
 [ç¹æç´è¾¾](https://github.com/CoderWanFeng/PyOfficeRobot) | | 08-
 æ¶éç¾¤ä¿¡æ¯ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1eD4y1g7yZ) |
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw) | | 09-
 åæ¶æ¯å¦ä½æ¢è¡ï¼ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
 BV1Xg4y1s79z/) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/PyOfficeRobot/
-blob/main/demo/08-new_line.py) | | 10-å¾®ä¿¡ + ChatGPT | [ç¹æç´è¾¾](http://
-xhslink.com/zXZAeo) |[ç¹æç´è¾¾](https://blog.51cto.com/u_15493782/6131326)
-| > æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥](http://www.python4office.cn/
+blob/main/demo/08-new_line.py) | | ç¹å«ç¯-å¾®ä¿¡ + ChatGPT | [ç¹æç´è¾¾]
+(http://xhslink.com/zXZAeo) |[ç¹æç´è¾¾](https://blog.51cto.com/u_15493782/
+6131326) | | 10-æ¹éå å¥½å | [ç¹æç´è¾¾](https://www.bilibili.com/
+video/BV1DV4y1o7t2) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/
+PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py) | >
+æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥](http://www.python4office.cn/
 wechat-group/) #### å¾®ä¿¡æºå¨äºº-å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢
 |ä»£ç  | | -------------- | -------- |-------- | | æºå¨äºº.exe |
 [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Q64y1Z7TB/) | | |
 ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Dx4y157qy) |
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-
 24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
 BV11L411L7oi/) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
```

### Comparing `PyOfficeRobot-0.1.5/setup.cfg` & `PyOfficeRobot-0.1.6/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 794f 6666 6963 6552 6f62 6f74   = PyOfficeRobot
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 312e  ..version = 0.1.
-00000030: 350d 0a64 6573 6372 6970 7469 6f6e 203d  5..description =
+00000030: 360d 0a64 6573 6372 6970 7469 6f6e 203d  6..description =
 00000040: 2070 6970 2069 6e73 7461 6c6c 2050 794f   pip install PyO
 00000050: 6666 6963 6552 6f62 6f74 0d0a 6c6f 6e67  fficeRobot..long
 00000060: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000070: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000080: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000090: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 000000a0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
@@ -37,15 +37,17 @@
 00000240: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
 00000250: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
 00000260: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
 00000270: 200d 0a09 7569 6175 746f 6d61 7469 6f6e   ...uiautomation
 00000280: 0d0a 0973 6368 6564 756c 650d 0a09 7061  ...schedule...pa
 00000290: 6e64 6173 0d0a 0970 6f61 690d 0a09 7079  ndas...poai...py
 000002a0: 7769 6e33 320d 0a09 7079 7769 6e61 7574  win32...pywinaut
-000002b0: 6f0d 0a70 7974 686f 6e5f 7265 7175 6972  o..python_requir
-000002c0: 6573 203d 203e 3d33 2e36 0d0a 696e 636c  es = >=3.6..incl
-000002d0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
-000002e0: 203d 2054 7275 650d 0a7a 6970 5f73 6166   = True..zip_saf
-000002f0: 6520 3d20 4661 6c73 650d 0a0d 0a5b 6567  e = False....[eg
-00000300: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000310: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000320: 3d20 300d 0a0d 0a                        = 0....
+000002b0: 6f0d 0a09 786c 7774 0d0a 0978 6c72 643d  o...xlwt...xlrd=
+000002c0: 3d31 2e32 2e30 0d0a 0950 7953 6964 6536  =1.2.0...PySide6
+000002d0: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+000002e0: 7320 3d20 3e3d 332e 360d 0a69 6e63 6c75  s = >=3.6..inclu
+000002f0: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+00000300: 3d20 5472 7565 0d0a 7a69 705f 7361 6665  = True..zip_safe
+00000310: 203d 2046 616c 7365 0d0a 0d0a 5b65 6767   = False....[egg
+00000320: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000330: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000340: 2030 0d0a 0d0a                            0....
```

### Comparing `PyOfficeRobot-0.1.5/tests/test_file.py` & `PyOfficeRobot-0.1.6/tests/test_file.py`

 * *Files identical despite different names*


# Comparing `tmp/nonebot_plugin_todo_nlp-0.1.8rc0.tar.gz` & `tmp/nonebot_plugin_todo_nlp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_todo_nlp-0.1.8rc0.tar", max compression
+gzip compressed data, was "nonebot_plugin_todo_nlp-0.1.9.tar", max compression
```

## Comparing `nonebot_plugin_todo_nlp-0.1.8rc0.tar` & `nonebot_plugin_todo_nlp-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rwxr-xr-x   0        0        0     1084 2022-08-29 04:11:48.116493 nonebot_plugin_todo_nlp-0.1.8rc0/LICENSE
--rwxr-xr-x   0        0        0      126 2022-09-04 08:49:07.240906 nonebot_plugin_todo_nlp-0.1.8rc0/nonebot_plugin_todo_nlp/__init__.py
--rwxr-xr-x   0        0        0      588 2022-09-04 09:09:53.203259 nonebot_plugin_todo_nlp-0.1.8rc0/nonebot_plugin_todo_nlp/config.py
--rwxr-xr-x   0        0        0     1817 2023-02-13 16:18:44.725991 nonebot_plugin_todo_nlp-0.1.8rc0/nonebot_plugin_todo_nlp/nlp_util.py
--rwxr-xr-x   0        0        0     1615 2022-08-21 10:57:23.494000 nonebot_plugin_todo_nlp-0.1.8rc0/nonebot_plugin_todo_nlp/templates/css/style.css
--rwxr-xr-x   0        0        0      987 2022-08-21 14:52:38.392885 nonebot_plugin_todo_nlp-0.1.8rc0/nonebot_plugin_todo_nlp/templates/template.html
--rwxr-xr-x   0        0        0     8647 2022-09-04 08:57:01.412915 nonebot_plugin_todo_nlp-0.1.8rc0/nonebot_plugin_todo_nlp/todo.py
--rwxr-xr-x   0        0        0     5992 2022-09-04 08:50:23.922673 nonebot_plugin_todo_nlp-0.1.8rc0/nonebot_plugin_todo_nlp/todo_manage.py
--rwxr-xr-x   0        0        0      614 2023-02-13 16:19:36.320117 nonebot_plugin_todo_nlp-0.1.8rc0/pyproject.toml
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 nonebot_plugin_todo_nlp-0.1.8rc0/setup.py
--rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 nonebot_plugin_todo_nlp-0.1.8rc0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-29 15:29:34.616368 nonebot_plugin_todo_nlp-0.1.9/LICENSE
+-rw-r--r--   0        0        0      124 2023-04-29 11:42:46.097261 nonebot_plugin_todo_nlp-0.1.9/nonebot_plugin_todo_nlp/__init__.py
+-rw-r--r--   0        0        0      597 2023-04-29 13:24:05.548862 nonebot_plugin_todo_nlp-0.1.9/nonebot_plugin_todo_nlp/config.py
+-rw-r--r--   0        0        0     3911 2023-04-29 13:24:00.251862 nonebot_plugin_todo_nlp-0.1.9/nonebot_plugin_todo_nlp/nlp_util.py
+-rw-r--r--   0        0        0     1531 2023-04-29 11:42:46.098261 nonebot_plugin_todo_nlp-0.1.9/nonebot_plugin_todo_nlp/templates/css/style.css
+-rw-r--r--   0        0        0      954 2023-04-29 11:42:46.098261 nonebot_plugin_todo_nlp-0.1.9/nonebot_plugin_todo_nlp/templates/template.html
+-rw-r--r--   0        0        0     8396 2023-04-29 11:42:46.098261 nonebot_plugin_todo_nlp-0.1.9/nonebot_plugin_todo_nlp/todo.py
+-rw-r--r--   0        0        0     5856 2023-04-29 11:42:46.098261 nonebot_plugin_todo_nlp-0.1.9/nonebot_plugin_todo_nlp/todo_manage.py
+-rw-r--r--   0        0        0      609 2023-04-29 15:30:28.042364 nonebot_plugin_todo_nlp-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 nonebot_plugin_todo_nlp-0.1.9/PKG-INFO
```

### Comparing `nonebot_plugin_todo_nlp-0.1.8rc0/LICENSE` & `nonebot_plugin_todo_nlp-0.1.9/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 CofinCup
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2022 CofinCup
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `nonebot_plugin_todo_nlp-0.1.8rc0/nonebot_plugin_todo_nlp/templates/css/style.css` & `nonebot_plugin_todo_nlp-0.1.9/nonebot_plugin_todo_nlp/templates/css/style.css`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-html,
-body {
-    margin: 0;
-    padding: 0;
-    font-family: sans-serif;
-}
-* {box-sizing: border-box;}
-html,body,div,ul,ol,li,span,p,a,b,i,h1,h2,h3,img,input,select,textarea,button{margin:0;padding:0;border:0}
-ul,ol,li{list-style:none;}
-
-main {
-    display: flex;
-    align-items: center;
-    height: 100vh;
-    justify-content: center;
-    background-color: #1e272e;
-}
-
-.task_tit{
-	width:180px;
-	font-size: 20px;
-	color: #d2dae2;
-	padding-bottom: 22px;	
-	position: relative;
-}
-.task_tit::after{
-	content: '';
-	position: absolute;
-	bottom: 0;
-	left: 0;
-	width: 90%;
-	height: 1px;
-	background-image: linear-gradient(to right, #d2dae2 0%, #d2dae2 50%, transparent 50%);
-	background-size: 8px 1px;
-	background-repeat: repeat-x;
-	margin: 0 auto;
-}
-
-.task_con {
-    width: 500px;
-	margin-top: 28px;
-}
-.task_con .task_con_li{
-	margin-bottom: 38px;
-}
-.task_con .task_con_li .date{
-	font-size: 18px;
-	color: #d2dae2;
-}
-.task_con_li ul{
-	margin-top: 10px;
-}
-.task_con_li li {    
-    color: #d2dae2;
-    font-size: 16px;
-    margin: 0 0 18px;
-}
-
-.task_con_li li .process{
-    width: 100%;
-    display: block;
-    height: 16px;
-    background-color: #1f4a59;
-    position: relative;
-    border-radius: 6px;
-	position: relative;
-	margin-top: 10px;
-}
-
-.task_con_li li::before{
-    box-shadow: 0 0 6px rgba(75,207,250,0.2)
-}
-
-.task_con_li li span{
-    position: absolute;
-    bottom: 0;
-    height: 16px;
-    border-radius: 6px;
-    display: block;
-    background-image: linear-gradient(
-        90deg,
-        #0fbcf9,
-        #34e7e4
-    );
+html,
+body {
+    margin: 0;
+    padding: 0;
+    font-family: sans-serif;
+}
+* {box-sizing: border-box;}
+html,body,div,ul,ol,li,span,p,a,b,i,h1,h2,h3,img,input,select,textarea,button{margin:0;padding:0;border:0}
+ul,ol,li{list-style:none;}
+
+main {
+    display: flex;
+    align-items: center;
+    height: 100vh;
+    justify-content: center;
+    background-color: #1e272e;
+}
+
+.task_tit{
+	width:180px;
+	font-size: 20px;
+	color: #d2dae2;
+	padding-bottom: 22px;	
+	position: relative;
+}
+.task_tit::after{
+	content: '';
+	position: absolute;
+	bottom: 0;
+	left: 0;
+	width: 90%;
+	height: 1px;
+	background-image: linear-gradient(to right, #d2dae2 0%, #d2dae2 50%, transparent 50%);
+	background-size: 8px 1px;
+	background-repeat: repeat-x;
+	margin: 0 auto;
+}
+
+.task_con {
+    width: 500px;
+	margin-top: 28px;
+}
+.task_con .task_con_li{
+	margin-bottom: 38px;
+}
+.task_con .task_con_li .date{
+	font-size: 18px;
+	color: #d2dae2;
+}
+.task_con_li ul{
+	margin-top: 10px;
+}
+.task_con_li li {    
+    color: #d2dae2;
+    font-size: 16px;
+    margin: 0 0 18px;
+}
+
+.task_con_li li .process{
+    width: 100%;
+    display: block;
+    height: 16px;
+    background-color: #1f4a59;
+    position: relative;
+    border-radius: 6px;
+	position: relative;
+	margin-top: 10px;
+}
+
+.task_con_li li::before{
+    box-shadow: 0 0 6px rgba(75,207,250,0.2)
+}
+
+.task_con_li li span{
+    position: absolute;
+    bottom: 0;
+    height: 16px;
+    border-radius: 6px;
+    display: block;
+    background-image: linear-gradient(
+        90deg,
+        #0fbcf9,
+        #34e7e4
+    );
 }
```

### Comparing `nonebot_plugin_todo_nlp-0.1.8rc0/nonebot_plugin_todo_nlp/todo_manage.py` & `nonebot_plugin_todo_nlp-0.1.9/nonebot_plugin_todo_nlp/todo_manage.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-from datetime import datetime
-from typing import Union, AnyStr, List
-import nonebot
-from nonebot import on_keyword
-from nonebot import require
-from nonebot.adapters.onebot.v11 import MessageSegment, PrivateMessageEvent, GroupMessageEvent
-from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER, PRIVATE_FRIEND
-import time
-
-from .nlp_util import get_time_from_text, get_name_from_text, get_priority_from_text
-from .todo import TodoToken, TodoUtil
-from .config import Config
-
-global_config = nonebot.get_driver().config
-plugin_config = Config(**global_config.dict())
-
-add_todo = on_keyword({'提醒', 'nonebot_todo'}, permission=GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND)
-remove_todo = on_keyword({'删除', '去掉'}, permission=GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND)
-finish_todo = on_keyword({'完成'}, permission=GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND)
-change_todo_time = on_keyword({'更正', '改'}, permission=GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND)
-get_todo_pic = on_keyword({'获取todo'}, permission=GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND)
-scheduler = require("nonebot_plugin_apscheduler").scheduler
-
-
-@add_todo.handle()
-async def add_todo_handle(event: Union[PrivateMessageEvent, GroupMessageEvent]):
-    text: str = event.raw_message
-    exceed_time, time_valid, time_error_doc = get_time_from_text(text)
-    name, name_valid, name_error_doc = get_name_from_text(text)
-    priority, priority_valid, priority_error_doc = get_priority_from_text(text)
-    if not time_valid:
-        await add_todo.finish(time_error_doc)
-    elif not name_valid:
-        await add_todo.finish(name_error_doc)
-    elif not priority_valid:
-        await add_todo.finish(priority_error_doc)
-    if isinstance(event, PrivateMessageEvent):
-        todo_util = TodoUtil(str(event.user_id))
-    else:
-        todo_util = TodoUtil(str(event.group_id))
-    todo_token = TodoToken(name, datetime.today(), exceed_time, priority)
-    if todo_util.add_data_to_list(todo_token):
-        await add_todo.send(f"已将{name}加入清单，ddl为{exceed_time}，优先级为{priority}。\n当前共{todo_util.list_size}项待办。")
-        img = await todo_util.get_list_img()
-        await remove_todo.finish(MessageSegment.image(img))
-    else:
-        await add_todo.finish(f"{name}已在清单中。")
-
-
-@remove_todo.handle()
-async def remove_todo_handle(event: Union[PrivateMessageEvent, GroupMessageEvent]):
-    text: str = event.raw_message
-    name, name_valid, name_error_doc = get_name_from_text(text)
-    if isinstance(event, PrivateMessageEvent):
-        todo_util = TodoUtil(str(event.user_id))
-    else:
-        todo_util = TodoUtil(str(event.group_id))
-    if not name_valid:
-        await remove_todo.finish(name_error_doc)
-    elif todo_util.remove_data(name) == 0:
-        await remove_todo.finish(f"不存在名为{name}的表项。")
-    else:
-        img = await todo_util.get_list_img()
-        await remove_todo.send(f"已删除{name}。")
-        await remove_todo.finish(MessageSegment.image(img))
-
-
-@finish_todo.handle()
-async def finish_todo_handle(event: Union[PrivateMessageEvent, GroupMessageEvent]):
-    text: str = event.raw_message
-    name, name_valid, name_error_doc = get_name_from_text(text)
-    if isinstance(event, PrivateMessageEvent):
-        todo_util = TodoUtil(str(event.user_id))
-    else:
-        todo_util = TodoUtil(str(event.group_id))
-    if not name_valid:
-        await remove_todo.finish(name_error_doc)
-    elif todo_util.finish_job(name) == 0:
-        await remove_todo.finish(f"不存在名为{name}的表项。")
-    else:
-        await remove_todo.send(f"已完成{name}。还剩{todo_util.list_size}项。")
-        img = await todo_util.get_list_img()
-        await remove_todo.finish(MessageSegment.image(img))
-
-
-@change_todo_time.handle()
-async def change_todo_time_handle(event: Union[PrivateMessageEvent, GroupMessageEvent]):
-    text: str = event.raw_message
-    name, name_valid, name_error_doc = get_name_from_text(text)
-    expire_time, time_valid, time_error_doc = get_time_from_text(text)
-    if isinstance(event, PrivateMessageEvent):
-        todo_util = TodoUtil(str(event.user_id))
-    else:
-        todo_util = TodoUtil(str(event.group_id))
-    if not time_valid:
-        await add_todo.finish(time_error_doc)
-    elif not name_valid:
-        await add_todo.finish(name_error_doc)
-    else:
-        changed_count = todo_util.change_time(name, expire_time)
-        if not changed_count == 0:
-            await change_todo_time.send(f"将{name}改至{expire_time}")
-            img = await todo_util.get_list_img()
-            await change_todo_time.finish(MessageSegment.image(img))
-        else:
-            await change_todo_time.finish(f"没有名为{name}的项目。")
-
-
-@get_todo_pic.handle()
-async def _handle(event: Union[PrivateMessageEvent, GroupMessageEvent]):
-    if isinstance(event, PrivateMessageEvent):
-        todo_util = TodoUtil(str(event.user_id))
-    else:
-        todo_util = TodoUtil(str(event.group_id))
-    img = await todo_util.get_list_img()
-    await get_todo_pic.finish(MessageSegment.image(img))
-
-
-async def send_todo():
-    for user in plugin_config.todo_users:
-        todo_util = TodoUtil(str(user))
-        img = await todo_util.get_list_img()
-        await nonebot.get_bot().send_private_msg(user_id=user, message=MessageSegment.image(img))
-        time.sleep(5)
-        # 防止风控
-
-    for group in plugin_config.todo_groups:
-        todo_util = TodoUtil(str(group))
-        img = await todo_util.get_list_img()
-        await nonebot.get_bot().send_group_msg(group_id=group, message=MessageSegment.image(img))
-        time.sleep(5)
-        # 防止风控
-
-
-for index, _time in enumerate(plugin_config.todo_send_time):
-    scheduler.add_job(send_todo, "cron", hour=_time.hour, minute=_time.minute, id=str(f"send_todo_for_{index}"))
+from datetime import datetime
+from typing import Union, AnyStr, List
+import nonebot
+from nonebot import on_keyword
+from nonebot import require
+from nonebot.adapters.onebot.v11 import MessageSegment, PrivateMessageEvent, GroupMessageEvent
+from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER, PRIVATE_FRIEND
+import time
+
+from .nlp_util import get_time_from_text, get_name_from_text, get_priority_from_text
+from .todo import TodoToken, TodoUtil
+from .config import Config
+
+global_config = nonebot.get_driver().config
+plugin_config = Config(**global_config.dict())
+
+add_todo = on_keyword({'提醒', 'nonebot_todo'}, permission=GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND)
+remove_todo = on_keyword({'删除', '去掉'}, permission=GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND)
+finish_todo = on_keyword({'完成'}, permission=GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND)
+change_todo_time = on_keyword({'更正', '改'}, permission=GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND)
+get_todo_pic = on_keyword({'获取todo'}, permission=GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND)
+scheduler = require("nonebot_plugin_apscheduler").scheduler
+
+
+@add_todo.handle()
+async def add_todo_handle(event: Union[PrivateMessageEvent, GroupMessageEvent]):
+    text: str = event.raw_message
+    exceed_time, time_valid, time_error_doc = get_time_from_text(text)
+    name, name_valid, name_error_doc = get_name_from_text(text)
+    priority, priority_valid, priority_error_doc = get_priority_from_text(text)
+    if not time_valid:
+        await add_todo.finish(time_error_doc)
+    elif not name_valid:
+        await add_todo.finish(name_error_doc)
+    elif not priority_valid:
+        await add_todo.finish(priority_error_doc)
+    if isinstance(event, PrivateMessageEvent):
+        todo_util = TodoUtil(str(event.user_id))
+    else:
+        todo_util = TodoUtil(str(event.group_id))
+    todo_token = TodoToken(name, datetime.today(), exceed_time, priority)
+    if todo_util.add_data_to_list(todo_token):
+        await add_todo.send(f"已将{name}加入清单，ddl为{exceed_time}，优先级为{priority}。\n当前共{todo_util.list_size}项待办。")
+        img = await todo_util.get_list_img()
+        await remove_todo.finish(MessageSegment.image(img))
+    else:
+        await add_todo.finish(f"{name}已在清单中。")
+
+
+@remove_todo.handle()
+async def remove_todo_handle(event: Union[PrivateMessageEvent, GroupMessageEvent]):
+    text: str = event.raw_message
+    name, name_valid, name_error_doc = get_name_from_text(text)
+    if isinstance(event, PrivateMessageEvent):
+        todo_util = TodoUtil(str(event.user_id))
+    else:
+        todo_util = TodoUtil(str(event.group_id))
+    if not name_valid:
+        await remove_todo.finish(name_error_doc)
+    elif todo_util.remove_data(name) == 0:
+        await remove_todo.finish(f"不存在名为{name}的表项。")
+    else:
+        img = await todo_util.get_list_img()
+        await remove_todo.send(f"已删除{name}。")
+        await remove_todo.finish(MessageSegment.image(img))
+
+
+@finish_todo.handle()
+async def finish_todo_handle(event: Union[PrivateMessageEvent, GroupMessageEvent]):
+    text: str = event.raw_message
+    name, name_valid, name_error_doc = get_name_from_text(text)
+    if isinstance(event, PrivateMessageEvent):
+        todo_util = TodoUtil(str(event.user_id))
+    else:
+        todo_util = TodoUtil(str(event.group_id))
+    if not name_valid:
+        await remove_todo.finish(name_error_doc)
+    elif todo_util.finish_job(name) == 0:
+        await remove_todo.finish(f"不存在名为{name}的表项。")
+    else:
+        await remove_todo.send(f"已完成{name}。还剩{todo_util.list_size}项。")
+        img = await todo_util.get_list_img()
+        await remove_todo.finish(MessageSegment.image(img))
+
+
+@change_todo_time.handle()
+async def change_todo_time_handle(event: Union[PrivateMessageEvent, GroupMessageEvent]):
+    text: str = event.raw_message
+    name, name_valid, name_error_doc = get_name_from_text(text)
+    expire_time, time_valid, time_error_doc = get_time_from_text(text)
+    if isinstance(event, PrivateMessageEvent):
+        todo_util = TodoUtil(str(event.user_id))
+    else:
+        todo_util = TodoUtil(str(event.group_id))
+    if not time_valid:
+        await add_todo.finish(time_error_doc)
+    elif not name_valid:
+        await add_todo.finish(name_error_doc)
+    else:
+        changed_count = todo_util.change_time(name, expire_time)
+        if not changed_count == 0:
+            await change_todo_time.send(f"将{name}改至{expire_time}")
+            img = await todo_util.get_list_img()
+            await change_todo_time.finish(MessageSegment.image(img))
+        else:
+            await change_todo_time.finish(f"没有名为{name}的项目。")
+
+
+@get_todo_pic.handle()
+async def _handle(event: Union[PrivateMessageEvent, GroupMessageEvent]):
+    if isinstance(event, PrivateMessageEvent):
+        todo_util = TodoUtil(str(event.user_id))
+    else:
+        todo_util = TodoUtil(str(event.group_id))
+    img = await todo_util.get_list_img()
+    await get_todo_pic.finish(MessageSegment.image(img))
+
+
+async def send_todo():
+    for user in plugin_config.todo_users:
+        todo_util = TodoUtil(str(user))
+        img = await todo_util.get_list_img()
+        await nonebot.get_bot().send_private_msg(user_id=user, message=MessageSegment.image(img))
+        time.sleep(5)
+        # 防止风控
+
+    for group in plugin_config.todo_groups:
+        todo_util = TodoUtil(str(group))
+        img = await todo_util.get_list_img()
+        await nonebot.get_bot().send_group_msg(group_id=group, message=MessageSegment.image(img))
+        time.sleep(5)
+        # 防止风控
+
+
+for index, _time in enumerate(plugin_config.todo_send_time):
+    scheduler.add_job(send_todo, "cron", hour=_time.hour, minute=_time.minute, id=str(f"send_todo_for_{index}"))
```

### Comparing `nonebot_plugin_todo_nlp-0.1.8rc0/pyproject.toml` & `nonebot_plugin_todo_nlp-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-[tool.poetry]
-name = "nonebot-plugin-todo-nlp"
-version = "0.1.8c"
-description = "一款自动识别提醒内容，可生成todo图片并定时推送的nonebot2插件"
-authors = ["CofinCup <864341840@qq.com>"]
-license = "MIT license"
-
-[tool.poetry.dependencies]
-python = "^3.8"
-jionlp = "^1.4.17"
-pandas = "^1.4.3"
-nonebot2 = "^2.0.0-beta.5"
-nonebot-plugin-htmlrender = "^0.1.1"
-pathlib = "^1.0.1"
-nonebot-plugin-apscheduler = "0.2.0"
-nonebot-adapter-onebot = "^2.1.3"
-
-[tool.poetry.dev-dependencies]
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "nonebot-plugin-todo-nlp"
+version = "0.1.9"
+description = "一款自动识别提醒内容，可生成todo图片并定时推送的nonebot2插件"
+authors = ["CofinCup <864341840@qq.com>"]
+license = "MIT license"
+
+[tool.poetry.dependencies]
+python = "^3.8"
+jionlp = "^1.4.17"
+pandas = "^1.4.3"
+nonebot2 = "^2.0.0-beta.5"
+nonebot-plugin-htmlrender = "^0.1.1"
+pathlib = "^1.0.1"
+nonebot-plugin-apscheduler = "0.2.0"
+nonebot-adapter-onebot = "^2.1.3"
+jieba = "^0.42.1"
+
+[tool.poetry.dev-dependencies]
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_todo_nlp-0.1.8rc0/PKG-INFO` & `nonebot_plugin_todo_nlp-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-todo-nlp
-Version: 0.1.8rc0
+Version: 0.1.9
 Summary: 一款自动识别提醒内容，可生成todo图片并定时推送的nonebot2插件
 License: MIT
 Author: CofinCup
 Author-email: 864341840@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: jieba (>=0.42.1,<0.43.0)
 Requires-Dist: jionlp (>=1.4.17,<2.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (==0.2.0)
 Requires-Dist: nonebot-plugin-htmlrender (>=0.1.1,<0.2.0)
 Requires-Dist: nonebot2 (>=2.0.0-beta.5,<3.0.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
```


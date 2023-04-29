# Comparing `tmp/weibo-poster-0.0.8.tar.gz` & `tmp/weibo-poster-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weibo-poster-0.0.8.tar", last modified: Mon Feb 27 11:37:42 2023, max compression
+gzip compressed data, was "weibo-poster-0.0.9.tar", last modified: Sat Apr 29 11:50:34 2023, max compression
```

## Comparing `weibo-poster-0.0.8.tar` & `weibo-poster-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 11:37:42.627234 weibo-poster-0.0.8/
--rw-rw-rw-   0        0        0     1086 2023-02-23 17:16:45.000000 weibo-poster-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       24 2023-02-26 12:01:51.000000 weibo-poster-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2423 2023-02-27 11:37:42.627234 weibo-poster-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1701 2023-02-26 11:26:16.000000 weibo-poster-0.0.8/README.md
--rw-rw-rw-   0        0        0       59 2023-02-26 13:59:14.000000 weibo-poster-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-27 11:37:42.628235 weibo-poster-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-02-27 11:37:22.000000 weibo-poster-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:37:42.591599 weibo-poster-0.0.8/weibo_poster/
--rw-rw-rw-   0        0        0      192 2023-02-25 16:40:12.000000 weibo-poster-0.0.8/weibo_poster/__init__.py
--rw-rw-rw-   0        0        0     3626 2023-02-25 16:51:42.000000 weibo-poster-0.0.8/weibo_poster/biligo.py
--rw-rw-rw-   0        0        0     8238 2023-02-27 11:25:13.000000 weibo-poster-0.0.8/weibo_poster/utils.py
--rw-rw-rw-   0        0        0     5555 2023-02-26 13:57:41.000000 weibo-poster-0.0.8/weibo_poster/weibo.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:37:42.624234 weibo-poster-0.0.8/weibo_poster.egg-info/
--rw-rw-rw-   0        0        0     2423 2023-02-27 11:37:42.000000 weibo-poster-0.0.8/weibo_poster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-02-27 11:37:42.000000 weibo-poster-0.0.8/weibo_poster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 11:37:42.000000 weibo-poster-0.0.8/weibo_poster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-02-27 11:37:42.000000 weibo-poster-0.0.8/weibo_poster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-27 11:37:42.000000 weibo-poster-0.0.8/weibo_poster.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 11:50:34.732729 weibo-poster-0.0.9/
+-rw-rw-rw-   0        0        0     1086 2023-02-23 17:16:45.000000 weibo-poster-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-02-26 12:01:51.000000 weibo-poster-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2423 2023-04-29 11:50:34.732729 weibo-poster-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1701 2023-02-26 11:26:16.000000 weibo-poster-0.0.9/README.md
+-rw-rw-rw-   0        0        0       59 2023-02-26 13:59:14.000000 weibo-poster-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 11:50:34.733724 weibo-poster-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-04-29 11:50:29.000000 weibo-poster-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:50:34.703825 weibo-poster-0.0.9/weibo_poster/
+-rw-rw-rw-   0        0        0      197 2023-03-02 12:53:54.000000 weibo-poster-0.0.9/weibo_poster/__init__.py
+-rw-rw-rw-   0        0        0     3749 2023-03-03 10:51:52.000000 weibo-poster-0.0.9/weibo_poster/biligo.py
+-rw-rw-rw-   0        0        0     8559 2023-03-02 07:08:47.000000 weibo-poster-0.0.9/weibo_poster/utils.py
+-rw-rw-rw-   0        0        0     5555 2023-02-26 13:57:41.000000 weibo-poster-0.0.9/weibo_poster/weibo.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:50:34.729738 weibo-poster-0.0.9/weibo_poster.egg-info/
+-rw-rw-rw-   0        0        0     2423 2023-04-29 11:50:34.000000 weibo-poster-0.0.9/weibo_poster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-04-29 11:50:34.000000 weibo-poster-0.0.9/weibo_poster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:50:34.000000 weibo-poster-0.0.9/weibo_poster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-29 11:50:34.000000 weibo-poster-0.0.9/weibo_poster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-29 11:50:34.000000 weibo-poster-0.0.9/weibo_poster.egg-info/top_level.txt
```

### Comparing `weibo-poster-0.0.8/LICENSE` & `weibo-poster-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `weibo-poster-0.0.8/PKG-INFO` & `weibo-poster-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weibo-poster
-Version: 0.0.8
+Version: 0.0.9
 Summary: 对应 weibo-webhook 的提交器
 Home-page: https://github.com/Drelf2018/weibo-poster
 Author: Drelf2018
 Author-email: drelf2018@outlook.com
 License: MIT
 Keywords: python,weibo,webhook
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: weibo-poster Version: 0.0.8 Summary: å¯¹åº weibo-
+Metadata-Version: 2.1 Name: weibo-poster Version: 0.0.9 Summary: å¯¹åº weibo-
 webhook çæäº¤å¨ Home-page: https://github.com/Drelf2018/weibo-poster
 Author: Drelf2018 Author-email: drelf2018@outlook.com License: MIT Keywords:
 python,weibo,webhook Platform: UNKNOWN Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `weibo-poster-0.0.8/README.md` & `weibo-poster-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `weibo-poster-0.0.8/setup.py` & `weibo-poster-0.0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r", encoding="utf8") as f:
     requires = f.read()
 
 setup(
     name="weibo-poster",
-    version="0.0.8",
+    version="0.0.9",
     license="MIT",
     author="Drelf2018",
     author_email="drelf2018@outlook.com",
     description="对应 weibo-webhook 的提交器",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

### Comparing `weibo-poster-0.0.8/weibo_poster/biligo.py` & `weibo-poster-0.0.9/weibo_poster/biligo.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,33 +84,36 @@
 
     def __init__(self, aid: str, url: str, *listening_rooms):
         super().__init__()
         #  接入 biligo-ws-live 时的 id 用来区分不同监控程序
         self.aid = aid
         # biligo-ws-live 运行地址
         self.url = url
+        self.update(listening_rooms)
+    
+    def update(self, listening_rooms):
         # 将监听房间号告知 biligo-ws-live
         httpx.post(self.url+'/subscribe', headers={"Authorization": self.aid}, data={'subscribes': list(listening_rooms)})
 
     def on(self, event_name: str, filter: Callable = lambda *_, **__: True) -> Callable:
         """
         装饰器注册事件监听器。
 
         Args:
             event_name (str): 事件名。
         """
         def decorator(func: Coroutine):
             isAsyncFunction = isAsync(filter)
-            async def wapper(args):
+            async def wapper(*args, **kwargs):
                 if isAsyncFunction:
-                    if not await filter(*args):
+                    if not await filter(*args, **kwargs):
                         return
-                elif not filter(*args):
+                elif not filter(*args, **kwargs):
                     return
-                return await func(*args)
+                return await func(*args, **kwargs)
             self.add_event_listener(event_name, wapper)
 
             return func
 
         return decorator
 
     async def run(self):
@@ -118,8 +121,8 @@
         阻塞异步连接
         """
 
         async with AioWebSocket(self.url + f"/ws?id={self.aid}") as aws:
             logger.info('Adapter 连接成功')
             async for evt in Receive(aws.manipulator.receive):
                 if evt["command"] == "DANMU_MSG":
-                    self.dispatch(evt["command"], (RoomInfo(**evt["live_info"]), DanmakuPost.parse(evt)))
+                    self.dispatch(evt["command"], RoomInfo(**evt["live_info"]), DanmakuPost.parse(evt))
```

### Comparing `weibo-poster-0.0.8/weibo_poster/utils.py` & `weibo-poster-0.0.9/weibo_poster/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,23 @@
             times += 1
             return await fn(*arg, **kwargs)
         return wapper
     return inner
 
 
 @dataclass
+class Job:
+    patten: str
+    method: str
+    url: str
+    headers: Dict[str, str] = field(default_factory=dict)
+    data: Dict[str, str] = field(default_factory=dict)
+
+
+@dataclass
 class User:
     level: int
     xp: int
     uid: int
     file: str
 
 
@@ -203,17 +212,20 @@
         data = res.json()
         if data["code"] == 0:
             return data["data"]
         else:
             logger.error(data["data"])
             return []
 
-    async def config(self, data):
+    async def config(self, listening: List[str], jobs: List[Job]):
         "配"
-        res = await self.session.post(f"{self.baseurl}/config", params={"token": self.token}, json=data)
+        res = await self.session.post(f"{self.baseurl}/config", params={"token": self.token}, json={
+            "listening": listening,
+            "jobs": [job.__dict__ for job in jobs]
+        })
         data = res.json()
         if data["code"] == 0:
             return data["data"]
         else:
             logger.error(data["data"])
             return ""
```

### Comparing `weibo-poster-0.0.8/weibo_poster/weibo.py` & `weibo-poster-0.0.9/weibo_poster/weibo.py`

 * *Files identical despite different names*

### Comparing `weibo-poster-0.0.8/weibo_poster.egg-info/PKG-INFO` & `weibo-poster-0.0.9/weibo_poster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weibo-poster
-Version: 0.0.8
+Version: 0.0.9
 Summary: 对应 weibo-webhook 的提交器
 Home-page: https://github.com/Drelf2018/weibo-poster
 Author: Drelf2018
 Author-email: drelf2018@outlook.com
 License: MIT
 Keywords: python,weibo,webhook
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: weibo-poster Version: 0.0.8 Summary: å¯¹åº weibo-
+Metadata-Version: 2.1 Name: weibo-poster Version: 0.0.9 Summary: å¯¹åº weibo-
 webhook çæäº¤å¨ Home-page: https://github.com/Drelf2018/weibo-poster
 Author: Drelf2018 Author-email: drelf2018@outlook.com License: MIT Keywords:
 python,weibo,webhook Platform: UNKNOWN Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Requires-Python: >=3.8 Description-Content-Type: text/markdown
```


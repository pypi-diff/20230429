# Comparing `tmp/Vulncapture-0.0.5.tar.gz` & `tmp/Vulncapture-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Vulncapture-0.0.5.tar", last modified: Sat Apr 29 16:41:45 2023, max compression
+gzip compressed data, was "Vulncapture-1.0.0.tar", last modified: Sat Apr 29 17:44:44 2023, max compression
```

## Comparing `Vulncapture-0.0.5.tar` & `Vulncapture-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 16:41:45.804551 Vulncapture-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-04-26 08:28:29.000000 Vulncapture-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1037 2023-04-29 16:41:45.804551 Vulncapture-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-04-29 16:41:15.000000 Vulncapture-0.0.5/README.md
--rw-rw-rw-   0        0        0      635 2023-04-29 16:31:10.000000 Vulncapture-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 16:41:45.805552 Vulncapture-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      189 2023-04-29 16:24:14.000000 Vulncapture-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:41:45.758453 Vulncapture-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 16:41:45.786548 Vulncapture-0.0.5/src/Vulncapture/
--rw-rw-rw-   0        0        0    20287 2023-04-29 16:40:13.000000 Vulncapture-0.0.5/src/Vulncapture/Vulncapture.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:29:13.000000 Vulncapture-0.0.5/src/Vulncapture/__init__.py
--rw-rw-rw-   0        0        0     1559 2022-11-09 05:08:38.000000 Vulncapture-0.0.5/src/Vulncapture/dialogui.png
--rw-rw-rw-   0        0        0 15044440 2022-11-09 06:03:08.000000 Vulncapture-0.0.5/src/Vulncapture/mshei.ttf
--rw-rw-rw-   0        0        0       30 2023-04-26 03:34:33.000000 Vulncapture-0.0.5/src/Vulncapture/requirements.txt
--rw-rw-rw-   0        0        0     7710 2022-11-09 05:30:26.000000 Vulncapture-0.0.5/src/Vulncapture/titlegui.png
-drwxrwxrwx   0        0        0        0 2023-04-29 16:41:45.803548 Vulncapture-0.0.5/src/Vulncapture.egg-info/
--rw-rw-rw-   0        0        0     1037 2023-04-29 16:41:45.000000 Vulncapture-0.0.5/src/Vulncapture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-04-29 16:41:45.000000 Vulncapture-0.0.5/src/Vulncapture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 16:41:45.000000 Vulncapture-0.0.5/src/Vulncapture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 16:41:45.000000 Vulncapture-0.0.5/src/Vulncapture.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 17:44:44.206363 Vulncapture-1.0.0/
+-rw-rw-rw-   0        0        0     1091 2023-04-26 08:28:29.000000 Vulncapture-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1238 2023-04-29 17:44:44.205361 Vulncapture-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2023-04-29 17:43:46.000000 Vulncapture-1.0.0/README.md
+-rw-rw-rw-   0        0        0      630 2023-04-29 17:44:27.000000 Vulncapture-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 17:44:44.206363 Vulncapture-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      189 2023-04-29 17:26:11.000000 Vulncapture-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:44:44.156981 Vulncapture-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 17:44:44.187357 Vulncapture-1.0.0/src/Vulncapture/
+-rw-rw-rw-   0        0        0    18802 2023-04-29 17:41:21.000000 Vulncapture-1.0.0/src/Vulncapture/Vulncapture.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:29:13.000000 Vulncapture-1.0.0/src/Vulncapture/__init__.py
+-rw-rw-rw-   0        0        0     1559 2022-11-09 05:08:38.000000 Vulncapture-1.0.0/src/Vulncapture/dialogui.png
+-rw-rw-rw-   0        0        0 15044440 2022-11-09 06:03:08.000000 Vulncapture-1.0.0/src/Vulncapture/mshei.ttf
+-rw-rw-rw-   0        0        0       30 2023-04-26 03:34:33.000000 Vulncapture-1.0.0/src/Vulncapture/requirements.txt
+-rw-rw-rw-   0        0        0     7710 2022-11-09 05:30:26.000000 Vulncapture-1.0.0/src/Vulncapture/titlegui.png
+drwxrwxrwx   0        0        0        0 2023-04-29 17:44:44.204359 Vulncapture-1.0.0/src/Vulncapture.egg-info/
+-rw-rw-rw-   0        0        0     1238 2023-04-29 17:44:44.000000 Vulncapture-1.0.0/src/Vulncapture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-04-29 17:44:44.000000 Vulncapture-1.0.0/src/Vulncapture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 17:44:44.000000 Vulncapture-1.0.0/src/Vulncapture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 17:44:44.000000 Vulncapture-1.0.0/src/Vulncapture.egg-info/top_level.txt
```

### Comparing `Vulncapture-0.0.5/LICENSE` & `Vulncapture-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Vulncapture-0.0.5/PKG-INFO` & `Vulncapture-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,37 @@
-Metadata-Version: 2.1
-Name: Vulncapture
-Version: 0.0.5
-Summary: A small example package for Vulncapture 
-Author-email: jiangyangcreate <jiangyangcreate@gamil.com>
-Project-URL: Homepage, https://github.com/jiangmiemie/Vulncapture
-Project-URL: Bug Tracker, https://github.com/jiangmiemie/Vulncapture/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 A capture moudle return base64image
 
 # Install
 
 pip install Vulncapture
 
 # Use
 
 ```
-from Vulncapture import Vulncaptureimage 
+from Vulncapture import Vulncapture
+import base64
 image=Vulncapture.run_snapshot(url='http://www.baidu.com',keyword='换一换')
 print(image) # str
 imgdata=base64.b64decode(image)
 file=open('1.jpg','wb')
 file.write(imgdata)
 file.close()
 ```
-
 run_snapshot()
+'''
+url : aim url
+keyword : str
+cookie = ''
+'''
+if your aim url need to login , please set cookie
 
-    '''
-
-    url : aim url
-
-    keyword : str
-
-    cookie = ''
+```
+from Vulncapture import Vulncapture
+import base64
+imgdata2= Vulncapture.txt2image('123','1',False)
+print(imgdata2)
+imgdata=base64.b64decode(imgdata2)
+file=open('2.jpg','wb')
+file.write(imgdata)
+file.close()
+```
 
-    '''
-if your aim url need to login , please set cookie
```

### Comparing `Vulncapture-0.0.5/src/Vulncapture/Vulncapture.py` & `Vulncapture-1.0.0/src/Vulncapture/Vulncapture.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,54 +53,14 @@
         return text
     elif mode == 2:
         text_start = source_str.find(key)
         text_end = text_start + len(key)
 
         return source_str[:text_start], source_str[text_start:text_end], source_str[text_end:]
 
-
-def get_txt(capture_type: str, data: dict, keyword: str):
-
-    if capture_type == 'headers':
-        txt = ""
-        request_headers_txt = data['request']['headers']
-        response_headers_txt = data['response']['headers']
-        txt += 'Request_Headers\n'
-        for key in request_headers_txt:
-            txt = txt + str(key) + ":" + str(request_headers_txt[key]) + '\n'
-
-        txt += "\n"
-
-        txt += 'Response_Headers\n'
-        for key in response_headers_txt:
-            txt = txt + str(key) + ":" + str(response_headers_txt[key]) + '\n'
-        return txt
-
-    elif capture_type == 'http':
-        request_txt = data['request']
-        method = request_txt["method"].upper()
-        http_path = request_txt["path"].upper()
-
-        http_scheme = request_txt["scheme"].upper()
-        http_version = request_txt["http_version"].upper()
-        http_host = request_txt["host"].upper()
-        http_port = request_txt["port"]
-
-        txt = f"{method} {http_path} {http_scheme}/{http_version}\nHost:{http_host}:{http_port}\n"
-
-        request_headers_txt = data['request']['headers']
-        for key in request_headers_txt:
-            txt = txt + str(key) + ":" + str(request_headers_txt[key]) + '\n'
-        return txt
-
-    elif capture_type == 'response':
-        txt = slicing_str(data['response']["response_body"], keyword)
-    return str(txt)
-
-
 def high_light_html(html5: str, lightwords: str = '') -> str:
     if lightwords == '':  # 如果没有需要高亮的关键字，则不处理页面
         return html5
 
     html5 = html5.replace(' />', '>')
     html = ''
     for i in re.findall(f'([\s\S]*?)?(<[/]?[a-zA-Z].*?>)', html5):
@@ -137,15 +97,15 @@
 
         draw = ImageDraw.Draw(pic_down)   # 贴上文字
         draw.text((pic_insert+20, 20),  # 设置字出現的位置
                   message,         # 文字
                   black,  # 字体颜色为黑色
                   font=setFont,         # 读取样式
                   direction=None)
-        pic_down.save(outpath, format='PNG')  # 保存
+        pic_down  # 保存
 
     elif ui == 'titlegui.png':
         message = get_len_num(message, 94)
         draw = ImageDraw.Draw(pic_up)
         draw.text((0+177, 50),  # 设置URL
                   message,         # 文字
                   white,
@@ -386,28 +346,24 @@
                 text, cfg["font-antialiasing"], cfg["font-color"], cfg["background-color"])
             sio = BytesIO()
             pygame.image.save(rtext, sio)
             sio.seek(0)
             ln_im = Image.open(sio)
             im.paste(ln_im, (x, y))
 
-    def txt2im(self, txt, keyword, save=False, show=False):
+    def txt2im(self, txt, keyword, show=False):
 
         self.keyword = keyword
         font = self.getFontForPyGame(
             self.cfg["font-family"], self.cfg["font-size"])
         title_font = self.getFontForPyGame(
             self.cfg["font-family"], self.cfg["title-font-size"])
 
         data = self.makeMatrix(txt, font, title_font, self.cfg)
         image = self.makeImage(data, self.cfg)
-        if save:
-            image.save('test.png')
-        if show:
-            image.show()
         return image
 
 
 class Capture:
     def __init__(self):
         self.keyword = ""
         self.screen = BytesIO()
@@ -472,59 +428,57 @@
             html = self.page.content()
             html = html.replace("b'", '')
             html = html.replace(r"\r", '')
             html = html.replace(r"\n", '')
             html = html.replace(r"\t", '')
             html_new = high_light_html(html, self.keyword)
             self.page.set_content(html_new)
-            self.screenshot(capture_type)    # 调用screenshot方法，存贮图像至内存
+            self.screenshot()    # 调用screenshot方法，存贮图像至内存
             browser.close()  # 关闭整个浏览器（区别于关闭单个页面）
 
     def screenshot(self, capture_type):
-        if capture_type == 'page':
-            screen = BytesIO()
-            if self.xss_flag != True:  # 如果沒有检测到弹窗
-                screen.write(self.page.screenshot(full_page=True, type="png"))
-            else:
-                screen_diolog = BytesIO()
-                screen_diolog.write(self.page.screenshot(
-                    full_page=True, type="png"))
-                stitching_pictures(screen_diolog, self.xss_message,
-                                   outpath=screen, ui='dialogui.png')
-            stitching_pictures(
-                screen, self.url, self.screen, ui='titlegui.png')
-
-        elif capture_type == 'headers':
-            txt = get_txt(capture_type, self.data, self.keyword)
-            txttoimage = TxtToImage()
-            self.screen = txttoimage.txt2im(txt, self.keyword, show=False)
+        screen = BytesIO()
+        if self.xss_flag != True:  # 如果沒有检测到弹窗
+            screen.write(self.page.screenshot(full_page=True, type="png"))
+        else:
+            screen_diolog = BytesIO()
+            screen_diolog.write(self.page.screenshot(
+                full_page=True, type="png"))
+            stitching_pictures(screen_diolog, self.xss_message,
+                                outpath=screen, ui='dialogui.png')
+        stitching_pictures(
+            screen, self.url, self.screen, ui='titlegui.png')
 
     def image(self, show=False):
         if show:
             img = Image.open(self.screen)
             img.show()
         screen = base64.b64encode(self.screen.getvalue()).decode("utf-8")
         return screen
 
 
 def run_snapshot(url,
                  keyword='',
                  cookie = '',
+                 body = '',
                  method = 'GET',
                  capture_type='page',
                  ):
     '''
     url : aim url
     keyword : str
+    body = '',
+    method = 'GET',
+    capture_type='page', 
     '''
     data = {'request': {
         'url': url,
         'method': method,
         'headers': {'cookie': cookie},
-        'body': '', },
+        'body': body, },
         'response': {
         'headers': {'cookie': cookie}, }
     }
     request = data['request']
     request['headers']['cookie'] = 'security_level=0; PHPSESSID=gttrr52vcv5fpdm140afqher14; security=low'
     ca = Capture()
     ca.capture(url=request['url'],
@@ -535,7 +489,15 @@
                keyword=keyword,
                capture_type=capture_type)
     img = ca.image(show=False)
     if len(img) > 0:
         return img
     else:
         return None
+    
+def txt2image(data='',keyword='',show=False):
+    screen = BytesIO()
+    txttoimage = TxtToImage()
+    img = txttoimage.txt2im(data, keyword, show=show)
+    img.save(screen, format='PNG')
+    screen = base64.b64encode(screen.getvalue()).decode("utf-8")
+    return screen
```

### Comparing `Vulncapture-0.0.5/src/Vulncapture/dialogui.png` & `Vulncapture-1.0.0/src/Vulncapture/dialogui.png`

 * *Files identical despite different names*

### Comparing `Vulncapture-0.0.5/src/Vulncapture/mshei.ttf` & `Vulncapture-1.0.0/src/Vulncapture/mshei.ttf`

 * *Files identical despite different names*

### Comparing `Vulncapture-0.0.5/src/Vulncapture/titlegui.png` & `Vulncapture-1.0.0/src/Vulncapture/titlegui.png`

 * *Files identical despite different names*

### Comparing `Vulncapture-0.0.5/src/Vulncapture.egg-info/PKG-INFO` & `Vulncapture-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Vulncapture
-Version: 0.0.5
-Summary: A small example package for Vulncapture 
+Version: 1.0.0
+Summary: A capture moudle return base64image
 Author-email: jiangyangcreate <jiangyangcreate@gamil.com>
 Project-URL: Homepage, https://github.com/jiangmiemie/Vulncapture
 Project-URL: Bug Tracker, https://github.com/jiangmiemie/Vulncapture/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -17,28 +17,35 @@
 # Install
 
 pip install Vulncapture
 
 # Use
 
 ```
-from Vulncapture import Vulncaptureimage 
+from Vulncapture import Vulncapture
+import base64
 image=Vulncapture.run_snapshot(url='http://www.baidu.com',keyword='换一换')
 print(image) # str
 imgdata=base64.b64decode(image)
 file=open('1.jpg','wb')
 file.write(imgdata)
 file.close()
 ```
-
 run_snapshot()
+'''
+url : aim url
+keyword : str
+cookie = ''
+'''
+if your aim url need to login , please set cookie
 
-    '''
-
-    url : aim url
-
-    keyword : str
-
-    cookie = ''
+```
+from Vulncapture import Vulncapture
+import base64
+imgdata2= Vulncapture.txt2image('123','1',False)
+print(imgdata2)
+imgdata=base64.b64decode(imgdata2)
+file=open('2.jpg','wb')
+file.write(imgdata)
+file.close()
+```
 
-    '''
-if your aim url need to login , please set cookie
```


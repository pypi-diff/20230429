# Comparing `tmp/remote-drawing-provider-1.0.0.tar.gz` & `tmp/remote-drawing-provider-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote-drawing-provider-1.0.0.tar", last modified: Tue Apr 25 06:29:17 2023, max compression
+gzip compressed data, was "remote-drawing-provider-1.0.1.tar", last modified: Sat Apr 29 08:42:31 2023, max compression
```

## Comparing `remote-drawing-provider-1.0.0.tar` & `remote-drawing-provider-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 06:29:17.499254 remote-drawing-provider-1.0.0/
--rw-rw-rw-   0        0        0     1066 2023-04-25 05:29:24.000000 remote-drawing-provider-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      812 2023-04-25 06:29:17.499254 remote-drawing-provider-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-04-25 05:02:34.000000 remote-drawing-provider-1.0.0/README.md
--rw-rw-rw-   0        0        0      565 2023-04-25 06:28:03.000000 remote-drawing-provider-1.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-25 06:29:17.481387 remote-drawing-provider-1.0.0/remote_drawing_provider/
--rw-rw-rw-   0        0        0      159 2023-04-25 06:28:03.000000 remote-drawing-provider-1.0.0/remote_drawing_provider/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-25 02:41:07.000000 remote-drawing-provider-1.0.0/remote_drawing_provider/logger.py
--rw-rw-rw-   0        0        0     1006 2023-04-25 06:28:52.000000 remote-drawing-provider-1.0.0/remote_drawing_provider/provider.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:29:17.497265 remote-drawing-provider-1.0.0/remote_drawing_provider.egg-info/
--rw-rw-rw-   0        0        0      812 2023-04-25 06:29:17.000000 remote-drawing-provider-1.0.0/remote_drawing_provider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-25 06:29:17.000000 remote-drawing-provider-1.0.0/remote_drawing_provider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 06:29:17.000000 remote-drawing-provider-1.0.0/remote_drawing_provider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-25 06:29:17.000000 remote-drawing-provider-1.0.0/remote_drawing_provider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-25 06:29:17.000000 remote-drawing-provider-1.0.0/remote_drawing_provider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 06:29:17.500251 remote-drawing-provider-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      366 2023-04-25 06:28:03.000000 remote-drawing-provider-1.0.0/setup.py
+drwxrwxr-x   0 xyqian    (1004) xyqian    (1004)        0 2023-04-29 08:42:31.578202 remote-drawing-provider-1.0.1/
+-rw-rw-r--   0 xyqian    (1004) xyqian    (1004)     1061 2023-04-29 08:32:54.000000 remote-drawing-provider-1.0.1/LICENSE
+-rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      777 2023-04-29 08:42:31.578202 remote-drawing-provider-1.0.1/PKG-INFO
+-rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      207 2023-04-29 08:32:54.000000 remote-drawing-provider-1.0.1/README.md
+-rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      543 2023-04-29 08:38:15.000000 remote-drawing-provider-1.0.1/pyproject.toml
+drwxrwxr-x   0 xyqian    (1004) xyqian    (1004)        0 2023-04-29 08:42:31.578202 remote-drawing-provider-1.0.1/remote_drawing_provider/
+-rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      152 2023-04-29 08:32:54.000000 remote-drawing-provider-1.0.1/remote_drawing_provider/__init__.py
+-rw-rw-r--   0 xyqian    (1004) xyqian    (1004)     1146 2023-04-29 08:32:54.000000 remote-drawing-provider-1.0.1/remote_drawing_provider/logger.py
+-rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      972 2023-04-29 08:32:54.000000 remote-drawing-provider-1.0.1/remote_drawing_provider/provider.py
+drwxrwxr-x   0 xyqian    (1004) xyqian    (1004)        0 2023-04-29 08:42:31.578202 remote-drawing-provider-1.0.1/remote_drawing_provider.egg-info/
+-rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      777 2023-04-29 08:42:31.000000 remote-drawing-provider-1.0.1/remote_drawing_provider.egg-info/PKG-INFO
+-rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      381 2023-04-29 08:42:31.000000 remote-drawing-provider-1.0.1/remote_drawing_provider.egg-info/SOURCES.txt
+-rw-rw-r--   0 xyqian    (1004) xyqian    (1004)        1 2023-04-29 08:42:31.000000 remote-drawing-provider-1.0.1/remote_drawing_provider.egg-info/dependency_links.txt
+-rw-rw-r--   0 xyqian    (1004) xyqian    (1004)       31 2023-04-29 08:42:31.000000 remote-drawing-provider-1.0.1/remote_drawing_provider.egg-info/requires.txt
+-rw-rw-r--   0 xyqian    (1004) xyqian    (1004)       24 2023-04-29 08:42:31.000000 remote-drawing-provider-1.0.1/remote_drawing_provider.egg-info/top_level.txt
+-rw-rw-r--   0 xyqian    (1004) xyqian    (1004)       38 2023-04-29 08:42:31.578202 remote-drawing-provider-1.0.1/setup.cfg
+-rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      355 2023-04-29 08:38:23.000000 remote-drawing-provider-1.0.1/setup.py
```

### Comparing `remote-drawing-provider-1.0.0/LICENSE` & `remote-drawing-provider-1.0.1/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,14 @@
-Copyright 2023 XiaoyanQian
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Copyright 2023 XiaoyanQian
+
+Permission is hereby granted, free of charge, 
+to any person obtaining a copy of this software and associated documentation files (the “Software”), 
+to deal in the Software without restriction, including without limitation the rights to use, copy,
+modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
+and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
+INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `remote-drawing-provider-1.0.0/PKG-INFO` & `remote-drawing-provider-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: remote-drawing-provider
-Version: 1.0.0
-Summary: Remote Drawing Provider
-Home-page: https://github.com/XiaoyanQian/remote-drawing
-Author: XiaoyanQian
-Author-email: thinkershare <thinkershare@163.com>
-Project-URL: Homepage, https://github.com/XiaoyanQian/remote-drawing
-Project-URL: Bug Tracker, https://github.com/XiaoyanQian/remote-drawing/issues
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# remote-drawing-provider
-
-## install
-
-```bash
-pip install remote-drawing-provider
-```
-
-## using
-
-```python
-from remote-drawing-provider.provider import send
-
-send(method='visualize_point_cloud',[args])
-```
+Metadata-Version: 2.1
+Name: remote-drawing-provider
+Version: 1.0.1
+Summary: Remote Drawing Provider
+Home-page: https://github.com/XiaoyanQian/remote-drawing
+Author: XY-qian
+Author-email: XY-qian <xiaoyanqian1010@gmail.com>
+Project-URL: Homepage, https://github.com/XiaoyanQian/remote-drawing
+Project-URL: Bug Tracker, https://github.com/XiaoyanQian/remote-drawing/issues
+Platform: any
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# remote-drawing-provider
+
+## install
+
+```bash
+pip install remote-drawing-provider
+```
+
+## using
+
+```python
+from remote-drawing-provider.provider import send
+
+send(method='visualize_point_cloud',[args])
+```
```

### Comparing `remote-drawing-provider-1.0.0/pyproject.toml` & `remote-drawing-provider-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-[project]
-name = "remote-drawing-provider"
-version = "1.0.0"
-authors = [
-  { name="thinkershare", email="thinkershare@163.com" },
-]
-description = "Remote Drawing Provider"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License"
-]
-dependencies = [
-    "numpy",
-    "torch",
-    "websockets>=11.0.2"
-]
-
-[project.urls]
-"Homepage" = "https://github.com/XiaoyanQian/remote-drawing"
-"Bug Tracker" = "https://github.com/XiaoyanQian/remote-drawing/issues"
+[project]
+name = "remote-drawing-provider"
+version = "1.0.1"
+authors = [
+  { name="XY-qian", email="xiaoyanqian1010@gmail.com" },
+]
+description = "Remote Drawing Provider"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License"
+]
+dependencies = [
+    "numpy",
+    "torch",
+    "websockets>=11.0.2"
+]
+
+[project.urls]
+"Homepage" = "https://github.com/XiaoyanQian/remote-drawing"
+"Bug Tracker" = "https://github.com/XiaoyanQian/remote-drawing/issues"
```

### Comparing `remote-drawing-provider-1.0.0/remote_drawing_provider/logger.py` & `remote-drawing-provider-1.0.1/remote_drawing_provider/logger.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import os
-
-from datetime import datetime
-
-from colorama import init
-from colorama import Fore, Back, Style
-
-__all__ = ['log_info', 'log_warn', 'log_error', 'log_end', 'format_capacity']
-init()
-
-
-def get_time():
-    return datetime.utcnow().isoformat(sep=' ', timespec='milliseconds')
-
-
-def format_capacity(buffer):
-    size = len(buffer)
-    if size > 1024:
-        return f'{size/1024:.2F} KB'
-    else:
-        return f'{size/1024/1024:.2f} MB'
-
-
-def log_end(end):
-    if end:
-        separator = '-' * os.get_terminal_size().columns
-        print(separator+'\n\n')
-
-
-def log_info(message, end=False):
-    message = f"[{get_time()}]: {message}"
-    print(Fore.BLACK, Back.WHITE, '[ INFO]-'+message)
-    print(Style.RESET_ALL)
-    log_end(end)
-
-
-def log_warn(message, end=False):
-    message = f"[{get_time()}]: {message}"
-    print(Fore.CYAN, Back.YELLOW, '[ WARN]-'+message)
-    print(Style.RESET_ALL)
-    log_end(end)
-
-
-def log_error(message, error=None, end=False):
-    message = f"[{get_time()}]: {message}"
-    print(Fore.CYAN, Back.RED, '[ERROR]-'+message)
-
-    if error:
-        print(error)
-
-    print(Style.RESET_ALL)
-    log_end(end)
+import os
+
+from datetime import datetime
+
+from colorama import init
+from colorama import Fore, Back, Style
+
+__all__ = ['log_info', 'log_warn', 'log_error', 'log_end', 'format_capacity']
+init()
+
+
+def get_time():
+    return datetime.utcnow().isoformat(sep=' ', timespec='milliseconds')
+
+
+def format_capacity(buffer):
+    size = len(buffer)
+    if size > 1024:
+        return f'{size/1024:.2F} KB'
+    else:
+        return f'{size/1024/1024:.2f} MB'
+
+
+def log_end(end):
+    if end:
+        separator = '-' * os.get_terminal_size().columns
+        print(separator+'\n\n')
+
+
+def log_info(message, end=False):
+    message = f"[{get_time()}]: {message}"
+    print(Fore.BLACK, Back.WHITE, '[ INFO]-'+message)
+    print(Style.RESET_ALL)
+    log_end(end)
+
+
+def log_warn(message, end=False):
+    message = f"[{get_time()}]: {message}"
+    print(Fore.CYAN, Back.YELLOW, '[ WARN]-'+message)
+    print(Style.RESET_ALL)
+    log_end(end)
+
+
+def log_error(message, error=None, end=False):
+    message = f"[{get_time()}]: {message}"
+    print(Fore.CYAN, Back.RED, '[ERROR]-'+message)
+
+    if error:
+        print(error)
+
+    print(Style.RESET_ALL)
+    log_end(end)
```

### Comparing `remote-drawing-provider-1.0.0/remote_drawing_provider/provider.py` & `remote-drawing-provider-1.0.1/remote_drawing_provider/provider.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import zlib
-import torch
-from io import BytesIO
-from logger import *
-from websockets.sync.client import connect
-
-Port = 65532
-RenderType = 'Provider'
-TypeHeader = 'X-Client-Type'
-Headers = {TypeHeader: RenderType}
-
-__all__ = ['send']
-
-
-def get_bytes(args) -> bytes:
-    buffer = BytesIO()
-    torch.save(args, buffer, _use_new_zipfile_serialization=False)
-    buffer = zlib.compress(buffer.getvalue())
-
-    log_info(f'正在创建渲染请求,包大小: {format_capacity(buffer)}')
-    return buffer
-
-
-def send(method='visualize_point_cloud', **args):
-    if len(args) == 0:
-        raise ValueError('渲染需要至少一个有效的参数')
-
-    args['method'] = method
-    message = get_bytes(args)
-
-    with connect(f'ws://localhost:{Port}', additional_headers=Headers, max_size=500*1024*1024) as socket:
-        socket.send(message)
-        socket.close(code=1000, reason='主动断开')
-        log_info('渲染请求创建成功,请在渲染终端上查看效果')
+import zlib
+import torch
+from io import BytesIO
+from logger import *
+from websockets.sync.client import connect
+
+Port = 65532
+RenderType = 'Provider'
+TypeHeader = 'X-Client-Type'
+Headers = {TypeHeader: RenderType}
+
+__all__ = ['send']
+
+
+def get_bytes(args) -> bytes:
+    buffer = BytesIO()
+    torch.save(args, buffer, _use_new_zipfile_serialization=False)
+    buffer = zlib.compress(buffer.getvalue())
+
+    log_info(f'正在创建渲染请求,包大小: {format_capacity(buffer)}')
+    return buffer
+
+
+def send(method='visualize_point_cloud', **args):
+    if len(args) == 0:
+        raise ValueError('渲染需要至少一个有效的参数')
+
+    args['method'] = method
+    message = get_bytes(args)
+
+    with connect(f'ws://localhost:{Port}', additional_headers=Headers, max_size=500*1024*1024) as socket:
+        socket.send(message)
+        socket.close(code=1000, reason='主动断开')
+        log_info('渲染请求创建成功,请在渲染终端上查看效果')
```

### Comparing `remote-drawing-provider-1.0.0/remote_drawing_provider.egg-info/PKG-INFO` & `remote-drawing-provider-1.0.1/remote_drawing_provider.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: remote-drawing-provider
-Version: 1.0.0
-Summary: Remote Drawing Provider
-Home-page: https://github.com/XiaoyanQian/remote-drawing
-Author: XiaoyanQian
-Author-email: thinkershare <thinkershare@163.com>
-Project-URL: Homepage, https://github.com/XiaoyanQian/remote-drawing
-Project-URL: Bug Tracker, https://github.com/XiaoyanQian/remote-drawing/issues
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# remote-drawing-provider
-
-## install
-
-```bash
-pip install remote-drawing-provider
-```
-
-## using
-
-```python
-from remote-drawing-provider.provider import send
-
-send(method='visualize_point_cloud',[args])
-```
+Metadata-Version: 2.1
+Name: remote-drawing-provider
+Version: 1.0.1
+Summary: Remote Drawing Provider
+Home-page: https://github.com/XiaoyanQian/remote-drawing
+Author: XY-qian
+Author-email: XY-qian <xiaoyanqian1010@gmail.com>
+Project-URL: Homepage, https://github.com/XiaoyanQian/remote-drawing
+Project-URL: Bug Tracker, https://github.com/XiaoyanQian/remote-drawing/issues
+Platform: any
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# remote-drawing-provider
+
+## install
+
+```bash
+pip install remote-drawing-provider
+```
+
+## using
+
+```python
+from remote-drawing-provider.provider import send
+
+send(method='visualize_point_cloud',[args])
+```
```


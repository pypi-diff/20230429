# Comparing `tmp/spiderx-1.8.2.tar.gz` & `tmp/spiderx-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiderx-1.8.2.tar", last modified: Thu Nov 17 12:31:35 2022, max compression
+gzip compressed data, was "spiderx-1.8.9.tar", last modified: Fri Nov 25 08:35:18 2022, max compression
```

## Comparing `spiderx-1.8.2.tar` & `spiderx-1.8.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-11-17 12:31:35.757698 spiderx-1.8.2/
--rw-rw-rw-   0        0        0      270 2022-11-17 12:31:35.756696 spiderx-1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0       52 2021-09-05 06:23:16.000000 spiderx-1.8.2/README.md
--rw-rw-rw-   0        0        0       42 2022-11-17 12:31:35.757698 spiderx-1.8.2/setup.cfg
--rw-rw-rw-   0        0        0     2348 2022-11-17 12:31:14.000000 spiderx-1.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-17 12:31:35.748695 spiderx-1.8.2/spiderx/
--rw-rw-rw-   0        0        0        0 2022-11-04 14:32:45.000000 spiderx-1.8.2/spiderx/__init__.py
--rw-rw-rw-   0        0        0        0 2022-11-04 14:32:45.000000 spiderx-1.8.2/spiderx/brower.py
--rw-rw-rw-   0        0        0      643 2022-11-04 14:32:45.000000 spiderx-1.8.2/spiderx/flask_server.py
--rw-rw-rw-   0        0        0     8495 2022-11-04 14:32:45.000000 spiderx-1.8.2/spiderx/gui.py
--rw-rw-rw-   0        0        0    74872 2022-11-04 14:32:45.000000 spiderx-1.8.2/spiderx/info.py
--rw-rw-rw-   0        0        0     6089 2022-11-05 04:58:59.000000 spiderx-1.8.2/spiderx/my_pyqt.py
--rw-rw-rw-   0        0        0     1092 2022-11-04 14:32:45.000000 spiderx-1.8.2/spiderx/my_sqlalchemy.py
--rw-rw-rw-   0        0        0     6298 2022-11-04 14:32:45.000000 spiderx-1.8.2/spiderx/orm.py
--rw-rw-rw-   0        0        0     4874 2022-11-04 14:32:45.000000 spiderx-1.8.2/spiderx/shiti.py
--rw-rw-rw-   0        0        0     2264 2022-11-04 14:32:45.000000 spiderx-1.8.2/spiderx/sql.py
--rw-rw-rw-   0        0        0   111275 2022-11-17 12:29:57.000000 spiderx-1.8.2/spiderx/sx.py
--rw-rw-rw-   0        0        0    32853 2022-11-05 03:56:25.000000 spiderx-1.8.2/spiderx/tools.py
--rw-rw-rw-   0        0        0       44 2022-11-04 14:32:45.000000 spiderx-1.8.2/spiderx/utils.py
--rw-rw-rw-   0        0        0     7941 2022-11-04 14:32:45.000000 spiderx-1.8.2/spiderx/win32.py
-drwxrwxrwx   0        0        0        0 2022-11-17 12:31:35.755696 spiderx-1.8.2/spiderx.egg-info/
--rw-rw-rw-   0        0        0      270 2022-11-17 12:31:35.000000 spiderx-1.8.2/spiderx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2022-11-17 12:31:35.000000 spiderx-1.8.2/spiderx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-17 12:31:35.000000 spiderx-1.8.2/spiderx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      320 2022-11-17 12:31:35.000000 spiderx-1.8.2/spiderx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-11-17 12:31:35.000000 spiderx-1.8.2/spiderx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-11-25 08:35:18.489265 spiderx-1.8.9/
+-rw-rw-rw-   0        0        0      270 2022-11-25 08:35:18.489265 spiderx-1.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2021-09-05 06:23:16.000000 spiderx-1.8.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-11-25 08:35:18.489265 spiderx-1.8.9/setup.cfg
+-rw-rw-rw-   0        0        0     2571 2022-11-24 10:32:22.000000 spiderx-1.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-25 08:35:18.481265 spiderx-1.8.9/spiderx/
+-rw-rw-rw-   0        0        0        0 2022-11-04 14:32:45.000000 spiderx-1.8.9/spiderx/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-11-04 14:32:45.000000 spiderx-1.8.9/spiderx/brower.py
+-rw-rw-rw-   0        0        0      643 2022-11-04 14:32:45.000000 spiderx-1.8.9/spiderx/flask_server.py
+-rw-rw-rw-   0        0        0     8495 2022-11-04 14:32:45.000000 spiderx-1.8.9/spiderx/gui.py
+-rw-rw-rw-   0        0        0    74872 2022-11-04 14:32:45.000000 spiderx-1.8.9/spiderx/info.py
+-rw-rw-rw-   0        0        0     6089 2022-11-05 04:58:59.000000 spiderx-1.8.9/spiderx/my_pyqt.py
+-rw-rw-rw-   0        0        0     1092 2022-11-04 14:32:45.000000 spiderx-1.8.9/spiderx/my_sqlalchemy.py
+-rw-rw-rw-   0        0        0     6298 2022-11-04 14:32:45.000000 spiderx-1.8.9/spiderx/orm.py
+-rw-rw-rw-   0        0        0     4874 2022-11-04 14:32:45.000000 spiderx-1.8.9/spiderx/shiti.py
+-rw-rw-rw-   0        0        0     2264 2022-11-04 14:32:45.000000 spiderx-1.8.9/spiderx/sql.py
+-rw-rw-rw-   0        0        0   112767 2022-11-24 17:23:31.000000 spiderx-1.8.9/spiderx/sx.py
+-rw-rw-rw-   0        0        0    34008 2022-11-25 08:30:04.000000 spiderx-1.8.9/spiderx/tools.py
+-rw-rw-rw-   0        0        0       44 2022-11-04 14:32:45.000000 spiderx-1.8.9/spiderx/utils.py
+-rw-rw-rw-   0        0        0     7941 2022-11-04 14:32:45.000000 spiderx-1.8.9/spiderx/win32.py
+drwxrwxrwx   0        0        0        0 2022-11-25 08:35:18.487265 spiderx-1.8.9/spiderx.egg-info/
+-rw-rw-rw-   0        0        0      270 2022-11-25 08:35:17.000000 spiderx-1.8.9/spiderx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2022-11-25 08:35:18.000000 spiderx-1.8.9/spiderx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-25 08:35:18.000000 spiderx-1.8.9/spiderx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      327 2022-11-25 08:35:18.000000 spiderx-1.8.9/spiderx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-11-25 08:35:18.000000 spiderx-1.8.9/spiderx.egg-info/top_level.txt
```

### Comparing `spiderx-1.8.2/setup.py` & `spiderx-1.8.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages,setup
 setup(
     name = 'spiderx',#模块名
-    version = '1.8.2', #版本
+    version = '1.8.9', #版本
     description='spiderx function',
     license='https://pypi.org/project/spiderx/',
     packages = find_packages(exclude=[]), #目录所有文件
     url='https://pypi.org/project/spiderx/', #文件文档下载地址
     author='wgnms', #作者名
     author_email='wgnms@qq.com', #邮箱
     install_requires=['requests>=2.25.0',
@@ -17,15 +17,15 @@
                       'pyinstaller>=4.5.0',
                       'openpyxl>=3.0.7',
                       'js2py>=0.71',
                       'pyexecjs>=1.5.1',
                       'pillow>=8.3.1',
                       'pymysql>=1.0.2',
                       'psutil>=5.9.0',
-                      'chardet>=4.0.0',
+                      'chardet>=4.0.0,<5.0.0',
                       'loguru>=0.6.0',
                       'jsonpath>=0.82',
                       'pyserial>=3.5',
                       'uncurl>=0.0.11',
                       'ntplib>=0.3.3',
                       'pyzbar>=0.1.9',
                       'qrcode>=7.3.1',
@@ -62,8 +62,13 @@
 python C:\Python\Python38-32\Scripts\pywin32_postinstall.py -install  
 
 no module named Crypto  模块错误
 解决办法:
   site-packages目录下修改crypto文件夹为Crypto
   
 运行 N_m3u8dl_Cli.exe 需要模拟输出控制台中的终端 选上
+
+访问资源文件
+pyinstaller -F  key.py  --add-data "image;image" --clean
+base_path = getattr(sys, '_MEIPASS', os.path.dirname(os.path.abspath("__file__")))
+return os.path.join(base_path, 文件相对路径)
 '''
```

### Comparing `spiderx-1.8.2/spiderx/flask_server.py` & `spiderx-1.8.9/spiderx/flask_server.py`

 * *Files identical despite different names*

### Comparing `spiderx-1.8.2/spiderx/gui.py` & `spiderx-1.8.9/spiderx/gui.py`

 * *Files identical despite different names*

### Comparing `spiderx-1.8.2/spiderx/info.py` & `spiderx-1.8.9/spiderx/info.py`

 * *Files identical despite different names*

### Comparing `spiderx-1.8.2/spiderx/my_pyqt.py` & `spiderx-1.8.9/spiderx/my_pyqt.py`

 * *Files identical despite different names*

### Comparing `spiderx-1.8.2/spiderx/my_sqlalchemy.py` & `spiderx-1.8.9/spiderx/my_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `spiderx-1.8.2/spiderx/orm.py` & `spiderx-1.8.9/spiderx/orm.py`

 * *Files identical despite different names*

### Comparing `spiderx-1.8.2/spiderx/shiti.py` & `spiderx-1.8.9/spiderx/shiti.py`

 * *Files identical despite different names*

### Comparing `spiderx-1.8.2/spiderx/sql.py` & `spiderx-1.8.9/spiderx/sql.py`

 * *Files identical despite different names*

### Comparing `spiderx-1.8.2/spiderx/sx.py` & `spiderx-1.8.9/spiderx/sx.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 from hashlib import md5, sha1
 from functools import reduce
 from PIL import Image as PILimage
 from io import StringIO, BytesIO
 from smtplib import SMTP
 from email.mime.text import MIMEText
 from collections import namedtuple
-from js2py import EvalJs
-from execjs import compile
 from http.cookiejar import LWPCookieJar
 from http import cookiejar
 from html import unescape, escape
 from contextlib import contextmanager
 from .info import *
 import threading
 import subprocess
@@ -29,19 +27,17 @@
 import winreg
 import jsonpath
 import signal
 import serial
 import serial.tools.list_ports
 from threading import Thread
 from loguru import logger
+from decimal import Decimal
+import asyncio
 
-try:
-    import asyncio
-except:
-    pass
 threading.stack_size(4096*1000) #创建的线程的堆栈大小  默认40960
 sys.setrecursionlimit(100000) #无限递归次数  默认1000
 warnings.filterwarnings('ignore')
 cmd_color(autoreset=True)
 lock = threading.Lock
 
 #全局变量
@@ -934,24 +930,30 @@
     return 总数 // 分页数 if 总数 % 分页数 == 0 else (总数 // 分页数) + 1
 def 字符串缩略(字符串, 位数, 结尾符号='...'):
     '''('xxxx',6,'...')'''
     if len(字符串) <= 位数:
         return 字符串
     else:
         return 字符串[:位数 - len(结尾符号)] + 结尾符号
-def 获取_URL参数(网址: str) -> dict:
+def 获取_URL_参数(网址: str,解析:bool=True) -> dict:
+    if 解析:
+        网址=unquote(网址)
     query = {}
     for x in urlparse(网址).query.split('&'):
         if x:
             a, b = x.split('=')
             query[a.lower()] = b
     return query
 def 获取_URL_HOST(网址:str)->str:
     return urlparse(网址).hostname
-def 获取_URL_QUERY(网址:str)->str:
+def 获取_URL_HTTP(网址:str)->str:
+    return urlparse(网址).scheme
+def 获取_URL_QUERY(网址:str,解析:bool=True)->str:
+    if 解析:
+        网址=unquote(网址)
     return urlparse(网址).query
 def 提取m3u8List(字符串:str,倒叙=0)->list():
     lst=[]
     for row in 字符串.split('\n'):
         a=re.search('(http.*?\.m3u8.*?)(\n|$|\s+)', row.strip())
         if a:
             lst.append(a.group(1))
@@ -1023,14 +1025,20 @@
         tm_year, tm_mon, tm_mday, tm_hour, tm_min, tm_sec, tm_wday, tm_yday, tm_isdst = time.gmtime(time_utc)
         win32api.SetSystemTime(tm_year, tm_mon, tm_wday, tm_mday, tm_hour, tm_min, tm_sec, 0)
         print('设置时间:{}'.format(time_str))
         return True
     except Exception as e:
         打印错误(e)
         return False
+def 设置_添加目录到环境(path):
+    '临时搜索路径，程序退出后失效'
+    if path:
+        sys.path.append(path)
+    else:
+        sys.path.append(os.path.abspath(os.path.dirname(__file__)))
 def 保存二维码图片(文件路径:str, qrcode_url:str,size=8,border=1):
     '''
     pip install qrcode
     :param 文件路径:  保存路径
     :param qrcode_url: 链接地址
     :return: bool
     '''
@@ -1133,30 +1141,41 @@
     """
     Get absolute path to resource, works for dev and for PyInstaller
     spec文件  datas=[('a.exe','.')],
     资源路径("a.exe")
     """
     base_path = getattr(sys, '_MEIPASS', os.path.dirname(os.path.abspath("__file__")))
     return os.path.join(base_path, 文件相对路径)
+def 小数(num):
+    return Decimal(str(num))
 # js函数转换
 def 执行JS代码(js代码):
     '''执行JS代码('return 123') 无需js环境'''
+    from js2py import EvalJs
     sss = '''
     function func(){
         %s
     }
     ''' % js代码
     js = EvalJs()
     js.execute(sss)
     return js.func()
 def 执行EXECJS(js代码):
+    from functools import partial
+    subprocess.Popen = partial(subprocess.Popen, encoding='utf-8')
+    from execjs import compile
     '''执行JS代码('return 123')  需要nodejs环境'''
     sss = ''' function func(){ %s } ''' % js代码
     js = compile(sss)
     return js.call('func')
+def 执行EXECJS_FUNC(js代码:str,函数名:str,*args):
+    from functools import partial
+    subprocess.Popen = partial(subprocess.Popen, encoding='utf-8')
+    from execjs import compile
+    return compile(js代码).call(函数名,*args)
 def JS_Uint8Array(lst:list)->bytes:
     return bytes(lst)
 def JS_parseInt(a,b):
     return int(a,b)
 def JS_int8arry_to_uint8arry(lst:list)->list:
     return [x if x>=0 else x+256 for x in lst]
 def join(列表:list,分割=''):
@@ -1217,14 +1236,15 @@
         else:
             return jsonpath.jsonpath(josn对象,表达式)
     except:
         if first:
             return None
         else:
             return []
+
 # 请求
 def get_proxies(ip_port:str='')->dict:
     '''
     自定义 代理IP  '127.0.0.1:8080'
     或者获取本地代理
     返回列表{} 或者 None
     '''
@@ -1250,133 +1270,130 @@
     '''
     hKey = winreg.OpenKey(winreg.HKEY_CURRENT_USER, "Software\Microsoft\Windows\CurrentVersion\Internet Settings", 0, winreg.KEY_WRITE)
     winreg.SetValueEx(hKey, "ProxyEnable", 0, winreg.REG_DWORD, 开启代理)
     winreg.SetValueEx(hKey, "ProxyServer", 0, winreg.REG_SZ, ip_port)
     winreg.SetValueEx(hKey, "ProxyOverride", 0, winreg.REG_SZ, 白名单)
     winreg.CloseKey(hKey)
 default_proxies=get_proxies()
-def get_request(url, headers=None, verify=False, proxies=None, allow_redirects=True, cookies=None, stream=False,curl=False, timeout=30, try_num=1):
+def get_request(url, headers=None,params=None, verify=False, proxies=None, allow_redirects=True, cookies=None, stream=False,curl=False, timeout=30, try_num=1):
     proxies = proxies if proxies else default_proxies
     if headers and isinstance(headers,str):headers=dict_From_HeadersStr(headers)
     if cookies and isinstance(cookies,str):cookies=dict_From_CookieStr(cookies)
+    if params and isinstance(params,str):params=dict_From_HeadersStr(params)
     if curl:
         if 'cookie' in headers:
             if not cookies:
                 cookies=dict_From_CookieStr(headers['cookie'])
     for i in range(try_num):
         try:
             if stream:
-                return requests.get(url, timeout=timeout, headers=headers if headers else get_headers('chrome'), verify=verify, proxies=proxies,
-                                  allow_redirects=allow_redirects, cookies=cookies, stream=stream)
+                return requests.get(url, timeout=timeout, headers=headers if headers else get_headers('chrome'),params=params, verify=verify, proxies=proxies, allow_redirects=allow_redirects, cookies=cookies, stream=stream)
             else:
-                with requests.get(url, timeout=timeout, headers=headers if headers else get_headers('chrome'), verify=verify, proxies=proxies,
-                                  allow_redirects=allow_redirects, cookies=cookies, stream=stream) as resp:
+                with requests.get(url, timeout=timeout, headers=headers if headers else get_headers('chrome'),params=params, verify=verify, proxies=proxies, allow_redirects=allow_redirects, cookies=cookies, stream=stream) as resp:
                     return resp
         except Exception as e:
             if i == try_num - 1:
                 raise Exception(跟踪函数(-3)+' '+str(e))
 def post_request(url, headers=None, data=None, verify=False, proxies=None, allow_redirects=True, cookies=None,stream=False, json_=None,curl=False, timeout=30, try_num=1):
     proxies = proxies if proxies else default_proxies
-    if headers and isinstance(headers,str):
-        headers=dict_From_HeadersStr(headers)
-    if cookies and isinstance(cookies,str):
-        cookies=dict_From_CookieStr(cookies)
+    if headers and isinstance(headers,str): headers=dict_From_HeadersStr(headers)
+    if cookies and isinstance(cookies,str): cookies=dict_From_CookieStr(cookies)
     if curl:
         if 'cookie' in headers:
             if not cookies:
                 cookies=dict_From_CookieStr(headers['cookie'])
     for i in range(try_num):
         try:
             if stream:
-                return requests.post(url, timeout=timeout, headers=headers if headers else get_headers('chrome'), verify=verify, proxies=proxies,
-                                   allow_redirects=allow_redirects, data=data, json=json_, cookies=cookies,stream=stream)
+                return requests.post(url, timeout=timeout, headers=headers if headers else get_headers('chrome'), verify=verify, proxies=proxies, allow_redirects=allow_redirects, data=data, json=json_, cookies=cookies,stream=stream)
             else:
-                with requests.post(url, timeout=timeout, headers=headers if headers else get_headers('chrome'), verify=verify, proxies=proxies,
-                                   allow_redirects=allow_redirects, data=data, json=json_, cookies=cookies,stream=stream) as resp:
+                with requests.post(url, timeout=timeout, headers=headers if headers else get_headers('chrome'), verify=verify, proxies=proxies, allow_redirects=allow_redirects, data=data, json=json_, cookies=cookies,stream=stream) as resp:
                     return resp
-
         except Exception as e:
             if i == try_num - 1:
                 raise Exception(跟踪函数(-3)+' '+str(e))
 def curl(Copy_as_cURL_bash:str,文本:bool=False):
     '''copy->copy as cURL(bash)'''
     import uncurl
     if 文本:
         return uncurl.parse(Copy_as_cURL_bash)
     else:
         return eval(uncurl.parse(Copy_as_cURL_bash))
-def 获取_网络文件大小(网址,headers=None,proxies=None,cookies=None,verify=False,allow_redirects=True)->int:
+def 获取_网络文件大小(网址,headers=None,params=None,proxies=None,cookies=None,verify=False,allow_redirects=True)->int:
     proxies = proxies if proxies else default_proxies
     if headers and isinstance(headers,str):headers=dict_From_HeadersStr(headers)
     if cookies and isinstance(cookies,str):cookies=dict_From_CookieStr(cookies)
+    if params and isinstance(params,str):params=dict_From_HeadersStr(params)
     try:
-        with requests.get(网址, stream=True, headers=headers if headers else get_headers('chrome'), proxies=proxies, cookies=cookies,
-                          verify=verify,allow_redirects=allow_redirects) as resp:
+        with requests.get(网址, stream=True, headers=headers if headers else get_headers('chrome'),params=params, proxies=proxies, cookies=cookies, verify=verify,allow_redirects=allow_redirects) as resp:
             return resp.headers['content-length']
     except Exception as e:
         打印错误(e)
     return 0
-def 下载文件(文件路径: str = None, 网址: str = '', headers=None, proxies=None, verify=False, allow_redirects=True, cookies=None, try_num=3) -> int:
+def 下载文件(文件路径: str = None, 网址: str = '', headers=None,params=None, proxies=None, verify=False, allow_redirects=True, cookies=None, try_num=3) -> int:
     proxies = proxies if proxies else default_proxies
     if headers and isinstance(headers,str):headers=dict_From_HeadersStr(headers)
     if cookies and isinstance(cookies,str):cookies=dict_From_CookieStr(cookies)
+    if params and isinstance(params, str): params = dict_From_HeadersStr(params)
     if not 文件路径:
         文件路径 = 网址.rsplit('/', 1)[-1]
     for i in range(try_num):
         try:
-            with requests.get(网址, timeout=15, verify=verify, proxies=proxies, allow_redirects=allow_redirects, headers=headers if headers else get_headers('chrome'),
-                              cookies=cookies) as res:
+            with requests.get(网址, timeout=15, verify=verify, proxies=proxies, allow_redirects=allow_redirects, headers=headers if headers else get_headers('chrome'), params=params,cookies=cookies) as res:
                 if res.status_code == 200:
                     res = res.content
                     with open(文件路径, 'wb') as f:
                         f.write(res)
                     return len(res)
                 else:
                     if str(res.status_code) in http_err_code.keys():
                         raise Exception(res.status_code, ','.join(http_err_code[str(res.status_code)].values()))
                     else:
                         raise Exception('下载文件失败')
         except Exception as e:
             if i == (try_num - 1):
                 pcolor('下载文件错误:{},{}'.format(e.args, e.__traceback__.tb_lineno), 'error')
     return 0
-def 下载文件_进度条(文件路径: str = None, 网址: str = '', 分段长度: int = 5*1024, 多线程=False, 线程数=5, headers=None, proxies=None,allow_redirects=True, verify=False, cookies=None, 进度条函数=None, 打印错误=True, try_num=2) -> int:  # 分段长度 kb
+def 下载文件_进度条(文件路径: str = None, 网址: str = '', 分段长度: int = 5*1024, 多线程=False, 线程数=5, headers=None,params=None, proxies=None,allow_redirects=True, verify=False, cookies=None, 进度条函数=None, 打印错误=True, try_num=2) -> int:  # 分段长度 kb
     '''覆盖已存在的文件'''
     if not 文件路径:
         文件路径='默认文件名'
     proxies = proxies if proxies else default_proxies
     if headers and isinstance(headers,str):headers=dict_From_HeadersStr(headers)
     if cookies and isinstance(cookies,str):cookies=dict_From_CookieStr(cookies)
+    if params and isinstance(params, str): params = dict_From_HeadersStr(params)
     headers = headers if headers else get_headers('chrome')
     print('[ {} ] : {}'.format(scolor('下载文件', 'warn'), scolor(文件路径, 'yes')))
     for num in range(try_num):
         if not 文件路径:
             文件路径 = 网址.rsplit('/', 1)[-1]
         if os.path.exists(文件路径):
             os.remove(文件路径)
         try:
-            with requests.get(网址, stream=True, headers=headers, proxies=proxies, cookies=cookies, verify=verify,allow_redirects=allow_redirects) as resp:
+            with requests.get(网址, stream=True, headers=headers,params=params, proxies=proxies, cookies=cookies, verify=verify,allow_redirects=allow_redirects) as resp:
                 if 'content-length' in resp.headers:
                     size = int(resp.headers['content-length'])
                     chunk_size = 1024 * 分段长度  # 分段接收
                     c = size / chunk_size
                     total_size = c / 1024 * 分段长度
                     count = int(size / chunk_size) if size % chunk_size == 0 else int(size / chunk_size) + 1
                     start_time = time.time()
                     if 多线程:
                         n = 0
-
+                        flag_error=False
                         def get_one(网址, str_range):
                             nonlocal n
+                            nonlocal flag_error
+                            if flag_error:
+                                return None
                             head = headers.copy()
                             head['range'] = str_range
                             for i in range(try_num):
                                 try:
-                                    with requests.get(网址, stream=True, headers=head, proxies=proxies, cookies=cookies,
-                                                      verify=verify,allow_redirects=allow_redirects) as resp:
+                                    with requests.get(网址, stream=True, headers=head, proxies=proxies,params=params, cookies=cookies, verify=verify,allow_redirects=allow_redirects) as resp:
                                         content = resp.content
                                         if 进度条函数:
                                             进度条函数(int((n + 1) / count * 100), '{:.2f}mb'.format(total_size))
                                         t=time.time()-start_time
                                         seconds = t * count / (i + 1) - t
                                         if seconds<1:
                                             剩余时间 = ' '*12
@@ -1386,28 +1403,29 @@
                                             剩余时间 = ' {:0=2.0f}:{:0=2.0f}:{:0=2.0f}'.format(h,m,s)
                                         speed = '{:.2f}MB/S{}'.format(
                                             (n + 1) * chunk_size / 1024 / 1024 / t,剩余时间)
                                         打印_进度条('{:.2f}MB'.format(total_size), n, count, 1, 下载速度=speed)  # 步长1
                                         n += 1
                                         return content
                                 except:
-                                    return b''
-
+                                    pass
+                            flag_error=True
                         pool = ThreadPoolExecutor(max_workers=线程数)
                         tasks = []
                         for i in range(count):
                             if i == count - 1:
                                 r = 'bytes={}-'.format(chunk_size * i)
                             else:
                                 r = 'bytes={}-{}'.format(chunk_size * i, chunk_size * (i + 1) - 1)
                             tasks.append(pool.submit(get_one, 网址, r))
                         pool.shutdown(wait=True)
-                        with open(文件路径, mode='wb') as f:
-                            for task in tasks:
-                                f.write(task.result())
+                        if not flag_error:
+                            with open(文件路径, mode='wb') as f:
+                                for task in tasks:
+                                    f.write(task.result())
                         del tasks
                     else:
                         with open(文件路径, 'wb') as f:
                             for i, content in enumerate(resp.iter_content(chunk_size=chunk_size)):
                                 f.write(content)
                                 if 进度条函数:
                                     进度条函数(int((i + 1) / count * 100), '{:.2f}mb'.format(total_size))
@@ -1527,22 +1545,23 @@
         cmd += ' {}'.format(' '.join(lst))
     for i in range(try_num):
         if CMD_SYSTEM(cmd)==0:
             #没有文件夹 并且 存在文件 返回真
             if not os.path.exists(文件路径+'/') and os.path.exists(save_path):
                 return True
     return False
-def 获取_网络图片(图片网址: str, headers=None, proxies=None, cookies=None, verify=False,allow_redirects=True, pil=True, show=False, try_num=3) -> PILimage:
+def 获取_网络图片(图片网址: str, headers=None,params=None, proxies=None, cookies=None, verify=False,allow_redirects=True, pil=True, show=False, try_num=3) -> PILimage:
     '''获取网络图片("http://...")'''
     proxies = proxies if proxies else default_proxies
     if headers and isinstance(headers,str):headers=dict_From_HeadersStr(headers)
     if cookies and isinstance(cookies,str):cookies=dict_From_CookieStr(cookies)
+    if params and isinstance(params, str): params = dict_From_HeadersStr(params)
     for num in range(try_num):
         try:
-            with requests.get(图片网址, headers=headers if headers else get_headers('chrome'), proxies=proxies, cookies=cookies, verify=verify,allow_redirects=allow_redirects) as res:
+            with requests.get(图片网址, headers=headers if headers else get_headers('chrome'),params=params, proxies=proxies, cookies=cookies, verify=verify,allow_redirects=allow_redirects) as res:
                 if res.status_code == 200:
                     # 返回本地图片内存对象
                     # from PIL import Image
                     # img=Image.open(obj)  打开图片
                     # Image._show(img) 显示图片
                     img = BytesIO(res.content)
                     if pil:
@@ -1553,21 +1572,22 @@
                     else:
                         return img
                 else:
                     raise Exception('获取网络图片错误')
         except Exception as e:
             if num == (try_num - 1):
                 raise Exception('{},{}'.format(e.args, e.__traceback__.tb_lineno))
-def 获取_网络文件(文件网址: str, headers=None, proxies=None, cookies=None, verify=False,allow_redirects=True, try_num=3) -> bytes:
+def 获取_网络文件(文件网址: str, headers=None,params=None, proxies=None, cookies=None, verify=False,allow_redirects=True, try_num=3) -> bytes:
     proxies = proxies if proxies else default_proxies
     if headers and isinstance(headers, str): headers = dict_From_HeadersStr(headers)
     if cookies and isinstance(cookies, str): cookies = dict_From_CookieStr(cookies)
+    if params and isinstance(params, str): params = dict_From_HeadersStr(params)
     for num in range(try_num):
         try:
-            with requests.get(文件网址, headers=headers if headers else get_headers('chrome'), proxies=proxies, cookies=cookies, verify=verify,allow_redirects=allow_redirects) as res:
+            with requests.get(文件网址, headers=headers if headers else get_headers('chrome'),params=params, proxies=proxies, cookies=cookies, verify=verify,allow_redirects=allow_redirects) as res:
                 if res.status_code == 200:
                     return res.content
                 else:
                     raise Exception('获取网络文件错误')
         except Exception as e:
             if num == (try_num - 1):
                 raise Exception('{},{}'.format(e.args, e.__traceback__.tb_lineno))
```

### Comparing `spiderx-1.8.2/spiderx/tools.py` & `spiderx-1.8.9/spiderx/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+# encoding: utf-8
 import rsa
+#pip install pycryptodome
 from Crypto.Cipher import AES,DES,PKCS1_v1_5
 from Crypto.PublicKey import RSA
 from Crypto.Util.Padding import unpad,pad  #补位
-#b2a_hex 字符串->十六进制  a2b_hex 十六进制->字符串
 from binascii import b2a_hex, a2b_hex #
+from urllib.parse import urlparse
 from PIL import Image
 from uuid import uuid1
 from serial import Serial
 from .sx import *
 
 #需要第三方包的模块
 def add_block(content:bytes, block_size:int=16, style:bytes=b'\x00')->bytes:
@@ -308,73 +310,72 @@
                 lines=self.m3u8字符串
                 if self.show:
                     print('[ {} ] [ {} ] : {}'.format(scolor('文本'),scolor('视频链接'), self.url if self.url else '无视频链接'))
             else:
                 if self.show:
                     print('[ {} ] : {}'.format(scolor('视频链接'), self.url))
                 req_m3u8 = self.get_url(self.url, type_='url',stream=True)
-                req_headers = req_m3u8.headers
-                if 'content-type' in req_headers:
-                    #m3u8 类型
-                    if 'mpegurl' in req_headers['content-type'].lower() or 'text' in  req_headers['content-type'].lower():
-                        pass
-                    #其他类型
-                    else:
-                        # 返回文件长度
-                        return 下载文件_进度条(文件路径=self.fpath, 网址=self.url, 线程数=self.线程数, 多线程=True, 分段长度=10 * 1024)
 
-                lines = b''
-                for chunk in req_m3u8.iter_content(chunk_size=5 * 1024):
-                    lines += chunk
-                lines = lines.decode()  # 获取M3U8的文件内容
+                # 获取M3U8的文件内容  分段获取
+                lines = ''
+                try:
+                    for chunk in req_m3u8.iter_content(chunk_size=1 * 1024):
+                        # 假设是文本那么就可以转文本
+                        chunk = chunk.decode()
+                        lines += chunk
+                except:
+                    return 下载文件_进度条(文件路径=self.fpath, 网址=self.url, 线程数=self.线程数, 多线程=True, 分段长度=5 * 1024,headers=self.headers,try_num=self.try_num)
+
                 req_m3u8.close()
                 self.m3u8字符串 = lines
             # 读取文件里的每一行
             file_line = lines.split("\n")
             # 通过判断文件头来确定是否是M3U8文件
             if '#EXTM3U' not in file_line[0].upper():
                 raise Exception('非M3U8的链接')
             else:
                 self.链接前缀 = self.url.rsplit("/", 1)[0]
                 self.域名前缀 = '/'.join(self.url.split('/')[:3])
+                self.hostname = urlparse(self.url).hostname
+                self.http = urlparse(self.url).scheme
                 self.flag_域名前缀 = None
                 unknow = True  # 用来判断是否找到了下载的地址
                 n = 1
                 # ----------------------------------------------ts行
                 for index, line in enumerate(file_line):
                     if "EXTINF" in line:
                         unknow = False
                         ts_url=file_line[index+1]
                         if self.TS地址回调函数:  # 如果设置了回调
                             # def TS地址回调函数(line):return url
                             ts_url_new = self.TS地址回调函数(ts_url)
                         else:
-                            if 'http' not in ts_url and self.url:
-                                if ts_url[0] == '/':
-                                    ts_url_new = self.链接前缀 + ts_url
+                            ts_url=ts_url.lstrip('/')
+                            if 'http' not in ts_url and self.url.lower():
+
+                                if self.hostname in ts_url:
+                                    ts_url_new = f'{self.http}://' + ts_url
                                 else:
-                                    ts_url_new = self.链接前缀 + "/" + ts_url
+                                    ts_url_new = f"{self.链接前缀}/" + ts_url
 
                                 if self.flag_域名前缀 == None:
                                     try:
                                         req = self.get_url(ts_url_new, type_='ts',stream=True)
                                         code = req.status_code
                                     except:
                                         code = 404
 
                                     if code == 404:
                                         self.flag_域名前缀 = True
                                     else:
                                         self.flag_域名前缀 = False
 
                                 if self.flag_域名前缀:
-                                    if ts_url[0] == '/':
-                                        ts_url_new = self.域名前缀 + ts_url
-                                    else:
-                                        ts_url_new = self.域名前缀 + "/" + ts_url
+                                    ts_url_new =f"{self.域名前缀}/" + ts_url
+
                             else:
                                 ts_url_new = ts_url
                         if self.打印TS链接:
                             print(ts_url_new)
                         self.items.append({'i': n, 'url': ts_url_new})
                         n += 1
                 if unknow:
@@ -416,27 +417,53 @@
                     raise Exception('AES KEY 输入错误')
             else:
                 if 'URI' not in 加密信息:
                     raise Exception('没有URI链接地址')
                 if self.__uri_temp_data['uri'] == 加密信息['URI']:
                     KEY = self.__uri_temp_data['key']
                 else:
-                    KEY = self.get_url(加密信息['URI'],type_='uri').content  # 不加headers
+                    if self.URI地址回调函数:
+                        KEY = self.get_url(加密信息['URI'],type_='uri').content
+                    else:
+                        uri=加密信息['URI'].lstrip('/')
+                        #链接类型
+                        if '/' in uri:
+                            if 'http' in uri:
+                                uri_url=uri
+                            else:
+                                if self.hostname in uri:
+                                    uri_url=f'{self.http}://' + uri
+                                else:
+                                    if self.flag_域名前缀:
+                                        uri_url=f'{self.域名前缀}/'+uri
+                                    else:
+                                        uri_url = f'{self.链接前缀}/' + uri
+                            KEY = self.get_url(uri_url, type_='uri').content
+                        #非链接类型
+                        else:
+                            if len(uri)==16:
+                                KEY=uri.encode()
+                            if len(uri)==32:
+                                KEY=bytes.fromhex(uri)
+                            elif len(uri)==34:
+                                KEY = ytes.fromhex(uri[2:])
+                            else:
+                                raise Exception(f'URI错误:{uri} {len(uri)}')
                     if len(KEY) != 16:
-                        raise Exception('AES KEY 长度 {}'.format(len(KEY)))
+                        raise Exception(f'URI错误:{KEY} {len(KEY)}')
             if self.iv:  # 自定义iv判断类型 转成bytes
                 IV = self.iv
                 if type(IV) == list:
                     IV = bytes(IV)
                 elif type(IV) == bytes and len(IV) == 16:
                     pass
                 elif type(IV) == str and len(IV) == 34:
                     IV = bytes.fromhex(IV[2:])
                 else:
-                    raise Exception('AES IV 输入错误')
+                    raise Exception(f'IV错误:{IV} {len(IV)}')
             else:
                 if 'IV' in 加密信息 and 加密信息['IV']:
                     IV=加密信息['IV']
                     if len(IV) == 34:  # 16进制转成字节
                         IV = bytes.fromhex(IV[2:])
                     else:
                         IV = IV.encode() #转bytes
```

### Comparing `spiderx-1.8.2/spiderx/win32.py` & `spiderx-1.8.9/spiderx/win32.py`

 * *Files identical despite different names*


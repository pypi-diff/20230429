# Comparing `tmp/gqylpy_log-1.0.4.tar.gz` & `tmp/gqylpy_log-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqylpy_log-1.0.4.tar", last modified: Sat Apr 15 04:48:04 2023, max compression
+gzip compressed data, was "gqylpy_log-1.1.tar", last modified: Sat Apr 29 02:03:23 2023, max compression
```

## Comparing `gqylpy_log-1.0.4.tar` & `gqylpy_log-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:48:04.567498 gqylpy_log-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-04-15 04:47:51.000000 gqylpy_log-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-15 04:48:04.567498 gqylpy_log-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-15 04:47:51.000000 gqylpy_log-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:48:04.567498 gqylpy_log-1.0.4/gqylpy_log/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-15 04:47:51.000000 gqylpy_log-1.0.4/gqylpy_log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-15 04:47:51.000000 gqylpy_log-1.0.4/gqylpy_log/g log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:48:04.567498 gqylpy_log-1.0.4/gqylpy_log.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-15 04:48:04.000000 gqylpy_log-1.0.4/gqylpy_log.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-15 04:48:04.000000 gqylpy_log-1.0.4/gqylpy_log.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 04:48:04.000000 gqylpy_log-1.0.4/gqylpy_log.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 04:48:04.000000 gqylpy_log-1.0.4/gqylpy_log.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 04:48:04.567498 gqylpy_log-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-15 04:47:51.000000 gqylpy_log-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:03:23.085207 gqylpy_log-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-04-29 02:03:11.000000 gqylpy_log-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-29 02:03:23.085207 gqylpy_log-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-29 02:03:11.000000 gqylpy_log-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:03:23.085207 gqylpy_log-1.1/gqylpy_log/
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-04-29 02:03:11.000000 gqylpy_log-1.1/gqylpy_log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-29 02:03:11.000000 gqylpy_log-1.1/gqylpy_log/g log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:03:23.085207 gqylpy_log-1.1/gqylpy_log.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-29 02:03:23.000000 gqylpy_log-1.1/gqylpy_log.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-29 02:03:23.000000 gqylpy_log-1.1/gqylpy_log.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 02:03:23.000000 gqylpy_log-1.1/gqylpy_log.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 02:03:23.000000 gqylpy_log-1.1/gqylpy_log.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 02:03:23.085207 gqylpy_log-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-29 02:03:11.000000 gqylpy_log-1.1/setup.py
```

### Comparing `gqylpy_log-1.0.4/LICENSE` & `gqylpy_log-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gqylpy_log-1.0.4/PKG-INFO` & `gqylpy_log-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqylpy_log
-Version: 1.0.4
+Version: 1.1
 Summary: 二次封装 logging，更方便快捷的创建日志记录器。使用 gqylpy_log 模块可以快速创建 logging.Logger 实例并完成一系列的日志配置，使你的代码更简洁。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-log
 Classifier: Environment :: Web Environment
@@ -25,15 +25,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-log.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-log/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_log)](https://pypi.org/project/gqylpy_log)
 [![License](https://img.shields.io/pypi/l/gqylpy_log)](https://github.com/gqylpy/gqylpy-log/blob/master/LICENSE)
-[![Downloads](https://pepy.tech/badge/gqylpy_log/month)](https://pepy.tech/project/gqylpy_log)
+[![Downloads](https://pepy.tech/badge/gqylpy_log)](https://pepy.tech/project/gqylpy_log)
 
 # gqylpy-log
 
 > 二次封装 `logging`，更方便快捷的创建日志记录器。使用 `gqylpy_log` 模块可以快速创建 `logging.Logger` 实例并完成一系列的日志配置，使你的代码更简洁。  
 > > 另外 `gqylpy_log` 中还内置了一个基于 `logging.StreamHandler` 的日志记录器，你可以直接调用它，它是在你第一次调用时自动创建的，前提是你未创建任何指定了参数 `gname` 的日志记录器，否则会使用你第一次创建的指定了参数 `ganme` 的日志记录器作为默认日志记录器，并自动替换和销毁掉内置的日志记录器。
 
 <kbd>pip3 install gqylpy_log</kbd>
@@ -44,15 +44,15 @@
 
 glog.debug(...)
 glog.info(...)
 glog.warning(...)
 glog.error(...)
 glog.critical(...)
 ```
-像上面这样直接调用，使用的便是内置的日志记录器，它的配置信息是这样的：
+像上面这样直接调用，使用的便是内置的日志记录器，它的默认配置是这样的：
 ```python
 level   = 'NOTSET'
 output  = 'stream'
 logfile = '/var/log/{default is your startup filename}.log'
 datefmt = '%F %T'
 logfmt  = '[%(asctime)s] [%(module)s.%(funcName)s.line%(lineno)d] [%(levelname)s] %(message)s'
 ```
```

### Comparing `gqylpy_log-1.0.4/README.md` & `gqylpy_log-1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-log.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-log/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_log)](https://pypi.org/project/gqylpy_log)
 [![License](https://img.shields.io/pypi/l/gqylpy_log)](https://github.com/gqylpy/gqylpy-log/blob/master/LICENSE)
-[![Downloads](https://pepy.tech/badge/gqylpy_log/month)](https://pepy.tech/project/gqylpy_log)
+[![Downloads](https://pepy.tech/badge/gqylpy_log)](https://pepy.tech/project/gqylpy_log)
 
 # gqylpy-log
 
 > 二次封装 `logging`，更方便快捷的创建日志记录器。使用 `gqylpy_log` 模块可以快速创建 `logging.Logger` 实例并完成一系列的日志配置，使你的代码更简洁。  
 > > 另外 `gqylpy_log` 中还内置了一个基于 `logging.StreamHandler` 的日志记录器，你可以直接调用它，它是在你第一次调用时自动创建的，前提是你未创建任何指定了参数 `gname` 的日志记录器，否则会使用你第一次创建的指定了参数 `ganme` 的日志记录器作为默认日志记录器，并自动替换和销毁掉内置的日志记录器。
 
 <kbd>pip3 install gqylpy_log</kbd>
@@ -17,15 +17,15 @@
 
 glog.debug(...)
 glog.info(...)
 glog.warning(...)
 glog.error(...)
 glog.critical(...)
 ```
-像上面这样直接调用，使用的便是内置的日志记录器，它的配置信息是这样的：
+像上面这样直接调用，使用的便是内置的日志记录器，它的默认配置是这样的：
 ```python
 level   = 'NOTSET'
 output  = 'stream'
 logfile = '/var/log/{default is your startup filename}.log'
 datefmt = '%F %T'
 logfmt  = '[%(asctime)s] [%(module)s.%(funcName)s.line%(lineno)d] [%(levelname)s] %(message)s'
 ```
```

### Comparing `gqylpy_log-1.0.4/gqylpy_log/g log.py` & `gqylpy_log-1.1/gqylpy_log/g log.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                        '[%(levelname)s] %(message)s',
         datefmt: str = '%F %T',
         logfile: str = None,
         gname:   str = None
 ) -> logging.Logger:
     if output.replace(' ', '') not in \
             ("stream", "file", "stream,file", "file,stream"):
-        raise type('ParameterError', (TypeError,), {'__module__': 'builtins'})(
+        raise TypeError(
             'parameter "output" can only be "stream", "file", or '
             f'"file,stream", not "{output}"'
         )
 
     logger    = logging.Logger(name, level)
     formatter = logging.Formatter(logfmt, datefmt)
 
@@ -67,15 +67,22 @@
             gcode.__first__ = logger
         setattr(gpack, gname, logger)
 
     return logger
 
 
 def __call__(func):
-    def inner(msg, *, gname: (str, logging.Logger) = None, **kw):
+    def inner(
+            *msg,
+            sep:     str  = ' ',
+            oneline: bool = False,
+            linesep: str  = '; ',
+            gname:   (str, logging.Logger) = None,
+            **kw
+    ):
         if gname is None:
             if not hasattr(gcode, '__first__'):
                 gobj: logging.Logger = __init__(
                     name='built-in',
                     level=gpack.level,
                     output=gpack.output,
                     logfmt=gpack.logfmt,
@@ -91,34 +98,38 @@
             gobj: logging.Logger = getattr(gpack, gname, None)
             if gobj.__class__ is not logging.Logger:
                 raise NameError(f'gname "{gname}" not found in {__package__}.')
         elif gname.__class__ is logging.Logger:
             gobj: logging.Logger = gname
         else:
             raise TypeError(
-                'parameter "gname" type must be a "str" or "logging.Logger", '
+                'parameter "gname" type must be "str" or "logging.Logger", '
                 f'not "{gname.__class__.__name__}".'
             )
 
         if sys.version_info >= (3, 8):
             if 'stacklevel' in kw:
                 if kw['stacklevel'].__class__ is not int:
                     if not kw['stacklevel'].isdigit():
                         raise TypeError(
-                            'Parameter "stacklevel" type must be a "int", '
+                            'parameter "stacklevel" type must be "int", '
                             f'not "{kw["stacklevel"].__class__.__name__}".'
                         )
                     kw['stacklevel'] = int(kw['stacklevel'])
                 if kw['stacklevel'] < 2:
                     kw['stacklevel'] = 2
             else:
                 kw['stacklevel'] = 2
 
-        if msg.__class__ is str:
-            msg = msg.strip()
+        msg: str = sep.join(str(m) for m in msg)
+
+        if oneline:
+            msg: str = linesep.join(
+                m.strip() for m in msg.split('\n') if m and not m.isspace()
+            )
 
         getattr(gobj, func.__name__)(msg, **kw)
 
     return inner
 
 
 @__call__
```

### Comparing `gqylpy_log-1.0.4/gqylpy_log.egg-info/PKG-INFO` & `gqylpy_log-1.1/gqylpy_log.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqylpy-log
-Version: 1.0.4
+Version: 1.1
 Summary: 二次封装 logging，更方便快捷的创建日志记录器。使用 gqylpy_log 模块可以快速创建 logging.Logger 实例并完成一系列的日志配置，使你的代码更简洁。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-log
 Classifier: Environment :: Web Environment
@@ -25,15 +25,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-log.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-log/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_log)](https://pypi.org/project/gqylpy_log)
 [![License](https://img.shields.io/pypi/l/gqylpy_log)](https://github.com/gqylpy/gqylpy-log/blob/master/LICENSE)
-[![Downloads](https://pepy.tech/badge/gqylpy_log/month)](https://pepy.tech/project/gqylpy_log)
+[![Downloads](https://pepy.tech/badge/gqylpy_log)](https://pepy.tech/project/gqylpy_log)
 
 # gqylpy-log
 
 > 二次封装 `logging`，更方便快捷的创建日志记录器。使用 `gqylpy_log` 模块可以快速创建 `logging.Logger` 实例并完成一系列的日志配置，使你的代码更简洁。  
 > > 另外 `gqylpy_log` 中还内置了一个基于 `logging.StreamHandler` 的日志记录器，你可以直接调用它，它是在你第一次调用时自动创建的，前提是你未创建任何指定了参数 `gname` 的日志记录器，否则会使用你第一次创建的指定了参数 `ganme` 的日志记录器作为默认日志记录器，并自动替换和销毁掉内置的日志记录器。
 
 <kbd>pip3 install gqylpy_log</kbd>
@@ -44,15 +44,15 @@
 
 glog.debug(...)
 glog.info(...)
 glog.warning(...)
 glog.error(...)
 glog.critical(...)
 ```
-像上面这样直接调用，使用的便是内置的日志记录器，它的配置信息是这样的：
+像上面这样直接调用，使用的便是内置的日志记录器，它的默认配置是这样的：
 ```python
 level   = 'NOTSET'
 output  = 'stream'
 logfile = '/var/log/{default is your startup filename}.log'
 datefmt = '%F %T'
 logfmt  = '[%(asctime)s] [%(module)s.%(funcName)s.line%(lineno)d] [%(levelname)s] %(message)s'
 ```
```

### Comparing `gqylpy_log-1.0.4/setup.py` & `gqylpy_log-1.1/setup.py`

 * *Files identical despite different names*


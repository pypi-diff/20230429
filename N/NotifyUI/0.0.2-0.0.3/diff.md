# Comparing `tmp/NotifyUI-0.0.2.tar.gz` & `tmp/NotifyUI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NotifyUI-0.0.2.tar", last modified: Wed Apr 26 17:04:02 2023, max compression
+gzip compressed data, was "NotifyUI-0.0.3.tar", last modified: Sat Apr 29 07:52:33 2023, max compression
```

## Comparing `NotifyUI-0.0.2.tar` & `NotifyUI-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:04:02.633781 NotifyUI-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    12654 2023-04-26 17:03:34.000000 NotifyUI-0.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:04:02.629781 NotifyUI-0.0.2/NotifyUI/
--rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-04-26 17:03:34.000000 NotifyUI-0.0.2/NotifyUI/NotifyElements.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:34.000000 NotifyUI-0.0.2/NotifyUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:04:02.633781 NotifyUI-0.0.2/NotifyUI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-04-26 17:04:02.000000 NotifyUI-0.0.2/NotifyUI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-26 17:04:02.000000 NotifyUI-0.0.2/NotifyUI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:04:02.000000 NotifyUI-0.0.2/NotifyUI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 17:04:02.000000 NotifyUI-0.0.2/NotifyUI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 17:04:02.000000 NotifyUI-0.0.2/NotifyUI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-04-26 17:04:02.633781 NotifyUI-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-04-26 17:03:34.000000 NotifyUI-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:04:02.633781 NotifyUI-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-26 17:03:34.000000 NotifyUI-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 07:52:33.534804 NotifyUI-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    12654 2023-04-29 07:52:21.000000 NotifyUI-0.0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 07:52:33.534804 NotifyUI-0.0.3/NotifyUI/
+-rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-04-29 07:52:21.000000 NotifyUI-0.0.3/NotifyUI/NotifyElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 07:52:21.000000 NotifyUI-0.0.3/NotifyUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 07:52:33.534804 NotifyUI-0.0.3/NotifyUI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-04-29 07:52:33.000000 NotifyUI-0.0.3/NotifyUI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-29 07:52:33.000000 NotifyUI-0.0.3/NotifyUI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 07:52:33.000000 NotifyUI-0.0.3/NotifyUI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 07:52:33.000000 NotifyUI-0.0.3/NotifyUI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 07:52:33.000000 NotifyUI-0.0.3/NotifyUI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-04-29 07:52:33.534804 NotifyUI-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-04-29 07:52:21.000000 NotifyUI-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 07:52:33.534804 NotifyUI-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-29 07:52:21.000000 NotifyUI-0.0.3/setup.py
```

### Comparing `NotifyUI-0.0.2/LICENSE` & `NotifyUI-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NotifyUI-0.0.2/NotifyUI/NotifyElements.py` & `NotifyUI-0.0.3/NotifyUI/NotifyElements.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     Note:- Declare this as a variable to keep the timer alive.
     """
 
     time = QTime(0, 0, 0)
     end_time = QTime(0, 0, 0)
 
-    def __init__(self, call_at_end: function, end_qtime: QTime, *args, **kargs) -> None:
+    def __init__(self, call_at_end, end_qtime: QTime, *args, **kargs) -> None:
         self.timer = QTimer()
         self.call_at_end = call_at_end
         self.end_time = end_qtime
         self.args = args[2:]
         self.kargs = kargs
         self.timer.timeout.connect(self.callbackFunc)
         self.timer.start(1000)
```

### Comparing `NotifyUI-0.0.2/NotifyUI.egg-info/PKG-INFO` & `NotifyUI-0.0.3/NotifyUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NotifyUI
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Notification library integrated with PyQt6
 Home-page: https://github.com/chetan0402/NotifyUI
 Author: Chetan0402
 License: CC BY 4.0
 Classifier: Programming Language :: Python :: 3
 Requires: PyQt6
 Description-Content-Type: text/markdown
```

### Comparing `NotifyUI-0.0.2/PKG-INFO` & `NotifyUI-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NotifyUI
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Notification library integrated with PyQt6
 Home-page: https://github.com/chetan0402/NotifyUI
 Author: Chetan0402
 License: CC BY 4.0
 Classifier: Programming Language :: Python :: 3
 Requires: PyQt6
 Description-Content-Type: text/markdown
```

### Comparing `NotifyUI-0.0.2/README.md` & `NotifyUI-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `NotifyUI-0.0.2/setup.py` & `NotifyUI-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="NotifyUI",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     url="https://github.com/chetan0402/NotifyUI",
     license="CC BY 4.0",
     author="Chetan0402",
     description="Python Notification library integrated with PyQt6",
     long_description=long_description,
     long_description_content_type="text/markdown",
```


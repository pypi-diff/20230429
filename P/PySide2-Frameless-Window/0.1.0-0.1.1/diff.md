# Comparing `tmp/PySide2-Frameless-Window-0.1.0.tar.gz` & `tmp/PySide2-Frameless-Window-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide2-Frameless-Window-0.1.0.tar", last modified: Mon Apr 17 07:28:47 2023, max compression
+gzip compressed data, was "dist\PySide2-Frameless-Window-0.1.1.tar", last modified: Sat Apr 29 16:04:25 2023, max compression
```

## Comparing `PySide2-Frameless-Window-0.1.0.tar` & `PySide2-Frameless-Window-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 07:28:47.540415 PySide2-Frameless-Window-0.1.0/
--rw-rw-rw-   0        0        0     7815 2023-04-17 07:22:03.000000 PySide2-Frameless-Window-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     5496 2023-04-17 07:28:47.538566 PySide2-Frameless-Window-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 07:28:47.497669 PySide2-Frameless-Window-0.1.0/PySide2_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5496 2023-04-17 07:28:47.000000 PySide2-Frameless-Window-0.1.0/PySide2_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-04-17 07:28:47.000000 PySide2-Frameless-Window-0.1.0/PySide2_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 07:28:47.000000 PySide2-Frameless-Window-0.1.0/PySide2_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-04-17 07:28:47.000000 PySide2-Frameless-Window-0.1.0/PySide2_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-17 07:28:47.000000 PySide2-Frameless-Window-0.1.0/PySide2_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4906 2023-04-17 07:27:02.000000 PySide2-Frameless-Window-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 07:28:47.499861 PySide2-Frameless-Window-0.1.0/qframelesswindow/
--rw-rw-rw-   0        0        0     2251 2023-04-17 07:27:29.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:28:47.505424 PySide2-Frameless-Window-0.1.0/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2730 2023-04-17 07:27:02.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:28:47.509830 PySide2-Frameless-Window-0.1.0/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     2878 2023-04-17 07:27:02.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     2683 2023-04-17 07:27:02.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:28:47.515355 PySide2-Frameless-Window-0.1.0/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     3024 2023-04-17 07:27:02.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4085 2023-04-17 07:27:02.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:28:47.519631 PySide2-Frameless-Window-0.1.0/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     4942 2023-04-17 07:27:02.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9039 2023-04-17 07:27:02.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:28:47.528371 PySide2-Frameless-Window-0.1.0/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     1216 2023-04-17 07:27:02.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1844 2023-04-17 07:27:02.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     7973 2023-04-17 07:27:33.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:28:47.536500 PySide2-Frameless-Window-0.1.0/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     6806 2023-04-17 07:27:02.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4013 2023-04-17 07:27:02.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8346 2023-04-17 07:27:02.000000 PySide2-Frameless-Window-0.1.0/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-04-17 07:28:47.540415 PySide2-Frameless-Window-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1001 2023-04-17 07:27:22.000000 PySide2-Frameless-Window-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.734097 PySide2-Frameless-Window-0.1.1/
+-rw-rw-rw-   0        0        0     7815 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5496 2023-04-29 16:04:25.733096 PySide2-Frameless-Window-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.682230 PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5496 2023-04-29 16:04:25.000000 PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-04-29 16:04:25.000000 PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 16:04:25.000000 PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-04-29 16:04:25.000000 PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-29 16:04:25.000000 PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4906 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.692734 PySide2-Frameless-Window-0.1.1/qframelesswindow/
+-rw-rw-rw-   0        0        0     2251 2023-04-29 16:03:35.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.697582 PySide2-Frameless-Window-0.1.1/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2730 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.702695 PySide2-Frameless-Window-0.1.1/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     2878 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     2683 2023-04-27 01:27:44.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.707445 PySide2-Frameless-Window-0.1.1/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     3024 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4085 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.713342 PySide2-Frameless-Window-0.1.1/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     4942 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9039 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.723432 PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     1216 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1844 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     7973 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:04:25.729934 PySide2-Frameless-Window-0.1.1/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     7078 2023-04-29 16:01:31.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4013 2023-04-27 01:27:44.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     8346 2023-04-29 15:59:29.000000 PySide2-Frameless-Window-0.1.1/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-04-29 16:04:25.734097 PySide2-Frameless-Window-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1001 2023-04-29 16:03:39.000000 PySide2-Frameless-Window-0.1.1/setup.py
```

### Comparing `PySide2-Frameless-Window-0.1.0/LICENSE` & `PySide2-Frameless-Window-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/PKG-INFO` & `PySide2-Frameless-Window-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Frameless-Window
-Version: 0.1.0
+Version: 0.1.1
 Summary: A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside2 frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PySide2-Frameless-Window-0.1.0/PySide2_Frameless_Window.egg-info/PKG-INFO` & `PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Frameless-Window
-Version: 0.1.0
+Version: 0.1.1
 Summary: A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside2 frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PySide2-Frameless-Window-0.1.0/PySide2_Frameless_Window.egg-info/SOURCES.txt` & `PySide2-Frameless-Window-0.1.1/PySide2_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/README.md` & `PySide2-Frameless-Window-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/__init__.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: LGPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 import sys
 
 from PySide2.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
```

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/_rc/resource.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/linux/__init__.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/linux/window_effect.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/mac/__init__.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/mac/window_effect.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/titlebar/__init__.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/titlebar/title_bar_buttons.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/utils/__init__.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/utils/linux_utils.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/utils/mac_utils.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/utils/win32_utils.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/windows/__init__.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/windows/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,18 @@
         self.windowEffect = WindowsWindowEffect(self)
         self.titleBar = TitleBar(self)
         self._isResizeEnabled = True
 
         # remove window border
         if not win_utils.isWin7():
             self.setWindowFlags(self.windowFlags() | Qt.FramelessWindowHint)
+        elif self.parent():
+            self.setWindowFlags(self.parent().windowFlags() | Qt.FramelessWindowHint | Qt.WindowMinMaxButtonsHint)
         else:
-            self.setWindowFlags(Qt.FramelessWindowHint |
-                                Qt.WindowMinMaxButtonsHint)
+            self.setWindowFlags(Qt.FramelessWindowHint | Qt.WindowMinMaxButtonsHint)
 
         # add DWM shadow and window animation
         self.windowEffect.addWindowAnimation(self.winId())
         if not isinstance(self, AcrylicWindow):
             self.windowEffect.addShadowEffect(self.winId())
 
         # solve issue #5
@@ -149,16 +150,20 @@
     def __init__(self, parent=None):
         super().__init__(parent=parent)
         self.__closedByKey = False
 
     def _initFrameless(self):
         super()._initFrameless()
         QtWin.enableBlurBehindWindow(self)
-        self.setWindowFlags(Qt.FramelessWindowHint |
-                            Qt.WindowMinMaxButtonsHint)
+
+        if win_utils.isWin7() and self.parent():
+            self.setWindowFlags(self.parent().windowFlags() | Qt.FramelessWindowHint | Qt.WindowMinMaxButtonsHint)
+        else:
+            self.setWindowFlags(Qt.FramelessWindowHint | Qt.WindowMinMaxButtonsHint)
+
         self.windowEffect.addWindowAnimation(self.winId())
 
         if win_utils.isWin7():
             self.windowEffect.addShadowEffect(self.winId())
             self.windowEffect.setAeroEffect(self.winId())
         else:
             self.windowEffect.setAcrylicEffect(self.winId())
```

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/windows/c_structures.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/qframelesswindow/windows/window_effect.py` & `PySide2-Frameless-Window-0.1.1/qframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.1.0/setup.py` & `PySide2-Frameless-Window-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide2-Frameless-Window",
-    version="0.1.0",
+    version="0.1.1",
     keywords="pyside2 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="LGPLv3",
```


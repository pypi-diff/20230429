# Comparing `tmp/PyQt5-Frameless-Window-0.2.5.tar.gz` & `tmp/PyQt5-Frameless-Window-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt5-Frameless-Window-0.2.5.tar", last modified: Mon Apr 17 07:13:39 2023, max compression
+gzip compressed data, was "dist\PyQt5-Frameless-Window-0.2.6.tar", last modified: Sat Apr 29 15:58:52 2023, max compression
```

## Comparing `PyQt5-Frameless-Window-0.2.5.tar` & `PyQt5-Frameless-Window-0.2.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.696361 PyQt5-Frameless-Window-0.2.5/
--rw-rw-rw-   0        0        0    35823 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     5051 2023-04-17 07:13:39.695228 PyQt5-Frameless-Window-0.2.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.654105 PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5051 2023-04-17 07:13:39.000000 PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-04-17 07:13:39.000000 PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 07:13:39.000000 PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-04-17 07:13:39.000000 PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-17 07:13:39.000000 PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4481 2023-04-14 02:48:03.000000 PyQt5-Frameless-Window-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.656305 PyQt5-Frameless-Window-0.2.5/qframelesswindow/
--rw-rw-rw-   0        0        0     1616 2023-04-17 07:12:34.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.660694 PyQt5-Frameless-Window-0.2.5/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.665463 PyQt5-Frameless-Window-0.2.5/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     2891 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     2683 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.670902 PyQt5-Frameless-Window-0.2.5/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     2994 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     3898 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.674582 PyQt5-Frameless-Window-0.2.5/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     4984 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9057 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.684873 PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     5299 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1850 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     8190 2023-04-17 06:53:54.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:13:39.692056 PyQt5-Frameless-Window-0.2.5/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     6715 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4013 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8344 2023-04-14 02:47:40.000000 PyQt5-Frameless-Window-0.2.5/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-04-17 07:13:39.696361 PyQt5-Frameless-Window-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-04-17 07:12:27.000000 PyQt5-Frameless-Window-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.260164 PyQt5-Frameless-Window-0.2.6/
+-rw-rw-rw-   0        0        0    35823 2023-04-27 01:27:43.000000 PyQt5-Frameless-Window-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     5051 2023-04-29 15:58:52.259155 PyQt5-Frameless-Window-0.2.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.222398 PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5051 2023-04-29 15:58:51.000000 PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-04-29 15:58:52.000000 PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 15:58:51.000000 PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-04-29 15:58:51.000000 PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-29 15:58:51.000000 PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4481 2023-04-27 01:27:43.000000 PyQt5-Frameless-Window-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.224504 PyQt5-Frameless-Window-0.2.6/qframelesswindow/
+-rw-rw-rw-   0        0        0     1616 2023-04-29 15:58:33.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.228510 PyQt5-Frameless-Window-0.2.6/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.232684 PyQt5-Frameless-Window-0.2.6/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     2891 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     2683 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.237120 PyQt5-Frameless-Window-0.2.6/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     2994 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     3898 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.241467 PyQt5-Frameless-Window-0.2.6/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     4984 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9057 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.250211 PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     5299 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1850 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8190 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:58:52.256726 PyQt5-Frameless-Window-0.2.6/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     6975 2023-04-29 15:57:34.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4013 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     8344 2023-04-27 01:27:44.000000 PyQt5-Frameless-Window-0.2.6/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-04-29 15:58:52.261214 PyQt5-Frameless-Window-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-04-29 15:58:28.000000 PyQt5-Frameless-Window-0.2.6/setup.py
```

### Comparing `PyQt5-Frameless-Window-0.2.5/LICENSE` & `PyQt5-Frameless-Window-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/PKG-INFO` & `PyQt5-Frameless-Window-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt5-Frameless-Window
-Version: 0.2.5
+Version: 0.2.6
 Summary: A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/PKG-INFO` & `PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt5-Frameless-Window
-Version: 0.2.5
+Version: 0.2.6
 Summary: A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt frameless
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyQt5-Frameless-Window-0.2.5/PyQt5_Frameless_Window.egg-info/SOURCES.txt` & `PyQt5-Frameless-Window-0.2.6/PyQt5_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/README.md` & `PyQt5-Frameless-Window-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/__init__.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/master/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 import sys
 
 from PyQt5.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
```

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/_rc/resource.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/linux/__init__.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/linux/window_effect.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/mac/__init__.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/mac/window_effect.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/titlebar/__init__.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/titlebar/title_bar_buttons.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/__init__.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/linux_utils.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/mac_utils.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/utils/win32_utils.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/windows/__init__.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/windows/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,17 +28,18 @@
         self.windowEffect = WindowsWindowEffect(self)
         self.titleBar = TitleBar(self)
         self._isResizeEnabled = True
 
         # remove window border
         if not win_utils.isWin7():
             self.setWindowFlags(self.windowFlags() | Qt.FramelessWindowHint)
+        elif parent:
+            self.setWindowFlags(parent.windowFlags() | Qt.FramelessWindowHint | Qt.WindowMinMaxButtonsHint)
         else:
-            self.setWindowFlags(Qt.FramelessWindowHint |
-                                Qt.WindowMinMaxButtonsHint)
+            self.setWindowFlags(Qt.FramelessWindowHint | Qt.WindowMinMaxButtonsHint)
 
         # add DWM shadow and window animation
         self.windowEffect.addWindowAnimation(self.winId())
         if not isinstance(self, AcrylicWindow):
             self.windowEffect.addShadowEffect(self.winId())
 
         # solve issue #5
@@ -145,16 +146,20 @@
     """ A frameless window with acrylic effect """
 
     def __init__(self, parent=None):
         super().__init__(parent=parent)
         self.__closedByKey = False
 
         QtWin.enableBlurBehindWindow(self)
-        self.setWindowFlags(Qt.FramelessWindowHint |
-                            Qt.WindowMinMaxButtonsHint)
+        
+        if win_utils.isWin7() and parent:
+            self.setWindowFlags(parent.windowFlags() | Qt.FramelessWindowHint | Qt.WindowMinMaxButtonsHint)
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

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/windows/c_structures.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/qframelesswindow/windows/window_effect.py` & `PyQt5-Frameless-Window-0.2.6/qframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `PyQt5-Frameless-Window-0.2.5/setup.py` & `PyQt5-Frameless-Window-0.2.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt5-Frameless-Window",
-    version="0.2.5",
+    version="0.2.6",
     keywords="pyqt frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyqt5, support Win32, X11, Wayland and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```


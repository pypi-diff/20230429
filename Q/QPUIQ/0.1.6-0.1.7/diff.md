# Comparing `tmp/QPUIQ-0.1.6.tar.gz` & `tmp/QPUIQ-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QPUIQ-0.1.6.tar", last modified: Sat Apr 29 20:14:38 2023, max compression
+gzip compressed data, was "QPUIQ-0.1.7.tar", last modified: Sat Apr 29 21:13:42 2023, max compression
```

## Comparing `QPUIQ-0.1.6.tar` & `QPUIQ-0.1.7.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 20:14:38.745086 QPUIQ-0.1.6/
--rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.1.6/LICENSE.txt
--rw-r--r--   0 Bug        (504) staff       (20)     2885 2023-04-29 20:14:38.744945 QPUIQ-0.1.6/PKG-INFO
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 20:14:38.731565 QPUIQ-0.1.6/PUI/
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 20:14:38.734530 QPUIQ-0.1.6/PUI/PySide6/
--rw-r--r--   0 Bug        (504) staff       (20)      857 2023-04-29 20:10:13.000000 QPUIQ-0.1.6/PUI/PySide6/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      498 2023-04-29 18:30:29.000000 QPUIQ-0.1.6/PUI/PySide6/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     1188 2023-04-29 16:10:01.000000 QPUIQ-0.1.6/PUI/PySide6/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-29 06:22:40.000000 QPUIQ-0.1.6/PUI/PySide6/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     2138 2023-04-29 14:36:14.000000 QPUIQ-0.1.6/PUI/PySide6/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:43:52.000000 QPUIQ-0.1.6/PUI/PySide6/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      543 2023-04-26 17:57:33.000000 QPUIQ-0.1.6/PUI/PySide6/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:43:58.000000 QPUIQ-0.1.6/PUI/PySide6/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:06.000000 QPUIQ-0.1.6/PUI/PySide6/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1299 2023-04-29 16:58:24.000000 QPUIQ-0.1.6/PUI/PySide6/window.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 20:14:38.737173 QPUIQ-0.1.6/PUI/Qt5/
--rw-r--r--   0 Bug        (504) staff       (20)      417 2023-04-29 17:06:45.000000 QPUIQ-0.1.6/PUI/Qt5/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      496 2023-04-29 18:30:13.000000 QPUIQ-0.1.6/PUI/Qt5/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     1139 2023-04-29 17:07:47.000000 QPUIQ-0.1.6/PUI/Qt5/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-23 17:44:21.000000 QPUIQ-0.1.6/PUI/Qt5/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1527 2023-04-26 17:40:36.000000 QPUIQ-0.1.6/PUI/Qt5/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:44:32.000000 QPUIQ-0.1.6/PUI/Qt5/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      541 2023-03-13 15:01:12.000000 QPUIQ-0.1.6/PUI/Qt5/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:44:38.000000 QPUIQ-0.1.6/PUI/Qt5/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:41.000000 QPUIQ-0.1.6/PUI/Qt5/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1297 2023-04-29 17:05:56.000000 QPUIQ-0.1.6/PUI/Qt5/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      486 2023-04-29 20:14:17.000000 QPUIQ-0.1.6/PUI/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      458 2023-04-29 06:46:04.000000 QPUIQ-0.1.6/PUI/decorator.py
--rw-r--r--   0 Bug        (504) staff       (20)     2627 2023-04-29 19:40:07.000000 QPUIQ-0.1.6/PUI/dom.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 20:14:38.739843 QPUIQ-0.1.6/PUI/flet/
--rw-r--r--   0 Bug        (504) staff       (20)      452 2023-04-29 19:08:30.000000 QPUIQ-0.1.6/PUI/flet/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      551 2023-04-29 19:19:55.000000 QPUIQ-0.1.6/PUI/flet/application.py
--rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.1.6/PUI/flet/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      647 2023-03-15 07:54:51.000000 QPUIQ-0.1.6/PUI/flet/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.1.6/PUI/flet/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      943 2023-04-14 18:19:33.000000 QPUIQ-0.1.6/PUI/flet/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:58:06.000000 QPUIQ-0.1.6/PUI/flet/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.1.6/PUI/flet/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      482 2023-04-29 19:19:13.000000 QPUIQ-0.1.6/PUI/flet/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     3827 2023-04-29 17:35:11.000000 QPUIQ-0.1.6/PUI/node.py
--rw-r--r--   0 Bug        (504) staff       (20)     8766 2023-04-29 09:38:11.000000 QPUIQ-0.1.6/PUI/state.py
--rw-r--r--   0 Bug        (504) staff       (20)      983 2023-03-16 07:50:08.000000 QPUIQ-0.1.6/PUI/timeline.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 20:14:38.742165 QPUIQ-0.1.6/PUI/tkinter/
--rw-r--r--   0 Bug        (504) staff       (20)      414 2023-04-29 18:25:14.000000 QPUIQ-0.1.6/PUI/tkinter/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      568 2023-04-29 18:55:09.000000 QPUIQ-0.1.6/PUI/tkinter/application.py
--rw-r--r--   0 Bug        (504) staff       (20)      541 2023-04-29 19:57:02.000000 QPUIQ-0.1.6/PUI/tkinter/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      528 2023-04-23 17:43:10.000000 QPUIQ-0.1.6/PUI/tkinter/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      954 2023-04-29 19:31:18.000000 QPUIQ-0.1.6/PUI/tkinter/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      403 2023-04-23 17:43:21.000000 QPUIQ-0.1.6/PUI/tkinter/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1636 2023-04-29 19:55:02.000000 QPUIQ-0.1.6/PUI/tkinter/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      468 2023-04-23 17:43:25.000000 QPUIQ-0.1.6/PUI/tkinter/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      866 2023-04-23 17:43:29.000000 QPUIQ-0.1.6/PUI/tkinter/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1530 2023-04-29 19:56:35.000000 QPUIQ-0.1.6/PUI/tkinter/window.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 20:14:38.744129 QPUIQ-0.1.6/PUI/urwid/
--rw-r--r--   0 Bug        (504) staff       (20)      429 2023-04-29 17:20:40.000000 QPUIQ-0.1.6/PUI/urwid/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)     1246 2023-04-29 19:07:03.000000 QPUIQ-0.1.6/PUI/urwid/application.py
--rw-r--r--   0 Bug        (504) staff       (20)       63 2023-03-14 09:21:15.000000 QPUIQ-0.1.6/PUI/urwid/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      678 2023-03-15 07:59:17.000000 QPUIQ-0.1.6/PUI/urwid/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      356 2023-03-16 07:54:05.000000 QPUIQ-0.1.6/PUI/urwid/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      734 2023-03-16 07:54:02.000000 QPUIQ-0.1.6/PUI/urwid/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      462 2023-03-15 00:27:06.000000 QPUIQ-0.1.6/PUI/urwid/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      315 2023-04-29 19:07:06.000000 QPUIQ-0.1.6/PUI/urwid/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     2494 2023-04-29 16:05:56.000000 QPUIQ-0.1.6/PUI/view.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 20:14:38.744763 QPUIQ-0.1.6/QPUIQ.egg-info/
--rw-r--r--   0 Bug        (504) staff       (20)     2885 2023-04-29 20:14:38.000000 QPUIQ-0.1.6/QPUIQ.egg-info/PKG-INFO
--rw-r--r--   0 Bug        (504) staff       (20)     1251 2023-04-29 20:14:38.000000 QPUIQ-0.1.6/QPUIQ.egg-info/SOURCES.txt
--rw-r--r--   0 Bug        (504) staff       (20)        1 2023-04-29 20:14:38.000000 QPUIQ-0.1.6/QPUIQ.egg-info/dependency_links.txt
--rw-r--r--   0 Bug        (504) staff       (20)        4 2023-04-29 20:14:38.000000 QPUIQ-0.1.6/QPUIQ.egg-info/top_level.txt
--rw-r--r--   0 Bug        (504) staff       (20)     2625 2023-04-29 20:10:38.000000 QPUIQ-0.1.6/README.md
--rw-r--r--   0 Bug        (504) staff       (20)       38 2023-04-29 20:14:38.745128 QPUIQ-0.1.6/setup.cfg
--rw-r--r--   0 Bug        (504) staff       (20)      539 2023-04-29 10:19:13.000000 QPUIQ-0.1.6/setup.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.781408 QPUIQ-0.1.7/
+-rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.1.7/LICENSE.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     2889 2023-04-29 21:13:42.781267 QPUIQ-0.1.7/PKG-INFO
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.768460 QPUIQ-0.1.7/PUI/
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.770999 QPUIQ-0.1.7/PUI/PySide6/
+-rw-r--r--   0 Bug        (504) staff       (20)      857 2023-04-29 20:10:13.000000 QPUIQ-0.1.7/PUI/PySide6/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      498 2023-04-29 18:30:29.000000 QPUIQ-0.1.7/PUI/PySide6/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1188 2023-04-29 16:10:01.000000 QPUIQ-0.1.7/PUI/PySide6/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-29 06:22:40.000000 QPUIQ-0.1.7/PUI/PySide6/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2138 2023-04-29 14:36:14.000000 QPUIQ-0.1.7/PUI/PySide6/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:43:52.000000 QPUIQ-0.1.7/PUI/PySide6/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      543 2023-04-26 17:57:33.000000 QPUIQ-0.1.7/PUI/PySide6/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:43:58.000000 QPUIQ-0.1.7/PUI/PySide6/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:06.000000 QPUIQ-0.1.7/PUI/PySide6/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1299 2023-04-29 16:58:24.000000 QPUIQ-0.1.7/PUI/PySide6/window.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.773580 QPUIQ-0.1.7/PUI/Qt5/
+-rw-r--r--   0 Bug        (504) staff       (20)      417 2023-04-29 17:06:45.000000 QPUIQ-0.1.7/PUI/Qt5/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      496 2023-04-29 18:30:13.000000 QPUIQ-0.1.7/PUI/Qt5/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1139 2023-04-29 17:07:47.000000 QPUIQ-0.1.7/PUI/Qt5/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-23 17:44:21.000000 QPUIQ-0.1.7/PUI/Qt5/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1527 2023-04-26 17:40:36.000000 QPUIQ-0.1.7/PUI/Qt5/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:44:32.000000 QPUIQ-0.1.7/PUI/Qt5/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      541 2023-03-13 15:01:12.000000 QPUIQ-0.1.7/PUI/Qt5/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:44:38.000000 QPUIQ-0.1.7/PUI/Qt5/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:41.000000 QPUIQ-0.1.7/PUI/Qt5/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1297 2023-04-29 17:05:56.000000 QPUIQ-0.1.7/PUI/Qt5/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      486 2023-04-29 21:13:28.000000 QPUIQ-0.1.7/PUI/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      458 2023-04-29 06:46:04.000000 QPUIQ-0.1.7/PUI/decorator.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2627 2023-04-29 19:40:07.000000 QPUIQ-0.1.7/PUI/dom.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.776066 QPUIQ-0.1.7/PUI/flet/
+-rw-r--r--   0 Bug        (504) staff       (20)      452 2023-04-29 19:08:30.000000 QPUIQ-0.1.7/PUI/flet/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      551 2023-04-29 19:19:55.000000 QPUIQ-0.1.7/PUI/flet/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.1.7/PUI/flet/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      647 2023-03-15 07:54:51.000000 QPUIQ-0.1.7/PUI/flet/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.1.7/PUI/flet/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      943 2023-04-14 18:19:33.000000 QPUIQ-0.1.7/PUI/flet/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:58:06.000000 QPUIQ-0.1.7/PUI/flet/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.1.7/PUI/flet/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      482 2023-04-29 19:19:13.000000 QPUIQ-0.1.7/PUI/flet/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3075 2023-04-29 20:53:50.000000 QPUIQ-0.1.7/PUI/node.py
+-rw-r--r--   0 Bug        (504) staff       (20)     8973 2023-04-29 20:54:27.000000 QPUIQ-0.1.7/PUI/state.py
+-rw-r--r--   0 Bug        (504) staff       (20)      983 2023-03-16 07:50:08.000000 QPUIQ-0.1.7/PUI/timeline.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.778418 QPUIQ-0.1.7/PUI/tkinter/
+-rw-r--r--   0 Bug        (504) staff       (20)      414 2023-04-29 18:25:14.000000 QPUIQ-0.1.7/PUI/tkinter/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      568 2023-04-29 18:55:09.000000 QPUIQ-0.1.7/PUI/tkinter/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)      541 2023-04-29 19:57:02.000000 QPUIQ-0.1.7/PUI/tkinter/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      528 2023-04-23 17:43:10.000000 QPUIQ-0.1.7/PUI/tkinter/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      954 2023-04-29 19:31:18.000000 QPUIQ-0.1.7/PUI/tkinter/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      403 2023-04-23 17:43:21.000000 QPUIQ-0.1.7/PUI/tkinter/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1636 2023-04-29 19:55:02.000000 QPUIQ-0.1.7/PUI/tkinter/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      468 2023-04-23 17:43:25.000000 QPUIQ-0.1.7/PUI/tkinter/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      866 2023-04-23 17:43:29.000000 QPUIQ-0.1.7/PUI/tkinter/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1530 2023-04-29 19:56:35.000000 QPUIQ-0.1.7/PUI/tkinter/window.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.780417 QPUIQ-0.1.7/PUI/urwid/
+-rw-r--r--   0 Bug        (504) staff       (20)      429 2023-04-29 17:20:40.000000 QPUIQ-0.1.7/PUI/urwid/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1246 2023-04-29 19:07:03.000000 QPUIQ-0.1.7/PUI/urwid/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)       63 2023-03-14 09:21:15.000000 QPUIQ-0.1.7/PUI/urwid/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      678 2023-03-15 07:59:17.000000 QPUIQ-0.1.7/PUI/urwid/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      356 2023-03-16 07:54:05.000000 QPUIQ-0.1.7/PUI/urwid/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      734 2023-03-16 07:54:02.000000 QPUIQ-0.1.7/PUI/urwid/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      462 2023-03-15 00:27:06.000000 QPUIQ-0.1.7/PUI/urwid/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      315 2023-04-29 19:07:06.000000 QPUIQ-0.1.7/PUI/urwid/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2604 2023-04-29 21:12:02.000000 QPUIQ-0.1.7/PUI/view.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.781069 QPUIQ-0.1.7/QPUIQ.egg-info/
+-rw-r--r--   0 Bug        (504) staff       (20)     2889 2023-04-29 21:13:42.000000 QPUIQ-0.1.7/QPUIQ.egg-info/PKG-INFO
+-rw-r--r--   0 Bug        (504) staff       (20)     1251 2023-04-29 21:13:42.000000 QPUIQ-0.1.7/QPUIQ.egg-info/SOURCES.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        1 2023-04-29 21:13:42.000000 QPUIQ-0.1.7/QPUIQ.egg-info/dependency_links.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        4 2023-04-29 21:13:42.000000 QPUIQ-0.1.7/QPUIQ.egg-info/top_level.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     2629 2023-04-29 21:00:52.000000 QPUIQ-0.1.7/README.md
+-rw-r--r--   0 Bug        (504) staff       (20)       38 2023-04-29 21:13:42.781449 QPUIQ-0.1.7/setup.cfg
+-rw-r--r--   0 Bug        (504) staff       (20)      539 2023-04-29 10:19:13.000000 QPUIQ-0.1.7/setup.py
```

### Comparing `QPUIQ-0.1.6/LICENSE.txt` & `QPUIQ-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PKG-INFO` & `QPUIQ-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.1.6
+Version: 0.1.7
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -107,15 +107,15 @@
 
 # reloadium: after_reload
 def after_reload(actions):
     PUIView.reload()
 ```
 
 # Progress
-* Use threading.locals() instead of inspect
+* ~~Use threading.locals() instead of inspect~~
 * State
     * ~~Update Trigger~~
     * ~~Binding~~
     * ~~StateList~~
     * ~~StateDict~~
     * Lazy UI?
 * Passing state to subview
```

### Comparing `QPUIQ-0.1.6/PUI/PySide6/__init__.py` & `QPUIQ-0.1.7/PUI/PySide6/__init__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/PySide6/base.py` & `QPUIQ-0.1.7/PUI/PySide6/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/PySide6/button.py` & `QPUIQ-0.1.7/PUI/PySide6/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/PySide6/canvas.py` & `QPUIQ-0.1.7/PUI/PySide6/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/PySide6/layout.py` & `QPUIQ-0.1.7/PUI/PySide6/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/PySide6/textfield.py` & `QPUIQ-0.1.7/PUI/PySide6/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/PySide6/window.py` & `QPUIQ-0.1.7/PUI/PySide6/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/Qt5/base.py` & `QPUIQ-0.1.7/PUI/Qt5/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/Qt5/button.py` & `QPUIQ-0.1.7/PUI/Qt5/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/Qt5/canvas.py` & `QPUIQ-0.1.7/PUI/Qt5/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/Qt5/layout.py` & `QPUIQ-0.1.7/PUI/Qt5/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/Qt5/textfield.py` & `QPUIQ-0.1.7/PUI/Qt5/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/Qt5/window.py` & `QPUIQ-0.1.7/PUI/Qt5/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/dom.py` & `QPUIQ-0.1.7/PUI/dom.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/flet/application.py` & `QPUIQ-0.1.7/PUI/flet/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/flet/button.py` & `QPUIQ-0.1.7/PUI/flet/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/flet/layout.py` & `QPUIQ-0.1.7/PUI/flet/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/flet/textfield.py` & `QPUIQ-0.1.7/PUI/flet/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/state.py` & `QPUIQ-0.1.7/PUI/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import inspect
 from .view import *
 
 class AttrBinding():
     def __init__(self, state, key):
         try:
-            root, parent, viewkey = find_pui()
-            self.viewroot = root
-            self.viewparent = parent
+            self.viewroot = find_puiview()
+            self.viewparent = self.viewroot.frames[-1]
         except:
             pass
         self.state = state
         self.key = key
         dt = type(getattr(self.state, self.key))
         if dt is str:
             self.func = str
@@ -31,17 +29,16 @@
             setattr(self.state, self.key, self.func(value))
         except:
             pass
 
 class KeyBinding():
     def __init__(self, state, key):
         try:
-            root, parent, viewkey = find_pui()
-            self.viewroot = root
-            self.viewparent = parent
+            self.viewroot = find_puiview()
+            self.viewparent = self.viewroot.frames[-1]
         except PuiViewNotFoundError:
             pass
         self.state = state
         self.key = key
         dt = type(self.state[self.key])
         if dt is str:
             self.func = str
@@ -99,17 +96,18 @@
         if key.startswith("_"):
             object.__setattr__(self, key, value)
         else:
             if type(value) is list:
                 value = StateList(value)
             elif type(value) is dict:
                 value = StateDict(value)
-            setattr(self.__values, key, value)
-            for l in self.__listeners:
-                l.redraw()
+            if not hasattr(self.__values, key) or getattr(self.__values, key) != value:
+                setattr(self.__values, key, value)
+                for l in self.__listeners:
+                    l.redraw()
 
     def __repr__(self):
         return f"StateObject({self.__values.__repr__()})"
 
 class StateList(BaseState):
     def __init__(self, values=None):
         self.__listeners = set()
@@ -126,17 +124,18 @@
             view = find_puiview()
             self.__listeners.add(view)
         except PuiViewNotFoundError:
             pass
         return self.__values[key]
 
     def __setitem__(self, key, value):
-        self.__values[key] = value
-        for l in self.__listeners:
-            l.redraw()
+        if key >= len (self.values) or self.__values[key] != value:
+            self.__values[key] = value
+            for l in self.__listeners:
+                l.redraw()
 
     def __len__(self):
         try:
             view = find_puiview()
             self.__listeners.add(view)
         except PuiViewNotFoundError:
             pass
@@ -273,17 +272,18 @@
             view = find_puiview()
             self.__listeners.add(view)
         except PuiViewNotFoundError:
             pass
         return self.__values.__repr__()
 
     def __setitem__(self, key, value):
-        self.__values[key] = value
-        for l in self.__listeners:
-            l.redraw()
+        if not key in self.__values or self.__values[key] != value:
+            self.__values[key] = value
+            for l in self.__listeners:
+                l.redraw()
 
     def clear(self):
         self.__values.clear()
         for l in self.__listeners:
             l.redraw()
 
     def get(self, key, default=None):
```

### Comparing `QPUIQ-0.1.6/PUI/timeline.py` & `QPUIQ-0.1.7/PUI/timeline.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/tkinter/application.py` & `QPUIQ-0.1.7/PUI/tkinter/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/tkinter/base.py` & `QPUIQ-0.1.7/PUI/tkinter/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/tkinter/button.py` & `QPUIQ-0.1.7/PUI/tkinter/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/tkinter/canvas.py` & `QPUIQ-0.1.7/PUI/tkinter/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/tkinter/layout.py` & `QPUIQ-0.1.7/PUI/tkinter/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/tkinter/textfield.py` & `QPUIQ-0.1.7/PUI/tkinter/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/tkinter/window.py` & `QPUIQ-0.1.7/PUI/tkinter/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/urwid/application.py` & `QPUIQ-0.1.7/PUI/urwid/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/urwid/button.py` & `QPUIQ-0.1.7/PUI/urwid/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/urwid/layout.py` & `QPUIQ-0.1.7/PUI/urwid/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/PUI/view.py` & `QPUIQ-0.1.7/PUI/view.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         dprint(f"content() time: {time.time()-start:.5f}", self.key)
         return scope
 
     def redraw(self):
         self.update()
 
     def update(self, prev=None):
+        update_start = time.time()
         dprint("update()", self.key)
         if prev:
             self.last_children = prev.children
 
         self.children = []
         try:
             dprint(f"content() start", self.key)
@@ -78,11 +79,12 @@
 
         start = time.time()
         dprint("sync() start", self.key)
         sync(self, self.last_children, self.children, self.children_first)
         dprint(f"sync() time: {time.time()-start:.5f}", self.key)
 
         self.last_children = self.children
+        dprint(f"update() time: {time.time()-update_start:.5f}", self.key)
 
     def run(self):
         self.redraw()
         self.start()
```

### Comparing `QPUIQ-0.1.6/QPUIQ.egg-info/PKG-INFO` & `QPUIQ-0.1.7/QPUIQ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.1.6
+Version: 0.1.7
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -107,15 +107,15 @@
 
 # reloadium: after_reload
 def after_reload(actions):
     PUIView.reload()
 ```
 
 # Progress
-* Use threading.locals() instead of inspect
+* ~~Use threading.locals() instead of inspect~~
 * State
     * ~~Update Trigger~~
     * ~~Binding~~
     * ~~StateList~~
     * ~~StateDict~~
     * Lazy UI?
 * Passing state to subview
```

### Comparing `QPUIQ-0.1.6/QPUIQ.egg-info/SOURCES.txt` & `QPUIQ-0.1.7/QPUIQ.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.6/README.md` & `QPUIQ-0.1.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 # reloadium: after_reload
 def after_reload(actions):
     PUIView.reload()
 ```
 
 # Progress
-* Use threading.locals() instead of inspect
+* ~~Use threading.locals() instead of inspect~~
 * State
     * ~~Update Trigger~~
     * ~~Binding~~
     * ~~StateList~~
     * ~~StateDict~~
     * Lazy UI?
 * Passing state to subview
```

### Comparing `QPUIQ-0.1.6/setup.py` & `QPUIQ-0.1.7/setup.py`

 * *Files identical despite different names*


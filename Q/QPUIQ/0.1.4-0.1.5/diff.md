# Comparing `tmp/QPUIQ-0.1.4.tar.gz` & `tmp/QPUIQ-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QPUIQ-0.1.4.tar", last modified: Sat Apr 29 10:15:13 2023, max compression
+gzip compressed data, was "QPUIQ-0.1.5.tar", last modified: Sat Apr 29 10:23:18 2023, max compression
```

## Comparing `QPUIQ-0.1.4.tar` & `QPUIQ-0.1.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.101821 QPUIQ-0.1.4/
--rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.1.4/LICENSE.txt
--rw-r--r--   0 Bug        (504) staff       (20)     2830 2023-04-29 10:15:13.101688 QPUIQ-0.1.4/PKG-INFO
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.088677 QPUIQ-0.1.4/PUI/
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.091366 QPUIQ-0.1.4/PUI/PySide6/
--rw-r--r--   0 Bug        (504) staff       (20)      362 2023-03-14 19:58:34.000000 QPUIQ-0.1.4/PUI/PySide6/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:58:40.000000 QPUIQ-0.1.4/PUI/PySide6/__main__.py
--rw-r--r--   0 Bug        (504) staff       (20)      903 2023-04-29 07:20:32.000000 QPUIQ-0.1.4/PUI/PySide6/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-29 06:22:40.000000 QPUIQ-0.1.4/PUI/PySide6/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1708 2023-04-29 05:49:06.000000 QPUIQ-0.1.4/PUI/PySide6/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:43:52.000000 QPUIQ-0.1.4/PUI/PySide6/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      543 2023-04-26 17:57:33.000000 QPUIQ-0.1.4/PUI/PySide6/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:43:58.000000 QPUIQ-0.1.4/PUI/PySide6/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:06.000000 QPUIQ-0.1.4/PUI/PySide6/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1610 2023-04-29 09:00:05.000000 QPUIQ-0.1.4/PUI/PySide6/window.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.093966 QPUIQ-0.1.4/PUI/Qt5/
--rw-r--r--   0 Bug        (504) staff       (20)      362 2023-03-14 19:52:55.000000 QPUIQ-0.1.4/PUI/Qt5/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:53:05.000000 QPUIQ-0.1.4/PUI/Qt5/__main__.py
--rw-r--r--   0 Bug        (504) staff       (20)      850 2023-04-14 18:19:33.000000 QPUIQ-0.1.4/PUI/Qt5/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-23 17:44:21.000000 QPUIQ-0.1.4/PUI/Qt5/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1527 2023-04-26 17:40:36.000000 QPUIQ-0.1.4/PUI/Qt5/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:44:32.000000 QPUIQ-0.1.4/PUI/Qt5/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      541 2023-03-13 15:01:12.000000 QPUIQ-0.1.4/PUI/Qt5/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:44:38.000000 QPUIQ-0.1.4/PUI/Qt5/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:41.000000 QPUIQ-0.1.4/PUI/Qt5/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1557 2023-04-14 18:19:33.000000 QPUIQ-0.1.4/PUI/Qt5/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      463 2023-03-16 06:42:21.000000 QPUIQ-0.1.4/PUI/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      458 2023-04-29 06:46:04.000000 QPUIQ-0.1.4/PUI/decorator.py
--rw-r--r--   0 Bug        (504) staff       (20)     2627 2023-04-29 08:37:44.000000 QPUIQ-0.1.4/PUI/dom.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.096612 QPUIQ-0.1.4/PUI/flet/
--rw-r--r--   0 Bug        (504) staff       (20)      398 2023-03-14 19:57:42.000000 QPUIQ-0.1.4/PUI/flet/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:55:09.000000 QPUIQ-0.1.4/PUI/flet/__main__.py
--rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.1.4/PUI/flet/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      647 2023-03-15 07:54:51.000000 QPUIQ-0.1.4/PUI/flet/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.1.4/PUI/flet/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      943 2023-04-14 18:19:33.000000 QPUIQ-0.1.4/PUI/flet/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:58:06.000000 QPUIQ-0.1.4/PUI/flet/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.1.4/PUI/flet/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      682 2023-04-14 18:25:52.000000 QPUIQ-0.1.4/PUI/flet/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     3821 2023-04-29 08:38:00.000000 QPUIQ-0.1.4/PUI/node.py
--rw-r--r--   0 Bug        (504) staff       (20)     8766 2023-04-29 09:38:11.000000 QPUIQ-0.1.4/PUI/state.py
--rw-r--r--   0 Bug        (504) staff       (20)      983 2023-03-16 07:50:08.000000 QPUIQ-0.1.4/PUI/timeline.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.098902 QPUIQ-0.1.4/PUI/tkinter/
--rw-r--r--   0 Bug        (504) staff       (20)      359 2023-03-14 19:48:08.000000 QPUIQ-0.1.4/PUI/tkinter/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:43:49.000000 QPUIQ-0.1.4/PUI/tkinter/__main__.py
--rw-r--r--   0 Bug        (504) staff       (20)      359 2023-03-14 19:48:57.000000 QPUIQ-0.1.4/PUI/tkinter/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      528 2023-04-23 17:43:10.000000 QPUIQ-0.1.4/PUI/tkinter/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      893 2023-04-29 08:02:29.000000 QPUIQ-0.1.4/PUI/tkinter/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      403 2023-04-23 17:43:21.000000 QPUIQ-0.1.4/PUI/tkinter/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1102 2023-03-14 19:49:35.000000 QPUIQ-0.1.4/PUI/tkinter/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      468 2023-04-23 17:43:25.000000 QPUIQ-0.1.4/PUI/tkinter/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      866 2023-04-23 17:43:29.000000 QPUIQ-0.1.4/PUI/tkinter/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1272 2023-03-16 07:43:13.000000 QPUIQ-0.1.4/PUI/tkinter/window.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.100945 QPUIQ-0.1.4/PUI/urwid/
--rw-r--r--   0 Bug        (504) staff       (20)      375 2023-03-14 19:40:06.000000 QPUIQ-0.1.4/PUI/urwid/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:36:22.000000 QPUIQ-0.1.4/PUI/urwid/__main__.py
--rw-r--r--   0 Bug        (504) staff       (20)       63 2023-03-14 09:21:15.000000 QPUIQ-0.1.4/PUI/urwid/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      678 2023-03-15 07:59:17.000000 QPUIQ-0.1.4/PUI/urwid/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      356 2023-03-16 07:54:05.000000 QPUIQ-0.1.4/PUI/urwid/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      734 2023-03-16 07:54:02.000000 QPUIQ-0.1.4/PUI/urwid/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      462 2023-03-15 00:27:06.000000 QPUIQ-0.1.4/PUI/urwid/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)     1318 2023-04-29 09:00:34.000000 QPUIQ-0.1.4/PUI/urwid/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     2494 2023-04-29 09:01:06.000000 QPUIQ-0.1.4/PUI/view.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.101502 QPUIQ-0.1.4/QPUIQ.egg-info/
--rw-r--r--   0 Bug        (504) staff       (20)     2830 2023-04-29 10:15:13.000000 QPUIQ-0.1.4/QPUIQ.egg-info/PKG-INFO
--rw-r--r--   0 Bug        (504) staff       (20)     1236 2023-04-29 10:15:13.000000 QPUIQ-0.1.4/QPUIQ.egg-info/SOURCES.txt
--rw-r--r--   0 Bug        (504) staff       (20)        1 2023-04-29 10:15:13.000000 QPUIQ-0.1.4/QPUIQ.egg-info/dependency_links.txt
--rw-r--r--   0 Bug        (504) staff       (20)        4 2023-04-29 10:15:13.000000 QPUIQ-0.1.4/QPUIQ.egg-info/top_level.txt
--rw-r--r--   0 Bug        (504) staff       (20)     2570 2023-04-25 08:07:34.000000 QPUIQ-0.1.4/README.md
--rw-r--r--   0 Bug        (504) staff       (20)       38 2023-04-29 10:15:13.101855 QPUIQ-0.1.4/setup.cfg
--rw-r--r--   0 Bug        (504) staff       (20)      507 2023-04-29 08:47:28.000000 QPUIQ-0.1.4/setup.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:23:18.907995 QPUIQ-0.1.5/
+-rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.1.5/LICENSE.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     2830 2023-04-29 10:23:18.907859 QPUIQ-0.1.5/PKG-INFO
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:23:18.894449 QPUIQ-0.1.5/PUI/
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:23:18.897191 QPUIQ-0.1.5/PUI/PySide6/
+-rw-r--r--   0 Bug        (504) staff       (20)      362 2023-03-14 19:58:34.000000 QPUIQ-0.1.5/PUI/PySide6/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:58:40.000000 QPUIQ-0.1.5/PUI/PySide6/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      903 2023-04-29 07:20:32.000000 QPUIQ-0.1.5/PUI/PySide6/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-29 06:22:40.000000 QPUIQ-0.1.5/PUI/PySide6/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1708 2023-04-29 05:49:06.000000 QPUIQ-0.1.5/PUI/PySide6/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:43:52.000000 QPUIQ-0.1.5/PUI/PySide6/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      543 2023-04-26 17:57:33.000000 QPUIQ-0.1.5/PUI/PySide6/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:43:58.000000 QPUIQ-0.1.5/PUI/PySide6/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:06.000000 QPUIQ-0.1.5/PUI/PySide6/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1610 2023-04-29 09:00:05.000000 QPUIQ-0.1.5/PUI/PySide6/window.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:23:18.899897 QPUIQ-0.1.5/PUI/Qt5/
+-rw-r--r--   0 Bug        (504) staff       (20)      362 2023-03-14 19:52:55.000000 QPUIQ-0.1.5/PUI/Qt5/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:53:05.000000 QPUIQ-0.1.5/PUI/Qt5/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      850 2023-04-14 18:19:33.000000 QPUIQ-0.1.5/PUI/Qt5/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-23 17:44:21.000000 QPUIQ-0.1.5/PUI/Qt5/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1527 2023-04-26 17:40:36.000000 QPUIQ-0.1.5/PUI/Qt5/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:44:32.000000 QPUIQ-0.1.5/PUI/Qt5/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      541 2023-03-13 15:01:12.000000 QPUIQ-0.1.5/PUI/Qt5/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:44:38.000000 QPUIQ-0.1.5/PUI/Qt5/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:41.000000 QPUIQ-0.1.5/PUI/Qt5/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1557 2023-04-14 18:19:33.000000 QPUIQ-0.1.5/PUI/Qt5/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      486 2023-04-29 10:23:03.000000 QPUIQ-0.1.5/PUI/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      458 2023-04-29 06:46:04.000000 QPUIQ-0.1.5/PUI/decorator.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2627 2023-04-29 08:37:44.000000 QPUIQ-0.1.5/PUI/dom.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:23:18.902843 QPUIQ-0.1.5/PUI/flet/
+-rw-r--r--   0 Bug        (504) staff       (20)      398 2023-03-14 19:57:42.000000 QPUIQ-0.1.5/PUI/flet/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:55:09.000000 QPUIQ-0.1.5/PUI/flet/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.1.5/PUI/flet/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      647 2023-03-15 07:54:51.000000 QPUIQ-0.1.5/PUI/flet/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.1.5/PUI/flet/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      943 2023-04-14 18:19:33.000000 QPUIQ-0.1.5/PUI/flet/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:58:06.000000 QPUIQ-0.1.5/PUI/flet/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.1.5/PUI/flet/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      682 2023-04-14 18:25:52.000000 QPUIQ-0.1.5/PUI/flet/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3821 2023-04-29 08:38:00.000000 QPUIQ-0.1.5/PUI/node.py
+-rw-r--r--   0 Bug        (504) staff       (20)     8766 2023-04-29 09:38:11.000000 QPUIQ-0.1.5/PUI/state.py
+-rw-r--r--   0 Bug        (504) staff       (20)      983 2023-03-16 07:50:08.000000 QPUIQ-0.1.5/PUI/timeline.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:23:18.905138 QPUIQ-0.1.5/PUI/tkinter/
+-rw-r--r--   0 Bug        (504) staff       (20)      359 2023-03-14 19:48:08.000000 QPUIQ-0.1.5/PUI/tkinter/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:43:49.000000 QPUIQ-0.1.5/PUI/tkinter/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      359 2023-03-14 19:48:57.000000 QPUIQ-0.1.5/PUI/tkinter/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      528 2023-04-23 17:43:10.000000 QPUIQ-0.1.5/PUI/tkinter/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      893 2023-04-29 08:02:29.000000 QPUIQ-0.1.5/PUI/tkinter/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      403 2023-04-23 17:43:21.000000 QPUIQ-0.1.5/PUI/tkinter/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1102 2023-03-14 19:49:35.000000 QPUIQ-0.1.5/PUI/tkinter/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      468 2023-04-23 17:43:25.000000 QPUIQ-0.1.5/PUI/tkinter/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      866 2023-04-23 17:43:29.000000 QPUIQ-0.1.5/PUI/tkinter/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1272 2023-03-16 07:43:13.000000 QPUIQ-0.1.5/PUI/tkinter/window.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:23:18.907111 QPUIQ-0.1.5/PUI/urwid/
+-rw-r--r--   0 Bug        (504) staff       (20)      375 2023-03-14 19:40:06.000000 QPUIQ-0.1.5/PUI/urwid/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:36:22.000000 QPUIQ-0.1.5/PUI/urwid/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)       63 2023-03-14 09:21:15.000000 QPUIQ-0.1.5/PUI/urwid/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      678 2023-03-15 07:59:17.000000 QPUIQ-0.1.5/PUI/urwid/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      356 2023-03-16 07:54:05.000000 QPUIQ-0.1.5/PUI/urwid/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      734 2023-03-16 07:54:02.000000 QPUIQ-0.1.5/PUI/urwid/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      462 2023-03-15 00:27:06.000000 QPUIQ-0.1.5/PUI/urwid/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1318 2023-04-29 09:00:34.000000 QPUIQ-0.1.5/PUI/urwid/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2494 2023-04-29 09:01:06.000000 QPUIQ-0.1.5/PUI/view.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:23:18.907689 QPUIQ-0.1.5/QPUIQ.egg-info/
+-rw-r--r--   0 Bug        (504) staff       (20)     2830 2023-04-29 10:23:18.000000 QPUIQ-0.1.5/QPUIQ.egg-info/PKG-INFO
+-rw-r--r--   0 Bug        (504) staff       (20)     1236 2023-04-29 10:23:18.000000 QPUIQ-0.1.5/QPUIQ.egg-info/SOURCES.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        1 2023-04-29 10:23:18.000000 QPUIQ-0.1.5/QPUIQ.egg-info/dependency_links.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        4 2023-04-29 10:23:18.000000 QPUIQ-0.1.5/QPUIQ.egg-info/top_level.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     2570 2023-04-25 08:07:34.000000 QPUIQ-0.1.5/README.md
+-rw-r--r--   0 Bug        (504) staff       (20)       38 2023-04-29 10:23:18.908134 QPUIQ-0.1.5/setup.cfg
+-rw-r--r--   0 Bug        (504) staff       (20)      539 2023-04-29 10:19:13.000000 QPUIQ-0.1.5/setup.py
```

### Comparing `QPUIQ-0.1.4/LICENSE.txt` & `QPUIQ-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PKG-INFO` & `QPUIQ-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.1.4
+Version: 0.1.5
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `QPUIQ-0.1.4/PUI/PySide6/__main__.py` & `QPUIQ-0.1.5/PUI/PySide6/__main__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/PySide6/base.py` & `QPUIQ-0.1.5/PUI/PySide6/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/PySide6/button.py` & `QPUIQ-0.1.5/PUI/PySide6/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/PySide6/canvas.py` & `QPUIQ-0.1.5/PUI/PySide6/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/PySide6/layout.py` & `QPUIQ-0.1.5/PUI/PySide6/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/PySide6/textfield.py` & `QPUIQ-0.1.5/PUI/PySide6/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/PySide6/window.py` & `QPUIQ-0.1.5/PUI/PySide6/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/Qt5/__main__.py` & `QPUIQ-0.1.5/PUI/Qt5/__main__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/Qt5/base.py` & `QPUIQ-0.1.5/PUI/Qt5/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/Qt5/button.py` & `QPUIQ-0.1.5/PUI/Qt5/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/Qt5/canvas.py` & `QPUIQ-0.1.5/PUI/Qt5/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/Qt5/layout.py` & `QPUIQ-0.1.5/PUI/Qt5/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/Qt5/textfield.py` & `QPUIQ-0.1.5/PUI/Qt5/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/Qt5/window.py` & `QPUIQ-0.1.5/PUI/Qt5/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/dom.py` & `QPUIQ-0.1.5/PUI/dom.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/flet/__main__.py` & `QPUIQ-0.1.5/PUI/flet/__main__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/flet/button.py` & `QPUIQ-0.1.5/PUI/flet/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/flet/layout.py` & `QPUIQ-0.1.5/PUI/flet/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/flet/textfield.py` & `QPUIQ-0.1.5/PUI/flet/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/flet/window.py` & `QPUIQ-0.1.5/PUI/flet/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/node.py` & `QPUIQ-0.1.5/PUI/node.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/state.py` & `QPUIQ-0.1.5/PUI/state.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/timeline.py` & `QPUIQ-0.1.5/PUI/timeline.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/tkinter/__main__.py` & `QPUIQ-0.1.5/PUI/tkinter/__main__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/tkinter/button.py` & `QPUIQ-0.1.5/PUI/tkinter/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/tkinter/canvas.py` & `QPUIQ-0.1.5/PUI/tkinter/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/tkinter/layout.py` & `QPUIQ-0.1.5/PUI/tkinter/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/tkinter/textfield.py` & `QPUIQ-0.1.5/PUI/tkinter/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/tkinter/window.py` & `QPUIQ-0.1.5/PUI/tkinter/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/urwid/__main__.py` & `QPUIQ-0.1.5/PUI/urwid/__main__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/urwid/button.py` & `QPUIQ-0.1.5/PUI/urwid/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/urwid/layout.py` & `QPUIQ-0.1.5/PUI/urwid/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/urwid/window.py` & `QPUIQ-0.1.5/PUI/urwid/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/PUI/view.py` & `QPUIQ-0.1.5/PUI/view.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/QPUIQ.egg-info/PKG-INFO` & `QPUIQ-0.1.5/QPUIQ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.1.4
+Version: 0.1.5
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `QPUIQ-0.1.4/QPUIQ.egg-info/SOURCES.txt` & `QPUIQ-0.1.5/QPUIQ.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.4/README.md` & `QPUIQ-0.1.5/README.md`

 * *Files identical despite different names*


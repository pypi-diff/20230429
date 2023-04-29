# Comparing `tmp/QPUIQ-0.1.3.tar.gz` & `tmp/QPUIQ-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QPUIQ-0.1.3.tar", last modified: Fri Apr 14 18:26:32 2023, max compression
+gzip compressed data, was "QPUIQ-0.1.4.tar", last modified: Sat Apr 29 10:15:13 2023, max compression
```

## Comparing `QPUIQ-0.1.3.tar` & `QPUIQ-0.1.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.184424 QPUIQ-0.1.3/
--rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.1.3/LICENSE.txt
--rw-r--r--   0 Bug        (504) staff       (20)     2786 2023-04-14 18:26:32.184251 QPUIQ-0.1.3/PKG-INFO
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.172098 QPUIQ-0.1.3/PUI/
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.174467 QPUIQ-0.1.3/PUI/PySide6/
--rw-r--r--   0 Bug        (504) staff       (20)      362 2023-03-14 19:58:34.000000 QPUIQ-0.1.3/PUI/PySide6/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:58:40.000000 QPUIQ-0.1.3/PUI/PySide6/__main__.py
--rw-r--r--   0 Bug        (504) staff       (20)      853 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/PySide6/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      638 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/PySide6/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1625 2023-03-13 15:01:12.000000 QPUIQ-0.1.3/PUI/PySide6/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      374 2023-03-13 15:01:12.000000 QPUIQ-0.1.3/PUI/PySide6/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      543 2023-03-16 10:07:28.000000 QPUIQ-0.1.3/PUI/PySide6/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      486 2023-03-14 19:58:20.000000 QPUIQ-0.1.3/PUI/PySide6/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      814 2023-03-13 15:01:12.000000 QPUIQ-0.1.3/PUI/PySide6/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1595 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/PySide6/window.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.177054 QPUIQ-0.1.3/PUI/Qt5/
--rw-r--r--   0 Bug        (504) staff       (20)      362 2023-03-14 19:52:55.000000 QPUIQ-0.1.3/PUI/Qt5/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:53:05.000000 QPUIQ-0.1.3/PUI/Qt5/__main__.py
--rw-r--r--   0 Bug        (504) staff       (20)      850 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/Qt5/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      638 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/Qt5/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1619 2023-03-13 15:01:12.000000 QPUIQ-0.1.3/PUI/Qt5/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      374 2023-03-13 15:01:12.000000 QPUIQ-0.1.3/PUI/Qt5/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      541 2023-03-13 15:01:12.000000 QPUIQ-0.1.3/PUI/Qt5/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      486 2023-03-14 19:54:41.000000 QPUIQ-0.1.3/PUI/Qt5/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      814 2023-03-13 15:01:12.000000 QPUIQ-0.1.3/PUI/Qt5/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1557 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/Qt5/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      463 2023-03-16 06:42:21.000000 QPUIQ-0.1.3/PUI/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      236 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/decorator.py
--rw-r--r--   0 Bug        (504) staff       (20)     1953 2023-03-16 09:17:17.000000 QPUIQ-0.1.3/PUI/dom.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.179061 QPUIQ-0.1.3/PUI/flet/
--rw-r--r--   0 Bug        (504) staff       (20)      398 2023-03-14 19:57:42.000000 QPUIQ-0.1.3/PUI/flet/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:55:09.000000 QPUIQ-0.1.3/PUI/flet/__main__.py
--rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.1.3/PUI/flet/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      647 2023-03-15 07:54:51.000000 QPUIQ-0.1.3/PUI/flet/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.1.3/PUI/flet/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      943 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/flet/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:58:06.000000 QPUIQ-0.1.3/PUI/flet/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.1.3/PUI/flet/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      682 2023-04-14 18:25:52.000000 QPUIQ-0.1.3/PUI/flet/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     3171 2023-04-14 18:23:56.000000 QPUIQ-0.1.3/PUI/node.py
--rw-r--r--   0 Bug        (504) staff       (20)     8425 2023-04-14 18:23:56.000000 QPUIQ-0.1.3/PUI/state.py
--rw-r--r--   0 Bug        (504) staff       (20)      983 2023-03-16 07:50:08.000000 QPUIQ-0.1.3/PUI/timeline.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.181464 QPUIQ-0.1.3/PUI/tkinter/
--rw-r--r--   0 Bug        (504) staff       (20)      359 2023-03-14 19:48:08.000000 QPUIQ-0.1.3/PUI/tkinter/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:43:49.000000 QPUIQ-0.1.3/PUI/tkinter/__main__.py
--rw-r--r--   0 Bug        (504) staff       (20)      359 2023-03-14 19:48:57.000000 QPUIQ-0.1.3/PUI/tkinter/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      550 2023-03-14 19:48:50.000000 QPUIQ-0.1.3/PUI/tkinter/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      896 2023-03-14 19:49:44.000000 QPUIQ-0.1.3/PUI/tkinter/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:49:39.000000 QPUIQ-0.1.3/PUI/tkinter/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1102 2023-03-14 19:49:35.000000 QPUIQ-0.1.3/PUI/tkinter/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      490 2023-03-14 19:50:09.000000 QPUIQ-0.1.3/PUI/tkinter/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      890 2023-03-14 19:49:07.000000 QPUIQ-0.1.3/PUI/tkinter/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1272 2023-03-16 07:43:13.000000 QPUIQ-0.1.3/PUI/tkinter/window.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.183511 QPUIQ-0.1.3/PUI/urwid/
--rw-r--r--   0 Bug        (504) staff       (20)      375 2023-03-14 19:40:06.000000 QPUIQ-0.1.3/PUI/urwid/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:36:22.000000 QPUIQ-0.1.3/PUI/urwid/__main__.py
--rw-r--r--   0 Bug        (504) staff       (20)       63 2023-03-14 09:21:15.000000 QPUIQ-0.1.3/PUI/urwid/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      678 2023-03-15 07:59:17.000000 QPUIQ-0.1.3/PUI/urwid/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      356 2023-03-16 07:54:05.000000 QPUIQ-0.1.3/PUI/urwid/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      734 2023-03-16 07:54:02.000000 QPUIQ-0.1.3/PUI/urwid/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      462 2023-03-15 00:27:06.000000 QPUIQ-0.1.3/PUI/urwid/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)     1318 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/urwid/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     1268 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/view.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.184028 QPUIQ-0.1.3/QPUIQ.egg-info/
--rw-r--r--   0 Bug        (504) staff       (20)     2786 2023-04-14 18:26:32.000000 QPUIQ-0.1.3/QPUIQ.egg-info/PKG-INFO
--rw-r--r--   0 Bug        (504) staff       (20)     1236 2023-04-14 18:26:32.000000 QPUIQ-0.1.3/QPUIQ.egg-info/SOURCES.txt
--rw-r--r--   0 Bug        (504) staff       (20)        1 2023-04-14 18:26:32.000000 QPUIQ-0.1.3/QPUIQ.egg-info/dependency_links.txt
--rw-r--r--   0 Bug        (504) staff       (20)        4 2023-04-14 18:26:32.000000 QPUIQ-0.1.3/QPUIQ.egg-info/top_level.txt
--rw-r--r--   0 Bug        (504) staff       (20)     2526 2023-04-14 18:25:52.000000 QPUIQ-0.1.3/README.md
--rw-r--r--   0 Bug        (504) staff       (20)       38 2023-04-14 18:26:32.184467 QPUIQ-0.1.3/setup.cfg
--rw-r--r--   0 Bug        (504) staff       (20)      507 2023-04-14 18:25:24.000000 QPUIQ-0.1.3/setup.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.101821 QPUIQ-0.1.4/
+-rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.1.4/LICENSE.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     2830 2023-04-29 10:15:13.101688 QPUIQ-0.1.4/PKG-INFO
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.088677 QPUIQ-0.1.4/PUI/
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.091366 QPUIQ-0.1.4/PUI/PySide6/
+-rw-r--r--   0 Bug        (504) staff       (20)      362 2023-03-14 19:58:34.000000 QPUIQ-0.1.4/PUI/PySide6/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:58:40.000000 QPUIQ-0.1.4/PUI/PySide6/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      903 2023-04-29 07:20:32.000000 QPUIQ-0.1.4/PUI/PySide6/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-29 06:22:40.000000 QPUIQ-0.1.4/PUI/PySide6/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1708 2023-04-29 05:49:06.000000 QPUIQ-0.1.4/PUI/PySide6/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:43:52.000000 QPUIQ-0.1.4/PUI/PySide6/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      543 2023-04-26 17:57:33.000000 QPUIQ-0.1.4/PUI/PySide6/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:43:58.000000 QPUIQ-0.1.4/PUI/PySide6/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:06.000000 QPUIQ-0.1.4/PUI/PySide6/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1610 2023-04-29 09:00:05.000000 QPUIQ-0.1.4/PUI/PySide6/window.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.093966 QPUIQ-0.1.4/PUI/Qt5/
+-rw-r--r--   0 Bug        (504) staff       (20)      362 2023-03-14 19:52:55.000000 QPUIQ-0.1.4/PUI/Qt5/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:53:05.000000 QPUIQ-0.1.4/PUI/Qt5/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      850 2023-04-14 18:19:33.000000 QPUIQ-0.1.4/PUI/Qt5/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-23 17:44:21.000000 QPUIQ-0.1.4/PUI/Qt5/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1527 2023-04-26 17:40:36.000000 QPUIQ-0.1.4/PUI/Qt5/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:44:32.000000 QPUIQ-0.1.4/PUI/Qt5/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      541 2023-03-13 15:01:12.000000 QPUIQ-0.1.4/PUI/Qt5/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:44:38.000000 QPUIQ-0.1.4/PUI/Qt5/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:41.000000 QPUIQ-0.1.4/PUI/Qt5/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1557 2023-04-14 18:19:33.000000 QPUIQ-0.1.4/PUI/Qt5/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      463 2023-03-16 06:42:21.000000 QPUIQ-0.1.4/PUI/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      458 2023-04-29 06:46:04.000000 QPUIQ-0.1.4/PUI/decorator.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2627 2023-04-29 08:37:44.000000 QPUIQ-0.1.4/PUI/dom.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.096612 QPUIQ-0.1.4/PUI/flet/
+-rw-r--r--   0 Bug        (504) staff       (20)      398 2023-03-14 19:57:42.000000 QPUIQ-0.1.4/PUI/flet/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:55:09.000000 QPUIQ-0.1.4/PUI/flet/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.1.4/PUI/flet/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      647 2023-03-15 07:54:51.000000 QPUIQ-0.1.4/PUI/flet/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.1.4/PUI/flet/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      943 2023-04-14 18:19:33.000000 QPUIQ-0.1.4/PUI/flet/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:58:06.000000 QPUIQ-0.1.4/PUI/flet/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.1.4/PUI/flet/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      682 2023-04-14 18:25:52.000000 QPUIQ-0.1.4/PUI/flet/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3821 2023-04-29 08:38:00.000000 QPUIQ-0.1.4/PUI/node.py
+-rw-r--r--   0 Bug        (504) staff       (20)     8766 2023-04-29 09:38:11.000000 QPUIQ-0.1.4/PUI/state.py
+-rw-r--r--   0 Bug        (504) staff       (20)      983 2023-03-16 07:50:08.000000 QPUIQ-0.1.4/PUI/timeline.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.098902 QPUIQ-0.1.4/PUI/tkinter/
+-rw-r--r--   0 Bug        (504) staff       (20)      359 2023-03-14 19:48:08.000000 QPUIQ-0.1.4/PUI/tkinter/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:43:49.000000 QPUIQ-0.1.4/PUI/tkinter/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      359 2023-03-14 19:48:57.000000 QPUIQ-0.1.4/PUI/tkinter/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      528 2023-04-23 17:43:10.000000 QPUIQ-0.1.4/PUI/tkinter/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      893 2023-04-29 08:02:29.000000 QPUIQ-0.1.4/PUI/tkinter/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      403 2023-04-23 17:43:21.000000 QPUIQ-0.1.4/PUI/tkinter/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1102 2023-03-14 19:49:35.000000 QPUIQ-0.1.4/PUI/tkinter/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      468 2023-04-23 17:43:25.000000 QPUIQ-0.1.4/PUI/tkinter/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      866 2023-04-23 17:43:29.000000 QPUIQ-0.1.4/PUI/tkinter/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1272 2023-03-16 07:43:13.000000 QPUIQ-0.1.4/PUI/tkinter/window.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.100945 QPUIQ-0.1.4/PUI/urwid/
+-rw-r--r--   0 Bug        (504) staff       (20)      375 2023-03-14 19:40:06.000000 QPUIQ-0.1.4/PUI/urwid/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:36:22.000000 QPUIQ-0.1.4/PUI/urwid/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)       63 2023-03-14 09:21:15.000000 QPUIQ-0.1.4/PUI/urwid/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      678 2023-03-15 07:59:17.000000 QPUIQ-0.1.4/PUI/urwid/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      356 2023-03-16 07:54:05.000000 QPUIQ-0.1.4/PUI/urwid/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      734 2023-03-16 07:54:02.000000 QPUIQ-0.1.4/PUI/urwid/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      462 2023-03-15 00:27:06.000000 QPUIQ-0.1.4/PUI/urwid/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1318 2023-04-29 09:00:34.000000 QPUIQ-0.1.4/PUI/urwid/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2494 2023-04-29 09:01:06.000000 QPUIQ-0.1.4/PUI/view.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 10:15:13.101502 QPUIQ-0.1.4/QPUIQ.egg-info/
+-rw-r--r--   0 Bug        (504) staff       (20)     2830 2023-04-29 10:15:13.000000 QPUIQ-0.1.4/QPUIQ.egg-info/PKG-INFO
+-rw-r--r--   0 Bug        (504) staff       (20)     1236 2023-04-29 10:15:13.000000 QPUIQ-0.1.4/QPUIQ.egg-info/SOURCES.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        1 2023-04-29 10:15:13.000000 QPUIQ-0.1.4/QPUIQ.egg-info/dependency_links.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        4 2023-04-29 10:15:13.000000 QPUIQ-0.1.4/QPUIQ.egg-info/top_level.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     2570 2023-04-25 08:07:34.000000 QPUIQ-0.1.4/README.md
+-rw-r--r--   0 Bug        (504) staff       (20)       38 2023-04-29 10:15:13.101855 QPUIQ-0.1.4/setup.cfg
+-rw-r--r--   0 Bug        (504) staff       (20)      507 2023-04-29 08:47:28.000000 QPUIQ-0.1.4/setup.py
```

### Comparing `QPUIQ-0.1.3/LICENSE.txt` & `QPUIQ-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PKG-INFO` & `QPUIQ-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.1.3
+Version: 0.1.4
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -110,14 +110,15 @@
 
 # reloadium: after_reload
 def after_reload(actions):
     PUIView.reload()
 ```
 
 # Progress
+* Use threading.locals() instead of inspect
 * State
     * ~~Update Trigger~~
     * ~~Binding~~
     * ~~StateList~~
     * ~~StateDict~~
     * Lazy UI?
 * Passing state to subview
```

### Comparing `QPUIQ-0.1.3/PUI/PySide6/__main__.py` & `QPUIQ-0.1.4/PUI/PySide6/__main__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/PySide6/base.py` & `QPUIQ-0.1.4/PUI/Qt5/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from .. import *
-
-from PySide6 import QtCore, QtWidgets
+from PyQt5 import QtCore, QtWidgets
 
 class QtBaseWidget(PUINode):
     def destroy(self):
         self.ui.deleteLater()
 
 class QtBaseLayout(PUINode):
     def addChild(self, idx, child):
```

### Comparing `QPUIQ-0.1.3/PUI/PySide6/button.py` & `QPUIQ-0.1.4/PUI/PySide6/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,7 @@
                 self.ui.clicked.disconnect()
             except:
                 pass
             self.ui.clicked.connect(self.callback)
         else:
             self.ui = QtWidgets.QPushButton(text=self.text)
             self.ui.clicked.connect(self.callback)
-        return self.ui
```

### Comparing `QPUIQ-0.1.3/PUI/PySide6/canvas.py` & `QPUIQ-0.1.4/PUI/PySide6/canvas.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,50 +2,45 @@
 from .base import *
 
 from PySide6 import QtWidgets
 from PySide6.QtGui import QPainter, QColor
 from PySide6.QtCore import QPoint
 
 class PUIQtCanvas(QtWidgets.QWidget):
-    def __init__(self, puinode):
+    def __init__(self, puinode, width=None, height=None):
         self.puinode = puinode
+        self.width = width
+        self.height = height
         super().__init__()
 
-    def setPUINode(self, puinode):
-        self.puinode = puinode
+    def sizeHint(self):
+        return QtCore.QSize(self.width, self.height)
 
     def paintEvent(self, event):
         qpainter = QPainter()
         qpainter.begin(self)
 
         for c in self.puinode.children:
             c.draw(qpainter)
 
         qpainter.end()
 
 class QtCanvas(QtBaseWidget):
-    def __init__(self, size=None, **kwargs):
-        super().__init__(**kwargs)
-        self.size = size
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.ui = None
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
-            self.ui.setPUINode(self)
+            self.ui.puinode = self
         else:
-            self.ui = PUIQtCanvas(self)
-        x = 0
-        y = 0
-        w = 0
-        h = 0
-        if not self.size is None:
-            w, h = self.size
-        self.ui.setGeometry(x, y, w, h)
+            self.ui = PUIQtCanvas(self, self.layout_width or 0, self.layout_height or 0)
+        self.ui.resize(self.layout_width or 0, self.layout_height or 0)
         self.ui.update()
-        return self.ui
 
 class QtCanvasText(PUINode):
     def __init__(self, x, y, text):
         super().__init__()
         self.x = x
         self.y = y
         self.text = text
@@ -53,17 +48,19 @@
     def update(self, prev):
         pass
 
     def draw(self, qpainter):
         qpainter.drawText(QPoint(int(self.x), int(self.y)), self.text)
 
 class QtCanvasLine(PUINode):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, x1, y1, x2, y2):
         super().__init__()
-        self.args = args
-        self.kwargs = kwargs
+        self.x1 = x1
+        self.y1 = y1
+        self.x2 = x2
+        self.y2 = y2
 
     def update(self, prev):
         pass
 
     def draw(self, qpainter):
-        qpainter.drawLine(*self.args)
+        qpainter.drawLine(self.x1, self.y1, self.x2, self.y2)
```

### Comparing `QPUIQ-0.1.3/PUI/PySide6/layout.py` & `QPUIQ-0.1.4/PUI/PySide6/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/PySide6/textfield.py` & `QPUIQ-0.1.4/PUI/PySide6/textfield.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,11 +16,10 @@
                 self.ui.textChanged.connect(self.on_textchanged)
             self.last_value = value
         else:
             self.last_value = value
             self.ui = QtWidgets.QLineEdit()
             self.ui.setText(str(value))
             self.ui.textChanged.connect(self.on_textchanged)
-        return self.ui
 
     def on_textchanged(self):
         self.model.value = self.ui.text()
```

### Comparing `QPUIQ-0.1.3/PUI/PySide6/window.py` & `QPUIQ-0.1.4/PUI/PySide6/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,29 @@
         self.size = size
         self.signal = QtWindowSignal()
         self.signal.redraw.connect(self.update)
 
     def redraw(self):
         self.signal.redraw.emit()
 
-    def update(self):
+    def update(self, prev=None):
         if not hasattr(self, "window"):
             from PySide6 import QtWidgets
             self.app = QtWidgets.QApplication([])
             self.window = QtWidgets.QWidget()
             self.window.setObjectName("Window")
             self.box = QtWidgets.QBoxLayout(QtWidgets.QBoxLayout.Direction.LeftToRight)
             self.window.setLayout(self.box)
 
         if not self.title is None:
             self.window.setWindowTitle(self.title)
         if not self.size is None:
             self.window.resize(*self.size)
 
-        super().update()
+        super().update(prev)
 
     def addChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
             self.box.addLayout(child.ui)
         elif isinstance(child, QtBaseWidget):
             self.box.addWidget(child.ui)
         else:
```

### Comparing `QPUIQ-0.1.3/PUI/Qt5/__main__.py` & `QPUIQ-0.1.4/PUI/Qt5/__main__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/Qt5/base.py` & `QPUIQ-0.1.4/PUI/PySide6/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from .. import *
-from PyQt5 import QtCore, QtWidgets
+
+from PySide6 import QtCore, QtWidgets
 
 class QtBaseWidget(PUINode):
+    terminal = True
     def destroy(self):
         self.ui.deleteLater()
 
 class QtBaseLayout(PUINode):
     def addChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
             self.ui.addLayout(child.ui)
         elif isinstance(child, QtBaseWidget):
             params = {}
             if not child.layout_weight is None:
                 params["stretch"] = child.layout_weight
             self.ui.addWidget(child.ui, **params)
-        else:
+        elif child.children:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
             self.box.removeItem(child.ui)
         elif isinstance(child, QtBaseWidget):
             child.ui.setParent(None)
-        else:
+        elif child.children:
             self.removeChild(idx, child.children[0])
```

### Comparing `QPUIQ-0.1.3/PUI/Qt5/button.py` & `QPUIQ-0.1.4/PUI/Qt5/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,7 @@
                 self.ui.clicked.disconnect()
             except:
                 pass
             self.ui.clicked.connect(self.callback)
         else:
             self.ui = QtWidgets.QPushButton(text=self.text)
             self.ui.clicked.connect(self.callback)
-        return self.ui
```

### Comparing `QPUIQ-0.1.3/PUI/Qt5/canvas.py` & `QPUIQ-0.1.4/PUI/Qt5/canvas.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 from PyQt5.QtCore import QPoint
 
 class PUIQtCanvas(QtWidgets.QWidget):
     def __init__(self, puinode):
         self.puinode = puinode
         super().__init__()
 
-    def setPUINode(self, puinode):
-        self.puinode = puinode
-
     def paintEvent(self, event):
         qpainter = QPainter()
         qpainter.begin(self)
 
         for c in self.puinode.children:
             c.draw(qpainter)
 
@@ -26,26 +23,25 @@
     def __init__(self, size=None, **kwargs):
         super().__init__(**kwargs)
         self.size = size
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
-            self.ui.setPUINode(self)
+            self.ui.puinode = self
         else:
             self.ui = PUIQtCanvas(self)
         x = 0
         y = 0
         w = 0
         h = 0
         if not self.size is None:
             w, h = self.size
         self.ui.setGeometry(x, y, w, h)
         self.ui.update()
-        return self.ui
 
 class QtCanvasText(PUINode):
     def __init__(self, x, y, text):
         super().__init__()
         self.x = x
         self.y = y
         self.text = text
```

### Comparing `QPUIQ-0.1.3/PUI/Qt5/layout.py` & `QPUIQ-0.1.4/PUI/Qt5/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/Qt5/textfield.py` & `QPUIQ-0.1.4/PUI/Qt5/textfield.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,11 +16,10 @@
                 self.ui.textChanged.connect(self.on_textchanged)
             self.last_value = value
         else:
             self.last_value = value
             self.ui = QtWidgets.QLineEdit()
             self.ui.setText(str(value))
             self.ui.textChanged.connect(self.on_textchanged)
-        return self.ui
 
     def on_textchanged(self):
         self.model.value = self.ui.text()
```

### Comparing `QPUIQ-0.1.3/PUI/Qt5/window.py` & `QPUIQ-0.1.4/PUI/Qt5/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/dom.py` & `QPUIQ-0.1.4/PUI/dom.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,43 @@
+# dprint = print
+dprint = lambda *x: x
+
 def recur_delete(node, idx, child):
     for sidx,sc in enumerate(child.children):
         recur_delete(child, sidx, sc)
     node.removeChild(idx, child)
     child.destroy()
 
 def sync(node, oldDOM, newDOM, children_first):
+    dprint("syncing", node.key, len(oldDOM), len(newDOM))
+    dprint("  ===OLD===")
+    for c in oldDOM:
+        dprint("   ", c.key)
+    dprint("  ===NEW===")
+    for c in newDOM:
+        dprint("   ", c.key)
     oldMap = [x.key for x in oldDOM]
 
     skipHead = 0
     for i in range(0, min(len(oldDOM), len(newDOM))):
         if oldDOM[i].key == newDOM[i].key:
             oldMap[i] = None
             old = oldDOM[i]
             new = newDOM[i]
-            new.update(old)
-            sync(new, old.children, new.children, children_first)
+            try:
+                new.update(old)
+            except:
+                import traceback
+                print("## <ERROR OF sync() >")
+                print(node.key)
+                traceback.print_exc()
+                print("## </ERROR OF sync()>")
+
+            if not new.terminal:
+                sync(new, old.children, new.children, children_first)
             skipHead += 1
         else:
             break
 
     skipTail = 0
     # for i in range(0, min(len(oldDOM)-skipHead, len(newDOM)-skipHead)):
     #     if oldDOM[-1-i].key == newDOM[-1-i].key:
@@ -31,28 +50,31 @@
     #     else:
     #         break
 
     for i, new in enumerate(newDOM[skipHead:len(newDOM)-skipTail]):
         new_idx = skipHead + i
         try:
             old_idx = oldMap.index(new.key)
+        except:
+            old_idx = -1
+        if old_idx >= 0:
             oldMap[old_idx] = None
             old = oldDOM[old_idx]
             node.removeChild(old_idx, old)
             new.update(old)
-            if children_first:
+            if not new.terminal and children_first:
                 sync(new, old.children, new.children, children_first)
             node.addChild(new_idx, old)
-            if not children_first:
+            if not new.terminal and not children_first:
                 sync(new, old.children, new.children, children_first)
-        except:
+        else:
             new.update(None)
-            if children_first:
+            if not new.terminal and children_first:
                 sync(new, [], new.children, children_first)
             node.addChild(new_idx, new)
-            if not children_first:
+            if not new.terminal and not children_first:
                 sync(new, [], new.children, children_first)
 
     for old_idx, key in enumerate(oldMap):
         if key:
             old = oldDOM[old_idx]
             recur_delete(node, old_idx, old)
```

### Comparing `QPUIQ-0.1.3/PUI/flet/__main__.py` & `QPUIQ-0.1.4/PUI/flet/__main__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/flet/button.py` & `QPUIQ-0.1.4/PUI/flet/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/flet/layout.py` & `QPUIQ-0.1.4/PUI/flet/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/flet/textfield.py` & `QPUIQ-0.1.4/PUI/flet/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/flet/window.py` & `QPUIQ-0.1.4/PUI/flet/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/node.py` & `QPUIQ-0.1.4/PUI/view.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,112 +1,88 @@
-def find_pui():
-    import inspect
-    from .view import PUIView
-    frame = inspect.currentframe()
-    frames = []
-    while frame:
-        frames.insert(0, frame)
-        views = [v for k,v in frame.f_locals.items() if isinstance(v, PUIView) and v.frames]
-        if views:
-            root = views[0]
-            parent = root.frames[-1]
-
-            for f in frames:
-                fi = inspect.getframeinfo(f)
-                # print(repr(fi.function), fi.filename, fi.lineno)
-                if fi.function != "__wrapped_content__":
-                    key = f"{fi.filename}:{fi.lineno}"
-                    break
-
-            return root, parent, key
-        frame = frame.f_back
-    else:
-        raise RuntimeError("PUIView not found")
-
-class PUINode():
-    def __init__(self):
-        from .view import PUIView
-        self.layout_weight = None
-        self.ui = None
-        if isinstance(self, PUIView):
-            self.root = self
-            self.parent = self
-            self.key = "|".join([type(x).__name__ for x in self.root.frames]+[type(self).__name__])
-        else:
-            self.root, self.parent, key = find_pui()
-            self.key = "|".join([type(x).__name__ for x in self.root.frames]+[type(self).__name__]+[key])
-
-        self.children = []
-
-        if self.parent is self:
-            self.path = tuple()
-        else:
-            self.path = self.parent.path + tuple([len(self.parent.children)])
-            self.parent.children.append(self)
-        # print(type(self).__name__, self.path, "parent=", self.parent.path)
-
+from .node import *
+from .dom import *
+import time
+
+# dprint = print
+dprint = lambda *x: x
+
+class PUIView(PUINode):
+    __ALLVIEWS__  = []
+
+    @staticmethod
+    def reload():
+        for v in PUIView.__ALLVIEWS__:
+            v.redraw()
+
+    def __init__(self, *args, **kwargs):
+        self.children_first = True # default to bottom-up
+        self.frames = []
+        self.last_children = []
+        super().__init__(*args, **kwargs)
+        PUIView.__ALLVIEWS__.append(self)
 
     def __enter__(self):
+        if not hasattr(tls, "puistack"):
+            tls.puistack = []
+        tls.puistack.append(self)
         # print("enter", type(self).__name__, id(self))
         self.root.frames.append(self)
         return self
 
     def __exit__(self, ex_type, value, traceback):
+        tls.puistack.pop()
         # print("exit", type(self).__name__, id(self))
         self.root.frames.pop()
         if ex_type is None: # don't consume exception
             return self
 
-    def comment(self):
-        return None
-
-    def update(self, prev):
-        return None
-
     def destroy(self):
-        return None
-
-    def addChild(self, idx, ui):
-        pass
+        PUIView.__ALLVIEWS__.remove(self)
+        return super().destroy()
 
-    def removeChild(self, idx, ui):
-        pass
+    def content(self):
+        return None
 
-    def __repr__(self):
-        segs = []
-        headline = [
-            "  "*len(self.path),
-            type(self).__name__,
-            # f"@{str(id(self))}", # print view id
-            " {",
-        ]
-
-        # print view key
-        headline.append(" # ")
-        headline.append(self.key)
-
-        headline.append("\n")
-        segs.append("".join(headline))
-
-        comment = self.comment()
-        if comment:
-            segs.append("  "*(len(self.path)+1))
-            segs.append("# ")
-            segs.append(comment)
-            segs.append("\n")
-
-        for i,c in enumerate(self.children):
-            if i > 0:
-                segs.append(",\n")
-            segs.append(c.__repr__())
-        segs.append("\n")
-        segs.append("".join(["  "*len(self.path), "}"]))
-        return "".join(segs)
-
-    def layout(self, weight=None):
-        if not weight is None:
-            self.layout_weight = weight
-        return self
+    def dump(self):
+        dprint(f"content() start", self.key)
+        start = time.time()
+        with self as scope:
+            self.content()
+        dprint(f"content() time: {time.time()-start:.5f}", self.key)
+        return scope
+
+    def redraw(self):
+        self.update()
+
+    def update(self, prev=None):
+        dprint("update()", self.key)
+        if prev:
+            self.last_children = prev.children
 
-    def weight(self, v):
-        self.layout_weight = v
-        return self
+        self.children = []
+        try:
+            dprint(f"content() start", self.key)
+            start = time.time()
+            with self as scope: # CRITICAL: this is the searching target for find_pui()
+                self.content() # V-DOM builder
+            dprint(f"content() time: {time.time()-start:.5f}", self.key)
+        except:
+            # prevent crash in hot-reloading
+            self.children = self.last_children
+            import traceback
+            print("## <ERROR OF content() >")
+            traceback.print_exc()
+            print("## </ERROR OF content()>")
+
+
+        # print("PUIView.update", self) # print DOM
+
+        start = time.time()
+        dprint("sync() start", self.key)
+        sync(self, self.last_children, self.children, self.children_first)
+        dprint(f"sync() time: {time.time()-start:.5f}", self.key)
+
+        self.last_children = self.children
+
+    def run(self):
+        self.update()
+        self.start()
```

### Comparing `QPUIQ-0.1.3/PUI/state.py` & `QPUIQ-0.1.4/PUI/state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 from .view import *
 
 class AttrBinding():
     def __init__(self, state, key):
         try:
-            root, parent = find_pui()
+            root, parent, viewkey = find_pui()
             self.viewroot = root
             self.viewparent = parent
         except:
             pass
         self.state = state
         self.key = key
         dt = type(getattr(self.state, self.key))
@@ -31,18 +31,18 @@
             setattr(self.state, self.key, self.func(value))
         except:
             pass
 
 class KeyBinding():
     def __init__(self, state, key):
         try:
-            root, parent = find_pui()
+            root, parent, viewkey = find_pui()
             self.viewroot = root
             self.viewparent = parent
-        except:
+        except PuiViewNotFoundError:
             pass
         self.state = state
         self.key = key
         dt = type(self.state[self.key])
         if dt is str:
             self.func = str
         elif dt is int:
@@ -73,158 +73,164 @@
         return StateList(data)
     if isinstance(data, dict):
         return StateDict(data)
     return StateObject(data)
 
 class StateObject(BaseState):
     def __init__(self, values=None):
-        object.__setattr__(self, "__listeners", set())
+        self.__listeners = set()
         if values is None:
-            object.__setattr__(self, "__values", BaseState())
+            self.__values = BaseState()
         else:
-            object.__setattr__(self, "__values", values)
+            self.__values = values
 
     def __call__(self, key):
         return AttrBinding(self, key)
 
-    def __getattribute__(self, key):
+    def __getattr__(self, key):
         if not key.startswith("_"):
             try:
-                root, parent, viewkey = find_pui()
-                object.__getattribute__(self, "__listeners").add(root)
-            except:
+                view = find_puiview()
+                self.__listeners.add(view)
+            except PuiViewNotFoundError:
                 pass
-        return getattr(object.__getattribute__(self, "__values"), key)
+        return getattr(self.__values, key)
 
     def __setattr__(self, key, value):
-        if type(value) is list:
-            value = StateList(value)
-        elif type(value) is dict:
-            value = StateDict(value)
-        setattr(object.__getattribute__(self, "__values"), key, value)
-        for l in object.__getattribute__(self, "__listeners"):
-            l.update()
+        if key.startswith("_"):
+            object.__setattr__(self, key, value)
+        else:
+            if type(value) is list:
+                value = StateList(value)
+            elif type(value) is dict:
+                value = StateDict(value)
+            setattr(self.__values, key, value)
+            for l in self.__listeners:
+                l.redraw()
+
+    def __repr__(self):
+        return f"StateObject({self.__values.__repr__()})"
 
 class StateList(BaseState):
     def __init__(self, values=None):
         self.__listeners = set()
         if values is None:
             self.__values = []
         else:
             self.__values = values
 
     def __call__(self, key):
         return KeyBinding(self, key)
 
     def __getitem__(self, key):
         try:
-            root, parent, viewkey = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         return self.__values[key]
 
     def __setitem__(self, key, value):
         self.__values[key] = value
         for l in self.__listeners:
-            l.update()
+            l.redraw()
 
     def __len__(self):
         try:
-            root, parent, viewkey = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         n = len(self.__values)
         return n
 
     def __iter__(self):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         return self.__values.__iter__()
 
     def __repr__(self):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         return self.__values.__repr__()
 
     def append(self, obj):
         self.__values.append(obj)
         for l in self.__listeners:
-            l.update()
+            l.redraw()
 
     def clear(self):
         self.__values.clear()
         for l in self.__listeners:
-            l.update()
+            l.redraw()
 
     def count(self, value):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         return self.__values.count(value)
 
     def extend(self, iterable):
         self.__values.extend(iterable)
         for l in self.__listeners:
-            l.update()
+            l.redraw()
 
     def index(self, value, *args, **kwargs):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         return self.__values.index(value, *args, **kwargs)
 
     def insert(self, index, object):
         self.__values.insert(index, object)
         for l in self.__listeners:
-            l.update()
+            l.redraw()
 
     def pop(self, index=-1):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         r = self.__values.pop(index)
         for l in self.__listeners:
-            l.update()
+            l.redraw()
         return r
 
     def remove(self, value):
         self.__values.remove(value)
         for l in self.__listeners:
-            l.update()
+            l.redraw()
 
     def reverse(self, value):
         self.__values.reverse(value)
         for l in self.__listeners:
-            l.update()
+            l.redraw()
 
 
     def sort(self, *args, **kwargs):
         self.__values.sort(*args, **kwargs)
         for l in self.__listeners:
-            l.update()
+            l.redraw()
 
     def get(self, index, default=None):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         if index >= 0 and index < len(self.__values):
             return self.__values[index]
         else:
             return default
 
     def range(self):
@@ -240,96 +246,96 @@
 
     def __call__(self, key):
         return KeyBinding(self, key)
 
     def __delitem__(self, key):
         self.__values.__delitem__(key)
         for l in self.__listeners:
-            l.update()
+            l.redraw()
 
     def __getitem__(self, key):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         return self.__values[key]
 
     def __iter__(self):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         return self.__values.__iter__()
 
     def __repr__(self):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         return self.__values.__repr__()
 
     def __setitem__(self, key, value):
         self.__values[key] = value
         for l in self.__listeners:
-            l.update()
+            l.redraw()
 
     def clear(self):
         self.__values.clear()
         for l in self.__listeners:
-            l.update()
+            l.redraw()
 
     def get(self, key, default=None):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         return self.__values.get(key, default)
 
     def items(self):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         return self.__values.items()
 
     def keys(self):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         return self.__values.keys()
 
     def pop(self, key):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         r = self.__values.pop(key)
         for l in self.__listeners:
-            l.update()
+            l.redraw()
         return r
 
     def setdefault(self, key, default=None):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         r = self.__values.setdefault(key, default)
         for l in self.__listeners:
-            l.update()
+            l.redraw()
         return r
 
     def values(self):
         try:
-            root, parent = find_pui()
-            self.__listeners.add(root)
-        except:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
             pass
         return self.__values.values()
```

### Comparing `QPUIQ-0.1.3/PUI/timeline.py` & `QPUIQ-0.1.4/PUI/timeline.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/tkinter/__main__.py` & `QPUIQ-0.1.4/PUI/tkinter/__main__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/tkinter/button.py` & `QPUIQ-0.1.4/PUI/tkinter/button.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,8 +9,7 @@
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
             self.ui.config(text = self.text)
             self.ui.config(command = self.callback)
         else:
             self.ui = tk.Button(self.parent.ui, text=self.text, command=self.callback, **self.kwargs)
-        return self.ui
```

### Comparing `QPUIQ-0.1.3/PUI/tkinter/canvas.py` & `QPUIQ-0.1.4/PUI/tkinter/canvas.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from .. import *
 from .base import *
 class TkCanvas(TkBaseWidget):
+    terminal = True
     def __init__(self, size=None, **kwargs):
         super().__init__(**kwargs)
         self.size = size
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
             self.ui = tk.Canvas(self.parent.ui, **self.kwargs)
         self.ui.delete("all")
-        return self.ui
 
 class TkCanvasText(PUINode):
     def __init__(self, x, y, text):
         super().__init__()
         self.x = x
         self.y = y
         self.text = text
```

### Comparing `QPUIQ-0.1.3/PUI/tkinter/layout.py` & `QPUIQ-0.1.4/PUI/tkinter/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/tkinter/textfield.py` & `QPUIQ-0.1.4/PUI/tkinter/textfield.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,12 +16,10 @@
             self.last_value = value
         else:
             self.variable = tk.StringVar(self.parent.ui, str(value))
             self.variable.trace_add("write", self.on_variable_changed)
             self.last_value = value
             self.ui = tk.Entry(self.parent.ui, textvariable=self.variable, **self.kwargs)
 
-        return self.ui
-
     def on_variable_changed(self, var, index, mode):
         value = self.variable.get()
         self.model.value = value
```

### Comparing `QPUIQ-0.1.3/PUI/tkinter/window.py` & `QPUIQ-0.1.4/PUI/tkinter/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/urwid/__main__.py` & `QPUIQ-0.1.4/PUI/urwid/__main__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/urwid/button.py` & `QPUIQ-0.1.4/PUI/urwid/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/urwid/layout.py` & `QPUIQ-0.1.4/PUI/urwid/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/PUI/urwid/window.py` & `QPUIQ-0.1.4/PUI/urwid/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/QPUIQ.egg-info/PKG-INFO` & `QPUIQ-0.1.4/QPUIQ.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.1.3
+Version: 0.1.4
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -110,14 +110,15 @@
 
 # reloadium: after_reload
 def after_reload(actions):
     PUIView.reload()
 ```
 
 # Progress
+* Use threading.locals() instead of inspect
 * State
     * ~~Update Trigger~~
     * ~~Binding~~
     * ~~StateList~~
     * ~~StateDict~~
     * Lazy UI?
 * Passing state to subview
```

### Comparing `QPUIQ-0.1.3/QPUIQ.egg-info/SOURCES.txt` & `QPUIQ-0.1.4/QPUIQ.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.3/README.md` & `QPUIQ-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 
 # reloadium: after_reload
 def after_reload(actions):
     PUIView.reload()
 ```
 
 # Progress
+* Use threading.locals() instead of inspect
 * State
     * ~~Update Trigger~~
     * ~~Binding~~
     * ~~StateList~~
     * ~~StateDict~~
     * Lazy UI?
 * Passing state to subview
```


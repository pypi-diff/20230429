# Comparing `tmp/qt-custom-0.2.1.tar.gz` & `tmp/qt-custom-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\pip_package\qt-custom\dist\.tmp-479pn4us\qt-custom-0.2.1.tar", last modified: Fri Apr 28 05:27:43 2023, max compression
+gzip compressed data, was "C:\pip_package\qt-custom\dist\.tmp-jptz9e30\qt-custom-0.2.2.tar", last modified: Fri Apr 28 23:38:12 2023, max compression
```

## Comparing `qt-custom-0.2.1.tar` & `qt-custom-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 05:27:43.000000 qt-custom-0.2.1/
--rw-rw-rw-   0        0        0     1091 2021-12-14 06:26:44.000000 qt-custom-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2022-02-04 21:52:02.000000 qt-custom-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      485 2023-04-28 05:27:43.000000 qt-custom-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       17 2022-02-04 22:03:27.000000 qt-custom-0.2.1/README.md
--rw-rw-rw-   0        0        0      102 2021-12-14 05:48:57.000000 qt-custom-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      630 2023-04-28 05:27:43.000000 qt-custom-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 05:27:43.000000 qt-custom-0.2.1/source/
-drwxrwxrwx   0        0        0        0 2023-04-28 05:27:43.000000 qt-custom-0.2.1/source/qt_custom/
--rw-rw-rw-   0        0        0        0 2021-12-14 05:13:28.000000 qt-custom-0.2.1/source/qt_custom/__init__.py
--rw-rw-rw-   0        0        0   639488 2022-11-08 03:37:38.000000 qt-custom-0.2.1/source/qt_custom/custom_chart.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   136704 2022-11-08 03:37:40.000000 qt-custom-0.2.1/source/qt_custom/custom_color.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   123904 2022-11-08 03:37:40.000000 qt-custom-0.2.1/source/qt_custom/custom_lineseries.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   194048 2022-10-05 04:03:27.000000 qt-custom-0.2.1/source/qt_custom/custom_listview.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   347136 2022-11-08 03:37:43.000000 qt-custom-0.2.1/source/qt_custom/custom_markers.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0    90112 2022-10-05 04:03:29.000000 qt-custom-0.2.1/source/qt_custom/custom_menubar.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   131584 2022-10-05 04:03:27.000000 qt-custom-0.2.1/source/qt_custom/custom_tab.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   138240 2022-10-05 04:03:28.000000 qt-custom-0.2.1/source/qt_custom/custom_tableview.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   130048 2022-10-05 04:03:29.000000 qt-custom-0.2.1/source/qt_custom/custom_treeview.cp37-win_amd64.pyd
-drwxrwxrwx   0        0        0        0 2023-04-28 05:27:43.000000 qt-custom-0.2.1/source/qt_custom/qt6/
--rw-rw-rw-   0        0        0   685568 2023-04-28 05:24:55.000000 qt-custom-0.2.1/source/qt_custom/qt6/custom_chart.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   118784 2023-04-28 05:24:56.000000 qt-custom-0.2.1/source/qt_custom/qt6/custom_color.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   247808 2023-04-28 05:24:58.000000 qt-custom-0.2.1/source/qt_custom/qt6/custom_lineseries.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   230400 2023-04-28 05:06:51.000000 qt-custom-0.2.1/source/qt_custom/qt6/custom_listview.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   427520 2023-04-28 05:25:01.000000 qt-custom-0.2.1/source/qt_custom/qt6/custom_markers.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0    98816 2023-04-28 05:06:55.000000 qt-custom-0.2.1/source/qt_custom/qt6/custom_menubar.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   133632 2023-04-28 05:06:52.000000 qt-custom-0.2.1/source/qt_custom/qt6/custom_tab.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   145920 2023-04-28 05:06:53.000000 qt-custom-0.2.1/source/qt_custom/qt6/custom_tableview.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   131584 2023-04-28 05:06:54.000000 qt-custom-0.2.1/source/qt_custom/qt6/custom_treeview.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0    65024 2023-04-28 05:06:55.000000 qt-custom-0.2.1/source/qt_custom/qt6/logger_qt_custom.cp37-win_amd64.pyd
-drwxrwxrwx   0        0        0        0 2023-04-28 05:27:43.000000 qt-custom-0.2.1/source/qt_custom.egg-info/
--rw-rw-rw-   0        0        0      485 2023-04-28 05:27:43.000000 qt-custom-0.2.1/source/qt_custom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1256 2023-04-28 05:27:43.000000 qt-custom-0.2.1/source/qt_custom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 05:27:43.000000 qt-custom-0.2.1/source/qt_custom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-28 05:27:43.000000 qt-custom-0.2.1/source/qt_custom.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 23:38:12.000000 qt-custom-0.2.2/
+-rw-rw-rw-   0        0        0     1091 2021-12-14 06:26:44.000000 qt-custom-0.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2022-02-04 21:52:02.000000 qt-custom-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      485 2023-04-28 23:38:12.000000 qt-custom-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2022-02-04 22:03:27.000000 qt-custom-0.2.2/README.md
+-rw-rw-rw-   0        0        0      102 2021-12-14 05:48:57.000000 qt-custom-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      630 2023-04-28 23:38:12.000000 qt-custom-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 23:38:12.000000 qt-custom-0.2.2/source/
+drwxrwxrwx   0        0        0        0 2023-04-28 23:38:12.000000 qt-custom-0.2.2/source/qt_custom/
+-rw-rw-rw-   0        0        0        0 2021-12-14 05:13:28.000000 qt-custom-0.2.2/source/qt_custom/__init__.py
+-rw-rw-rw-   0        0        0   639488 2022-11-08 03:37:38.000000 qt-custom-0.2.2/source/qt_custom/custom_chart.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   136704 2022-11-08 03:37:40.000000 qt-custom-0.2.2/source/qt_custom/custom_color.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   123904 2022-11-08 03:37:40.000000 qt-custom-0.2.2/source/qt_custom/custom_lineseries.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   194048 2022-10-05 04:03:27.000000 qt-custom-0.2.2/source/qt_custom/custom_listview.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   347136 2022-11-08 03:37:43.000000 qt-custom-0.2.2/source/qt_custom/custom_markers.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0    90112 2022-10-05 04:03:29.000000 qt-custom-0.2.2/source/qt_custom/custom_menubar.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   131584 2022-10-05 04:03:27.000000 qt-custom-0.2.2/source/qt_custom/custom_tab.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   138240 2022-10-05 04:03:28.000000 qt-custom-0.2.2/source/qt_custom/custom_tableview.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   130048 2022-10-05 04:03:29.000000 qt-custom-0.2.2/source/qt_custom/custom_treeview.cp37-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2023-04-28 23:38:12.000000 qt-custom-0.2.2/source/qt_custom/qt6/
+-rw-rw-rw-   0        0        0   665600 2023-04-28 19:26:51.000000 qt-custom-0.2.2/source/qt_custom/qt6/custom_chart.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   118784 2023-04-28 19:26:52.000000 qt-custom-0.2.2/source/qt_custom/qt6/custom_color.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   247808 2023-04-28 19:26:54.000000 qt-custom-0.2.2/source/qt_custom/qt6/custom_lineseries.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   230400 2023-04-28 05:06:51.000000 qt-custom-0.2.2/source/qt_custom/qt6/custom_listview.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   427520 2023-04-28 19:26:57.000000 qt-custom-0.2.2/source/qt_custom/qt6/custom_markers.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0    98816 2023-04-28 05:06:55.000000 qt-custom-0.2.2/source/qt_custom/qt6/custom_menubar.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   133632 2023-04-28 05:06:52.000000 qt-custom-0.2.2/source/qt_custom/qt6/custom_tab.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   145920 2023-04-28 05:06:53.000000 qt-custom-0.2.2/source/qt_custom/qt6/custom_tableview.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   131584 2023-04-28 05:06:54.000000 qt-custom-0.2.2/source/qt_custom/qt6/custom_treeview.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0    65024 2023-04-28 05:06:55.000000 qt-custom-0.2.2/source/qt_custom/qt6/logger_qt_custom.cp37-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2023-04-28 23:38:12.000000 qt-custom-0.2.2/source/qt_custom.egg-info/
+-rw-rw-rw-   0        0        0      485 2023-04-28 23:38:12.000000 qt-custom-0.2.2/source/qt_custom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1256 2023-04-28 23:38:12.000000 qt-custom-0.2.2/source/qt_custom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 23:38:12.000000 qt-custom-0.2.2/source/qt_custom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-28 23:38:12.000000 qt-custom-0.2.2/source/qt_custom.egg-info/top_level.txt
```

### Comparing `qt-custom-0.2.1/LICENSE.txt` & `qt-custom-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qt-custom-0.2.1/setup.cfg` & `qt-custom-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 742d 6375 7374 6f6d 0d0a 7665   = qt-custom..ve
-00000020: 7273 696f 6e20 3d20 302e 322e 310d 0a61  rsion = 0.2.1..a
+00000020: 7273 696f 6e20 3d20 302e 322e 320d 0a61  rsion = 0.2.2..a
 00000030: 7574 686f 7220 3d20 616e 6f6e 796d 6f75  uthor = anonymou
 00000040: 730d 0a61 7574 686f 725f 656d 6169 6c20  s..author_email 
 00000050: 3d20 616e 6f6e 796d 6f75 7340 676d 6169  = anonymous@gmai
 00000060: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
 00000070: 6f6e 203d 2043 7573 746f 6d69 7a65 6420  on = Customized 
 00000080: 5174 2043 6c61 7373 6573 0d0a 6c6f 6e67  Qt Classes..long
 00000090: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
```

### Comparing `qt-custom-0.2.1/source/qt_custom.egg-info/SOURCES.txt` & `qt-custom-0.2.2/source/qt_custom.egg-info/SOURCES.txt`

 * *Files identical despite different names*


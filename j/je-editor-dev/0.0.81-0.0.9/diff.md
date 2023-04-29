# Comparing `tmp/je_editor_dev-0.0.81.tar.gz` & `tmp/je_editor_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_editor_dev-0.0.81.tar", last modified: Sat Apr 29 10:41:32 2023, max compression
+gzip compressed data, was "je_editor_dev-0.0.9.tar", last modified: Fri Jan 14 21:02:54 2022, max compression
```

## Comparing `je_editor_dev-0.0.81.tar` & `je_editor_dev-0.0.9.tar`

### file list

```diff
@@ -1,97 +1,106 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.989744 je_editor_dev-0.0.81/
--rw-rw-rw-   0        0        0     1085 2023-04-20 11:44:51.000000 je_editor_dev-0.0.81/LICENSE
--rw-rw-rw-   0        0        0     2835 2023-04-29 10:41:32.988745 je_editor_dev-0.0.81/PKG-INFO
--rw-rw-rw-   0        0        0     2201 2023-04-29 10:40:11.000000 je_editor_dev-0.0.81/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.896482 je_editor_dev-0.0.81/je_editor/
--rw-rw-rw-   0        0        0     1429 2023-04-27 11:03:49.000000 je_editor_dev-0.0.81/je_editor/__init__.py
--rw-rw-rw-   0        0        0      598 2023-04-20 11:44:51.000000 je_editor_dev-0.0.81/je_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.897480 je_editor_dev-0.0.81/je_editor/pyside_ui/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:44:51.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.899508 je_editor_dev-0.0.81/je_editor/pyside_ui/auto_save/
--rw-rw-rw-   0        0        0        0 2023-04-24 10:50:54.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/auto_save/__init__.py
--rw-rw-rw-   0        0        0     1071 2023-04-24 10:50:54.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/auto_save/auto_save_thread.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.902466 je_editor_dev-0.0.81/je_editor/pyside_ui/code_editor/
--rw-rw-rw-   0        0        0        0 2023-04-26 11:14:17.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/code_editor/__init__.py
--rw-rw-rw-   0        0        0     5355 2023-04-28 11:00:32.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.904494 je_editor_dev-0.0.81/je_editor/pyside_ui/code_process/
--rw-rw-rw-   0        0        0        0 2023-04-23 14:01:39.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/code_process/__init__.py
--rw-rw-rw-   0        0        0     7331 2023-04-27 11:33:59.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/code_process/code_exec.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.907453 je_editor_dev-0.0.81/je_editor/pyside_ui/code_result/
--rw-rw-rw-   0        0        0        0 2023-04-28 11:00:32.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/code_result/__init__.py
--rw-rw-rw-   0        0        0     1393 2023-04-28 11:00:32.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/code_result/code_record.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.909481 je_editor_dev-0.0.81/je_editor/pyside_ui/colors/
--rw-rw-rw-   0        0        0        0 2023-04-24 15:35:13.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/colors/__init__.py
--rw-rw-rw-   0        0        0      123 2023-04-24 15:37:08.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/colors/global_color.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.913471 je_editor_dev-0.0.81/je_editor/pyside_ui/file_dialog/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/file_dialog/__init__.py
--rw-rw-rw-   0        0        0     1058 2023-04-26 12:09:26.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/file_dialog/open_file_dialog.py
--rw-rw-rw-   0        0        0      995 2023-04-24 10:50:54.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/file_dialog/save_file_dialog.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.915432 je_editor_dev-0.0.81/je_editor/pyside_ui/main_ui/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/main_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.917426 je_editor_dev-0.0.81/je_editor/pyside_ui/main_ui/editor_main_ui/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
--rw-rw-rw-   0        0        0     4279 2023-04-28 11:00:32.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.920418 je_editor_dev-0.0.81/je_editor/pyside_ui/main_ui_setting/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/main_ui_setting/__init__.py
--rw-rw-rw-   0        0        0     1634 2023-04-28 11:00:32.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/main_ui_setting/ui_setting.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.922412 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:44:51.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.924407 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.926401 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
--rw-rw-rw-   0        0        0        0 2023-04-26 11:14:17.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
--rw-rw-rw-   0        0        0     1646 2023-04-28 11:00:32.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.929393 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/file_menu/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
--rw-rw-rw-   0        0        0     1034 2023-04-26 11:14:17.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.931388 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/help_menu/
--rw-rw-rw-   0        0        0        0 2023-04-26 11:14:17.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
--rw-rw-rw-   0        0        0     1223 2023-04-28 11:00:32.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.934380 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/run_menu/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
--rw-rw-rw-   0        0        0     2021 2023-04-26 12:09:57.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
--rw-rw-rw-   0        0        0     1118 2023-04-26 13:11:18.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.938370 je_editor_dev-0.0.81/je_editor/pyside_ui/search_ui/
--rw-rw-rw-   0        0        0        0 2023-04-28 11:00:32.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/search_ui/__init__.py
--rw-rw-rw-   0        0        0      865 2023-04-28 11:00:32.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/search_ui/search_error_box.py
--rw-rw-rw-   0        0        0      857 2023-04-28 11:00:32.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/search_ui/search_text_box.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.940364 je_editor_dev-0.0.81/je_editor/pyside_ui/shell_process/
--rw-rw-rw-   0        0        0        0 2023-04-23 14:01:47.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/shell_process/__init__.py
--rw-rw-rw-   0        0        0     6028 2023-04-26 12:07:18.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/shell_process/shell_exec.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.942359 je_editor_dev-0.0.81/je_editor/pyside_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-04-24 10:50:54.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0     3749 2023-04-26 11:14:17.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/syntax/python_syntax.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.944354 je_editor_dev-0.0.81/je_editor/pyside_ui/treeview/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/treeview/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.946349 je_editor_dev-0.0.81/je_editor/pyside_ui/treeview/project_treeview/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/treeview/project_treeview/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-04-28 11:00:32.000000 je_editor_dev-0.0.81/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
--rw-rw-rw-   0        0        0      393 2023-04-26 11:14:17.000000 je_editor_dev-0.0.81/je_editor/start_editor.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.948381 je_editor_dev-0.0.81/je_editor/utils/
--rw-rw-rw-   0        0        0        2 2023-04-20 11:44:51.000000 je_editor_dev-0.0.81/je_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.952333 je_editor_dev-0.0.81/je_editor/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-04-20 11:44:51.000000 je_editor_dev-0.0.81/je_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      960 2023-04-26 11:14:17.000000 je_editor_dev-0.0.81/je_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      506 2023-04-20 11:44:51.000000 je_editor_dev-0.0.81/je_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.954327 je_editor_dev-0.0.81/je_editor/utils/file/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:44:51.000000 je_editor_dev-0.0.81/je_editor/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.956322 je_editor_dev-0.0.81/je_editor/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-04-20 11:44:51.000000 je_editor_dev-0.0.81/je_editor/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      962 2023-04-23 13:34:13.000000 je_editor_dev-0.0.81/je_editor/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.960312 je_editor_dev-0.0.81/je_editor/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-04-20 11:44:51.000000 je_editor_dev-0.0.81/je_editor/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      719 2023-04-26 12:08:16.000000 je_editor_dev-0.0.81/je_editor/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.963303 je_editor_dev-0.0.81/je_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-04-20 11:44:51.000000 je_editor_dev-0.0.81/je_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      983 2023-04-29 07:51:28.000000 je_editor_dev-0.0.81/je_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.965299 je_editor_dev-0.0.81/je_editor/utils/redirect_manager/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:44:51.000000 je_editor_dev-0.0.81/je_editor/utils/redirect_manager/__init__.py
--rw-rw-rw-   0        0        0     1991 2023-04-20 11:44:51.000000 je_editor_dev-0.0.81/je_editor/utils/redirect_manager/redirect_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:32.987785 je_editor_dev-0.0.81/je_editor_dev.egg-info/
--rw-rw-rw-   0        0        0     2835 2023-04-29 10:41:32.000000 je_editor_dev-0.0.81/je_editor_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2811 2023-04-29 10:41:32.000000 je_editor_dev-0.0.81/je_editor_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:41:32.000000 je_editor_dev-0.0.81/je_editor_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 10:41:32.000000 je_editor_dev-0.0.81/je_editor_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-29 10:41:32.000000 je_editor_dev-0.0.81/je_editor_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      940 2023-04-29 10:41:15.000000 je_editor_dev-0.0.81/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 10:41:32.989744 je_editor_dev-0.0.81/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.296718 je_editor_dev-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1481 2022-01-14 21:02:54.294720 je_editor_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      860 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/README.md
+-rw-rw-rw-   0        0        0      909 2022-01-14 21:02:51.000000 je_editor_dev-0.0.9/dev_setup.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.033720 je_editor_dev-0.0.9/je_editor/
+-rw-rw-rw-   0        0        0      608 2022-01-14 18:33:11.000000 je_editor_dev-0.0.9/je_editor/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.036723 je_editor_dev-0.0.9/je_editor/ui/
+-rw-rw-rw-   0        0        0       28 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.041717 je_editor_dev-0.0.9/je_editor/ui/editor_main_ui/
+-rw-rw-rw-   0        0        0       43 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/editor_main_ui/__init__.py
+-rw-rw-rw-   0        0        0    11111 2022-01-14 21:02:13.000000 je_editor_dev-0.0.9/je_editor/ui/editor_main_ui/tkinter_editor.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.043734 je_editor_dev-0.0.9/je_editor/ui/ui_event/
+-rw-rw-rw-   0        0        0       37 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.046718 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/
+-rw-rw-rw-   0        0        0       47 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.052732 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/start_auto_save/
+-rw-rw-rw-   0        0        0       65 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/start_auto_save/__init__.py
+-rw-rw-rw-   0        0        0      460 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/start_auto_save/start_auto_save.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.057723 je_editor_dev-0.0.9/je_editor/ui/ui_event/change_font/
+-rw-rw-rw-   0        0        0       49 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/change_font/__init__.py
+-rw-rw-rw-   0        0        0      844 2022-01-14 11:49:29.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/change_font/change_font.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.064718 je_editor_dev-0.0.9/je_editor/ui/ui_event/close/
+-rw-rw-rw-   0        0        0       43 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/close/__init__.py
+-rw-rw-rw-   0        0        0      532 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/close/close_event.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.069721 je_editor_dev-0.0.9/je_editor/ui/ui_event/encoding/
+-rw-rw-rw-   0        0        0       46 2022-01-14 11:46:17.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/encoding/__init__.py
+-rw-rw-rw-   0        0        0       89 2022-01-14 11:49:29.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/encoding/set_encoding.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.071718 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/
+-rw-rw-rw-   0        0        0       45 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.076726 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_code/
+-rw-rw-rw-   0        0        0       58 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_code/__init__.py
+-rw-rw-rw-   0        0        0      538 2022-01-09 13:01:31.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_code/exec_code.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.082720 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_shell_command/
+-rw-rw-rw-   0        0        0       67 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_shell_command/__init__.py
+-rw-rw-rw-   0        0        0      726 2022-01-06 02:44:24.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_shell_command/run_on_shell.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.087718 je_editor_dev-0.0.9/je_editor/ui/ui_event/language/
+-rw-rw-rw-   0        0        0       46 2022-01-14 12:08:46.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/language/__init__.py
+-rw-rw-rw-   0        0        0       89 2022-01-14 12:08:46.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/language/set_language.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.090719 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/
+-rw-rw-rw-   0        0        0        2 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.096719 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_file_to_read/
+-rw-rw-rw-   0        0        0       65 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_file_to_read/__init__.py
+-rw-rw-rw-   0        0        0      655 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_file_to_read/open_file_to_read.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.103719 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_last_edit_file/
+-rw-rw-rw-   0        0        0       67 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_last_edit_file/__init__.py
+-rw-rw-rw-   0        0        0      638 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_last_edit_file/open_last_edit_file.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.105717 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/
+-rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.112718 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/save_file_to_open/
+-rw-rw-rw-   0        0        0       65 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/save_file_to_open/__init__.py
+-rw-rw-rw-   0        0        0      593 2022-01-06 18:18:59.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/save_file_to_open/save_file_to_open.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.115717 je_editor_dev-0.0.9/je_editor/ui/ui_utils/
+-rw-rw-rw-   0        0        0       37 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/je_editor/ui/ui_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.122717 je_editor_dev-0.0.9/je_editor/ui/ui_utils/font/
+-rw-rw-rw-   0        0        0       42 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/je_editor/ui/ui_utils/font/__init__.py
+-rw-rw-rw-   0        0        0      292 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/je_editor/ui/ui_utils/font/font.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.126718 je_editor_dev-0.0.9/je_editor/utils/
+-rw-rw-rw-   0        0        0       31 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.140721 je_editor_dev-0.0.9/je_editor/utils/code_tag/
+-rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/code_tag/__init__.py
+-rw-rw-rw-   0        0        0       96 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/code_tag/keyword_list.py
+-rw-rw-rw-   0        0        0     1805 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/code_tag/tag_keyword.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.153718 je_editor_dev-0.0.9/je_editor/utils/editor_content/
+-rw-rw-rw-   0        0        0       46 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/editor_content/__init__.py
+-rw-rw-rw-   0        0        0     1519 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/editor_content/content_save.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.164717 je_editor_dev-0.0.9/je_editor/utils/encoding/
+-rw-rw-rw-   0        0        0       40 2022-01-14 11:17:11.000000 je_editor_dev-0.0.9/je_editor/utils/encoding/__init__.py
+-rw-rw-rw-   0        0        0     1717 2022-01-14 11:17:11.000000 je_editor_dev-0.0.9/je_editor/utils/encoding/encoding_data_module.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.176718 je_editor_dev-0.0.9/je_editor/utils/exception/
+-rw-rw-rw-   0        0        0       41 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      497 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/exception/je_editor_exception_tag.py
+-rw-rw-rw-   0        0        0      488 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/exception/je_editor_exceptions.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.179718 je_editor_dev-0.0.9/je_editor/utils/file/
+-rw-rw-rw-   0        0        0       36 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.184719 je_editor_dev-0.0.9/je_editor/utils/file/open/
+-rw-rw-rw-   0        0        0       41 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0     1532 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.190721 je_editor_dev-0.0.9/je_editor/utils/file/save/
+-rw-rw-rw-   0        0        0       39 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0     2423 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.196718 je_editor_dev-0.0.9/je_editor/utils/language/
+-rw-rw-rw-   0        0        0       40 2022-01-14 11:56:38.000000 je_editor_dev-0.0.9/je_editor/utils/language/__init__.py
+-rw-rw-rw-   0        0        0       68 2022-01-14 12:01:15.000000 je_editor_dev-0.0.9/je_editor/utils/language/language_data_module.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.206727 je_editor_dev-0.0.9/je_editor/utils/string_translate/
+-rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/string_translate/__init__.py
+-rw-rw-rw-   0        0        0       54 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/string_translate/used_string.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.212718 je_editor_dev-0.0.9/je_editor/utils/text_process/
+-rw-rw-rw-   0        0        0       44 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.228718 je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/
+-rw-rw-rw-   0        0        0       57 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/__init__.py
+-rw-rw-rw-   0        0        0     5984 2022-01-14 18:36:19.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/exec_text.py
+-rw-rw-rw-   0        0        0      327 2022-01-07 18:49:28.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/process_error.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.237720 je_editor_dev-0.0.9/je_editor/utils/text_process/shell/
+-rw-rw-rw-   0        0        0       50 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/shell/__init__.py
+-rw-rw-rw-   0        0        0      448 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/shell/shell_text.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.242718 je_editor_dev-0.0.9/je_editor/utils/theme/
+-rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/theme/__init__.py
+-rw-rw-rw-   0        0        0       96 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/theme/theme.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.290718 je_editor_dev-0.0.9/je_editor_dev.egg-info/
+-rw-rw-rw-   0        0        0     1481 2022-01-14 21:02:53.000000 je_editor_dev-0.0.9/je_editor_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2968 2022-01-14 21:02:53.000000 je_editor_dev-0.0.9/je_editor_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-14 21:02:53.000000 je_editor_dev-0.0.9/je_editor_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2022-01-14 21:02:53.000000 je_editor_dev-0.0.9/je_editor_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-01-14 21:02:54.296718 je_editor_dev-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      901 2022-01-13 14:16:52.000000 je_editor_dev-0.0.9/setup.py
```

### Comparing `je_editor_dev-0.0.81/LICENSE` & `je_editor_dev-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.81/je_editor/pyside_ui/code_process/code_exec.py` & `je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/exec_text.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,173 +1,139 @@
+import sys
 import os.path
 import queue
 import shutil
 import subprocess
 from pathlib import Path
 from threading import Thread
+from tkinter import DISABLED
+from tkinter import END
+from tkinter import NORMAL
+
+from je_editor.utils.exception.je_editor_exception_tag import file_not_fond_error
+from je_editor.utils.exception.je_editor_exception_tag import python_not_found_error
+from je_editor.utils.exception.je_editor_exceptions import JEditorExecException
 
-from PySide6.QtCore import QTimer
-from PySide6.QtWidgets import QMainWindow, QTextEdit
-
-from je_editor.pyside_ui.colors.global_color import error_color, output_color
-from je_editor.utils.exception.exception_tags import compiler_not_found_error, je_editor_init_error
-from je_editor.utils.exception.exception_tags import file_not_fond_error
-from je_editor.utils.exception.exceptions import JEditorExecException, JEditorException
+language_compiler = {"java": "javac"}
+language_compiler_param = {"java": "-encoding UTF-8 -d -cp ."}
 
 
 class ExecManager(object):
 
     def __init__(
             self,
-            main_window=None,
+            run_result,
+            process_error_function,
+            main_window,
+            running_menu,
             program_language="python",
-            program_encoding="utf-8",
-            program_buffer=10240000,
+            program_encoding="utf-8"
     ):
-        """
-        :param main_window: tkinter main window
-        :param program_language: which program language
-        :param program_encoding: which encoding
-        """
         self.read_program_error_output_from_thread = None
         self.read_program_output_from_thread = None
-        self.main_window: QMainWindow = main_window
-        self.code_result: [QTextEdit, None] = None
-        self.timer: [QTimer, None] = None
+        self.main_window = main_window
         self.still_run_program = True
+        self.run_result = run_result
+        self.process_error_function = process_error_function
         self.process = None
         self.run_output_queue = queue.Queue()
         self.run_error_queue = queue.Queue()
         self.program_language = program_language
+        self.running_menu = running_menu
         self.program_encoding = program_encoding
-        self.program_buffer = program_buffer
-
-    def later_init(self):
-        if self.main_window is not None:
-            self.code_result: QTextEdit = self.main_window.code_result
-            self.timer = QTimer(self.main_window)
-        else:
-            raise JEditorException(je_editor_init_error)
 
     def exec_code(self, exec_file_name):
         """
         :param exec_file_name: string file will open to run
         :return: if error return result and True else return result and False
         """
+        self.exit_program()
+        self.running_menu.entryconfigure(1, label="Rerun")
+        self.running_menu.entryconfigure(3, state="normal")
+        self.run_result.configure(state=NORMAL)
+        self.run_result.delete("1.0", "end-1c")
+        self.run_result.configure(state=DISABLED)
+        reformat_os_file_path = os.path.abspath(exec_file_name)
         try:
-            self.exit_program()
-            self.code_result.setPlainText("")
-            reformat_os_file_path = os.path.abspath(exec_file_name)
-            # detect file is exist
-            try:
-                if not Path(exec_file_name).exists():
-                    raise JEditorExecException(file_not_fond_error)
-            except OSError as error:
-                raise JEditorExecException(error)
+            if not Path(exec_file_name).exists():
+                raise JEditorExecException(file_not_fond_error)
+        except OSError as error:
+            raise JEditorExecException(error)
+        if sys.platform in ["linux", "linux2", "win32", "cygwin", "msys"]:
             compiler_path = shutil.which(self.program_language)
-            if compiler_path is None and self.program_language == "python":
-                compiler_path = shutil.which("python3")
-            elif compiler_path is None and self.program_language == "python3":
-                compiler_path = shutil.which("python")
-            if compiler_path is None:
-                raise JEditorExecException(compiler_not_found_error)
-            exec_file = reformat_os_file_path
-            # run program
-            execute_program_list = [compiler_path, exec_file]
+        else:
+            compiler_path = shutil.which(self.program_language)
+        if compiler_path is None:
+            raise JEditorExecException(python_not_found_error)
+        exec_command = reformat_os_file_path
+
+        if self.program_language in language_compiler:
             self.process = subprocess.Popen(
-                execute_program_list,
+                [
+                    shutil.which(language_compiler.get(self.program_language)),
+                    language_compiler_param.get(self.program_language),
+                    reformat_os_file_path
+                ],
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
                 shell=False
             )
-            self.still_run_program = True
-            # program output message queue thread
-            self.read_program_output_from_thread = Thread(
-                target=self.read_program_output_from_process,
-                daemon=True
-            )
-            self.read_program_output_from_thread.start()
-            # program error message queue thread
-            self.read_program_error_output_from_thread = Thread(
-                target=self.read_program_error_output_from_process,
-                daemon=True
-            )
-            self.read_program_error_output_from_thread.start()
-            # show which file execute
-            self.code_result.append(compiler_path + " " + reformat_os_file_path)
-            # start tkinter_ui update
-            # start timer
-            self.timer = QTimer(self.main_window)
-            self.timer.setInterval(1)
-            self.timer.timeout.connect(self.pull_text)
-            self.timer.start()
-        except Exception as error:
-            self.code_result.setTextColor(error_color)
-            self.code_result.append(str(error))
-            self.code_result.setTextColor(output_color)
-
-    # tkinter_ui update method
-    def pull_text(self):
-        try:
-            self.code_result.setTextColor(error_color)
-            if not self.run_error_queue.empty():
-                error_message = self.run_error_queue.get_nowait()
-                error_message = str(error_message).strip()
-                if error_message:
-                    self.code_result.append(error_message)
-            self.code_result.setTextColor(output_color)
-            if not self.run_output_queue.empty():
-                output_message = self.run_output_queue.get_nowait()
-                output_message = str(output_message).strip()
-                if output_message:
-                    self.code_result.append(output_message)
-        except queue.Empty:
-            pass
-        if self.process.returncode == 0:
-            self.exit_program()
-        elif self.process.returncode is not None:
+            while self.process.returncode is None:
+                self.process.poll()
+        self.process = subprocess.Popen([compiler_path, exec_command],
+                                        stdout=subprocess.PIPE,
+                                        stderr=subprocess.PIPE,
+                                        shell=False)
+        self.still_run_program = True
+        self.read_program_output_from_thread = Thread(
+            target=self.read_program_output_from_process,
+        )
+        self.read_program_output_from_thread.setDaemon(True)
+        self.read_program_output_from_thread.start()
+        self.read_program_error_output_from_thread = Thread(
+            target=self.read_program_error_output_from_process,
+        )
+        self.read_program_error_output_from_thread.setDaemon(True)
+        self.read_program_error_output_from_thread.start()
+        self.run_result.configure(state=NORMAL)
+        self.run_result.insert(END, compiler_path + " " + reformat_os_file_path + "\n")
+        self.run_result.configure(state=DISABLED)
+        self.edit_tkinter_text()
+
+    def edit_tkinter_text(self):
+        self.run_result.configure(state=NORMAL)
+        if not self.run_error_queue.empty():
+            error_message = self.run_error_queue.get_nowait()
+            self.process_error_function(self.run_result, error_message)
+        if not self.run_output_queue.empty():
+            output_message = self.run_output_queue.get_nowait()
+            self.run_result.insert(END, output_message)
+        self.run_result.configure(state=DISABLED)
+        if self.process.returncode is not None:
             self.exit_program()
-            self.timer.stop()
         if self.still_run_program:
-            # poll return code
+            self.main_window.after(10, self.edit_tkinter_text)
             self.process.poll()
+        else:
+            self.running_menu.entryconfigure(1, label="Run")
+            self.running_menu.entryconfigure(3, state="disable")
 
-    # exit program change run flag to false and clean read thread and queue and process
     def exit_program(self):
         self.still_run_program = False
         if self.read_program_output_from_thread is not None:
             self.read_program_output_from_thread = None
         if self.read_program_error_output_from_thread is not None:
             self.read_program_error_output_from_thread = None
-        self.print_and_clear_queue()
-        if self.process is not None:
-            self.process.terminate()
-
-    def print_and_clear_queue(self):
-        try:
-            for std_output in iter(self.run_output_queue.get_nowait, None):
-                std_output = str(std_output).strip()
-                if std_output:
-                    self.code_result.append(std_output)
-            self.code_result.setTextColor(error_color)
-            for std_err in iter(self.run_error_queue.get_nowait, None):
-                std_err = str(std_err).strip()
-                if std_err:
-                    self.code_result.append(std_err)
-            self.code_result.setTextColor(output_color)
-        except queue.Empty:
-            pass
         self.run_output_queue = queue.Queue()
         self.run_error_queue = queue.Queue()
+        if self.process is not None:
+            self.process.terminate()
 
     def read_program_output_from_process(self):
         while self.still_run_program:
-            program_output_data = self.process.stdout.raw.read(self.program_buffer).decode(self.program_encoding)
-            self.run_output_queue.put_nowait(program_output_data)
+            program_output_data = self.process.stdout.raw.read(1024).decode(self.program_encoding)
+            self.run_output_queue.put(program_output_data)
 
     def read_program_error_output_from_process(self):
         while self.still_run_program:
-            program_error_output_data = self.process.stderr.raw.read(self.program_buffer).decode(self.program_encoding)
-            self.run_error_queue.put_nowait(program_error_output_data)
-
-
-exec_manage = ExecManager()
+            program_error_output_data = self.process.stderr.raw.read(1024).decode(self.program_encoding)
+            self.run_error_queue.put(program_error_output_data)
```

### Comparing `je_editor_dev-0.0.81/je_editor_dev.egg-info/SOURCES.txt` & `je_editor_dev-0.0.9/je_editor_dev.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 LICENSE
 README.md
-pyproject.toml
+dev_setup.py
+setup.py
 je_editor/__init__.py
-je_editor/__main__.py
-je_editor/start_editor.py
-je_editor/pyside_ui/__init__.py
-je_editor/pyside_ui/auto_save/__init__.py
-je_editor/pyside_ui/auto_save/auto_save_thread.py
-je_editor/pyside_ui/code_editor/__init__.py
-je_editor/pyside_ui/code_editor/code_edit_plaintext.py
-je_editor/pyside_ui/code_process/__init__.py
-je_editor/pyside_ui/code_process/code_exec.py
-je_editor/pyside_ui/code_result/__init__.py
-je_editor/pyside_ui/code_result/code_record.py
-je_editor/pyside_ui/colors/__init__.py
-je_editor/pyside_ui/colors/global_color.py
-je_editor/pyside_ui/file_dialog/__init__.py
-je_editor/pyside_ui/file_dialog/open_file_dialog.py
-je_editor/pyside_ui/file_dialog/save_file_dialog.py
-je_editor/pyside_ui/main_ui/__init__.py
-je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
-je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
-je_editor/pyside_ui/main_ui_setting/__init__.py
-je_editor/pyside_ui/main_ui_setting/ui_setting.py
-je_editor/pyside_ui/menu/__init__.py
-je_editor/pyside_ui/menu/menu_bar/__init__.py
-je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
-je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
-je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
-je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
-je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
-je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
-je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
-je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
-je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
-je_editor/pyside_ui/search_ui/__init__.py
-je_editor/pyside_ui/search_ui/search_error_box.py
-je_editor/pyside_ui/search_ui/search_text_box.py
-je_editor/pyside_ui/shell_process/__init__.py
-je_editor/pyside_ui/shell_process/shell_exec.py
-je_editor/pyside_ui/syntax/__init__.py
-je_editor/pyside_ui/syntax/python_syntax.py
-je_editor/pyside_ui/treeview/__init__.py
-je_editor/pyside_ui/treeview/project_treeview/__init__.py
-je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
+je_editor/ui/__init__.py
+je_editor/ui/editor_main_ui/__init__.py
+je_editor/ui/editor_main_ui/tkinter_editor.py
+je_editor/ui/ui_event/__init__.py
+je_editor/ui/ui_event/auto_save/__init__.py
+je_editor/ui/ui_event/auto_save/start_auto_save/__init__.py
+je_editor/ui/ui_event/auto_save/start_auto_save/start_auto_save.py
+je_editor/ui/ui_event/change_font/__init__.py
+je_editor/ui/ui_event/change_font/change_font.py
+je_editor/ui/ui_event/close/__init__.py
+je_editor/ui/ui_event/close/close_event.py
+je_editor/ui/ui_event/encoding/__init__.py
+je_editor/ui/ui_event/encoding/set_encoding.py
+je_editor/ui/ui_event/execute/__init__.py
+je_editor/ui/ui_event/execute/execute_code/__init__.py
+je_editor/ui/ui_event/execute/execute_code/exec_code.py
+je_editor/ui/ui_event/execute/execute_shell_command/__init__.py
+je_editor/ui/ui_event/execute/execute_shell_command/run_on_shell.py
+je_editor/ui/ui_event/language/__init__.py
+je_editor/ui/ui_event/language/set_language.py
+je_editor/ui/ui_event/open_file/__init__.py
+je_editor/ui/ui_event/open_file/open_file_to_read/__init__.py
+je_editor/ui/ui_event/open_file/open_file_to_read/open_file_to_read.py
+je_editor/ui/ui_event/open_file/open_last_edit_file/__init__.py
+je_editor/ui/ui_event/open_file/open_last_edit_file/open_last_edit_file.py
+je_editor/ui/ui_event/save_file/__init__.py
+je_editor/ui/ui_event/save_file/save_file_to_open/__init__.py
+je_editor/ui/ui_event/save_file/save_file_to_open/save_file_to_open.py
+je_editor/ui/ui_utils/__init__.py
+je_editor/ui/ui_utils/font/__init__.py
+je_editor/ui/ui_utils/font/font.py
 je_editor/utils/__init__.py
+je_editor/utils/code_tag/__init__.py
+je_editor/utils/code_tag/keyword_list.py
+je_editor/utils/code_tag/tag_keyword.py
+je_editor/utils/editor_content/__init__.py
+je_editor/utils/editor_content/content_save.py
+je_editor/utils/encoding/__init__.py
+je_editor/utils/encoding/encoding_data_module.py
 je_editor/utils/exception/__init__.py
-je_editor/utils/exception/exception_tags.py
-je_editor/utils/exception/exceptions.py
+je_editor/utils/exception/je_editor_exception_tag.py
+je_editor/utils/exception/je_editor_exceptions.py
 je_editor/utils/file/__init__.py
 je_editor/utils/file/open/__init__.py
 je_editor/utils/file/open/open_file.py
 je_editor/utils/file/save/__init__.py
 je_editor/utils/file/save/save_file.py
-je_editor/utils/json_format/__init__.py
-je_editor/utils/json_format/json_process.py
-je_editor/utils/redirect_manager/__init__.py
-je_editor/utils/redirect_manager/redirect_manager_class.py
+je_editor/utils/language/__init__.py
+je_editor/utils/language/language_data_module.py
+je_editor/utils/string_translate/__init__.py
+je_editor/utils/string_translate/used_string.py
+je_editor/utils/text_process/__init__.py
+je_editor/utils/text_process/program_exec/__init__.py
+je_editor/utils/text_process/program_exec/exec_text.py
+je_editor/utils/text_process/program_exec/process_error.py
+je_editor/utils/text_process/shell/__init__.py
+je_editor/utils/text_process/shell/shell_text.py
+je_editor/utils/theme/__init__.py
+je_editor/utils/theme/theme.py
 je_editor_dev.egg-info/PKG-INFO
 je_editor_dev.egg-info/SOURCES.txt
 je_editor_dev.egg-info/dependency_links.txt
-je_editor_dev.egg-info/requires.txt
 je_editor_dev.egg-info/top_level.txt
```


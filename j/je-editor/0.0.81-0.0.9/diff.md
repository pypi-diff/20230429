# Comparing `tmp/je_editor-0.0.81.tar.gz` & `tmp/je_editor-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_editor-0.0.81.tar", last modified: Sat Apr 29 10:40:30 2023, max compression
+gzip compressed data, was "dist\je_editor-0.0.9.tar", last modified: Sat Sep  4 14:08:51 2021, max compression
```

## Comparing `je_editor-0.0.81.tar` & `je_editor-0.0.9.tar`

### file list

```diff
@@ -1,97 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.220360 je_editor-0.0.81/
--rw-rw-rw-   0        0        0     1085 2023-04-20 11:44:51.000000 je_editor-0.0.81/LICENSE
--rw-rw-rw-   0        0        0     2831 2023-04-29 10:40:30.219393 je_editor-0.0.81/PKG-INFO
--rw-rw-rw-   0        0        0     2201 2023-04-29 10:40:11.000000 je_editor-0.0.81/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.115677 je_editor-0.0.81/je_editor/
--rw-rw-rw-   0        0        0     1429 2023-04-27 11:03:49.000000 je_editor-0.0.81/je_editor/__init__.py
--rw-rw-rw-   0        0        0      598 2023-04-20 11:44:51.000000 je_editor-0.0.81/je_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.150546 je_editor-0.0.81/je_editor/pyside_ui/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:44:51.000000 je_editor-0.0.81/je_editor/pyside_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.152542 je_editor-0.0.81/je_editor/pyside_ui/auto_save/
--rw-rw-rw-   0        0        0        0 2023-04-24 10:50:54.000000 je_editor-0.0.81/je_editor/pyside_ui/auto_save/__init__.py
--rw-rw-rw-   0        0        0     1071 2023-04-24 10:50:54.000000 je_editor-0.0.81/je_editor/pyside_ui/auto_save/auto_save_thread.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.155534 je_editor-0.0.81/je_editor/pyside_ui/code_editor/
--rw-rw-rw-   0        0        0        0 2023-04-26 11:14:17.000000 je_editor-0.0.81/je_editor/pyside_ui/code_editor/__init__.py
--rw-rw-rw-   0        0        0     5355 2023-04-28 11:00:32.000000 je_editor-0.0.81/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.158526 je_editor-0.0.81/je_editor/pyside_ui/code_process/
--rw-rw-rw-   0        0        0        0 2023-04-23 14:01:39.000000 je_editor-0.0.81/je_editor/pyside_ui/code_process/__init__.py
--rw-rw-rw-   0        0        0     7331 2023-04-27 11:33:59.000000 je_editor-0.0.81/je_editor/pyside_ui/code_process/code_exec.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.162515 je_editor-0.0.81/je_editor/pyside_ui/code_result/
--rw-rw-rw-   0        0        0        0 2023-04-28 11:00:32.000000 je_editor-0.0.81/je_editor/pyside_ui/code_result/__init__.py
--rw-rw-rw-   0        0        0     1393 2023-04-28 11:00:32.000000 je_editor-0.0.81/je_editor/pyside_ui/code_result/code_record.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.164510 je_editor-0.0.81/je_editor/pyside_ui/colors/
--rw-rw-rw-   0        0        0        0 2023-04-24 15:35:13.000000 je_editor-0.0.81/je_editor/pyside_ui/colors/__init__.py
--rw-rw-rw-   0        0        0      123 2023-04-24 15:37:08.000000 je_editor-0.0.81/je_editor/pyside_ui/colors/global_color.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.169496 je_editor-0.0.81/je_editor/pyside_ui/file_dialog/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor-0.0.81/je_editor/pyside_ui/file_dialog/__init__.py
--rw-rw-rw-   0        0        0     1058 2023-04-26 12:09:26.000000 je_editor-0.0.81/je_editor/pyside_ui/file_dialog/open_file_dialog.py
--rw-rw-rw-   0        0        0      995 2023-04-24 10:50:54.000000 je_editor-0.0.81/je_editor/pyside_ui/file_dialog/save_file_dialog.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.170493 je_editor-0.0.81/je_editor/pyside_ui/main_ui/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor-0.0.81/je_editor/pyside_ui/main_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.174483 je_editor-0.0.81/je_editor/pyside_ui/main_ui/editor_main_ui/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor-0.0.81/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
--rw-rw-rw-   0        0        0     4279 2023-04-28 11:00:32.000000 je_editor-0.0.81/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.177474 je_editor-0.0.81/je_editor/pyside_ui/main_ui_setting/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor-0.0.81/je_editor/pyside_ui/main_ui_setting/__init__.py
--rw-rw-rw-   0        0        0     1634 2023-04-28 11:00:32.000000 je_editor-0.0.81/je_editor/pyside_ui/main_ui_setting/ui_setting.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.179469 je_editor-0.0.81/je_editor/pyside_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:44:51.000000 je_editor-0.0.81/je_editor/pyside_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.182462 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.184456 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
--rw-rw-rw-   0        0        0        0 2023-04-26 11:14:17.000000 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
--rw-rw-rw-   0        0        0     1646 2023-04-28 11:00:32.000000 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.187447 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/file_menu/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
--rw-rw-rw-   0        0        0     1034 2023-04-26 11:14:17.000000 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.189442 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/help_menu/
--rw-rw-rw-   0        0        0        0 2023-04-26 11:14:17.000000 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
--rw-rw-rw-   0        0        0     1223 2023-04-28 11:00:32.000000 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.192434 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/run_menu/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
--rw-rw-rw-   0        0        0     2021 2023-04-26 12:09:57.000000 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
--rw-rw-rw-   0        0        0     1118 2023-04-26 13:11:18.000000 je_editor-0.0.81/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.195427 je_editor-0.0.81/je_editor/pyside_ui/search_ui/
--rw-rw-rw-   0        0        0        0 2023-04-28 11:00:32.000000 je_editor-0.0.81/je_editor/pyside_ui/search_ui/__init__.py
--rw-rw-rw-   0        0        0      865 2023-04-28 11:00:32.000000 je_editor-0.0.81/je_editor/pyside_ui/search_ui/search_error_box.py
--rw-rw-rw-   0        0        0      857 2023-04-28 11:00:32.000000 je_editor-0.0.81/je_editor/pyside_ui/search_ui/search_text_box.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.197422 je_editor-0.0.81/je_editor/pyside_ui/shell_process/
--rw-rw-rw-   0        0        0        0 2023-04-23 14:01:47.000000 je_editor-0.0.81/je_editor/pyside_ui/shell_process/__init__.py
--rw-rw-rw-   0        0        0     6028 2023-04-26 12:07:18.000000 je_editor-0.0.81/je_editor/pyside_ui/shell_process/shell_exec.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.199454 je_editor-0.0.81/je_editor/pyside_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-04-24 10:50:54.000000 je_editor-0.0.81/je_editor/pyside_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0     3749 2023-04-26 11:14:17.000000 je_editor-0.0.81/je_editor/pyside_ui/syntax/python_syntax.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.201412 je_editor-0.0.81/je_editor/pyside_ui/treeview/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor-0.0.81/je_editor/pyside_ui/treeview/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.203405 je_editor-0.0.81/je_editor/pyside_ui/treeview/project_treeview/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:07:20.000000 je_editor-0.0.81/je_editor/pyside_ui/treeview/project_treeview/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-04-28 11:00:32.000000 je_editor-0.0.81/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
--rw-rw-rw-   0        0        0      393 2023-04-26 11:14:17.000000 je_editor-0.0.81/je_editor/start_editor.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.204403 je_editor-0.0.81/je_editor/utils/
--rw-rw-rw-   0        0        0        2 2023-04-20 11:44:51.000000 je_editor-0.0.81/je_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.207402 je_editor-0.0.81/je_editor/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-04-20 11:44:51.000000 je_editor-0.0.81/je_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      960 2023-04-26 11:14:17.000000 je_editor-0.0.81/je_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      506 2023-04-20 11:44:51.000000 je_editor-0.0.81/je_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.209389 je_editor-0.0.81/je_editor/utils/file/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:44:51.000000 je_editor-0.0.81/je_editor/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.211384 je_editor-0.0.81/je_editor/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-04-20 11:44:51.000000 je_editor-0.0.81/je_editor/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      962 2023-04-23 13:34:13.000000 je_editor-0.0.81/je_editor/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.213378 je_editor-0.0.81/je_editor/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-04-20 11:44:51.000000 je_editor-0.0.81/je_editor/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      719 2023-04-26 12:08:16.000000 je_editor-0.0.81/je_editor/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.215373 je_editor-0.0.81/je_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-04-20 11:44:51.000000 je_editor-0.0.81/je_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      983 2023-04-29 07:51:28.000000 je_editor-0.0.81/je_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.218369 je_editor-0.0.81/je_editor/utils/redirect_manager/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:44:51.000000 je_editor-0.0.81/je_editor/utils/redirect_manager/__init__.py
--rw-rw-rw-   0        0        0     1991 2023-04-20 11:44:51.000000 je_editor-0.0.81/je_editor/utils/redirect_manager/redirect_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:40:30.148555 je_editor-0.0.81/je_editor.egg-info/
--rw-rw-rw-   0        0        0     2831 2023-04-29 10:40:30.000000 je_editor-0.0.81/je_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2791 2023-04-29 10:40:30.000000 je_editor-0.0.81/je_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:40:30.000000 je_editor-0.0.81/je_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 10:40:30.000000 je_editor-0.0.81/je_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-29 10:40:30.000000 je_editor-0.0.81/je_editor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      948 2023-04-29 10:40:11.000000 je_editor-0.0.81/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 10:40:30.220360 je_editor-0.0.81/setup.cfg
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:51.000000 je_editor-0.0.9/
+-rw-rw-rw-   0        0        0     1084 2021-07-27 15:59:34.000000 je_editor-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1476 2021-09-04 14:08:51.000000 je_editor-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      822 2021-08-29 10:01:10.000000 je_editor-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:50.000000 je_editor-0.0.9/je_editor/
+-rw-rw-rw-   0        0        0       54 2021-08-31 18:23:15.000000 je_editor-0.0.9/je_editor/__init__.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:50.000000 je_editor-0.0.9/je_editor/ui/
+-rw-rw-rw-   0        0        0       28 2021-07-27 21:06:38.000000 je_editor-0.0.9/je_editor/ui/__init__.py
+-rw-rw-rw-   0        0        0     8282 2021-09-04 14:05:47.000000 je_editor-0.0.9/je_editor/ui/tkinter_editor.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:50.000000 je_editor-0.0.9/je_editor/utils/
+-rw-rw-rw-   0        0        0       31 2021-07-27 21:06:38.000000 je_editor-0.0.9/je_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:50.000000 je_editor-0.0.9/je_editor/utils/code_tag/
+-rw-rw-rw-   0        0        0        0 2021-08-28 10:32:00.000000 je_editor-0.0.9/je_editor/utils/code_tag/__init__.py
+-rw-rw-rw-   0        0        0       65 2021-08-29 10:24:32.000000 je_editor-0.0.9/je_editor/utils/code_tag/keyword_list.py
+-rw-rw-rw-   0        0        0     1349 2021-09-01 14:06:56.000000 je_editor-0.0.9/je_editor/utils/code_tag/tag_keyword.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:51.000000 je_editor-0.0.9/je_editor/utils/editor_content/
+-rw-rw-rw-   0        0        0       46 2021-08-02 03:41:58.000000 je_editor-0.0.9/je_editor/utils/editor_content/__init__.py
+-rw-rw-rw-   0        0        0     1325 2021-08-31 09:42:51.000000 je_editor-0.0.9/je_editor/utils/editor_content/content_save.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:51.000000 je_editor-0.0.9/je_editor/utils/exception/
+-rw-rw-rw-   0        0        0       41 2021-07-30 21:21:05.000000 je_editor-0.0.9/je_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      413 2021-08-03 14:08:05.000000 je_editor-0.0.9/je_editor/utils/exception/je_editor_exception_tag.py
+-rw-rw-rw-   0        0        0     1600 2021-08-03 14:21:22.000000 je_editor-0.0.9/je_editor/utils/exception/je_editor_exceptions.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:51.000000 je_editor-0.0.9/je_editor/utils/file/
+-rw-rw-rw-   0        0        0       36 2021-07-31 00:44:48.000000 je_editor-0.0.9/je_editor/utils/file/__init__.py
+-rw-rw-rw-   0        0        0     1025 2021-09-04 13:51:29.000000 je_editor-0.0.9/je_editor/utils/file/open_file.py
+-rw-rw-rw-   0        0        0     1705 2021-09-04 13:54:28.000000 je_editor-0.0.9/je_editor/utils/file/save_file.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:51.000000 je_editor-0.0.9/je_editor/utils/string_translate/
+-rw-rw-rw-   0        0        0        0 2021-08-31 08:37:16.000000 je_editor-0.0.9/je_editor/utils/string_translate/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-08-31 08:37:26.000000 je_editor-0.0.9/je_editor/utils/string_translate/used_string.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:51.000000 je_editor-0.0.9/je_editor/utils/text_process/
+-rw-rw-rw-   0        0        0       44 2021-07-30 21:49:48.000000 je_editor-0.0.9/je_editor/utils/text_process/__init__.py
+-rw-rw-rw-   0        0        0      444 2021-08-31 11:45:46.000000 je_editor-0.0.9/je_editor/utils/text_process/exec_text.py
+-rw-rw-rw-   0        0        0      296 2021-08-31 11:44:13.000000 je_editor-0.0.9/je_editor/utils/text_process/shell_text.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:51.000000 je_editor-0.0.9/je_editor/utils/theme/
+-rw-rw-rw-   0        0        0        0 2021-09-02 08:09:26.000000 je_editor-0.0.9/je_editor/utils/theme/__init__.py
+-rw-rw-rw-   0        0        0       61 2021-09-02 08:09:26.000000 je_editor-0.0.9/je_editor/utils/theme/theme.py
+drwxrwxrwx   0        0        0        0 2021-09-04 14:08:50.000000 je_editor-0.0.9/je_editor.egg-info/
+-rw-rw-rw-   0        0        0     1476 2021-09-04 14:08:49.000000 je_editor-0.0.9/je_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      998 2021-09-04 14:08:49.000000 je_editor-0.0.9/je_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-09-04 14:08:49.000000 je_editor-0.0.9/je_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2021-09-04 14:08:49.000000 je_editor-0.0.9/je_editor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-09-04 14:08:51.000000 je_editor-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      900 2021-09-04 14:08:12.000000 je_editor-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `je_editor-0.0.81/LICENSE` & `je_editor-0.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `je_editor-0.0.81/je_editor/utils/file/open/open_file.py` & `je_editor-0.0.9/je_editor/utils/editor_content/content_save.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,49 @@
+import json
+import os
 from pathlib import Path
 from threading import Lock
 
-from je_editor.utils.exception.exceptions import JEditorOpenFileException
+from je_editor.utils.exception.je_editor_exceptions import JEditorContentFileException
 
+cwd = os.getcwd()
+lock = Lock()
 
-def read_file(file):
-    """
-    use to check file is exist and open
-    :param file: the file we want to read its whole file path
-    :return: read's file and file content
-    try
-        lock thread
-        find file is exist ? and is file ?
-        if both is true
-            try to open it and read
-            return file and content
-    finally
-        release lock
-    """
-    lock = Lock()
+editor_data = {
+    "last_file": None
+}
+
+
+def read_output_content():
     try:
         lock.acquire()
-        if file != "" and file is not None:
-            file_path = Path(file)
-            if file_path.exists() and file_path.is_file():
-                with open(file, "r+") as open_read_file:
-                    return [file, open_read_file.read()]
-    except JEditorOpenFileException:
-        raise JEditorOpenFileException
+        file_path = Path(cwd + "/je_editor_content.json")
+        if file_path.exists() and file_path.is_file():
+            with open(cwd + "/je_editor_content.json", "r+") as read_file:
+                return read_file.read()
+    except JEditorContentFileException:
+        raise JEditorContentFileException
     finally:
         lock.release()
 
 
+def write_output_content():
+    try:
+        lock.acquire()
+        with open(cwd + "/je_editor_content.json", "w+") as file_to_write:
+            file_to_write.write(json.dumps(editor_data))
+    except JEditorContentFileException:
+        raise JEditorContentFileException
+    finally:
+        lock.release()
+
+
+def save_content_and_quit(file):
+    editor_data["last_file"] = file
+    write_output_content()
+
 
+def open_content_and_start():
+    temp_content = read_output_content()
+    if temp_content is not None:
+        editor_data["last_file"] = json.loads(temp_content).get("last_file")
+    return editor_data.get("last_file")
```


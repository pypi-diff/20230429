# Comparing `tmp/automation_editor-0.0.1.tar.gz` & `tmp/automation_editor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_editor-0.0.1.tar", last modified: Sat Apr 29 10:03:18 2023, max compression
+gzip compressed data, was "automation_editor-0.0.2.tar", last modified: Sat Apr 29 10:30:02 2023, max compression
```

## Comparing `automation_editor-0.0.1.tar` & `automation_editor-0.0.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.468596 automation_editor-0.0.1/
--rw-rw-rw-   0        0        0     1085 2023-04-05 12:50:43.000000 automation_editor-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     5808 2023-04-29 10:03:18.467596 automation_editor-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5080 2023-04-29 09:58:28.000000 automation_editor-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.395789 automation_editor-0.0.1/automation_editor/
--rw-rw-rw-   0        0        0      130 2023-04-29 09:53:20.000000 automation_editor-0.0.1/automation_editor/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.415736 automation_editor-0.0.1/automation_editor/automation_editor_ui/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.417730 automation_editor-0.0.1/automation_editor/automation_editor_ui/editor_main/
--rw-rw-rw-   0        0        0        0 2023-04-24 10:50:57.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/editor_main/__init__.py
--rw-rw-rw-   0        0        0     1324 2023-04-29 09:53:20.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/editor_main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.419766 automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.421721 automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/api_testka_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
--rw-rw-rw-   0        0        0     3997 2023-04-29 09:53:20.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.423715 automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/auto_control_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
--rw-rw-rw-   0        0        0     4128 2023-04-29 09:53:20.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.426705 automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/load_density_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
--rw-rw-rw-   0        0        0     4160 2023-04-29 09:53:20.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.428701 automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/web_runner_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
--rw-rw-rw-   0        0        0     4041 2023-04-29 09:53:20.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.430706 automation_editor-0.0.1/automation_editor/automation_editor_ui/show_code_window/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/show_code_window/__init__.py
--rw-rw-rw-   0        0        0      791 2023-04-27 10:28:14.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/show_code_window/code_window.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.434686 automation_editor-0.0.1/automation_editor/automation_editor_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0      777 2023-04-29 09:53:20.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/syntax/syntax_extend.py
--rw-rw-rw-   0        0        0     3257 2023-04-27 10:28:14.000000 automation_editor-0.0.1/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.435682 automation_editor-0.0.1/automation_editor/extend/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.437677 automation_editor-0.0.1/automation_editor/extend/mail_thunder_extend/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/extend/mail_thunder_extend/__init__.py
--rw-rw-rw-   0        0        0     1696 2023-04-29 09:53:20.000000 automation_editor-0.0.1/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.439672 automation_editor-0.0.1/automation_editor/utils/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.442663 automation_editor-0.0.1/automation_editor/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1500 2023-04-27 10:28:14.000000 automation_editor-0.0.1/automation_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      608 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.445656 automation_editor-0.0.1/automation_editor/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-27 10:28:14.000000 automation_editor-0.0.1/automation_editor/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.448649 automation_editor-0.0.1/automation_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      991 2023-04-29 09:53:20.000000 automation_editor-0.0.1/automation_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.449645 automation_editor-0.0.1/automation_editor/utils/manager/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/utils/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.452638 automation_editor-0.0.1/automation_editor/utils/manager/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/utils/manager/package_manager/__init__.py
--rw-rw-rw-   0        0        0     1737 2023-04-28 11:00:21.000000 automation_editor-0.0.1/automation_editor/utils/manager/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.456626 automation_editor-0.0.1/automation_editor/utils/test_executor/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/utils/test_executor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.458620 automation_editor-0.0.1/automation_editor/utils/test_executor/api_testka/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/utils/test_executor/api_testka/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-04-29 09:53:20.000000 automation_editor-0.0.1/automation_editor/utils/test_executor/api_testka/api_testka_process.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.460616 automation_editor-0.0.1/automation_editor/utils/test_executor/auto_control/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/utils/test_executor/auto_control/__init__.py
--rw-rw-rw-   0        0        0     3939 2023-04-29 09:53:20.000000 automation_editor-0.0.1/automation_editor/utils/test_executor/auto_control/auto_control_process.py
--rw-rw-rw-   0        0        0      498 2023-04-29 09:53:20.000000 automation_editor-0.0.1/automation_editor/utils/test_executor/check_mail_thunder.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.463607 automation_editor-0.0.1/automation_editor/utils/test_executor/load_density/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/utils/test_executor/load_density/__init__.py
--rw-rw-rw-   0        0        0     3949 2023-04-29 09:53:20.000000 automation_editor-0.0.1/automation_editor/utils/test_executor/load_density/load_density_process.py
--rw-rw-rw-   0        0        0     5837 2023-04-28 11:00:21.000000 automation_editor-0.0.1/automation_editor/utils/test_executor/task_process_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.466600 automation_editor-0.0.1/automation_editor/utils/test_executor/web_runner/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.1/automation_editor/utils/test_executor/web_runner/__init__.py
--rw-rw-rw-   0        0        0     3897 2023-04-29 09:53:20.000000 automation_editor-0.0.1/automation_editor/utils/test_executor/web_runner/web_runner_process.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:03:18.413740 automation_editor-0.0.1/automation_editor.egg-info/
--rw-rw-rw-   0        0        0     5808 2023-04-29 10:03:18.000000 automation_editor-0.0.1/automation_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2931 2023-04-29 10:03:18.000000 automation_editor-0.0.1/automation_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:03:18.000000 automation_editor-0.0.1/automation_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-29 10:03:18.000000 automation_editor-0.0.1/automation_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-29 10:03:18.000000 automation_editor-0.0.1/automation_editor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1143 2023-04-29 09:53:20.000000 automation_editor-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 10:03:18.468596 automation_editor-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.025958 automation_editor-0.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-04-05 12:50:43.000000 automation_editor-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5751 2023-04-29 10:30:02.024960 automation_editor-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5023 2023-04-29 10:29:31.000000 automation_editor-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.952155 automation_editor-0.0.2/automation_editor/
+-rw-rw-rw-   0        0        0      130 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.969109 automation_editor-0.0.2/automation_editor/automation_editor_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.973100 automation_editor-0.0.2/automation_editor/automation_editor_ui/editor_main/
+-rw-rw-rw-   0        0        0        0 2023-04-24 10:50:57.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/editor_main/__init__.py
+-rw-rw-rw-   0        0        0     1324 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/editor_main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.976092 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.978087 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/api_testka_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
+-rw-rw-rw-   0        0        0     3998 2023-04-29 10:27:21.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.981078 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/auto_control_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
+-rw-rw-rw-   0        0        0     4129 2023-04-29 10:27:09.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.984071 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/load_density_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
+-rw-rw-rw-   0        0        0     4161 2023-04-29 10:27:56.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.986064 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/web_runner_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
+-rw-rw-rw-   0        0        0     4040 2023-04-29 10:27:42.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.989056 automation_editor-0.0.2/automation_editor/automation_editor_ui/show_code_window/
+-rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/show_code_window/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/show_code_window/code_window.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.993046 automation_editor-0.0.2/automation_editor/automation_editor_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/syntax/syntax_extend.py
+-rw-rw-rw-   0        0        0     3257 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.995042 automation_editor-0.0.2/automation_editor/extend/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.997036 automation_editor-0.0.2/automation_editor/extend/mail_thunder_extend/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/extend/mail_thunder_extend/__init__.py
+-rw-rw-rw-   0        0        0     1696 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.998033 automation_editor-0.0.2/automation_editor/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.002022 automation_editor-0.0.2/automation_editor/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1500 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      608 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.004016 automation_editor-0.0.2/automation_editor/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.007008 automation_editor-0.0.2/automation_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0      991 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.008006 automation_editor-0.0.2/automation_editor/utils/manager/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.011001 automation_editor-0.0.2/automation_editor/utils/manager/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/manager/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     1737 2023-04-28 11:00:21.000000 automation_editor-0.0.2/automation_editor/utils/manager/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.013990 automation_editor-0.0.2/automation_editor/utils/test_executor/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.015985 automation_editor-0.0.2/automation_editor/utils/test_executor/api_testka/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/api_testka/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/api_testka/api_testka_process.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.018976 automation_editor-0.0.2/automation_editor/utils/test_executor/auto_control/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/auto_control/__init__.py
+-rw-rw-rw-   0        0        0     3939 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/auto_control/auto_control_process.py
+-rw-rw-rw-   0        0        0      498 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/check_mail_thunder.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.020971 automation_editor-0.0.2/automation_editor/utils/test_executor/load_density/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/load_density/__init__.py
+-rw-rw-rw-   0        0        0     3949 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/load_density/load_density_process.py
+-rw-rw-rw-   0        0        0     5837 2023-04-28 11:00:21.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/task_process_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.023963 automation_editor-0.0.2/automation_editor/utils/test_executor/web_runner/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/web_runner/__init__.py
+-rw-rw-rw-   0        0        0     3897 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/web_runner/web_runner_process.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.968112 automation_editor-0.0.2/automation_editor.egg-info/
+-rw-rw-rw-   0        0        0     5751 2023-04-29 10:30:01.000000 automation_editor-0.0.2/automation_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2931 2023-04-29 10:30:01.000000 automation_editor-0.0.2/automation_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 10:30:01.000000 automation_editor-0.0.2/automation_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-04-29 10:30:01.000000 automation_editor-0.0.2/automation_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-29 10:30:01.000000 automation_editor-0.0.2/automation_editor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1143 2023-04-29 10:29:43.000000 automation_editor-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 10:30:02.025958 automation_editor-0.0.2/setup.cfg
```

### Comparing `automation_editor-0.0.1/LICENSE` & `automation_editor-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/PKG-INFO` & `automation_editor-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: automation_editor
-Version: 0.0.1
+Version: 0.0.2
 Summary: Automation Editor for GUI, WEB, API, Load Automation
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Integrated-Testing-Environment/AutomationEditor
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: full_extension
 License-File: LICENSE
 
 # Table of contents
 > Editor components \
 > GUI components \
 > WEB components \
 > API components \
 > Load components
 ---
-## What is ITE
+## What is Automation Editor
 > Project Kanban \
-> https://github.com/orgs/Integrated-Testing-Environment/projects/4/views/1 \
-> Integrated Testing Environment (ITE) 
-> * ITE mainly provides an integrated automation editor. 
-> * ITE is composed of the following components: 
+> https://github.com/orgs/Intergration-Automation-Testing/projects/2/views/1 \
+> Tool for automation
+> * Automation Editor is composed of the following components: 
 >> * Editor。
 >> * GUI Automation。
 >> * Web Automation。
 >> * API Automation。
 >> * Load Automation。
 ---
 ### JEditor
@@ -98,27 +97,27 @@
 
 ### Features
 
 > * GUI Automation (use AutoControl)
 > * API Automation (use APITestka)
 > * Web Automation (use WebRunner)
 > * Loading Automation (use LoadDensity)
-> * Multi test task runner (multi process, but without AutoControl)
+> * Multi test task runner (multiprocess, but without AutoControl)
 > * you can run multi testing on same time
 > * open log window to check testing result
 > * Send mail when testing failure (need to setting mail)
 
 ---
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b7d32ed8600b4bd2a2f3e960f46f2ad0)](https://www.codacy.com/gh/JE-Chen/Integration-testing-environment/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=JE-Chen/Integration-testing-environment&amp;utm_campaign=Badge_Grade)
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main)
 
-[![ITE GitHub Actions Dev](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml)
+[![GitHub Actions Dev](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml)
 
-[![ITE GitHub Actions Stable](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml)
+[![GitHub Actions Stable](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml)
 
 ### install
 #### we suggest install full package
 * pip install automation_editor[full_extension]
 #### if we don't want to use send after test
 * pip install automation_editor
```

### Comparing `automation_editor-0.0.1/README.md` & `automation_editor-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # Table of contents
 > Editor components \
 > GUI components \
 > WEB components \
 > API components \
 > Load components
 ---
-## What is ITE
+## What is Automation Editor
 > Project Kanban \
-> https://github.com/orgs/Integrated-Testing-Environment/projects/4/views/1 \
-> Integrated Testing Environment (ITE) 
-> * ITE mainly provides an integrated automation editor. 
-> * ITE is composed of the following components: 
+> https://github.com/orgs/Intergration-Automation-Testing/projects/2/views/1 \
+> Tool for automation
+> * Automation Editor is composed of the following components: 
 >> * Editor。
 >> * GUI Automation。
 >> * Web Automation。
 >> * API Automation。
 >> * Load Automation。
 ---
 ### JEditor
@@ -79,27 +78,27 @@
 
 ### Features
 
 > * GUI Automation (use AutoControl)
 > * API Automation (use APITestka)
 > * Web Automation (use WebRunner)
 > * Loading Automation (use LoadDensity)
-> * Multi test task runner (multi process, but without AutoControl)
+> * Multi test task runner (multiprocess, but without AutoControl)
 > * you can run multi testing on same time
 > * open log window to check testing result
 > * Send mail when testing failure (need to setting mail)
 
 ---
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b7d32ed8600b4bd2a2f3e960f46f2ad0)](https://www.codacy.com/gh/JE-Chen/Integration-testing-environment/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=JE-Chen/Integration-testing-environment&amp;utm_campaign=Badge_Grade)
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main)
 
-[![ITE GitHub Actions Dev](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml)
+[![GitHub Actions Dev](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml)
 
-[![ITE GitHub Actions Stable](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml)
+[![GitHub Actions Stable](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml)
 
 ### install
 #### we suggest install full package
 * pip install automation_editor[full_extension]
 #### if we don't want to use send after test
 * pip install automation_editor
```

### Comparing `automation_editor-0.0.1/automation_editor/automation_editor_ui/editor_main/main_ui.py` & `automation_editor-0.0.2/automation_editor/automation_editor_ui/editor_main/main_ui.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py` & `automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     ui_we_want_to_set.apitestka_help_menu.addAction(
         ui_we_want_to_set.open_apitestka_doc_action
     )
     # Open Github
     ui_we_want_to_set.open_apitestka_github_action = QAction("Open APITestka GitHub")
     ui_we_want_to_set.open_apitestka_github_action.triggered.connect(
         lambda: open_web_browser(
-            "https://github.com/Integrated-Testing-Environment/APITestka"
+            "https://github.com/Intergration-Automation-Testing/APITestka"
         )
     )
     ui_we_want_to_set.apitestka_help_menu.addAction(
         ui_we_want_to_set.open_apitestka_github_action
     )
     ui_we_want_to_set.apitestka_project_menu = ui_we_want_to_set.apitestka_menu.addMenu("Project")
     # Create Project
```

### Comparing `automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py` & `automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     ui_we_want_to_set.autocontrol_help_menu.addAction(
         ui_we_want_to_set.open_autocontrol_doc_action
     )
     # Open Github
     ui_we_want_to_set.open_autocontrol_github_action = QAction("Open AutoControl GitHub")
     ui_we_want_to_set.open_autocontrol_github_action.triggered.connect(
         lambda: open_web_browser(
-            "https://github.com/Integrated-Testing-Environment/AutoControl"
+            "https://github.com/Intergration-Automation-Testing/AutoControl"
         )
     )
     ui_we_want_to_set.autocontrol_help_menu.addAction(
         ui_we_want_to_set.open_autocontrol_github_action
     )
     ui_we_want_to_set.autocontrol_project_menu = ui_we_want_to_set.autocontrol_menu.addMenu("Project")
     # Create Project
```

### Comparing `automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py` & `automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     ui_we_want_to_set.load_density_help_menu.addAction(
         ui_we_want_to_set.open_load_density_doc_action
     )
     # Open Github
     ui_we_want_to_set.open_load_density_github_action = QAction("Open LoadDensity GitHub")
     ui_we_want_to_set.open_load_density_github_action.triggered.connect(
         lambda: open_web_browser(
-            "https://github.com/Integrated-Testing-Environment/LoadDensity"
+            "https://github.com/Intergration-Automation-Testing/LoadDensity"
         )
     )
     ui_we_want_to_set.load_density_help_menu.addAction(
         ui_we_want_to_set.open_load_density_github_action
     )
     ui_we_want_to_set.load_density_project_menu = ui_we_want_to_set.load_density_menu.addMenu("Project")
     # Create Project
```

### Comparing `automation_editor-0.0.1/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py` & `automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     ui_we_want_to_set.web_runner_help_menu.addAction(
         ui_we_want_to_set.open_web_runner_doc_action
     )
     # Open Github
     ui_we_want_to_set.open_web_runner_github_action = QAction("Open WebRunner GitHub")
     ui_we_want_to_set.open_web_runner_github_action.triggered.connect(
         lambda: open_web_browser(
-            "https://github.com/Integrated-Testing-Environment/LoadDensity"
+            "https://github.com/Intergration-Automation-Testing/WebRunner"
         )
     )
     ui_we_want_to_set.web_runner_help_menu.addAction(
         ui_we_want_to_set.open_web_runner_github_action
     )
     ui_we_want_to_set.web_runner_project_menu = ui_we_want_to_set.web_runner_menu.addMenu("Project")
     # Create Project
```

### Comparing `automation_editor-0.0.1/automation_editor/automation_editor_ui/show_code_window/code_window.py` & `automation_editor-0.0.2/automation_editor/automation_editor_ui/show_code_window/code_window.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor/automation_editor_ui/syntax/syntax_extend.py` & `automation_editor-0.0.2/automation_editor/automation_editor_ui/syntax/syntax_extend.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor/automation_editor_ui/syntax/syntax_keyword.py` & `automation_editor-0.0.2/automation_editor/automation_editor_ui/syntax/syntax_keyword.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py` & `automation_editor-0.0.2/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor/utils/exception/exception_tags.py` & `automation_editor-0.0.2/automation_editor/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor/utils/exception/exceptions.py` & `automation_editor-0.0.2/automation_editor/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor/utils/file_process/get_dir_file_list.py` & `automation_editor-0.0.2/automation_editor/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor/utils/json_format/json_process.py` & `automation_editor-0.0.2/automation_editor/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor/utils/manager/package_manager/package_manager_class.py` & `automation_editor-0.0.2/automation_editor/utils/manager/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor/utils/test_executor/api_testka/api_testka_process.py` & `automation_editor-0.0.2/automation_editor/utils/test_executor/api_testka/api_testka_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor/utils/test_executor/auto_control/auto_control_process.py` & `automation_editor-0.0.2/automation_editor/utils/test_executor/auto_control/auto_control_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor/utils/test_executor/load_density/load_density_process.py` & `automation_editor-0.0.2/automation_editor/utils/test_executor/load_density/load_density_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor/utils/test_executor/task_process_manager.py` & `automation_editor-0.0.2/automation_editor/utils/test_executor/task_process_manager.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor/utils/test_executor/web_runner/web_runner_process.py` & `automation_editor-0.0.2/automation_editor/utils/test_executor/web_runner/web_runner_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/automation_editor.egg-info/PKG-INFO` & `automation_editor-0.0.2/automation_editor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: automation-editor
-Version: 0.0.1
+Version: 0.0.2
 Summary: Automation Editor for GUI, WEB, API, Load Automation
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Integrated-Testing-Environment/AutomationEditor
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: full_extension
 License-File: LICENSE
 
 # Table of contents
 > Editor components \
 > GUI components \
 > WEB components \
 > API components \
 > Load components
 ---
-## What is ITE
+## What is Automation Editor
 > Project Kanban \
-> https://github.com/orgs/Integrated-Testing-Environment/projects/4/views/1 \
-> Integrated Testing Environment (ITE) 
-> * ITE mainly provides an integrated automation editor. 
-> * ITE is composed of the following components: 
+> https://github.com/orgs/Intergration-Automation-Testing/projects/2/views/1 \
+> Tool for automation
+> * Automation Editor is composed of the following components: 
 >> * Editor。
 >> * GUI Automation。
 >> * Web Automation。
 >> * API Automation。
 >> * Load Automation。
 ---
 ### JEditor
@@ -98,27 +97,27 @@
 
 ### Features
 
 > * GUI Automation (use AutoControl)
 > * API Automation (use APITestka)
 > * Web Automation (use WebRunner)
 > * Loading Automation (use LoadDensity)
-> * Multi test task runner (multi process, but without AutoControl)
+> * Multi test task runner (multiprocess, but without AutoControl)
 > * you can run multi testing on same time
 > * open log window to check testing result
 > * Send mail when testing failure (need to setting mail)
 
 ---
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b7d32ed8600b4bd2a2f3e960f46f2ad0)](https://www.codacy.com/gh/JE-Chen/Integration-testing-environment/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=JE-Chen/Integration-testing-environment&amp;utm_campaign=Badge_Grade)
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main)
 
-[![ITE GitHub Actions Dev](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml)
+[![GitHub Actions Dev](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml)
 
-[![ITE GitHub Actions Stable](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml)
+[![GitHub Actions Stable](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml)
 
 ### install
 #### we suggest install full package
 * pip install automation_editor[full_extension]
 #### if we don't want to use send after test
 * pip install automation_editor
```

### Comparing `automation_editor-0.0.1/automation_editor.egg-info/SOURCES.txt` & `automation_editor-0.0.2/automation_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.1/pyproject.toml` & `automation_editor-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # This is stable version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_editor"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "JE-Chen", email = "zenmailman@gmail.com" },
 ]
 description = "Automation Editor for GUI, WEB, API, Load Automation"
 readme = { file = "README.md", content-type = "text/markdown" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
     "je-editor", "je_auto_control", "je_web_runner",
     "je_load_density", "je_api_testka"
 ]
 classifiers = [
     "Programming Language :: Python :: 3.7",
```


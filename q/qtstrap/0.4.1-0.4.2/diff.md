# Comparing `tmp/qtstrap-0.4.1.tar.gz` & `tmp/qtstrap-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtstrap-0.4.1.tar", last modified: Tue Mar  7 15:44:10 2023, max compression
+gzip compressed data, was "qtstrap-0.4.2.tar", last modified: Sat Apr 29 17:00:22 2023, max compression
```

## Comparing `qtstrap-0.4.1.tar` & `qtstrap-0.4.2.tar`

### file list

```diff
@@ -1,174 +1,193 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.367062 qtstrap-0.4.1/
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:09.928563 qtstrap-0.4.1/.github/
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:09.991062 qtstrap-0.4.1/.github/workflows/
--rw-rw-rw-   0        0        0      978 2022-07-30 04:06:00.000000 qtstrap-0.4.1/.github/workflows/main.yml
--rw-rw-rw-   0        0        0      161 2022-11-24 04:51:10.000000 qtstrap-0.4.1/.gitignore
--rw-rw-rw-   0        0        0     1090 2021-04-01 21:16:04.000000 qtstrap-0.4.1/LICENSE
--rw-rw-rw-   0        0        0       96 2021-04-01 21:16:04.000000 qtstrap-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2600 2023-03-07 12:46:55.000000 qtstrap-0.4.1/Makefile
--rw-rw-rw-   0        0        0     2554 2023-03-07 15:44:10.367563 qtstrap-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1599 2022-11-09 07:55:58.000000 qtstrap-0.4.1/README.md
--rw-rw-rw-   0        0        0      272 2022-07-30 03:58:00.000000 qtstrap-0.4.1/build_docs.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:09.998561 qtstrap-0.4.1/docs/
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.082562 qtstrap-0.4.1/docs/api/
--rw-rw-rw-   0        0        0       68 2022-07-30 03:58:02.000000 qtstrap-0.4.1/docs/api/.pages
--rw-rw-rw-   0        0        0     4217 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.code_editor.code_editor.md
--rw-rw-rw-   0        0        0     1284 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.code_editor.code_line.md
--rw-rw-rw-   0        0        0      448 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.code_editor.highlighters.md
--rw-rw-rw-   0        0        0     2397 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.code_editor.highlighters.python.md
--rw-rw-rw-   0        0        0      464 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.code_editor.md
--rw-rw-rw-   0        0        0     7792 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.command_palette.command_palette.md
--rw-rw-rw-   0        0        0      439 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.command_palette.md
--rw-rw-rw-   0        0        0     2327 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.log_monitor.log_database_handler.md
--rw-rw-rw-   0        0        0    12203 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.log_monitor.log_filter_controls.md
--rw-rw-rw-   0        0        0     2706 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.log_monitor.log_profile.md
--rw-rw-rw-   0        0        0     3912 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.log_monitor.log_table_view.md
--rw-rw-rw-   0        0        0     4151 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.log_monitor.log_widget.md
--rw-rw-rw-   0        0        0      875 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.log_monitor.md
--rw-rw-rw-   0        0        0      342 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.md
--rw-rw-rw-   0        0        0      802 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.style.colors.md
--rw-rw-rw-   0        0        0      469 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.style.dark_palette.md
--rw-rw-rw-   0        0        0      416 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/extras.style.md
--rw-rw-rw-   0        0        0      546 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/options.md
--rw-rw-rw-   0        0        0     9012 2022-07-30 03:58:02.000000 qtstrap-0.4.1/docs/api/overview.md
--rw-rw-rw-   0        0        0      754 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/settings.md
--rw-rw-rw-   0        0        0     1307 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/utils.adapter.md
--rw-rw-rw-   0        0        0      599 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/utils.decorators.md
--rw-rw-rw-   0        0        0     1019 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/utils.defer.md
--rw-rw-rw-   0        0        0      438 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/utils.md
--rw-rw-rw-   0        0        0      946 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/utils.signals.md
--rw-rw-rw-   0        0        0      607 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/utils.singleton.md
--rw-rw-rw-   0        0        0     1597 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/utils.timestamp.md
--rw-rw-rw-   0        0        0     2534 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/utils.utils.md
--rw-rw-rw-   0        0        0     4169 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/widgets.buttons.md
--rw-rw-rw-   0        0        0     2832 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/widgets.labeledit.md
--rw-rw-rw-   0        0        0    13269 2022-07-30 03:58:02.000000 qtstrap-0.4.1/docs/api/widgets.layouts.md
--rw-rw-rw-   0        0        0     1443 2022-07-30 03:58:02.000000 qtstrap-0.4.1/docs/api/widgets.line_widgets.md
--rw-rw-rw-   0        0        0     1483 2022-07-30 03:58:02.000000 qtstrap-0.4.1/docs/api/widgets.link_label.md
--rw-rw-rw-   0        0        0      526 2022-07-30 03:58:01.000000 qtstrap-0.4.1/docs/api/widgets.md
--rw-rw-rw-   0        0        0     3019 2022-07-30 03:58:02.000000 qtstrap-0.4.1/docs/api/widgets.persistent_tab_widget.md
--rw-rw-rw-   0        0        0     6978 2022-07-30 03:58:02.000000 qtstrap-0.4.1/docs/api/widgets.persistent_widgets.md
--rw-rw-rw-   0        0        0      853 2021-04-01 21:16:04.000000 qtstrap-0.4.1/docs/index.md
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.091565 qtstrap-0.4.1/docs/quickstart/
--rw-rw-rw-   0        0        0     2618 2021-04-01 21:16:04.000000 qtstrap-0.4.1/docs/quickstart/baseapplication.md
--rw-rw-rw-   0        0        0      920 2021-04-01 21:16:04.000000 qtstrap-0.4.1/docs/quickstart/basemainwindow.md
--rw-rw-rw-   0        0        0     1700 2021-04-01 21:16:04.000000 qtstrap-0.4.1/docs/quickstart/context_layouts.md
--rw-rw-rw-   0        0        0     1264 2021-04-02 17:24:51.000000 qtstrap-0.4.1/docs/quickstart/gettingstarted.md
--rw-rw-rw-   0        0        0      857 2021-04-01 21:16:04.000000 qtstrap-0.4.1/docs/quickstart/installation.md
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.147564 qtstrap-0.4.1/docs/reference/
--rw-rw-rw-   0        0        0      759 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/base_application.md
--rw-rw-rw-   0        0        0      682 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/base_window.md
--rw-rw-rw-   0        0        0      653 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/options.md
--rw-rw-rw-   0        0        0      287 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/settings.md
--rw-rw-rw-   0        0        0      962 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/toolbar.md
--rw-rw-rw-   0        0        0     1484 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/utils.adapter.md
--rw-rw-rw-   0        0        0       88 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/utils.decorators.md
--rw-rw-rw-   0        0        0      618 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/utils.defer.md
--rw-rw-rw-   0        0        0      353 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/utils.md
--rw-rw-rw-   0        0        0      576 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/utils.signals.md
--rw-rw-rw-   0        0        0      105 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/utils.singleton.md
--rw-rw-rw-   0        0        0      690 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/utils.timestamp.md
--rw-rw-rw-   0        0        0     1349 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/utils.utils.md
--rw-rw-rw-   0        0        0     2361 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/widgets.buttons.md
--rw-rw-rw-   0        0        0     1196 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/widgets.labeledit.md
--rw-rw-rw-   0        0        0     4766 2022-07-30 03:40:51.000000 qtstrap-0.4.1/docs/reference/widgets.layouts.md
--rw-rw-rw-   0        0        0      516 2022-07-30 03:40:51.000000 qtstrap-0.4.1/docs/reference/widgets.line_widgets.md
--rw-rw-rw-   0        0        0      638 2022-07-30 03:40:51.000000 qtstrap-0.4.1/docs/reference/widgets.link_label.md
--rw-rw-rw-   0        0        0     1408 2022-07-30 03:40:50.000000 qtstrap-0.4.1/docs/reference/widgets.md
--rw-rw-rw-   0        0        0     1324 2022-07-30 03:40:51.000000 qtstrap-0.4.1/docs/reference/widgets.persistent_tab_widget.md
--rw-rw-rw-   0        0        0     3704 2022-07-30 03:40:51.000000 qtstrap-0.4.1/docs/reference/widgets.persistent_widgets.md
--rw-rw-rw-   0        0        0     2949 2021-04-01 21:16:04.000000 qtstrap-0.4.1/docs/screenshot1.png
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.150561 qtstrap-0.4.1/docs/structure/
--rw-rw-rw-   0        0        0     1193 2021-04-01 21:16:04.000000 qtstrap-0.4.1/docs/structure/makefile.md
--rw-rw-rw-   0        0        0     3013 2022-07-30 00:37:45.000000 qtstrap-0.4.1/docs/structure/structure.md
--rw-rw-rw-   0        0        0     7886 2022-07-30 03:01:48.000000 qtstrap-0.4.1/docs/test.md
--rw-rw-rw-   0        0        0      824 2022-07-30 03:45:13.000000 qtstrap-0.4.1/mkdocs.yml
--rw-rw-rw-   0        0        0      345 2022-07-30 04:03:13.000000 qtstrap-0.4.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.179063 qtstrap-0.4.1/qtstrap/
--rw-rw-rw-   0        0        0     1035 2023-03-07 12:33:33.000000 qtstrap-0.4.1/qtstrap/__init__.py
--rw-rw-rw-   0        0        0     1901 2022-10-26 06:40:59.000000 qtstrap-0.4.1/qtstrap/__main__.py
--rw-rw-rw-   0        0        0     2051 2023-03-07 12:17:44.000000 qtstrap-0.4.1/qtstrap/base_application.py
--rw-rw-rw-   0        0        0     2074 2023-03-07 12:38:24.000000 qtstrap-0.4.1/qtstrap/base_window.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.240062 qtstrap-0.4.1/qtstrap/extras/
--rw-rw-rw-   0        0        0        0 2021-04-08 13:05:51.000000 qtstrap-0.4.1/qtstrap/extras/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.245062 qtstrap-0.4.1/qtstrap/extras/code_editor/
--rw-rw-rw-   0        0        0      113 2022-05-01 01:28:19.000000 qtstrap-0.4.1/qtstrap/extras/code_editor/__init__.py
--rw-rw-rw-   0        0        0    12442 2023-03-03 10:10:47.000000 qtstrap-0.4.1/qtstrap/extras/code_editor/code_editor.py
--rw-rw-rw-   0        0        0      847 2022-12-10 23:54:46.000000 qtstrap-0.4.1/qtstrap/extras/code_editor/code_line.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.252068 qtstrap-0.4.1/qtstrap/extras/code_editor/highlighters/
--rw-rw-rw-   0        0        0       37 2021-04-25 18:57:56.000000 qtstrap-0.4.1/qtstrap/extras/code_editor/highlighters/__init__.py
--rw-rw-rw-   0        0        0     6354 2023-03-07 12:26:48.000000 qtstrap-0.4.1/qtstrap/extras/code_editor/highlighters/python.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.255063 qtstrap-0.4.1/qtstrap/extras/command_palette/
--rw-rw-rw-   0        0        0       52 2021-07-23 15:36:03.000000 qtstrap-0.4.1/qtstrap/extras/command_palette/__init__.py
--rw-rw-rw-   0        0        0    11581 2023-03-03 07:33:08.000000 qtstrap-0.4.1/qtstrap/extras/command_palette/command_palette.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.266063 qtstrap-0.4.1/qtstrap/extras/log_monitor/
--rw-rw-rw-   0        0        0     1124 2022-12-23 00:25:27.000000 qtstrap-0.4.1/qtstrap/extras/log_monitor/__init__.py
--rw-rw-rw-   0        0        0     2437 2022-12-23 00:25:31.000000 qtstrap-0.4.1/qtstrap/extras/log_monitor/log_database_handler.py
--rw-rw-rw-   0        0        0    16742 2023-01-09 23:30:38.000000 qtstrap-0.4.1/qtstrap/extras/log_monitor/log_filter_controls.py
--rw-rw-rw-   0        0        0     4165 2022-12-22 21:39:18.000000 qtstrap-0.4.1/qtstrap/extras/log_monitor/log_profile.py
--rw-rw-rw-   0        0        0     3791 2022-12-23 00:34:07.000000 qtstrap-0.4.1/qtstrap/extras/log_monitor/log_table_view.py
--rw-rw-rw-   0        0        0     4710 2023-03-03 07:38:29.000000 qtstrap-0.4.1/qtstrap/extras/log_monitor/log_widget.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.272064 qtstrap-0.4.1/qtstrap/extras/style/
--rw-rw-rw-   0        0        0      129 2023-03-03 07:24:23.000000 qtstrap-0.4.1/qtstrap/extras/style/__init__.py
--rw-rw-rw-   0        0        0     1085 2023-01-12 03:06:47.000000 qtstrap-0.4.1/qtstrap/extras/style/colors.py
--rw-rw-rw-   0        0        0     2040 2023-03-03 07:24:23.000000 qtstrap-0.4.1/qtstrap/extras/style/dark_palette.py
--rw-rw-rw-   0        0        0     4105 2023-03-07 12:55:24.000000 qtstrap-0.4.1/qtstrap/extras/style/themes.py
--rw-rw-rw-   0        0        0     1174 2022-12-10 01:10:44.000000 qtstrap-0.4.1/qtstrap/options.py
--rw-rw-rw-   0        0        0      694 2023-03-07 15:43:09.000000 qtstrap-0.4.1/qtstrap/qt.py
--rw-rw-rw-   0        0        0      504 2022-12-09 05:56:13.000000 qtstrap-0.4.1/qtstrap/settings.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.284062 qtstrap-0.4.1/qtstrap/template/
--rw-rw-rw-   0        0        0     3629 2022-07-30 00:00:03.000000 qtstrap-0.4.1/qtstrap/template/Makefile
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.286062 qtstrap-0.4.1/qtstrap/template/app/
--rw-rw-rw-   0        0        0      953 2021-04-02 17:24:51.000000 qtstrap-0.4.1/qtstrap/template/app/main.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.289561 qtstrap-0.4.1/qtstrap/template/app/resources/
--rw-rw-rw-   0        0        0    59285 2021-04-01 21:16:04.000000 qtstrap-0.4.1/qtstrap/template/app/resources/application.ico
--rw-rw-rw-   0        0        0     5523 2021-04-01 21:16:04.000000 qtstrap-0.4.1/qtstrap/template/app/resources/icon.svg
--rw-rw-rw-   0        0        0     1195 2022-09-11 05:33:04.000000 qtstrap-0.4.1/qtstrap/template/bundle.spec
--rw-rw-rw-   0        0        0     2450 2022-07-29 23:52:21.000000 qtstrap-0.4.1/qtstrap/template/installer.iss
--rw-rw-rw-   0        0        0        0 2021-04-01 21:16:04.000000 qtstrap-0.4.1/qtstrap/template/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.317562 qtstrap-0.4.1/qtstrap/utils/
--rw-rw-rw-   0        0        0      390 2022-12-08 21:10:40.000000 qtstrap-0.4.1/qtstrap/utils/__init__.py
--rw-rw-rw-   0        0        0     2367 2022-12-11 02:32:50.000000 qtstrap-0.4.1/qtstrap/utils/adapter.py
--rw-rw-rw-   0        0        0      265 2022-10-20 22:39:10.000000 qtstrap-0.4.1/qtstrap/utils/call_later.py
--rw-rw-rw-   0        0        0      652 2021-05-13 17:33:19.000000 qtstrap-0.4.1/qtstrap/utils/defer.py
--rw-rw-rw-   0        0        0     2800 2022-12-12 00:29:52.000000 qtstrap-0.4.1/qtstrap/utils/drag_and_drop.py
--rw-rw-rw-   0        0        0      629 2022-11-03 16:33:13.000000 qtstrap-0.4.1/qtstrap/utils/get_ip.py
--rw-rw-rw-   0        0        0      378 2023-02-04 21:57:48.000000 qtstrap-0.4.1/qtstrap/utils/signals.py
--rw-rw-rw-   0        0        0      255 2022-11-03 16:23:26.000000 qtstrap-0.4.1/qtstrap/utils/singleton.py
--rw-rw-rw-   0        0        0      751 2023-02-04 22:01:45.000000 qtstrap-0.4.1/qtstrap/utils/string_builder.py
--rw-rw-rw-   0        0        0      531 2021-10-30 07:31:06.000000 qtstrap-0.4.1/qtstrap/utils/timestamp.py
--rw-rw-rw-   0        0        0      291 2022-12-11 02:07:30.000000 qtstrap-0.4.1/qtstrap/utils/trace.py
--rw-rw-rw-   0        0        0     2491 2022-11-03 16:16:04.000000 qtstrap-0.4.1/qtstrap/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.340064 qtstrap-0.4.1/qtstrap/widgets/
--rw-rw-rw-   0        0        0      890 2023-02-23 14:40:05.000000 qtstrap-0.4.1/qtstrap/widgets/__init__.py
--rw-rw-rw-   0        0        0     2973 2022-12-09 06:51:34.000000 qtstrap-0.4.1/qtstrap/widgets/buttons.py
--rw-rw-rw-   0        0        0     1590 2022-05-15 05:13:52.000000 qtstrap-0.4.1/qtstrap/widgets/labeledit.py
--rw-rw-rw-   0        0        0     8325 2023-02-23 14:43:48.000000 qtstrap-0.4.1/qtstrap/widgets/layouts.py
--rw-rw-rw-   0        0        0      665 2021-04-01 21:16:04.000000 qtstrap-0.4.1/qtstrap/widgets/line_widgets.py
--rw-rw-rw-   0        0        0      824 2022-10-26 07:40:04.000000 qtstrap-0.4.1/qtstrap/widgets/link_label.py
--rw-rw-rw-   0        0        0     3161 2021-05-06 02:08:19.000000 qtstrap-0.4.1/qtstrap/widgets/persistent_tab_widget.py
--rw-rw-rw-   0        0        0     5473 2022-11-10 17:33:23.000000 qtstrap-0.4.1/qtstrap/widgets/persistent_widgets.py
--rw-rw-rw-   0        0        0     7568 2023-03-03 08:21:01.000000 qtstrap-0.4.1/qtstrap/widgets/toggle.py
--rw-rw-rw-   0        0        0      910 2022-11-07 02:00:59.000000 qtstrap-0.4.1/qtstrap/widgets/toolbar.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.239061 qtstrap-0.4.1/qtstrap.egg-info/
--rw-rw-rw-   0        0        0     2554 2023-03-07 15:44:09.000000 qtstrap-0.4.1/qtstrap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4468 2023-03-07 15:44:09.000000 qtstrap-0.4.1/qtstrap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 15:44:09.000000 qtstrap-0.4.1/qtstrap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-03-07 15:44:09.000000 qtstrap-0.4.1/qtstrap.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-12-23 00:34:54.000000 qtstrap-0.4.1/qtstrap.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       52 2023-03-07 15:44:09.000000 qtstrap-0.4.1/qtstrap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-07 15:44:09.000000 qtstrap-0.4.1/qtstrap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1141 2022-11-30 17:51:25.000000 qtstrap-0.4.1/requirements.txt
--rw-rw-rw-   0        0        0      529 2022-10-26 06:20:37.000000 qtstrap-0.4.1/requirements_build.txt
--rw-rw-rw-   0        0        0      520 2022-10-26 06:55:20.000000 qtstrap-0.4.1/requirements_test.txt
--rw-rw-rw-   0        0        0      158 2022-11-24 06:15:10.000000 qtstrap-0.4.1/run_tox_tests.py
--rw-rw-rw-   0        0        0     1254 2023-03-07 15:44:10.372061 qtstrap-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0       96 2022-07-30 01:23:30.000000 qtstrap-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.353062 qtstrap-0.4.1/test/
--rw-rw-rw-   0        0        0      876 2021-04-01 21:16:04.000000 qtstrap-0.4.1/test/test_base_app.py
--rw-rw-rw-   0        0        0     1073 2021-04-01 21:16:04.000000 qtstrap-0.4.1/test/test_base_window.py
--rw-rw-rw-   0        0        0      616 2022-11-24 06:02:31.000000 qtstrap-0.4.1/test/test_layouts.py
--rw-rw-rw-   0        0        0     2689 2022-11-24 05:29:55.000000 qtstrap-0.4.1/test/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-07 15:44:10.359561 qtstrap-0.4.1/test/utils/
--rw-rw-rw-   0        0        0      230 2022-11-24 04:25:54.000000 qtstrap-0.4.1/test/utils/test_defer.py
--rw-rw-rw-   0        0        0      348 2022-11-30 16:27:29.000000 qtstrap-0.4.1/tox.ini
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.424636 qtstrap-0.4.2/
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:21.287636 qtstrap-0.4.2/.github/
+-rw-rw-rw-   0        0        0      784 2023-03-26 02:17:30.000000 qtstrap-0.4.2/.github/FUNDING.yml
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:21.289135 qtstrap-0.4.2/.github/workflows/
+-rw-rw-rw-   0        0        0      978 2022-07-30 04:06:00.000000 qtstrap-0.4.2/.github/workflows/main.yml
+-rw-rw-rw-   0        0        0      161 2022-11-24 04:51:10.000000 qtstrap-0.4.2/.gitignore
+-rw-rw-rw-   0        0        0     1090 2021-04-01 21:16:04.000000 qtstrap-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0       96 2021-04-01 21:16:04.000000 qtstrap-0.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2600 2023-03-07 12:46:55.000000 qtstrap-0.4.2/Makefile
+-rw-rw-rw-   0        0        0     3396 2023-04-29 17:00:22.425138 qtstrap-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2441 2023-03-27 09:49:48.000000 qtstrap-0.4.2/README.md
+-rw-rw-rw-   0        0        0      272 2022-07-30 03:58:00.000000 qtstrap-0.4.2/build_docs.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:21.317633 qtstrap-0.4.2/docs/
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:21.776635 qtstrap-0.4.2/docs/api/
+-rw-rw-rw-   0        0        0       68 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/.pages
+-rw-rw-rw-   0        0        0     4540 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.code_editor.code_editor.md
+-rw-rw-rw-   0        0        0     1305 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.code_editor.code_line.md
+-rw-rw-rw-   0        0        0      448 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.code_editor.highlighters.md
+-rw-rw-rw-   0        0        0     3021 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.code_editor.highlighters.python.md
+-rw-rw-rw-   0        0        0      464 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.code_editor.md
+-rw-rw-rw-   0        0        0     8390 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.command_palette.command_palette.md
+-rw-rw-rw-   0        0        0      439 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.command_palette.md
+-rw-rw-rw-   0        0        0     2349 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.log_monitor.log_database_handler.md
+-rw-rw-rw-   0        0        0    13379 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.log_monitor.log_filter_controls.md
+-rw-rw-rw-   0        0        0     3604 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.log_monitor.log_profile.md
+-rw-rw-rw-   0        0        0     4181 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.log_monitor.log_table_view.md
+-rw-rw-rw-   0        0        0     4558 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.log_monitor.log_widget.md
+-rw-rw-rw-   0        0        0      887 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.log_monitor.md
+-rw-rw-rw-   0        0        0      342 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.md
+-rw-rw-rw-   0        0        0      802 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.style.colors.md
+-rw-rw-rw-   0        0        0      772 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.style.dark_palette.md
+-rw-rw-rw-   0        0        0      430 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.style.md
+-rw-rw-rw-   0        0        0     1259 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/extras.style.themes.md
+-rw-rw-rw-   0        0        0      546 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/options.md
+-rw-rw-rw-   0        0        0    11165 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/overview.md
+-rw-rw-rw-   0        0        0      754 2022-07-30 03:58:01.000000 qtstrap-0.4.2/docs/api/settings.md
+-rw-rw-rw-   0        0        0     1958 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.adapter.md
+-rw-rw-rw-   0        0        0      784 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.call_later.md
+-rw-rw-rw-   0        0        0      599 2022-07-30 03:58:01.000000 qtstrap-0.4.2/docs/api/utils.decorators.md
+-rw-rw-rw-   0        0        0     1019 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.defer.md
+-rw-rw-rw-   0        0        0     1641 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.drag_and_drop.md
+-rw-rw-rw-   0        0        0      742 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.get_ip.md
+-rw-rw-rw-   0        0        0      459 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.md
+-rw-rw-rw-   0        0        0      946 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.signals.md
+-rw-rw-rw-   0        0        0      607 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.singleton.md
+-rw-rw-rw-   0        0        0     1414 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.string_builder.md
+-rw-rw-rw-   0        0        0     1597 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.timestamp.md
+-rw-rw-rw-   0        0        0      641 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.trace.md
+-rw-rw-rw-   0        0        0     2555 2023-03-27 09:43:36.000000 qtstrap-0.4.2/docs/api/utils.utils.md
+-rw-rw-rw-   0        0        0     4948 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.buttons.md
+-rw-rw-rw-   0        0        0     2853 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.labeledit.md
+-rw-rw-rw-   0        0        0    16745 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.layouts.md
+-rw-rw-rw-   0        0        0     1464 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.line_widgets.md
+-rw-rw-rw-   0        0        0     1764 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.link_label.md
+-rw-rw-rw-   0        0        0      555 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.md
+-rw-rw-rw-   0        0        0     3040 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.persistent_tab_widget.md
+-rw-rw-rw-   0        0        0     7854 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.persistent_widgets.md
+-rw-rw-rw-   0        0        0     7763 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.toggle.md
+-rw-rw-rw-   0        0        0     1276 2023-03-27 09:43:37.000000 qtstrap-0.4.2/docs/api/widgets.toolbar.md
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:21.842636 qtstrap-0.4.2/docs/extras/
+-rw-rw-rw-   0        0        0      684 2023-03-27 09:12:02.000000 qtstrap-0.4.2/docs/extras/code_editor.md
+-rw-rw-rw-   0        0        0     1183 2023-03-27 09:27:16.000000 qtstrap-0.4.2/docs/extras/command_palette.md
+-rw-rw-rw-   0        0        0      105 2023-03-27 09:29:20.000000 qtstrap-0.4.2/docs/extras/index.md
+-rw-rw-rw-   0        0        0     1594 2023-03-27 09:42:00.000000 qtstrap-0.4.2/docs/extras/log_monitor.md
+-rw-rw-rw-   0        0        0       48 2023-03-27 09:41:38.000000 qtstrap-0.4.2/docs/extras/styles.md
+-rw-rw-rw-   0        0        0     1611 2023-03-26 02:25:27.000000 qtstrap-0.4.2/docs/index.md
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:21.910637 qtstrap-0.4.2/docs/quickstart/
+-rw-rw-rw-   0        0        0     2618 2021-04-01 21:16:04.000000 qtstrap-0.4.2/docs/quickstart/baseapplication.md
+-rw-rw-rw-   0        0        0      920 2021-04-01 21:16:04.000000 qtstrap-0.4.2/docs/quickstart/basemainwindow.md
+-rw-rw-rw-   0        0        0     1700 2021-04-01 21:16:04.000000 qtstrap-0.4.2/docs/quickstart/context_layouts.md
+-rw-rw-rw-   0        0        0     1264 2021-04-02 17:24:51.000000 qtstrap-0.4.2/docs/quickstart/gettingstarted.md
+-rw-rw-rw-   0        0        0      857 2021-04-01 21:16:04.000000 qtstrap-0.4.2/docs/quickstart/installation.md
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.166135 qtstrap-0.4.2/docs/reference/
+-rw-rw-rw-   0        0        0      759 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/base_application.md
+-rw-rw-rw-   0        0        0      682 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/base_window.md
+-rw-rw-rw-   0        0        0      653 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/options.md
+-rw-rw-rw-   0        0        0      287 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/settings.md
+-rw-rw-rw-   0        0        0      962 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/toolbar.md
+-rw-rw-rw-   0        0        0     1484 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.adapter.md
+-rw-rw-rw-   0        0        0       88 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.decorators.md
+-rw-rw-rw-   0        0        0      618 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.defer.md
+-rw-rw-rw-   0        0        0      353 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.md
+-rw-rw-rw-   0        0        0      576 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.signals.md
+-rw-rw-rw-   0        0        0      105 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.singleton.md
+-rw-rw-rw-   0        0        0      690 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.timestamp.md
+-rw-rw-rw-   0        0        0     1349 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/utils.utils.md
+-rw-rw-rw-   0        0        0     2361 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/widgets.buttons.md
+-rw-rw-rw-   0        0        0     1196 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/widgets.labeledit.md
+-rw-rw-rw-   0        0        0     4766 2022-07-30 03:40:51.000000 qtstrap-0.4.2/docs/reference/widgets.layouts.md
+-rw-rw-rw-   0        0        0      516 2022-07-30 03:40:51.000000 qtstrap-0.4.2/docs/reference/widgets.line_widgets.md
+-rw-rw-rw-   0        0        0      638 2022-07-30 03:40:51.000000 qtstrap-0.4.2/docs/reference/widgets.link_label.md
+-rw-rw-rw-   0        0        0     1408 2022-07-30 03:40:50.000000 qtstrap-0.4.2/docs/reference/widgets.md
+-rw-rw-rw-   0        0        0     1324 2022-07-30 03:40:51.000000 qtstrap-0.4.2/docs/reference/widgets.persistent_tab_widget.md
+-rw-rw-rw-   0        0        0     3704 2022-07-30 03:40:51.000000 qtstrap-0.4.2/docs/reference/widgets.persistent_widgets.md
+-rw-rw-rw-   0        0        0     2949 2021-04-01 21:16:04.000000 qtstrap-0.4.2/docs/screenshot1.png
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.194635 qtstrap-0.4.2/docs/structure/
+-rw-rw-rw-   0        0        0     1193 2021-04-01 21:16:04.000000 qtstrap-0.4.2/docs/structure/makefile.md
+-rw-rw-rw-   0        0        0     3013 2022-07-30 00:37:45.000000 qtstrap-0.4.2/docs/structure/structure.md
+-rw-rw-rw-   0        0        0     7886 2022-07-30 03:01:48.000000 qtstrap-0.4.2/docs/test.md
+-rw-rw-rw-   0        0        0      987 2023-03-27 08:50:48.000000 qtstrap-0.4.2/mkdocs.yml
+-rw-rw-rw-   0        0        0      345 2022-07-30 04:03:13.000000 qtstrap-0.4.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.232138 qtstrap-0.4.2/qtstrap/
+-rw-rw-rw-   0        0        0     1035 2023-03-07 12:33:33.000000 qtstrap-0.4.2/qtstrap/__init__.py
+-rw-rw-rw-   0        0        0     1901 2023-03-27 08:38:01.000000 qtstrap-0.4.2/qtstrap/__main__.py
+-rw-rw-rw-   0        0        0     2051 2023-03-07 12:17:44.000000 qtstrap-0.4.2/qtstrap/base_application.py
+-rw-rw-rw-   0        0        0     2074 2023-03-07 12:38:24.000000 qtstrap-0.4.2/qtstrap/base_window.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.303636 qtstrap-0.4.2/qtstrap/experimental/
+-rw-rw-rw-   0        0        0        0 2023-04-03 00:57:28.000000 qtstrap-0.4.2/qtstrap/experimental/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.305137 qtstrap-0.4.2/qtstrap/extras/
+-rw-rw-rw-   0        0        0        0 2021-04-08 13:05:51.000000 qtstrap-0.4.2/qtstrap/extras/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.311637 qtstrap-0.4.2/qtstrap/extras/code_editor/
+-rw-rw-rw-   0        0        0      113 2022-05-01 01:28:19.000000 qtstrap-0.4.2/qtstrap/extras/code_editor/__init__.py
+-rw-rw-rw-   0        0        0    12535 2023-03-27 09:14:21.000000 qtstrap-0.4.2/qtstrap/extras/code_editor/code_editor.py
+-rw-rw-rw-   0        0        0      847 2022-12-10 23:54:46.000000 qtstrap-0.4.2/qtstrap/extras/code_editor/code_line.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.316135 qtstrap-0.4.2/qtstrap/extras/code_editor/highlighters/
+-rw-rw-rw-   0        0        0       37 2021-04-25 18:57:56.000000 qtstrap-0.4.2/qtstrap/extras/code_editor/highlighters/__init__.py
+-rw-rw-rw-   0        0        0     6354 2023-03-07 12:26:48.000000 qtstrap-0.4.2/qtstrap/extras/code_editor/highlighters/python.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.318634 qtstrap-0.4.2/qtstrap/extras/command_palette/
+-rw-rw-rw-   0        0        0       52 2021-07-23 15:36:03.000000 qtstrap-0.4.2/qtstrap/extras/command_palette/__init__.py
+-rw-rw-rw-   0        0        0    11678 2023-03-27 09:27:44.000000 qtstrap-0.4.2/qtstrap/extras/command_palette/command_palette.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.332635 qtstrap-0.4.2/qtstrap/extras/log_monitor/
+-rw-rw-rw-   0        0        0     1124 2022-12-23 00:25:27.000000 qtstrap-0.4.2/qtstrap/extras/log_monitor/__init__.py
+-rw-rw-rw-   0        0        0     2437 2022-12-23 00:25:31.000000 qtstrap-0.4.2/qtstrap/extras/log_monitor/log_database_handler.py
+-rw-rw-rw-   0        0        0    16819 2023-04-29 15:39:56.000000 qtstrap-0.4.2/qtstrap/extras/log_monitor/log_filter_controls.py
+-rw-rw-rw-   0        0        0     4165 2022-12-22 21:39:18.000000 qtstrap-0.4.2/qtstrap/extras/log_monitor/log_profile.py
+-rw-rw-rw-   0        0        0     3935 2023-04-29 15:35:41.000000 qtstrap-0.4.2/qtstrap/extras/log_monitor/log_table_view.py
+-rw-rw-rw-   0        0        0     4710 2023-03-03 07:38:29.000000 qtstrap-0.4.2/qtstrap/extras/log_monitor/log_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.352135 qtstrap-0.4.2/qtstrap/extras/style/
+-rw-rw-rw-   0        0        0      129 2023-03-03 07:24:23.000000 qtstrap-0.4.2/qtstrap/extras/style/__init__.py
+-rw-rw-rw-   0        0        0     1085 2023-01-12 03:06:47.000000 qtstrap-0.4.2/qtstrap/extras/style/colors.py
+-rw-rw-rw-   0        0        0     2040 2023-03-03 07:24:23.000000 qtstrap-0.4.2/qtstrap/extras/style/dark_palette.py
+-rw-rw-rw-   0        0        0     4105 2023-03-07 12:55:24.000000 qtstrap-0.4.2/qtstrap/extras/style/themes.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.353636 qtstrap-0.4.2/qtstrap/optional/
+-rw-rw-rw-   0        0        0        0 2023-04-03 00:57:38.000000 qtstrap-0.4.2/qtstrap/optional/__init__.py
+-rw-rw-rw-   0        0        0     1174 2022-12-10 01:10:44.000000 qtstrap-0.4.2/qtstrap/options.py
+-rw-rw-rw-   0        0        0      694 2023-03-27 08:40:17.000000 qtstrap-0.4.2/qtstrap/qt.py
+-rw-rw-rw-   0        0        0      504 2022-12-09 05:56:13.000000 qtstrap-0.4.2/qtstrap/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.360637 qtstrap-0.4.2/qtstrap/template/
+-rw-rw-rw-   0        0        0     3629 2022-07-30 00:00:03.000000 qtstrap-0.4.2/qtstrap/template/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.362136 qtstrap-0.4.2/qtstrap/template/app/
+-rw-rw-rw-   0        0        0      953 2021-04-02 17:24:51.000000 qtstrap-0.4.2/qtstrap/template/app/main.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.366135 qtstrap-0.4.2/qtstrap/template/app/resources/
+-rw-rw-rw-   0        0        0    59285 2021-04-01 21:16:04.000000 qtstrap-0.4.2/qtstrap/template/app/resources/application.ico
+-rw-rw-rw-   0        0        0     5523 2021-04-01 21:16:04.000000 qtstrap-0.4.2/qtstrap/template/app/resources/icon.svg
+-rw-rw-rw-   0        0        0     1195 2022-09-11 05:33:04.000000 qtstrap-0.4.2/qtstrap/template/bundle.spec
+-rw-rw-rw-   0        0        0     2450 2022-07-29 23:52:21.000000 qtstrap-0.4.2/qtstrap/template/installer.iss
+-rw-rw-rw-   0        0        0        0 2021-04-01 21:16:04.000000 qtstrap-0.4.2/qtstrap/template/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.392636 qtstrap-0.4.2/qtstrap/utils/
+-rw-rw-rw-   0        0        0      390 2022-12-08 21:10:40.000000 qtstrap-0.4.2/qtstrap/utils/__init__.py
+-rw-rw-rw-   0        0        0     2469 2023-03-26 02:15:24.000000 qtstrap-0.4.2/qtstrap/utils/adapter.py
+-rw-rw-rw-   0        0        0      265 2022-10-20 22:39:10.000000 qtstrap-0.4.2/qtstrap/utils/call_later.py
+-rw-rw-rw-   0        0        0      652 2021-05-13 17:33:19.000000 qtstrap-0.4.2/qtstrap/utils/defer.py
+-rw-rw-rw-   0        0        0     2800 2022-12-12 00:29:52.000000 qtstrap-0.4.2/qtstrap/utils/drag_and_drop.py
+-rw-rw-rw-   0        0        0      629 2022-11-03 16:33:13.000000 qtstrap-0.4.2/qtstrap/utils/get_ip.py
+-rw-rw-rw-   0        0        0      378 2023-02-04 21:57:48.000000 qtstrap-0.4.2/qtstrap/utils/signals.py
+-rw-rw-rw-   0        0        0      255 2022-11-03 16:23:26.000000 qtstrap-0.4.2/qtstrap/utils/singleton.py
+-rw-rw-rw-   0        0        0      751 2023-02-04 22:01:45.000000 qtstrap-0.4.2/qtstrap/utils/string_builder.py
+-rw-rw-rw-   0        0        0      531 2021-10-30 07:31:06.000000 qtstrap-0.4.2/qtstrap/utils/timestamp.py
+-rw-rw-rw-   0        0        0      291 2022-12-11 02:07:30.000000 qtstrap-0.4.2/qtstrap/utils/trace.py
+-rw-rw-rw-   0        0        0     2491 2022-11-03 16:16:04.000000 qtstrap-0.4.2/qtstrap/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.411638 qtstrap-0.4.2/qtstrap/widgets/
+-rw-rw-rw-   0        0        0      890 2023-02-23 14:40:05.000000 qtstrap-0.4.2/qtstrap/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2973 2022-12-09 06:51:34.000000 qtstrap-0.4.2/qtstrap/widgets/buttons.py
+-rw-rw-rw-   0        0        0     1590 2022-05-15 05:13:52.000000 qtstrap-0.4.2/qtstrap/widgets/labeledit.py
+-rw-rw-rw-   0        0        0     8559 2023-04-29 16:55:24.000000 qtstrap-0.4.2/qtstrap/widgets/layouts.py
+-rw-rw-rw-   0        0        0      665 2021-04-01 21:16:04.000000 qtstrap-0.4.2/qtstrap/widgets/line_widgets.py
+-rw-rw-rw-   0        0        0      824 2022-10-26 07:40:04.000000 qtstrap-0.4.2/qtstrap/widgets/link_label.py
+-rw-rw-rw-   0        0        0     3161 2021-05-06 02:08:19.000000 qtstrap-0.4.2/qtstrap/widgets/persistent_tab_widget.py
+-rw-rw-rw-   0        0        0     5473 2022-11-10 17:33:23.000000 qtstrap-0.4.2/qtstrap/widgets/persistent_widgets.py
+-rw-rw-rw-   0        0        0     7568 2023-03-03 08:21:01.000000 qtstrap-0.4.2/qtstrap/widgets/toggle.py
+-rw-rw-rw-   0        0        0      910 2022-11-07 02:00:59.000000 qtstrap-0.4.2/qtstrap/widgets/toolbar.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.302640 qtstrap-0.4.2/qtstrap.egg-info/
+-rw-rw-rw-   0        0        0     3396 2023-04-29 17:00:21.000000 qtstrap-0.4.2/qtstrap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4908 2023-04-29 17:00:21.000000 qtstrap-0.4.2/qtstrap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 17:00:21.000000 qtstrap-0.4.2/qtstrap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-29 17:00:21.000000 qtstrap-0.4.2/qtstrap.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-12-23 00:34:54.000000 qtstrap-0.4.2/qtstrap.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       52 2023-04-29 17:00:21.000000 qtstrap-0.4.2/qtstrap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-29 17:00:21.000000 qtstrap-0.4.2/qtstrap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1141 2022-11-30 17:51:25.000000 qtstrap-0.4.2/requirements.txt
+-rw-rw-rw-   0        0        0      529 2022-10-26 06:20:37.000000 qtstrap-0.4.2/requirements_build.txt
+-rw-rw-rw-   0        0        0      520 2022-10-26 06:55:20.000000 qtstrap-0.4.2/requirements_test.txt
+-rw-rw-rw-   0        0        0      158 2022-11-24 06:15:10.000000 qtstrap-0.4.2/run_tox_tests.py
+-rw-rw-rw-   0        0        0     1254 2023-04-29 17:00:22.428137 qtstrap-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0       96 2022-07-30 01:23:30.000000 qtstrap-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.422135 qtstrap-0.4.2/test/
+-rw-rw-rw-   0        0        0      876 2021-04-01 21:16:04.000000 qtstrap-0.4.2/test/test_base_app.py
+-rw-rw-rw-   0        0        0     1073 2021-04-01 21:16:04.000000 qtstrap-0.4.2/test/test_base_window.py
+-rw-rw-rw-   0        0        0      616 2022-11-24 06:02:31.000000 qtstrap-0.4.2/test/test_layouts.py
+-rw-rw-rw-   0        0        0     2689 2022-11-24 05:29:55.000000 qtstrap-0.4.2/test/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:00:22.423635 qtstrap-0.4.2/test/utils/
+-rw-rw-rw-   0        0        0      230 2022-11-24 04:25:54.000000 qtstrap-0.4.2/test/utils/test_defer.py
+-rw-rw-rw-   0        0        0      348 2022-11-30 16:27:29.000000 qtstrap-0.4.2/tox.ini
```

### Comparing `qtstrap-0.4.1/.github/workflows/main.yml` & `qtstrap-0.4.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/LICENSE` & `qtstrap-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/Makefile` & `qtstrap-0.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/PKG-INFO` & `qtstrap-0.4.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtstrap
-Version: 0.4.1
+Version: 0.4.2
 Summary: Like Bootstrap, but qt-er.
 Home-page: https://github.com/qtstrap/qtstrap
 Author: David Kincaid
 Author-email: dlkincaid0@gmail.com
 License: MIT
 Project-URL: Documentation, https://qtstrap.github.io/qtstrap/
 Project-URL: Source, https://github.com/qtstrap/qtstrap
@@ -36,22 +36,60 @@
 
 # Features
 
 More complete docs are available [here](https://qtstrap.github.io/qtstrap/).
 
 * `qtstrap` command line tool to bootstrap new projects
 * crossplatform makefile with useful development commands
-* preconfigured pyinstaller spec file
-* preconfigured InnoSetup setup compiler script
+* preconfigured build system using PyInstaller and InnoSetup
 * custom Qt widgets with useful behaviors
 * Pythonic layout system using ContextLayouts
 * Some other stuff I haven't remembered yet
 
-# License
-This project is released under the MIT license.
+## Custom Widgets
+
+- `LabelEdit`
+- `HLine` and `VLine`
+- `LinkLabel`
+- Buttons:
+  - `StateButton`
+  - `IconToggleButton`
+  - `ConfirmToggleButton`
+  - `MenuButton`
+- Persistent Widgets (for rapid prototyping of saved data):
+  - `PersistentCheckableAction`
+  - `PersistentCheckBox`
+  - `PersistentComboBox`
+  - `PersistentLineEdit`
+  - `PersistentListWidget`
+  - `PersistentPlainTextEdit`
+  - `PersistentTabWidget`
+  - `PersistentTextEdit`
+  - `PersistentTreeWidget`
+
+## Utility Classes and Functions
+- `Adapter`
+- `TimeStamp`
+- `StringBuilder`
+- `call_later()`
+
+## decorators:
+- `@accepts_file_drops`
+- `@trace`
+- `@singleton`
+
+## context managers:
+- `Defer`
+- `SignalBlocker`
+
+## qtstrap.extras:
+  - `CommandPalette`, like VSCode or SublimeText
+  - Logging Subsystem: log to local database + log viewer widgets
+  - `CodeEditor`: Custom QTextEditor subclass customized for code editing
+
 
 # Dependencies
 
 * Python 3
 * PySide2 or PyQt5
 * Make(optional, but recommended)
```

### Comparing `qtstrap-0.4.1/docs/api/extras.code_editor.code_editor.md` & `qtstrap-0.4.2/docs/api/extras.code_editor.code_editor.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # <kbd>module</kbd> `extras.code_editor.code_editor`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 
 ---
@@ -20,15 +21,15 @@
 <a href="..\..\qtstrap\extras\code_editor\code_editor.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `CodeEditor`
 
 
 
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L7"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeEditor.__init__`
 
 ```python
 __init__(*args, changed=None, model=None, highlighter=None, **kwargs)
 ```
 
@@ -37,155 +38,169 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L43"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L211"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `CodeEditor.duplicate_selection`
+
+```python
+duplicate_selection(direction)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L47"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeEditor.eventFilter`
 
 ```python
 eventFilter(obj, event)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L138"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L161"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeEditor.expand_selection`
 
 ```python
 expand_selection(cursor)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L243"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L307"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeEditor.indent_selection`
 
 ```python
 indent_selection(direction)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L56"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L60"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeEditor.insert_completion`
 
 ```python
 insert_completion(completion)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L69"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L73"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeEditor.keyPressEvent`
 
 ```python
-keyPressEvent(event: PySide6.QtGui.QKeyEvent)
+keyPressEvent(event: PySide2.QtGui.QKeyEvent)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L187"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L251"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeEditor.move_selection`
 
 ```python
 move_selection(direction)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L309"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L373"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeEditor.text`
 
 ```python
 text()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L64"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L68"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeEditor.text_under_cursor`
 
 ```python
 text_under_cursor()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L141"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L164"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeEditor.toggle_comments`
 
 ```python
 toggle_comments()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L50"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L54"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeEditor.update_tab_width`
 
 ```python
 update_tab_width()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L292"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L356"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeEditor.wrap_selection`
 
 ```python
 wrap_selection(key)
 ```
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
 `extras.code_editor.code_editor` **Global Variables** --------------- -
-**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** --- [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ## class `CodeEditor` [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`CodeEditor.__init__` ```python __init__(*args, changed=None, model=None,
-highlighter=None, **kwargs) ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `CodeEditor.eventFilter` ```python
+**TYPE_CHECKING** - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** ---
+[https://img.shields.io/badge/-source-cccccc?style=flat-square] ## class
+`CodeEditor` [https://img.shields.io/badge/-source-cccccc?style=flat-square]
+### method `CodeEditor.__init__` ```python __init__(*args, changed=None,
+model=None, highlighter=None, **kwargs) ``` --- [https://img.shields.io/badge/-
+source-cccccc?style=flat-square] ### method `CodeEditor.duplicate_selection`
+```python duplicate_selection(direction) ``` --- [https://img.shields.io/badge/
+-source-cccccc?style=flat-square] ### method `CodeEditor.eventFilter` ```python
 eventFilter(obj, event) ``` --- [https://img.shields.io/badge/-source-
 cccccc?style=flat-square] ### method `CodeEditor.expand_selection` ```python
 expand_selection(cursor) ``` --- [https://img.shields.io/badge/-source-
 cccccc?style=flat-square] ### method `CodeEditor.indent_selection` ```python
 indent_selection(direction) ``` --- [https://img.shields.io/badge/-source-
 cccccc?style=flat-square] ### method `CodeEditor.insert_completion` ```python
 insert_completion(completion) ``` --- [https://img.shields.io/badge/-source-
 cccccc?style=flat-square] ### method `CodeEditor.keyPressEvent` ```python
-keyPressEvent(event: PySide6.QtGui.QKeyEvent) ``` --- [https://img.shields.io/
+keyPressEvent(event: PySide2.QtGui.QKeyEvent) ``` --- [https://img.shields.io/
 badge/-source-cccccc?style=flat-square] ### method `CodeEditor.move_selection`
 ```python move_selection(direction) ``` --- [https://img.shields.io/badge/-
 source-cccccc?style=flat-square] ### method `CodeEditor.text` ```python text()
 ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ###
 method `CodeEditor.text_under_cursor` ```python text_under_cursor() ``` ---
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CodeEditor.toggle_comments` ```python toggle_comments() ``` --- [https://
```

### Comparing `qtstrap-0.4.1/docs/api/extras.code_editor.code_line.md` & `qtstrap-0.4.2/docs/api/extras.code_editor.code_line.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # <kbd>module</kbd> `extras.code_editor.code_line`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 
 ---
@@ -42,15 +43,15 @@
 ---
 
 <a href="..\..\qtstrap\extras\code_editor\code_line.py#L13"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeLine.keyPressEvent`
 
 ```python
-keyPressEvent(event: PySide6.QtGui.QKeyEvent)
+keyPressEvent(event: PySide2.QtGui.QKeyEvent)
 ```
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
-`extras.code_editor.code_line` **Global Variables** --------------- - **PYQT6**
-- **PYQT5** - **PYSIDE2** - **PYSIDE6** --- [https://img.shields.io/badge/-
-source-cccccc?style=flat-square] ## class `CodeLine` [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ### method `CodeLine.__init__`
-```python __init__(*args, **kwargs) ``` --- [https://img.shields.io/badge/-
-source-cccccc?style=flat-square] ### method `CodeLine.keyPressEvent` ```python
-keyPressEvent(event: PySide6.QtGui.QKeyEvent) ``` --- _This file was
-automatically generated via [lazydocs](https://github.com/ml-tooling/
-lazydocs)._
+`extras.code_editor.code_line` **Global Variables** --------------- -
+**TYPE_CHECKING** - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** ---
+[https://img.shields.io/badge/-source-cccccc?style=flat-square] ## class
+`CodeLine` [https://img.shields.io/badge/-source-cccccc?style=flat-square] ###
+method `CodeLine.__init__` ```python __init__(*args, **kwargs) ``` --- [https:/
+/img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`CodeLine.keyPressEvent` ```python keyPressEvent(event:
+PySide2.QtGui.QKeyEvent) ``` --- _This file was automatically generated via
+[lazydocs](https://github.com/ml-tooling/lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/extras.code_editor.highlighters.python.md` & `qtstrap-0.4.2/docs/api/extras.code_editor.highlighters.python.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # <kbd>module</kbd> `extras.code_editor.highlighters.python`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 - **STYLES**
 
 ---
@@ -26,22 +27,35 @@
 ```
 
 Return a QTextCharFormat with the given attributes. 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L39"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L43"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+## <kbd>function</kbd> `get_style`
+
+```python
+get_style(kind)
+```
+
 
-## <kbd>class</kbd> `PythonHighlighter`
 
 
 
 
-<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L70"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+---
+
+<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L47"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+## <kbd>class</kbd> `PythonHighlighter`
+Syntax highlighter for the Python language. 
+
+<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L98"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PythonHighlighter.__init__`
 
 ```python
 __init__(document)
 ```
 
@@ -50,29 +64,41 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L113"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L108"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `PythonHighlighter.highlightBlock`
+### <kbd>method</kbd> `PythonHighlighter.build_rules`
 
 ```python
-highlightBlock(text)
+build_rules()
 ```
 
-Apply syntax highlighting to the given block of text.  
 
 
 
+
+---
+
+<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L137"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `PythonHighlighter.highlightBlock`
+
+```python
+highlightBlock(text)
+```
+
+Apply syntax highlighting to the given block of text. 
+
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L131"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L156"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PythonHighlighter.match_multiline`
 
 ```python
 match_multiline(text, delimiter, in_state, style)
 ```
```

#### html2text {}

```diff
@@ -1,20 +1,25 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
 `extras.code_editor.highlighters.python` **Global Variables** --------------- -
-**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** - **STYLES** --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ## function `format`
-```python format(color, style='') ``` Return a QTextCharFormat with the given
-attributes. --- [https://img.shields.io/badge/-source-cccccc?style=flat-square]
-## class `PythonHighlighter` [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `PythonHighlighter.__init__` ```python
-__init__(document) ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `PythonHighlighter.highlightBlock`
-```python highlightBlock(text) ``` Apply syntax highlighting to the given block
-of text. --- [https://img.shields.io/badge/-source-cccccc?style=flat-square]
-### method `PythonHighlighter.match_multiline` ```python match_multiline(text,
-delimiter, in_state, style) ``` Do highlighting of multi-line strings.
-``delimiter`` should be a ``QRegularExpression`` for triple-single-quotes or
-triple-double-quotes, and ``in_state`` should be a unique integer to represent
-the corresponding state changes when inside those strings. Returns True if
-we're still inside a multi-line string when this function is finished. --
-- _This file was automatically generated via [lazydocs](https://github.com/ml-
-tooling/lazydocs)._
+**TYPE_CHECKING** - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** -
+**STYLES** --- [https://img.shields.io/badge/-source-cccccc?style=flat-square]
+## function `format` ```python format(color, style='') ``` Return a
+QTextCharFormat with the given attributes. --- [https://img.shields.io/badge/-
+source-cccccc?style=flat-square] ## function `get_style` ```python get_style
+(kind) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square]
+## class `PythonHighlighter` Syntax highlighter for the Python language.
+[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`PythonHighlighter.__init__` ```python __init__(document) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`PythonHighlighter.build_rules` ```python build_rules() ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`PythonHighlighter.highlightBlock` ```python highlightBlock(text) ``` Apply
+syntax highlighting to the given block of text. --- [https://img.shields.io/
+badge/-source-cccccc?style=flat-square] ### method
+`PythonHighlighter.match_multiline` ```python match_multiline(text, delimiter,
+in_state, style) ``` Do highlighting of multi-line strings. ``delimiter``
+should be a ``QRegularExpression`` for triple-single-quotes or triple-double-
+quotes, and ``in_state`` should be a unique integer to represent the
+corresponding state changes when inside those strings. Returns True if we're
+still inside a multi-line string when this function is finished. --- _This file
+was automatically generated via [lazydocs](https://github.com/ml-tooling/
+lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/extras.command_palette.command_palette.md` & `qtstrap-0.4.2/docs/api/extras.command_palette.command_palette.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,45 +5,47 @@
 # <kbd>module</kbd> `extras.command_palette.command_palette`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
+- **COMMAND_PALETTE_COLORS**
 - **registry**
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L312"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L26"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>function</kbd> `CommandPalette`
+## <kbd>function</kbd> `get_color`
 
 ```python
-CommandPalette(parent=None)
+get_color(key)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L6"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L30"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `CommandRegistry`
 
 
 
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L7"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L31"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandRegistry.__init__`
 
 ```python
 __init__() → None
 ```
 
@@ -52,51 +54,51 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L16"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L40"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandRegistry.execute`
 
 ```python
 execute(command_name)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L11"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L35"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandRegistry.register_command`
 
 ```python
 register_command(command)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L23"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L47"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `Command`
 
 
 
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L24"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L48"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `Command.__init__`
 
 ```python
 __init__(*args, **kwargs)
 ```
 
@@ -105,37 +107,37 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L32"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L56"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `Command.used`
 
 ```python
 used()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L36"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L60"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PopupDelegate`
 
 
 
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L37"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L61"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PopupDelegate.__init__`
 
 ```python
 __init__(parent=None)
 ```
 
@@ -144,124 +146,138 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L47"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L65"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `PopupDelegate.get_colors`
+
+```python
+get_colors()
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L75"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PopupDelegate.paint`
 
 ```python
 paint(
-    painter: PySide6.QtGui.QPainter,
-    option: PySide6.QtWidgets.QStyleOptionViewItem,
-    index: PySide6.QtCore.QModelIndex
+    painter: PySide2.QtGui.QPainter,
+    option: PySide2.QtWidgets.QStyleOptionViewItem,
+    index: PySide2.QtCore.QModelIndex
 )
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L44"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L72"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PopupDelegate.set_prefix`
 
 ```python
 set_prefix(prefix)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L105"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L143"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `CommandModel`
 
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L117"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L155"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandModel.data`
 
 ```python
-data(index: PySide6.QtCore.QModelIndex, role: int) → Any
+data(index: PySide2.QtCore.QModelIndex, role: int) → Any
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L127"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L165"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandModel.index`
 
 ```python
-index(row: int, column: int, parent: PySide6.QtCore.QModelIndex) → QModelIndex
+index(row: int, column: int, parent: PySide2.QtCore.QModelIndex) → QModelIndex
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L114"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L152"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandModel.rowCount`
 
 ```python
-rowCount(parent: PySide6.QtCore.QModelIndex) → int
+rowCount(parent: PySide2.QtCore.QModelIndex) → int
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L108"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L146"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandModel.sort_commands`
 
 ```python
 sort_commands(prefix)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L131"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L169"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `CommandCompleter`
 
 
 
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L132"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L170"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.__init__`
 
 ```python
 __init__(parent=None)
 ```
 
@@ -270,85 +286,99 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L158"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L200"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.close`
 
 ```python
 close()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L189"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L231"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.get_selection`
 
 ```python
 get_selection()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L182"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L224"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.move_selection_down`
 
 ```python
 move_selection_down()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L175"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L217"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.move_selection_up`
 
 ```python
 move_selection_up()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L153"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L195"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.open`
 
 ```python
 open()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L163"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L192"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `CommandCompleter.reset`
+
+```python
+reset()
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L205"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.update_prefix`
 
 ```python
 update_prefix(prefix)
 ```
```

#### html2text {}

```diff
@@ -1,40 +1,42 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
 `extras.command_palette.command_palette` **Global Variables** --------------- -
-**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** - **registry** --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ## function
-`CommandPalette` ```python CommandPalette(parent=None) ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ## class
-`CommandRegistry` [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `CommandRegistry.__init__` ```python __init__() â None ```
---- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`CommandRegistry.execute` ```python execute(command_name) ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`CommandRegistry.register_command` ```python register_command(command) ``` ---
+**TYPE_CHECKING** - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** -
+**COMMAND_PALETTE_COLORS** - **registry** --- [https://img.shields.io/badge/-
+source-cccccc?style=flat-square] ## function `get_color` ```python get_color
+(key) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square]
+## class `CommandRegistry` [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `CommandRegistry.__init__` ```python
+__init__() â None ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `CommandRegistry.execute` ```python
+execute(command_name) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `CommandRegistry.register_command`
+```python register_command(command) ``` --- [https://img.shields.io/badge/-
+source-cccccc?style=flat-square] ## class `Command` [https://img.shields.io/
+badge/-source-cccccc?style=flat-square] ### method `Command.__init__` ```python
+__init__(*args, **kwargs) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `Command.used` ```python used() ``` ---
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ## class
-`Command` [https://img.shields.io/badge/-source-cccccc?style=flat-square] ###
-method `Command.__init__` ```python __init__(*args, **kwargs) ``` --- [https://
+`PopupDelegate` [https://img.shields.io/badge/-source-cccccc?style=flat-square]
+### method `PopupDelegate.__init__` ```python __init__(parent=None) ``` ---
+[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`PopupDelegate.get_colors` ```python get_colors() ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`Command.used` ```python used() ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ## class `PopupDelegate` [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ### method `PopupDelegate.__init__`
-```python __init__(parent=None) ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `PopupDelegate.paint` ```python paint
-( painter: PySide6.QtGui.QPainter, option:
-PySide6.QtWidgets.QStyleOptionViewItem, index: PySide6.QtCore.QModelIndex ) ```
+`PopupDelegate.paint` ```python paint( painter: PySide2.QtGui.QPainter, option:
+PySide2.QtWidgets.QStyleOptionViewItem, index: PySide2.QtCore.QModelIndex ) ```
 --- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `PopupDelegate.set_prefix` ```python set_prefix(prefix) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ## class `CommandModel`
 --- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`CommandModel.data` ```python data(index: PySide6.QtCore.QModelIndex, role:
+`CommandModel.data` ```python data(index: PySide2.QtCore.QModelIndex, role:
 int) â Any ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
 square] ### method `CommandModel.index` ```python index(row: int, column: int,
-parent: PySide6.QtCore.QModelIndex) â QModelIndex ``` --- [https://
+parent: PySide2.QtCore.QModelIndex) â QModelIndex ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`CommandModel.rowCount` ```python rowCount(parent: PySide6.QtCore.QModelIndex)
+`CommandModel.rowCount` ```python rowCount(parent: PySide2.QtCore.QModelIndex)
 â int ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square]
 ### method `CommandModel.sort_commands` ```python sort_commands(prefix) ``` --
 - [https://img.shields.io/badge/-source-cccccc?style=flat-square] ## class
 `CommandCompleter` [https://img.shields.io/badge/-source-cccccc?style=flat-
 square] ### method `CommandCompleter.__init__` ```python __init__(parent=None)
 ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ###
 method `CommandCompleter.close` ```python close() ``` --- [https://
@@ -42,10 +44,12 @@
 `CommandCompleter.get_selection` ```python get_selection() ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CommandCompleter.move_selection_down` ```python move_selection_down() ``` ---
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CommandCompleter.move_selection_up` ```python move_selection_up() ``` ---
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CommandCompleter.open` ```python open() ``` --- [https://img.shields.io/badge/
--source-cccccc?style=flat-square] ### method `CommandCompleter.update_prefix`
-```python update_prefix(prefix) ``` --- _This file was automatically generated
-via [lazydocs](https://github.com/ml-tooling/lazydocs)._
+-source-cccccc?style=flat-square] ### method `CommandCompleter.reset` ```python
+reset() ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square]
+### method `CommandCompleter.update_prefix` ```python update_prefix(prefix) ```
+--- _This file was automatically generated via [lazydocs](https://github.com/
+ml-tooling/lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/extras.log_monitor.log_database_handler.md` & `qtstrap-0.4.2/docs/api/extras.log_monitor.log_database_handler.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # <kbd>module</kbd> `extras.log_monitor.log_database_handler`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 - **db_conn_name**
 - **initial_sql**
 - **insertion_sql**
@@ -76,29 +77,29 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_database_handler.py#L96"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_database_handler.py#L103"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>classmethod</kbd> `DatabaseHandler.register_callback`
 
 ```python
 register_callback(cb)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_database_handler.py#L100"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_database_handler.py#L107"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `DatabaseHandler.write`
 
 ```python
 write(m)
 ```
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
 `extras.log_monitor.log_database_handler` **Global Variables** --------------
-- - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** - **db_conn_name** -
-**initial_sql** - **insertion_sql** --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ## class `DatabaseHandler` [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ### method `DatabaseHandler.__init__`
-```python __init__(database_name) ``` --- #### property DatabaseHandler.name --
-- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`DatabaseHandler.emit` ```python emit(record) ``` --- [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ### method
-`DatabaseHandler.format_time` ```python format_time(record) ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### classmethod
-`DatabaseHandler.register_callback` ```python register_callback(cb) ``` ---
-[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`DatabaseHandler.write` ```python write(m) ``` --- _This file was automatically
-generated via [lazydocs](https://github.com/ml-tooling/lazydocs)._
+- - **TYPE_CHECKING** - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** -
+**db_conn_name** - **initial_sql** - **insertion_sql** --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ## class
+`DatabaseHandler` [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `DatabaseHandler.__init__` ```python __init__(database_name)
+``` --- #### property DatabaseHandler.name --- [https://img.shields.io/badge/-
+source-cccccc?style=flat-square] ### method `DatabaseHandler.emit` ```python
+emit(record) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `DatabaseHandler.format_time` ```python format_time(record)
+``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ###
+classmethod `DatabaseHandler.register_callback` ```python register_callback(cb)
+``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ###
+method `DatabaseHandler.write` ```python write(m) ``` --- _This file was
+automatically generated via [lazydocs](https://github.com/ml-tooling/
+lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/extras.log_monitor.log_filter_controls.md` & `qtstrap-0.4.2/docs/api/extras.log_monitor.log_filter_controls.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,59 +5,73 @@
 # <kbd>module</kbd> `extras.log_monitor.log_filter_controls`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
-- **log_levels**
-- **level_map**
+- **LOG_FILTER_COLORS**
+
+---
+
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L31"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+## <kbd>function</kbd> `get_color`
+
+```python
+get_color(key)
+```
+
+
+
+
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L23"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L35"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LoggerDelegate`
 
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L24"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L36"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerDelegate.paint`
 
 ```python
 paint(painter, option, index)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L50"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L62"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LoggerTreeWidgetItem`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L51"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L63"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidgetItem.__init__`
 
 ```python
 __init__(parent, name, full_name)
 ```
 
@@ -66,107 +80,107 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L69"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L81"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidgetItem.clicked`
 
 ```python
 clicked(column)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L83"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L95"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidgetItem.double_clicked`
 
 ```python
 double_clicked(column)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L111"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L123"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidgetItem.get_levels`
 
 ```python
 get_levels()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L114"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L126"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidgetItem.set_all_levels`
 
 ```python
 set_all_levels(state: bool)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L104"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L116"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidgetItem.set_levels`
 
 ```python
 set_levels(level_filter=[])
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L98"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L110"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidgetItem.update_data`
 
 ```python
 update_data()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L120"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L132"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LoggerTreeWidget`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L123"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L135"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.__init__`
 
 ```python
 __init__()
 ```
 
@@ -175,233 +189,233 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L157"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L168"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.click`
 
 ```python
 click(item, column)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L197"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L204"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.contextMenuEvent`
 
 ```python
 contextMenuEvent(event)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L252"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L259"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.deselect_all`
 
 ```python
 deselect_all()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L227"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L234"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.disable_all_levels`
 
 ```python
 disable_all_levels(pos)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L219"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L226"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.disable_everything`
 
 ```python
 disable_everything()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L161"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L172"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.double_click`
 
 ```python
 double_click(item, column)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L223"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L230"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.enable_all_levels`
 
 ```python
 enable_all_levels(pos)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L215"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L222"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.enable_everything`
 
 ```python
 enable_everything()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L169"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L180"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.register_logger`
 
 ```python
 register_logger(full_name)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L189"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L200"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.register_loggers`
 
 ```python
 register_loggers(loggers)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L244"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L251"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.select_all`
 
 ```python
 select_all()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L256"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L263"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.select_only`
 
 ```python
 select_only(pos)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L165"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L176"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.selection_changed`
 
 ```python
 selection_changed()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L209"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L216"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.set_levels_of_children`
 
 ```python
 set_levels_of_children(item, state)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L231"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L238"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.set_visible_loggers`
 
 ```python
 set_visible_loggers(visible_loggers)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L262"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L269"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `ProfileSelector`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L267"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L274"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ProfileSelector.__init__`
 
 ```python
 __init__()
 ```
 
@@ -410,152 +424,194 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L305"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L297"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `ProfileSelector.eventFilter`
+
+```python
+eventFilter(source, event)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L319"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ProfileSelector.on_accept`
 
 ```python
 on_accept()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L298"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L314"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ProfileSelector.on_add`
 
 ```python
 on_add()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L294"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L328"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `ProfileSelector.on_cancel`
+
+```python
+on_cancel()
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L310"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ProfileSelector.on_change`
 
 ```python
 on_change()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L316"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L333"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ProfileSelector.on_remove`
 
 ```python
 on_remove()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L321"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L338"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `FilterControls`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L344"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L359"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `FilterControls.__init__`
 
 ```python
-__init__()
+__init__(table)
 ```
 
 
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L427"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L446"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `FilterControls.add_profile`
 
 ```python
 add_profile(name)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L440"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L459"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `FilterControls.change_profile`
 
 ```python
 change_profile(profile_name)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L433"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L467"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `FilterControls.columns_changed`
+
+```python
+columns_changed()
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L452"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `FilterControls.remove_profile`
 
 ```python
 remove_profile(name)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L424"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L442"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `FilterControls.save_settings`
 
 ```python
 save_settings()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L448"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L471"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `FilterControls.update_filter`
 
 ```python
 update_filter()
 ```
```

#### html2text {}

```diff
@@ -1,81 +1,89 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
 `extras.log_monitor.log_filter_controls` **Global Variables** --------------- -
-**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** - **log_levels** -
-**level_map** --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ## class `LoggerDelegate` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `LoggerDelegate.paint` ```python paint
-(painter, option, index) ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ## class `LoggerTreeWidgetItem` [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidgetItem.__init__` ```python __init__(parent, name, full_name) ```
---- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidgetItem.clicked` ```python clicked(column) ``` --- [https://
+**TYPE_CHECKING** - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** -
+**LOG_FILTER_COLORS** --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ## function `get_color` ```python get_color(key) ```
+--- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ## class
+`LoggerDelegate` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `LoggerDelegate.paint` ```python paint(painter, option,
+index) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square]
+## class `LoggerTreeWidgetItem` [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LoggerTreeWidgetItem.__init__` ```python
+__init__(parent, name, full_name) ``` --- [https://img.shields.io/badge/-
+source-cccccc?style=flat-square] ### method `LoggerTreeWidgetItem.clicked`
+```python clicked(column) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LoggerTreeWidgetItem.double_clicked`
+```python double_clicked(column) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LoggerTreeWidgetItem.get_levels`
+```python get_levels() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LoggerTreeWidgetItem.set_all_levels`
+```python set_all_levels(state: bool) ``` --- [https://img.shields.io/badge/-
+source-cccccc?style=flat-square] ### method `LoggerTreeWidgetItem.set_levels`
+```python set_levels(level_filter=[]) ``` --- [https://img.shields.io/badge/-
+source-cccccc?style=flat-square] ### method `LoggerTreeWidgetItem.update_data`
+```python update_data() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ## class `LoggerTreeWidget` [https://img.shields.io/
+badge/-source-cccccc?style=flat-square] ### method `LoggerTreeWidget.__init__`
+```python __init__() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LoggerTreeWidget.click` ```python click
+(item, column) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `LoggerTreeWidget.contextMenuEvent` ```python
+contextMenuEvent(event) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LoggerTreeWidget.deselect_all` ```python
+deselect_all() ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `LoggerTreeWidget.disable_all_levels` ```python
+disable_all_levels(pos) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LoggerTreeWidget.disable_everything`
+```python disable_everything() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LoggerTreeWidget.double_click` ```python
+double_click(item, column) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LoggerTreeWidget.enable_all_levels`
+```python enable_all_levels(pos) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LoggerTreeWidget.enable_everything`
+```python enable_everything() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LoggerTreeWidget.register_logger`
+```python register_logger(full_name) ``` --- [https://img.shields.io/badge/-
+source-cccccc?style=flat-square] ### method `LoggerTreeWidget.register_loggers`
+```python register_loggers(loggers) ``` --- [https://img.shields.io/badge/-
+source-cccccc?style=flat-square] ### method `LoggerTreeWidget.select_all`
+```python select_all() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LoggerTreeWidget.select_only` ```python
+select_only(pos) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LoggerTreeWidget.selection_changed`
+```python selection_changed() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LoggerTreeWidget.set_levels_of_children`
+```python set_levels_of_children(item, state) ``` --- [https://img.shields.io/
+badge/-source-cccccc?style=flat-square] ### method
+`LoggerTreeWidget.set_visible_loggers` ```python set_visible_loggers
+(visible_loggers) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ## class `ProfileSelector` [https://img.shields.io/
+badge/-source-cccccc?style=flat-square] ### method `ProfileSelector.__init__`
+```python __init__() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `ProfileSelector.eventFilter` ```python
+eventFilter(source, event) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `ProfileSelector.on_accept` ```python
+on_accept() ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `ProfileSelector.on_add` ```python on_add() ``` --- [https:/
+/img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`ProfileSelector.on_cancel` ```python on_cancel() ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidgetItem.double_clicked` ```python double_clicked(column) ``` ---
-[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidgetItem.get_levels` ```python get_levels() ``` --- [https://
+`ProfileSelector.on_change` ```python on_change() ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidgetItem.set_all_levels` ```python set_all_levels(state: bool) ```
---- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidgetItem.set_levels` ```python set_levels(level_filter=[]) ``` --
-- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidgetItem.update_data` ```python update_data() ``` --- [https://
+`ProfileSelector.on_remove` ```python on_remove() ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ## class
-`LoggerTreeWidget` [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `LoggerTreeWidget.__init__` ```python __init__() ``` ---
-[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidget.click` ```python click(item, column) ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidget.contextMenuEvent` ```python contextMenuEvent(event) ``` ---
-[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidget.deselect_all` ```python deselect_all() ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidget.disable_all_levels` ```python disable_all_levels(pos) ``` --
-- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidget.disable_everything` ```python disable_everything() ``` ---
-[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidget.double_click` ```python double_click(item, column) ``` ---
+`FilterControls` [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `FilterControls.__init__` ```python __init__(table) ``` ---
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidget.enable_all_levels` ```python enable_all_levels(pos) ``` ---
-[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidget.enable_everything` ```python enable_everything() ``` ---
-[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidget.register_logger` ```python register_logger(full_name) ``` --
-- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidget.register_loggers` ```python register_loggers(loggers) ``` --
-- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidget.select_all` ```python select_all() ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidget.select_only` ```python select_only(pos) ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidget.selection_changed` ```python selection_changed() ``` ---
-[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LoggerTreeWidget.set_levels_of_children` ```python set_levels_of_children
-(item, state) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `LoggerTreeWidget.set_visible_loggers` ```python
-set_visible_loggers(visible_loggers) ``` --- [https://img.shields.io/badge/-
-source-cccccc?style=flat-square] ## class `ProfileSelector` [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`ProfileSelector.__init__` ```python __init__() ``` --- [https://
+`FilterControls.add_profile` ```python add_profile(name) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`ProfileSelector.on_accept` ```python on_accept() ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`ProfileSelector.on_add` ```python on_add() ``` --- [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ### method `ProfileSelector.on_change`
-```python on_change() ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `ProfileSelector.on_remove` ```python
-on_remove() ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ## class `FilterControls` [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `FilterControls.__init__` ```python
-__init__() ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `FilterControls.add_profile` ```python add_profile(name) ```
---- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `FilterControls.change_profile` ```python change_profile(profile_name) ``` ---
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`FilterControls.columns_changed` ```python columns_changed() ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `FilterControls.remove_profile` ```python remove_profile(name) ``` --- [https:/
 /img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `FilterControls.save_settings` ```python save_settings() ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `FilterControls.update_filter` ```python update_filter() ``` --- _This file was
 automatically generated via [lazydocs](https://github.com/ml-tooling/
 lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/extras.log_monitor.log_profile.md` & `qtstrap-0.4.2/docs/api/extras.log_monitor.log_profile.md`

 * *Files 15% similar despite different names*

```diff
@@ -23,102 +23,152 @@
 
 
 <a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L8"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `Column.__init__`
 
 ```python
-__init__(name=None, title=None, visible=True, width=50)
+__init__(title=None, query=None, visible=True, width=0)
 ```
 
 
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L14"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L23"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `Column.get_data`
+
+```python
+get_data()
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L19"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `Column.set_data`
+
+```python
+set_data(data)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L16"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `Column.set_visibility`
 
 ```python
 set_visibility(visible)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L35"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L54"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LogProfile`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L36"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L55"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogProfile.__init__`
 
 ```python
 __init__()
 ```
 
 
 
 
 
 
 ---
 
+#### <kbd>property</kbd> LogProfile.column_data
+
+
+
+
+
+---
+
 #### <kbd>property</kbd> LogProfile.visible_columns
 
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L61"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L88"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogProfile.build_query`
 
 ```python
-build_query()
+build_query(row_count)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L51"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L74"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogProfile.get_log_level_column`
 
 ```python
 get_log_level_column()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L54"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L84"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `LogProfile.set_columns`
+
+```python
+set_columns(column_data)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\extras\log_monitor\log_profile.py#L77"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogProfile.set_filter`
 
 ```python
 set_filter(filt)
 ```
```

#### html2text {}

```diff
@@ -1,19 +1,25 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
 `extras.log_monitor.log_profile` **Global Variables** --------------- -
 **session_start_time** - **default_columns** --- [https://img.shields.io/badge/
 -source-cccccc?style=flat-square] ## class `Column` [https://img.shields.io/
 badge/-source-cccccc?style=flat-square] ### method `Column.__init__` ```python
-__init__(name=None, title=None, visible=True, width=50) ``` --- [https://
+__init__(title=None, query=None, visible=True, width=0) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`Column.set_visibility` ```python set_visibility(visible) ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ## class `LogProfile`
+`Column.get_data` ```python get_data() ``` --- [https://img.shields.io/badge/-
+source-cccccc?style=flat-square] ### method `Column.set_data` ```python
+set_data(data) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `Column.set_visibility` ```python set_visibility(visible)
+``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ##
+class `LogProfile` [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `LogProfile.__init__` ```python __init__() ``` --- ####
+property LogProfile.column_data --- #### property LogProfile.visible_columns --
+- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`LogProfile.build_query` ```python build_query(row_count) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`LogProfile.get_log_level_column` ```python get_log_level_column() ``` ---
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LogProfile.__init__` ```python __init__() ``` --- #### property
-LogProfile.visible_columns --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `LogProfile.build_query` ```python
-build_query() ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `LogProfile.get_log_level_column` ```python
-get_log_level_column() ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `LogProfile.set_filter` ```python
-set_filter(filt) ``` --- _This file was automatically generated via [lazydocs]
-(https://github.com/ml-tooling/lazydocs)._
+`LogProfile.set_columns` ```python set_columns(column_data) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`LogProfile.set_filter` ```python set_filter(filt) ``` --- _This file was
+automatically generated via [lazydocs](https://github.com/ml-tooling/
+lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/extras.log_monitor.log_table_view.md` & `qtstrap-0.4.2/docs/api/extras.log_monitor.log_table_view.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 # <kbd>module</kbd> `extras.log_monitor.log_table_view`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
-- **log_levels**
-- **default_columns**
 - **db_conn_name**
 - **session_start_time**
 
 
 ---
 
 <a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L12"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
@@ -46,15 +45,15 @@
 ---
 
 <a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L17"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogDbModel.data`
 
 ```python
-data(index, role=PySide6.QtCore.Qt.ItemDataRole.DisplayRole)
+data(index, role=PySide2.QtCore.Qt.ItemDataRole.DisplayRole)
 ```
 
 
 
 
 
 
@@ -63,15 +62,15 @@
 <a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L30"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LogTableView`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L31"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L33"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogTableView.__init__`
 
 ```python
 __init__()
 ```
 
@@ -80,99 +79,113 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L55"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L56"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogTableView.attempt_refresh`
 
 ```python
 attempt_refresh()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L83"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L93"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogTableView.eventFilter`
 
 ```python
 eventFilter(object, event)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L94"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L106"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogTableView.header_menu`
 
 ```python
 header_menu()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L89"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L99"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogTableView.mouse_released`
 
 ```python
 mouse_released()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L68"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L72"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogTableView.refresh`
 
 ```python
 refresh()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L61"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L62"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogTableView.schedule_refresh`
 
 ```python
 schedule_refresh()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L64"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L69"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `LogTableView.set_columns`
+
+```python
+set_columns(columns)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\extras\log_monitor\log_table_view.py#L65"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogTableView.set_filter`
 
 ```python
 set_filter(filt)
 ```
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
 `extras.log_monitor.log_table_view` **Global Variables** --------------- -
-**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** - **log_levels** -
-**default_columns** - **db_conn_name** - **session_start_time** --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ## class `LogDbModel`
-[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LogDbModel.__init__` ```python __init__(parent=None) ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LogDbModel.data` ```python data(index,
-role=PySide6.QtCore.Qt.ItemDataRole.DisplayRole) ``` --- [https://
+**TYPE_CHECKING** - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** -
+**db_conn_name** - **session_start_time** --- [https://img.shields.io/badge/-
+source-cccccc?style=flat-square] ## class `LogDbModel` [https://img.shields.io/
+badge/-source-cccccc?style=flat-square] ### method `LogDbModel.__init__`
+```python __init__(parent=None) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LogDbModel.data` ```python data(index,
+role=PySide2.QtCore.Qt.ItemDataRole.DisplayRole) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ## class `LogTableView`
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `LogTableView.__init__` ```python __init__() ``` --- [https://img.shields.io/
 badge/-source-cccccc?style=flat-square] ### method
 `LogTableView.attempt_refresh` ```python attempt_refresh() ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `LogTableView.eventFilter` ```python eventFilter(object, event) ``` --- [https:
@@ -20,10 +19,12 @@
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `LogTableView.mouse_released` ```python mouse_released() ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `LogTableView.refresh` ```python refresh() ``` --- [https://img.shields.io/
 badge/-source-cccccc?style=flat-square] ### method
 `LogTableView.schedule_refresh` ```python schedule_refresh() ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`LogTableView.set_columns` ```python set_columns(columns) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `LogTableView.set_filter` ```python set_filter(filt) ``` --- _This file was
 automatically generated via [lazydocs](https://github.com/ml-tooling/
 lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/extras.log_monitor.log_widget.md` & `qtstrap-0.4.2/docs/api/extras.log_monitor.log_widget.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 # <kbd>module</kbd> `extras.log_monitor.log_widget`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 - **db_conn_name**
 - **command_palette_available**
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L15"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L16"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LogMonitorWidget`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L16"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L17"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorWidget.__init__`
 
 ```python
 __init__(parent=None)
 ```
 
@@ -53,135 +54,149 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L51"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L50"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorWidget.query_existing_loggers`
 
 ```python
 query_existing_loggers()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L60"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L59"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LogMonitorDockWidget`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L61"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L60"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDockWidget.__init__`
 
 ```python
-__init__(parent=None)
+__init__(parent=None, shortcut='Ctrl+L')
 ```
 
 
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L83"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L84"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDockWidget.adjust_size`
 
 ```python
 adjust_size()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L87"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L88"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDockWidget.toggleViewAction`
 
 ```python
 toggleViewAction()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L93"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L94"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LogMonitorDropdown`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L94"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L95"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDropdown.__init__`
 
 ```python
-__init__(parent=None)
+__init__(parent=None, shortcut='`')
 ```
 
 
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L122"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L136"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDropdown.center_on_parent`
 
 ```python
 center_on_parent()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L109"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L114"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `LogMonitorDropdown.eventFilter`
+
+```python
+eventFilter(source: PySide2.QtCore.QObject, event: PySide2.QtCore.QEvent) → bool
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L123"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDropdown.toggleViewAction`
 
 ```python
 toggleViewAction()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L115"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L129"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDropdown.toggle_view`
 
 ```python
 toggle_view()
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,29 +1,33 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
 `extras.log_monitor.log_widget` **Global Variables** --------------- -
-**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** - **db_conn_name** -
-**command_palette_available** --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ## class `LogMonitorWidget` [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ### method `LogMonitorWidget.__init__`
-```python __init__(parent=None) ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `LogMonitorWidget.open_profile_prompt`
-```python open_profile_prompt() ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `LogMonitorWidget.query_existing_loggers`
-```python query_existing_loggers() ``` --- [https://img.shields.io/badge/-
-source-cccccc?style=flat-square] ## class `LogMonitorDockWidget` [https://
+**TYPE_CHECKING** - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** -
+**db_conn_name** - **command_palette_available** --- [https://img.shields.io/
+badge/-source-cccccc?style=flat-square] ## class `LogMonitorWidget` [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LogMonitorDockWidget.__init__` ```python __init__(parent=None) ``` --- [https:
-//img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LogMonitorDockWidget.adjust_size` ```python adjust_size() ``` --- [https://
+`LogMonitorWidget.__init__` ```python __init__(parent=None) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LogMonitorDockWidget.toggleViewAction` ```python toggleViewAction() ``` ---
-[https://img.shields.io/badge/-source-cccccc?style=flat-square] ## class
-`LogMonitorDropdown` [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `LogMonitorDropdown.__init__` ```python __init__
-(parent=None) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `LogMonitorDropdown.center_on_parent` ```python
-center_on_parent() ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `LogMonitorDropdown.toggleViewAction`
+`LogMonitorWidget.open_profile_prompt` ```python open_profile_prompt() ``` ---
+[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`LogMonitorWidget.query_existing_loggers` ```python query_existing_loggers()
+``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ##
+class `LogMonitorDockWidget` [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LogMonitorDockWidget.__init__` ```python
+__init__(parent=None, shortcut='Ctrl+L') ``` --- [https://img.shields.io/badge/
+-source-cccccc?style=flat-square] ### method `LogMonitorDockWidget.adjust_size`
+```python adjust_size() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LogMonitorDockWidget.toggleViewAction`
 ```python toggleViewAction() ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `LogMonitorDropdown.toggle_view` ```python
-toggle_view() ``` --- _This file was automatically generated via [lazydocs]
-(https://github.com/ml-tooling/lazydocs)._
+cccccc?style=flat-square] ## class `LogMonitorDropdown` [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`LogMonitorDropdown.__init__` ```python __init__(parent=None, shortcut='`') ```
+--- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`LogMonitorDropdown.center_on_parent` ```python center_on_parent() ``` ---
+[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`LogMonitorDropdown.eventFilter` ```python eventFilter(source:
+PySide2.QtCore.QObject, event: PySide2.QtCore.QEvent) â bool ``` --- [https:/
+/img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`LogMonitorDropdown.toggleViewAction` ```python toggleViewAction() ``` ---
+[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`LogMonitorDropdown.toggle_view` ```python toggle_view() ``` --- _This file was
+automatically generated via [lazydocs](https://github.com/ml-tooling/
+lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/extras.log_monitor.md` & `qtstrap-0.4.2/docs/api/extras.log_monitor.md`

 * *Files 16% similar despite different names*

```diff
@@ -11,25 +11,24 @@
 ---------------
 - **log_filter_controls**
 - **log_profile**
 - **log_database_handler**
 - **log_table_view**
 - **log_widget**
 - **db_path**
+- **exception_logger_name**
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\__init__.py#L14"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\log_monitor\__init__.py#L12"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `install`
 
 ```python
-install(
-    database_name='C:\\Users\\daelon\\AppData\\Local\\Daelonco\\qtstrap/log.db'
-)
+install(database_name='P:/qtstrap/qtstrap/log.db', install_excepthook=True)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
 `extras.log_monitor` **Global Variables** --------------- -
 **log_filter_controls** - **log_profile** - **log_database_handler** -
-**log_table_view** - **log_widget** - **db_path** --- [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ## function `install` ```python install
-( database_name='C:\\Users\\daelon\\AppData\\Local\\Daelonco\\qtstrap/log.db' )
-``` --- _This file was automatically generated via [lazydocs](https://
-github.com/ml-tooling/lazydocs)._
+**log_table_view** - **log_widget** - **db_path** - **exception_logger_name** -
+-- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ## function
+`install` ```python install(database_name='P:/qtstrap/qtstrap/log.db',
+install_excepthook=True) ``` --- _This file was automatically generated via
+[lazydocs](https://github.com/ml-tooling/lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/extras.style.colors.md` & `qtstrap-0.4.2/docs/api/extras.style.colors.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\style\colors.py#L24"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\extras\style\colors.py#L25"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `qcolors`
```

### Comparing `qtstrap-0.4.1/docs/api/options.md` & `qtstrap-0.4.2/docs/api/options.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/api/overview.md` & `qtstrap-0.4.2/docs/api/overview.md`

 * *Files 17% similar despite different names*

```diff
@@ -17,38 +17,44 @@
 - [`extras.log_monitor.log_filter_controls`](./extras.log_monitor.log_filter_controls.md#module-extraslog_monitorlog_filter_controls)
 - [`extras.log_monitor.log_profile`](./extras.log_monitor.log_profile.md#module-extraslog_monitorlog_profile)
 - [`extras.log_monitor.log_table_view`](./extras.log_monitor.log_table_view.md#module-extraslog_monitorlog_table_view)
 - [`extras.log_monitor.log_widget`](./extras.log_monitor.log_widget.md#module-extraslog_monitorlog_widget)
 - [`extras.style`](./extras.style.md#module-extrasstyle)
 - [`extras.style.colors`](./extras.style.colors.md#module-extrasstylecolors)
 - [`extras.style.dark_palette`](./extras.style.dark_palette.md#module-extrasstyledark_palette)
+- [`extras.style.themes`](./extras.style.themes.md#module-extrasstylethemes)
 - [`options`](./options.md#module-options)
-- [`settings`](./settings.md#module-settings)
 - [`utils`](./utils.md#module-utils)
 - [`utils.adapter`](./utils.adapter.md#module-utilsadapter)
-- [`utils.decorators`](./utils.decorators.md#module-utilsdecorators)
+- [`utils.call_later`](./utils.call_later.md#module-utilscall_later)
 - [`utils.defer`](./utils.defer.md#module-utilsdefer)
+- [`utils.drag_and_drop`](./utils.drag_and_drop.md#module-utilsdrag_and_drop)
+- [`utils.get_ip`](./utils.get_ip.md#module-utilsget_ip)
 - [`utils.signals`](./utils.signals.md#module-utilssignals)
 - [`utils.singleton`](./utils.singleton.md#module-utilssingleton)
+- [`utils.string_builder`](./utils.string_builder.md#module-utilsstring_builder)
 - [`utils.timestamp`](./utils.timestamp.md#module-utilstimestamp)
+- [`utils.trace`](./utils.trace.md#module-utilstrace)
 - [`utils.utils`](./utils.utils.md#module-utilsutils)
 - [`widgets`](./widgets.md#module-widgets)
 - [`widgets.buttons`](./widgets.buttons.md#module-widgetsbuttons)
 - [`widgets.labeledit`](./widgets.labeledit.md#module-widgetslabeledit)
 - [`widgets.layouts`](./widgets.layouts.md#module-widgetslayouts)
 - [`widgets.line_widgets`](./widgets.line_widgets.md#module-widgetsline_widgets)
 - [`widgets.link_label`](./widgets.link_label.md#module-widgetslink_label)
 - [`widgets.persistent_tab_widget`](./widgets.persistent_tab_widget.md#module-widgetspersistent_tab_widget)
 - [`widgets.persistent_widgets`](./widgets.persistent_widgets.md#module-widgetspersistent_widgets)
+- [`widgets.toggle`](./widgets.toggle.md#module-widgetstoggle)
+- [`widgets.toolbar`](./widgets.toolbar.md#module-widgetstoolbar)
 
 ## Classes
 
 - [`code_editor.CodeEditor`](./extras.code_editor.code_editor.md#class-codeeditor)
 - [`code_line.CodeLine`](./extras.code_editor.code_line.md#class-codeline)
-- [`python.PythonHighlighter`](./extras.code_editor.highlighters.python.md#class-pythonhighlighter)
+- [`python.PythonHighlighter`](./extras.code_editor.highlighters.python.md#class-pythonhighlighter): Syntax highlighter for the Python language.
 - [`command_palette.Command`](./extras.command_palette.command_palette.md#class-command)
 - [`command_palette.CommandCompleter`](./extras.command_palette.command_palette.md#class-commandcompleter)
 - [`command_palette.CommandModel`](./extras.command_palette.command_palette.md#class-commandmodel)
 - [`command_palette.CommandRegistry`](./extras.command_palette.command_palette.md#class-commandregistry)
 - [`command_palette.PopupDelegate`](./extras.command_palette.command_palette.md#class-popupdelegate)
 - [`log_database_handler.DatabaseHandler`](./extras.log_monitor.log_database_handler.md#class-databasehandler)
 - [`log_filter_controls.FilterControls`](./extras.log_monitor.log_filter_controls.md#class-filtercontrols)
@@ -62,22 +68,26 @@
 - [`log_table_view.LogTableView`](./extras.log_monitor.log_table_view.md#class-logtableview)
 - [`log_widget.LogMonitorDockWidget`](./extras.log_monitor.log_widget.md#class-logmonitordockwidget)
 - [`log_widget.LogMonitorDropdown`](./extras.log_monitor.log_widget.md#class-logmonitordropdown)
 - [`log_widget.LogMonitorWidget`](./extras.log_monitor.log_widget.md#class-logmonitorwidget)
 - [`colors.colors`](./extras.style.colors.md#class-colors)
 - [`colors.qcolors`](./extras.style.colors.md#class-qcolors)
 - [`options.OPTIONS`](./options.md#class-options)
-- [`adapter.Adapter`](./utils.adapter.md#class-adapter)
+- [`adapter.Adapter`](./utils.adapter.md#class-adapter): A signal adapter that helps create disposable connections between objects. 
 - [`defer.Defer`](./utils.defer.md#class-defer): A context manager that emulates the defer keyword from other languages.
+- [`drag_and_drop.PreviewDrag`](./utils.drag_and_drop.md#class-previewdrag)
 - [`signals.SignalBlocker`](./utils.signals.md#class-signalblocker): A context manager that blocks the signals of the provided widget.
+- [`string_builder.Builder`](./utils.string_builder.md#class-builder): Utility class for incrementally building strings.
 - [`timestamp.TimeStamp`](./utils.timestamp.md#class-timestamp)
 - [`buttons.ConfirmToggleButton`](./widgets.buttons.md#class-confirmtogglebutton)
 - [`buttons.IconToggleButton`](./widgets.buttons.md#class-icontogglebutton)
+- [`buttons.MenuButton`](./widgets.buttons.md#class-menubutton)
 - [`buttons.StateButton`](./widgets.buttons.md#class-statebutton)
 - [`labeledit.LabelEdit`](./widgets.labeledit.md#class-labeledit)
+- [`layouts.CFormLayout`](./widgets.layouts.md#class-cformlayout)
 - [`layouts.CGridLayout`](./widgets.layouts.md#class-cgridlayout)
 - [`layouts.CHBoxLayout`](./widgets.layouts.md#class-chboxlayout)
 - [`layouts.CScrollArea`](./widgets.layouts.md#class-cscrollarea)
 - [`layouts.CSplitter`](./widgets.layouts.md#class-csplitter)
 - [`layouts.CVBoxLayout`](./widgets.layouts.md#class-cvboxlayout)
 - [`layouts.ContextLayout`](./widgets.layouts.md#class-contextlayout)
 - [`layouts.PersistentCScrollArea`](./widgets.layouts.md#class-persistentcscrollarea)
@@ -87,26 +97,41 @@
 - [`link_label.LinkLabel`](./widgets.link_label.md#class-linklabel)
 - [`persistent_tab_widget.PersistentTabWidget`](./widgets.persistent_tab_widget.md#class-persistenttabwidget)
 - [`persistent_widgets.PersistentCheckBox`](./widgets.persistent_widgets.md#class-persistentcheckbox)
 - [`persistent_widgets.PersistentCheckableAction`](./widgets.persistent_widgets.md#class-persistentcheckableaction)
 - [`persistent_widgets.PersistentComboBox`](./widgets.persistent_widgets.md#class-persistentcombobox)
 - [`persistent_widgets.PersistentLineEdit`](./widgets.persistent_widgets.md#class-persistentlineedit)
 - [`persistent_widgets.PersistentListWidget`](./widgets.persistent_widgets.md#class-persistentlistwidget)
+- [`persistent_widgets.PersistentPlainTextEdit`](./widgets.persistent_widgets.md#class-persistentplaintextedit)
 - [`persistent_widgets.PersistentTextEdit`](./widgets.persistent_widgets.md#class-persistenttextedit)
 - [`persistent_widgets.PersistentTreeWidget`](./widgets.persistent_widgets.md#class-persistenttreewidget)
+- [`toggle.AnimatedToggle`](./widgets.toggle.md#class-animatedtoggle)
+- [`toggle.PersistentAnimatedToggle`](./widgets.toggle.md#class-persistentanimatedtoggle)
+- [`toggle.PersistentToggle`](./widgets.toggle.md#class-persistenttoggle)
+- [`toggle.Toggle`](./widgets.toggle.md#class-toggle)
+- [`toolbar.BaseToolbar`](./widgets.toolbar.md#class-basetoolbar)
 
 ## Functions
 
 - [`python.format`](./extras.code_editor.highlighters.python.md#function-format): Return a QTextCharFormat with the given attributes.
-- [`command_palette.CommandPalette`](./extras.command_palette.command_palette.md#function-commandpalette)
+- [`python.get_style`](./extras.code_editor.highlighters.python.md#function-get_style)
+- [`command_palette.get_color`](./extras.command_palette.command_palette.md#function-get_color)
 - [`log_monitor.install`](./extras.log_monitor.md#function-install)
-- [`settings.uncache`](./settings.md#function-uncache): Remove package modules from cache except excluded ones.
-- [`decorators.trace`](./utils.decorators.md#function-trace)
+- [`log_filter_controls.get_color`](./extras.log_monitor.log_filter_controls.md#function-get_color)
+- [`dark_palette.install_dark_palette`](./extras.style.dark_palette.md#function-install_dark_palette)
+- [`themes.apply_theme`](./extras.style.themes.md#function-apply_theme)
+- [`themes.dark`](./extras.style.themes.md#function-dark)
+- [`themes.light`](./extras.style.themes.md#function-light)
+- [`call_later.call_later`](./utils.call_later.md#function-call_later): call the given function after a specified delay
+- [`drag_and_drop.accepts_file_drops`](./utils.drag_and_drop.md#function-accepts_file_drops): Decorator that enables drag-and-drop on a QWidget.
+- [`drag_and_drop.draggable`](./utils.drag_and_drop.md#function-draggable)
+- [`get_ip.get_ip`](./utils.get_ip.md#function-get_ip): Get the current machine's IPv4 address.
 - [`singleton.singleton`](./utils.singleton.md#function-singleton):     
 - [`timestamp.time_since`](./utils.timestamp.md#function-time_since)
+- [`trace.trace`](./utils.trace.md#function-trace)
 - [`utils.disable_children`](./utils.utils.md#function-disable_children): Recursively walk the provided thing and disable all of its widget children.
 - [`utils.enable_children`](./utils.utils.md#function-enable_children): Recursively walk the provided thing and enable all of its widget children.
 - [`utils.get_children`](./utils.utils.md#function-get_children): Recursively visit all the children of the specified object and collect them in a list.
 - [`utils.print_children`](./utils.utils.md#function-print_children): Recursively visit all the children of the specified object and print them.
 - [`utils.set_font_options`](./utils.utils.md#function-set_font_options): Set the QFont options of the specified object.
```

### Comparing `qtstrap-0.4.1/docs/api/settings.md` & `qtstrap-0.4.2/docs/api/settings.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/api/utils.adapter.md` & `qtstrap-0.4.2/docs/api/widgets.toolbar.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,58 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\utils\adapter.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\toolbar.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-# <kbd>module</kbd> `utils.adapter`
+# <kbd>module</kbd> `widgets.toolbar`
 
 
 
 
+**Global Variables**
+---------------
+- **TYPE_CHECKING**
+- **PYQT6**
+- **PYQT5**
+- **PYSIDE2**
+- **PYSIDE6**
+- **location_map**
 
 
 ---
 
-<a href="..\..\qtstrap\utils\adapter.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\toolbar.py#L13"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>class</kbd> `Adapter`
+## <kbd>class</kbd> `BaseToolbar`
 
 
 
 
-<a href="..\..\qtstrap\utils\adapter.py#L18"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\toolbar.py#L14"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `Adapter.__init__`
+### <kbd>method</kbd> `BaseToolbar.__init__`
 
 ```python
-__init__(other=None)
+__init__(parent=None, name=None, location=None, size=40, **kwargs)
 ```
 
 
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\adapter.py#L47"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\toolbar.py#L27"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `Adapter.adapter`
+### <kbd>method</kbd> `BaseToolbar.add_spacer`
 
 ```python
-adapter()
-```
-
-
-
-
-
----
-
-<a href="..\..\qtstrap\utils\adapter.py#L50"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
-
-### <kbd>method</kbd> `Adapter.kill`
-
-```python
-kill()
+add_spacer()
 ```
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
-`utils.adapter` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ## class `Adapter` [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `Adapter.__init__` ```python __init__
-(other=None) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `Adapter.adapter` ```python adapter() ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`Adapter.kill` ```python kill() ``` --- _This file was automatically generated
-via [lazydocs](https://github.com/ml-tooling/lazydocs)._
+`widgets.toolbar` **Global Variables** --------------- - **TYPE_CHECKING** -
+**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** - **location_map** ---
+[https://img.shields.io/badge/-source-cccccc?style=flat-square] ## class
+`BaseToolbar` [https://img.shields.io/badge/-source-cccccc?style=flat-square]
+### method `BaseToolbar.__init__` ```python __init__(parent=None, name=None,
+location=None, size=40, **kwargs) ``` --- [https://img.shields.io/badge/-
+source-cccccc?style=flat-square] ### method `BaseToolbar.add_spacer` ```python
+add_spacer() ``` --- _This file was automatically generated via [lazydocs]
+(https://github.com/ml-tooling/lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/utils.decorators.md` & `qtstrap-0.4.2/docs/api/utils.decorators.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/api/utils.defer.md` & `qtstrap-0.4.2/docs/api/utils.defer.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/api/utils.signals.md` & `qtstrap-0.4.2/docs/api/utils.signals.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\signals.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\utils\signals.py#L3"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `SignalBlocker`
 A context manager that blocks the signals of the provided widget. 
 
 The signals are unblocked at the end of the with block. 
 
-<a href="..\..\qtstrap\utils\signals.py#L9"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\utils\signals.py#L8"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `SignalBlocker.__init__`
 
 ```python
 __init__(widget)
 ```
```

### Comparing `qtstrap-0.4.1/docs/api/utils.singleton.md` & `qtstrap-0.4.2/docs/api/utils.singleton.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/api/utils.timestamp.md` & `qtstrap-0.4.2/docs/api/utils.timestamp.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/api/utils.utils.md` & `qtstrap-0.4.2/docs/api/utils.utils.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,79 +5,80 @@
 # <kbd>module</kbd> `utils.utils`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 ---
 
 <a href="..\..\qtstrap\utils\utils.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `enable_children`
 
 ```python
-enable_children(thing: PySide6.QtCore.QObject) → None
+enable_children(thing: PySide2.QtCore.QObject) → None
 ```
 
 Recursively walk the provided thing and enable all of its widget children. 
 
 
 ---
 
 <a href="..\..\qtstrap\utils\utils.py#L23"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `disable_children`
 
 ```python
-disable_children(thing: PySide6.QtCore.QObject) → None
+disable_children(thing: PySide2.QtCore.QObject) → None
 ```
 
 Recursively walk the provided thing and disable all of its widget children. 
 
 
 ---
 
 <a href="..\..\qtstrap\utils\utils.py#L42"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `get_children`
 
 ```python
-get_children(obj: PySide6.QtCore.QObject) → list
+get_children(obj: PySide2.QtCore.QObject) → list
 ```
 
 Recursively visit all the children of the specified object and collect them in a list. 
 
 
 ---
 
 <a href="..\..\qtstrap\utils\utils.py#L58"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `print_children`
 
 ```python
-print_children(obj: PySide6.QtCore.QObject, prefix='') → None
+print_children(obj: PySide2.QtCore.QObject, prefix='') → None
 ```
 
 Recursively visit all the children of the specified object and print them. 
 
 
 ---
 
 <a href="..\..\qtstrap\utils\utils.py#L67"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `set_font_options`
 
 ```python
-set_font_options(obj: PySide6.QtCore.QObject, options={})
+set_font_options(obj: PySide2.QtCore.QObject, options={})
 ```
 
 Set the QFont options of the specified object. Font options are specified by providing the name of the QFont setter method. 
 
 
 
 **Example:**
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
-`utils.utils` **Global Variables** --------------- - **PYQT6** - **PYQT5** -
-**PYSIDE2** - **PYSIDE6** --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ## function `enable_children` ```python
-enable_children(thing: PySide6.QtCore.QObject) â None ``` Recursively walk
+`utils.utils` **Global Variables** --------------- - **TYPE_CHECKING** -
+**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** --- [https://img.shields.io/
+badge/-source-cccccc?style=flat-square] ## function `enable_children` ```python
+enable_children(thing: PySide2.QtCore.QObject) â None ``` Recursively walk
 the provided thing and enable all of its widget children. --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ## function
-`disable_children` ```python disable_children(thing: PySide6.QtCore.QObject)
+`disable_children` ```python disable_children(thing: PySide2.QtCore.QObject)
 â None ``` Recursively walk the provided thing and disable all of its widget
 children. --- [https://img.shields.io/badge/-source-cccccc?style=flat-square]
-## function `get_children` ```python get_children(obj: PySide6.QtCore.QObject)
+## function `get_children` ```python get_children(obj: PySide2.QtCore.QObject)
 â list ``` Recursively visit all the children of the specified object and
 collect them in a list. --- [https://img.shields.io/badge/-source-
 cccccc?style=flat-square] ## function `print_children` ```python print_children
-(obj: PySide6.QtCore.QObject, prefix='') â None ``` Recursively visit all the
+(obj: PySide2.QtCore.QObject, prefix='') â None ``` Recursively visit all the
 children of the specified object and print them. --- [https://img.shields.io/
 badge/-source-cccccc?style=flat-square] ## function `set_font_options`
-```python set_font_options(obj: PySide6.QtCore.QObject, options={}) ``` Set the
+```python set_font_options(obj: PySide2.QtCore.QObject, options={}) ``` Set the
 QFont options of the specified object. Font options are specified by providing
 the name of the QFont setter method. **Example:** set_font_options(widget,
 {'setPointSize': 12, 'setBold': True}) is equivalent to writing: font =
 widget.font() font.setPointSize(12) font.setBold(True) widget.setFont(font) --
 - _This file was automatically generated via [lazydocs](https://github.com/ml-
 tooling/lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/widgets.buttons.md` & `qtstrap-0.4.2/docs/api/widgets.buttons.md`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # <kbd>module</kbd> `widgets.buttons`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 
 ---
@@ -214,12 +215,51 @@
 ```
 
 
 
 
 
 
+---
+
+<a href="..\..\qtstrap\widgets\buttons.py#L106"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+## <kbd>class</kbd> `MenuButton`
+
+
+
+
+<a href="..\..\qtstrap\widgets\buttons.py#L107"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `MenuButton.__init__`
+
+```python
+__init__(*args, **kwargs)
+```
+
+
+
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\buttons.py#L113"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `MenuButton.addAction`
+
+```python
+addAction(*args, **kwargs)
+```
+
+
+
+
+
+
 
 
 ---
 
 _This file was automatically generated via [lazydocs](https://github.com/ml-tooling/lazydocs)._
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
-`widgets.buttons` **Global Variables** --------------- - **PYQT6** - **PYQT5**
-- **PYSIDE2** - **PYSIDE6** --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ## class `StateButton` [https://img.shields.io/badge/
--source-cccccc?style=flat-square] ### method `StateButton.__init__` ```python
-__init__(*args, **kwargs) ``` --- #### property StateButton.state --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`StateButton.next_state` ```python next_state() ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`StateButton.update_icon` ```python update_icon() ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ## class
+`widgets.buttons` **Global Variables** --------------- - **TYPE_CHECKING** -
+**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** --- [https://img.shields.io/
+badge/-source-cccccc?style=flat-square] ## class `StateButton` [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`StateButton.__init__` ```python __init__(*args, **kwargs) ``` --- ####
+property StateButton.state --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `StateButton.next_state` ```python
+next_state() ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `StateButton.update_icon` ```python update_icon() ``` ---
+[https://img.shields.io/badge/-source-cccccc?style=flat-square] ## class
 `IconToggleButton` [https://img.shields.io/badge/-source-cccccc?style=flat-
 square] ### method `IconToggleButton.__init__` ```python __init__(*args,
 **kwargs) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
 square] ### method `IconToggleButton.update_icon` ```python update_icon() ``` -
 -- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ## class
 `ConfirmToggleButton` [https://img.shields.io/badge/-source-cccccc?style=flat-
 square] ### method `ConfirmToggleButton.__init__` ```python __init__(*args,
@@ -22,10 +22,15 @@
 badge/-source-cccccc?style=flat-square] ### method
 `ConfirmToggleButton.confirm` ```python confirm() ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `ConfirmToggleButton.next_state` ```python next_state() ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `ConfirmToggleButton.uncheck` ```python uncheck() ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`ConfirmToggleButton.update_icon` ```python update_icon() ``` --- _This file
+`ConfirmToggleButton.update_icon` ```python update_icon() ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ## class `MenuButton`
+[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`MenuButton.__init__` ```python __init__(*args, **kwargs) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`MenuButton.addAction` ```python addAction(*args, **kwargs) ``` --- _This file
 was automatically generated via [lazydocs](https://github.com/ml-tooling/
 lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/widgets.labeledit.md` & `qtstrap-0.4.2/docs/api/widgets.labeledit.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # <kbd>module</kbd> `widgets.labeledit`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 
 ---
@@ -84,15 +85,15 @@
 ---
 
 <a href="..\..\qtstrap\widgets\labeledit.py#L34"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LabelEdit.mouseDoubleClickEvent`
 
 ```python
-mouseDoubleClickEvent(event: PySide6.QtGui.QMouseEvent) → None
+mouseDoubleClickEvent(event: PySide2.QtGui.QMouseEvent) → None
 ```
 
 
 
 
 
 ---
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
-`widgets.labeledit` **Global Variables** --------------- - **PYQT6** -
-**PYQT5** - **PYSIDE2** - **PYSIDE6** --- [https://img.shields.io/badge/-
-source-cccccc?style=flat-square] ## class `LabelEdit` [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ### method `LabelEdit.__init__`
-```python __init__(text, *args, changed=None, **kwargs) ``` --- [https://
+`widgets.labeledit` **Global Variables** --------------- - **TYPE_CHECKING** -
+**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** --- [https://img.shields.io/
+badge/-source-cccccc?style=flat-square] ## class `LabelEdit` [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LabelEdit.accept` ```python accept() ``` --- [https://img.shields.io/badge/-
-source-cccccc?style=flat-square] ### method `LabelEdit.dismiss` ```python
-dismiss() ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `LabelEdit.eventFilter` ```python eventFilter(source, event)
+`LabelEdit.__init__` ```python __init__(text, *args, changed=None, **kwargs)
 ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ###
-method `LabelEdit.mouseDoubleClickEvent` ```python mouseDoubleClickEvent(event:
-PySide6.QtGui.QMouseEvent) â None ``` --- [https://img.shields.io/badge/-
-source-cccccc?style=flat-square] ### method `LabelEdit.setText` ```python
-setText(text) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `LabelEdit.start_editing` ```python start_editing() ``` ---
-[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LabelEdit.text` ```python text() ``` --- _This file was automatically
-generated via [lazydocs](https://github.com/ml-tooling/lazydocs)._
+method `LabelEdit.accept` ```python accept() ``` --- [https://img.shields.io/
+badge/-source-cccccc?style=flat-square] ### method `LabelEdit.dismiss`
+```python dismiss() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LabelEdit.eventFilter` ```python
+eventFilter(source, event) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LabelEdit.mouseDoubleClickEvent`
+```python mouseDoubleClickEvent(event: PySide2.QtGui.QMouseEvent) â None ```
+--- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`LabelEdit.setText` ```python setText(text) ``` --- [https://img.shields.io/
+badge/-source-cccccc?style=flat-square] ### method `LabelEdit.start_editing`
+```python start_editing() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `LabelEdit.text` ```python text() ``` --
+- _This file was automatically generated via [lazydocs](https://github.com/ml-
+tooling/lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/widgets.layouts.md` & `qtstrap-0.4.2/docs/api/widgets.layouts.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 # <kbd>module</kbd> `widgets.layouts`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 - **alignments**
 - **orientations**
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L23"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L27"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `ContextLayout`
 
 
 
 
-<a href="..\..\qtstrap\widgets\layouts.py#L24"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L28"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ContextLayout.__init__`
 
 ```python
 __init__(parent=None, stretch=None, margins=None, align=None, **kwargs)
 ```
 
@@ -39,107 +40,121 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L68"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L75"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ContextLayout.add`
 
 ```python
 add(item, *args, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L87"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L98"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `ContextLayout.form`
+
+```python
+form(*args, **kwargs)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\layouts.py#L94"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ContextLayout.grid`
 
 ```python
 grid(*args, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L83"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L90"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ContextLayout.hbox`
 
 ```python
 hbox(*args, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L98"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L109"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ContextLayout.scroll`
 
 ```python
 scroll(name=None, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L91"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L102"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ContextLayout.split`
 
 ```python
 split(name=None, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L79"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L86"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ContextLayout.vbox`
 
 ```python
 vbox(*args, **kwargs)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L121"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L132"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `CVBoxLayout`
 
 
 
 
-<a href="..\..\qtstrap\widgets\layouts.py#L24"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L28"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CVBoxLayout.__init__`
 
 ```python
 __init__(parent=None, stretch=None, margins=None, align=None, **kwargs)
 ```
 
@@ -148,107 +163,121 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L68"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L75"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CVBoxLayout.add`
 
 ```python
 add(item, *args, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L87"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L98"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `CVBoxLayout.form`
+
+```python
+form(*args, **kwargs)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\layouts.py#L94"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CVBoxLayout.grid`
 
 ```python
 grid(*args, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L83"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L90"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CVBoxLayout.hbox`
 
 ```python
 hbox(*args, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L98"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L109"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CVBoxLayout.scroll`
 
 ```python
 scroll(name=None, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L91"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L102"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CVBoxLayout.split`
 
 ```python
 split(name=None, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L79"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L86"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CVBoxLayout.vbox`
 
 ```python
 vbox(*args, **kwargs)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L125"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L133"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `CHBoxLayout`
 
 
 
 
-<a href="..\..\qtstrap\widgets\layouts.py#L24"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L28"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CHBoxLayout.__init__`
 
 ```python
 __init__(parent=None, stretch=None, margins=None, align=None, **kwargs)
 ```
 
@@ -257,107 +286,121 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L68"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L75"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CHBoxLayout.add`
 
 ```python
 add(item, *args, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L87"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L98"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `CHBoxLayout.form`
+
+```python
+form(*args, **kwargs)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\layouts.py#L94"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CHBoxLayout.grid`
 
 ```python
 grid(*args, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L83"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L90"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CHBoxLayout.hbox`
 
 ```python
 hbox(*args, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L98"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L109"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CHBoxLayout.scroll`
 
 ```python
 scroll(name=None, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L91"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L102"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CHBoxLayout.split`
 
 ```python
 split(name=None, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L79"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L86"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CHBoxLayout.vbox`
 
 ```python
 vbox(*args, **kwargs)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L129"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L134"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `CGridLayout`
 
 
 
 
-<a href="..\..\qtstrap\widgets\layouts.py#L24"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L28"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CGridLayout.__init__`
 
 ```python
 __init__(parent=None, stretch=None, margins=None, align=None, **kwargs)
 ```
 
@@ -366,107 +409,244 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L68"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L75"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CGridLayout.add`
 
 ```python
 add(item, *args, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L87"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L98"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `CGridLayout.form`
+
+```python
+form(*args, **kwargs)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\layouts.py#L94"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CGridLayout.grid`
 
 ```python
 grid(*args, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L83"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L90"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CGridLayout.hbox`
 
 ```python
 hbox(*args, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L98"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L109"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CGridLayout.scroll`
 
 ```python
 scroll(name=None, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L91"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L102"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CGridLayout.split`
 
 ```python
 split(name=None, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L79"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L86"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CGridLayout.vbox`
 
 ```python
 vbox(*args, **kwargs)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L136"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L135"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+## <kbd>class</kbd> `CFormLayout`
+
+
+
+
+<a href="..\..\qtstrap\widgets\layouts.py#L28"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `CFormLayout.__init__`
+
+```python
+__init__(parent=None, stretch=None, margins=None, align=None, **kwargs)
+```
+
+
+
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\layouts.py#L75"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `CFormLayout.add`
+
+```python
+add(item, *args, **kwargs)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\layouts.py#L98"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `CFormLayout.form`
+
+```python
+form(*args, **kwargs)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\layouts.py#L94"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `CFormLayout.grid`
+
+```python
+grid(*args, **kwargs)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\layouts.py#L90"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `CFormLayout.hbox`
+
+```python
+hbox(*args, **kwargs)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\layouts.py#L109"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `CFormLayout.scroll`
+
+```python
+scroll(name=None, **kwargs)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\layouts.py#L102"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `CFormLayout.split`
+
+```python
+split(name=None, **kwargs)
+```
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\layouts.py#L86"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `CFormLayout.vbox`
+
+```python
+vbox(*args, **kwargs)
+```
+
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\layouts.py#L141"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `CSplitter`
 
 
 
 
-<a href="..\..\qtstrap\widgets\layouts.py#L137"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L142"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CSplitter.__init__`
 
 ```python
 __init__(parent=None, margins=None, orientation=None, **kwargs)
 ```
 
@@ -475,37 +655,37 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L151"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L159"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CSplitter.add`
 
 ```python
 add(item, stretch=None)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L172"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L180"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentCSplitter`
 
 
 
 
-<a href="..\..\qtstrap\widgets\layouts.py#L173"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L181"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentCSplitter.__init__`
 
 ```python
 __init__(name, parent=None, **kwargs)
 ```
 
@@ -514,51 +694,51 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L151"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L159"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentCSplitter.add`
 
 ```python
 add(item, stretch=None)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L179"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L187"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentCSplitter.restore_state`
 
 ```python
 restore_state()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L190"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L198"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `CScrollArea`
 
 
 
 
-<a href="..\..\qtstrap\widgets\layouts.py#L191"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L199"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CScrollArea.__init__`
 
 ```python
 __init__(parent=None, margins=None, orientation=None, **kwargs)
 ```
 
@@ -567,65 +747,65 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L213"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L221"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CScrollArea.add`
 
 ```python
 add(item, stretch=None)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L230"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L238"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CScrollArea.addLayout`
 
 ```python
 addLayout(*args, **kwargs)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L227"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L235"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CScrollArea.addWidget`
 
 ```python
 addWidget(*args, **kwargs)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L240"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L248"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentCScrollArea`
 
 
 
 
-<a href="..\..\qtstrap\widgets\layouts.py#L241"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L249"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentCScrollArea.__init__`
 
 ```python
 __init__(name, parent=None, **kwargs)
 ```
 
@@ -634,29 +814,29 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L251"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L258"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentCScrollArea.restore_state`
 
 ```python
 restore_state()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\layouts.py#L248"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\layouts.py#L255"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentCScrollArea.scroll_to`
 
 ```python
 scroll_to(value)
 ```
```

#### html2text {}

```diff
@@ -1,70 +1,96 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
-`widgets.layouts` **Global Variables** --------------- - **PYQT6** - **PYQT5**
-- **PYSIDE2** - **PYSIDE6** - **alignments** - **orientations** --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ## class `ContextLayout`
-[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`ContextLayout.__init__` ```python __init__(parent=None, stretch=None,
-margins=None, align=None, **kwargs) ``` --- [https://img.shields.io/badge/-
-source-cccccc?style=flat-square] ### method `ContextLayout.add` ```python add
-(item, *args, **kwargs) ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `ContextLayout.grid` ```python grid(*args,
-**kwargs) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `ContextLayout.hbox` ```python hbox(*args, **kwargs) ``` --
+`widgets.layouts` **Global Variables** --------------- - **TYPE_CHECKING** -
+**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** - **alignments** -
+**orientations** --- [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ## class `ContextLayout` [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `ContextLayout.__init__` ```python
+__init__(parent=None, stretch=None, margins=None, align=None, **kwargs) ``` --
 - [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`ContextLayout.add` ```python add(item, *args, **kwargs) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`ContextLayout.form` ```python form(*args, **kwargs) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`ContextLayout.grid` ```python grid(*args, **kwargs) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`ContextLayout.hbox` ```python hbox(*args, **kwargs) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `ContextLayout.scroll` ```python scroll(name=None, **kwargs) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `ContextLayout.split` ```python split(name=None, **kwargs) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `ContextLayout.vbox` ```python vbox(*args, **kwargs) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ## class `CVBoxLayout`
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CVBoxLayout.__init__` ```python __init__(parent=None, stretch=None,
 margins=None, align=None, **kwargs) ``` --- [https://img.shields.io/badge/-
 source-cccccc?style=flat-square] ### method `CVBoxLayout.add` ```python add
 (item, *args, **kwargs) ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `CVBoxLayout.grid` ```python grid(*args,
+cccccc?style=flat-square] ### method `CVBoxLayout.form` ```python form(*args,
 **kwargs) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `CVBoxLayout.hbox` ```python hbox(*args, **kwargs) ``` ---
+square] ### method `CVBoxLayout.grid` ```python grid(*args, **kwargs) ``` ---
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`CVBoxLayout.hbox` ```python hbox(*args, **kwargs) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CVBoxLayout.scroll` ```python scroll(name=None, **kwargs) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CVBoxLayout.split` ```python split(name=None, **kwargs) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CVBoxLayout.vbox` ```python vbox(*args, **kwargs) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ## class `CHBoxLayout`
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CHBoxLayout.__init__` ```python __init__(parent=None, stretch=None,
 margins=None, align=None, **kwargs) ``` --- [https://img.shields.io/badge/-
 source-cccccc?style=flat-square] ### method `CHBoxLayout.add` ```python add
 (item, *args, **kwargs) ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `CHBoxLayout.grid` ```python grid(*args,
+cccccc?style=flat-square] ### method `CHBoxLayout.form` ```python form(*args,
 **kwargs) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `CHBoxLayout.hbox` ```python hbox(*args, **kwargs) ``` ---
+square] ### method `CHBoxLayout.grid` ```python grid(*args, **kwargs) ``` ---
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`CHBoxLayout.hbox` ```python hbox(*args, **kwargs) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CHBoxLayout.scroll` ```python scroll(name=None, **kwargs) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CHBoxLayout.split` ```python split(name=None, **kwargs) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CHBoxLayout.vbox` ```python vbox(*args, **kwargs) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ## class `CGridLayout`
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CGridLayout.__init__` ```python __init__(parent=None, stretch=None,
 margins=None, align=None, **kwargs) ``` --- [https://img.shields.io/badge/-
 source-cccccc?style=flat-square] ### method `CGridLayout.add` ```python add
 (item, *args, **kwargs) ``` --- [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `CGridLayout.grid` ```python grid(*args,
+cccccc?style=flat-square] ### method `CGridLayout.form` ```python form(*args,
 **kwargs) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `CGridLayout.hbox` ```python hbox(*args, **kwargs) ``` ---
+square] ### method `CGridLayout.grid` ```python grid(*args, **kwargs) ``` ---
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`CGridLayout.hbox` ```python hbox(*args, **kwargs) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CGridLayout.scroll` ```python scroll(name=None, **kwargs) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CGridLayout.split` ```python split(name=None, **kwargs) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CGridLayout.vbox` ```python vbox(*args, **kwargs) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ## class `CFormLayout`
+[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`CFormLayout.__init__` ```python __init__(parent=None, stretch=None,
+margins=None, align=None, **kwargs) ``` --- [https://img.shields.io/badge/-
+source-cccccc?style=flat-square] ### method `CFormLayout.add` ```python add
+(item, *args, **kwargs) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `CFormLayout.form` ```python form(*args,
+**kwargs) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `CFormLayout.grid` ```python grid(*args, **kwargs) ``` ---
+[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`CFormLayout.hbox` ```python hbox(*args, **kwargs) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`CFormLayout.scroll` ```python scroll(name=None, **kwargs) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`CFormLayout.split` ```python split(name=None, **kwargs) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`CFormLayout.vbox` ```python vbox(*args, **kwargs) ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ## class `CSplitter`
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `CSplitter.__init__` ```python __init__(parent=None, margins=None,
 orientation=None, **kwargs) ``` --- [https://img.shields.io/badge/-source-
 cccccc?style=flat-square] ### method `CSplitter.add` ```python add(item,
 stretch=None) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
 square] ## class `PersistentCSplitter` [https://img.shields.io/badge/-source-
```

### Comparing `qtstrap-0.4.1/docs/api/widgets.line_widgets.md` & `qtstrap-0.4.2/docs/api/widgets.link_label.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,88 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\widgets\line_widgets.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\link_label.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-# <kbd>module</kbd> `widgets.line_widgets`
+# <kbd>module</kbd> `widgets.link_label`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\line_widgets.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\link_label.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>class</kbd> `VLine`
+## <kbd>class</kbd> `LinkLabel`
 
 
 
 
-<a href="..\..\qtstrap\widgets\line_widgets.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\link_label.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `VLine.__init__`
+### <kbd>method</kbd> `LinkLabel.__init__`
 
 ```python
-__init__(parent=None, line_width=1)
+__init__(text='', link='', both=None, parent=None)
 ```
 
 
 
 
 
 
 
 
-
 ---
 
-<a href="..\..\qtstrap\widgets\line_widgets.py#L13"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\link_label.py#L28"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `LinkLabel.setBoth`
+
+```python
+setBoth(value)
+```
+
 
-## <kbd>class</kbd> `HLine`
 
 
 
+---
 
-<a href="..\..\qtstrap\widgets\line_widgets.py#L14"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\link_label.py#L24"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `HLine.__init__`
+### <kbd>method</kbd> `LinkLabel.setLink`
 
 ```python
-__init__(parent=None, line_width=1)
+setLink(link)
 ```
 
 
 
 
 
+---
+
+<a href="..\..\qtstrap\widgets\link_label.py#L20"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `LinkLabel.setText`
+
+```python
+setText(text)
+```
+
+
 
 
 
 
 
 
 ---
```

#### html2text {}

```diff
@@ -1,10 +1,13 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
-`widgets.line_widgets` **Global Variables** --------------- - **PYQT6** -
-**PYQT5** - **PYSIDE2** - **PYSIDE6** --- [https://img.shields.io/badge/-
-source-cccccc?style=flat-square] ## class `VLine` [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ### method `VLine.__init__` ```python
-__init__(parent=None, line_width=1) ``` --- [https://img.shields.io/badge/-
-source-cccccc?style=flat-square] ## class `HLine` [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ### method `HLine.__init__` ```python
-__init__(parent=None, line_width=1) ``` --- _This file was automatically
-generated via [lazydocs](https://github.com/ml-tooling/lazydocs)._
+`widgets.link_label` **Global Variables** --------------- - **TYPE_CHECKING** -
+**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** --- [https://img.shields.io/
+badge/-source-cccccc?style=flat-square] ## class `LinkLabel` [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`LinkLabel.__init__` ```python __init__(text='', link='', both=None,
+parent=None) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `LinkLabel.setBoth` ```python setBoth(value) ``` --- [https:
+//img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`LinkLabel.setLink` ```python setLink(link) ``` --- [https://img.shields.io/
+badge/-source-cccccc?style=flat-square] ### method `LinkLabel.setText`
+```python setText(text) ``` --- _This file was automatically generated via
+[lazydocs](https://github.com/ml-tooling/lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/widgets.link_label.md` & `qtstrap-0.4.2/docs/api/widgets.line_widgets.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,69 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\widgets\link_label.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\line_widgets.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-# <kbd>module</kbd> `widgets.link_label`
+# <kbd>module</kbd> `widgets.line_widgets`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\link_label.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\line_widgets.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>class</kbd> `LinkLabel`
+## <kbd>class</kbd> `VLine`
 
 
 
 
-<a href="..\..\qtstrap\widgets\link_label.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\line_widgets.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `LinkLabel.__init__`
+### <kbd>method</kbd> `VLine.__init__`
 
 ```python
-__init__(text='', link='', both=None, parent=None)
+__init__(parent=None, line_width=1)
 ```
 
 
 
 
 
 
 
 
+
 ---
 
-<a href="..\..\qtstrap\widgets\link_label.py#L24"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\line_widgets.py#L13"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `LinkLabel.setLink`
+## <kbd>class</kbd> `HLine`
 
-```python
-setLink(link)
-```
 
 
 
+<a href="..\..\qtstrap\widgets\line_widgets.py#L14"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
+### <kbd>method</kbd> `HLine.__init__`
 
----
+```python
+__init__(parent=None, line_width=1)
+```
 
-<a href="..\..\qtstrap\widgets\link_label.py#L20"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `LinkLabel.setText`
 
-```python
-setText(text)
-```
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
-`widgets.link_label` **Global Variables** --------------- - **PYQT6** -
-**PYQT5** - **PYSIDE2** - **PYSIDE6** --- [https://img.shields.io/badge/-
-source-cccccc?style=flat-square] ## class `LinkLabel` [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ### method `LinkLabel.__init__`
-```python __init__(text='', link='', both=None, parent=None) ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`LinkLabel.setLink` ```python setLink(link) ``` --- [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ### method `LinkLabel.setText`
-```python setText(text) ``` --- _This file was automatically generated via
-[lazydocs](https://github.com/ml-tooling/lazydocs)._
+`widgets.line_widgets` **Global Variables** --------------- - **TYPE_CHECKING**
+- **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ## class `VLine` [https:
+//img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`VLine.__init__` ```python __init__(parent=None, line_width=1) ``` --- [https:/
+/img.shields.io/badge/-source-cccccc?style=flat-square] ## class `HLine`
+[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`HLine.__init__` ```python __init__(parent=None, line_width=1) ``` --- _This
+file was automatically generated via [lazydocs](https://github.com/ml-tooling/
+lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/widgets.md` & `qtstrap-0.4.2/docs/api/widgets.md`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 - **layouts**
 - **buttons**
 - **labeledit**
 - **link_label**
 - **line_widgets**
 - **persistent_widgets**
 - **persistent_tab_widget**
+- **toggle**
+- **toolbar**
 
 
 
 
 ---
 
 _This file was automatically generated via [lazydocs](https://github.com/ml-tooling/lazydocs)._
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
 `widgets` **Global Variables** --------------- - **layouts** - **buttons** -
 **labeledit** - **link_label** - **line_widgets** - **persistent_widgets** -
-**persistent_tab_widget** --- _This file was automatically generated via
-[lazydocs](https://github.com/ml-tooling/lazydocs)._
+**persistent_tab_widget** - **toggle** - **toolbar** --- _This file was
+automatically generated via [lazydocs](https://github.com/ml-tooling/
+lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/widgets.persistent_tab_widget.md` & `qtstrap-0.4.2/docs/api/widgets.persistent_tab_widget.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # <kbd>module</kbd> `widgets.persistent_tab_widget`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 
 ---
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
 `widgets.persistent_tab_widget` **Global Variables** --------------- -
-**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** --- [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ## class `PersistentTabWidget` [https:/
-/img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`PersistentTabWidget.__init__` ```python __init__(name, tabs=None, *args,
-**kwargs) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `PersistentTabWidget.close_tab` ```python close_tab(index)
+**TYPE_CHECKING** - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** ---
+[https://img.shields.io/badge/-source-cccccc?style=flat-square] ## class
+`PersistentTabWidget` [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `PersistentTabWidget.__init__` ```python __init__(name,
+tabs=None, *args, **kwargs) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `PersistentTabWidget.close_tab` ```python
+close_tab(index) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `PersistentTabWidget.menu` ```python menu
+(pos) â None ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `PersistentTabWidget.move_tab` ```python move_tab(old, new)
 ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ###
-method `PersistentTabWidget.menu` ```python menu(pos) â None ``` --- [https:/
-/img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`PersistentTabWidget.move_tab` ```python move_tab(old, new) ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`PersistentTabWidget.restore_state` ```python restore_state(tabs=None) ``` ---
-[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`PersistentTabWidget.tab_order` ```python tab_order() ``` --- [https://
+method `PersistentTabWidget.restore_state` ```python restore_state(tabs=None)
+``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ###
+method `PersistentTabWidget.tab_order` ```python tab_order() ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `PersistentTabWidget.unhide_all` ```python unhide_all() ``` --- [https://
 img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `PersistentTabWidget.visible_tabs` ```python visible_tabs() ``` --- _This file
 was automatically generated via [lazydocs](https://github.com/ml-tooling/
 lazydocs)._
```

### Comparing `qtstrap-0.4.1/docs/api/widgets.persistent_widgets.md` & `qtstrap-0.4.2/docs/api/widgets.persistent_widgets.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # <kbd>module</kbd> `widgets.persistent_widgets`
 
 
 
 
 **Global Variables**
 ---------------
+- **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 
 ---
@@ -52,22 +53,22 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L23"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L26"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentLineEdit`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L24"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L27"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentLineEdit.__init__`
 
 ```python
 __init__(name, *args, default='', changed=None, **kwargs)
 ```
 
@@ -76,37 +77,37 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L35"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L38"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentLineEdit.restore_state`
 
 ```python
 restore_state()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L39"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L42"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentTextEdit`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L40"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L43"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTextEdit.__init__`
 
 ```python
 __init__(name, *args, default='', changed=None, **kwargs)
 ```
 
@@ -115,37 +116,76 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L51"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L54"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTextEdit.restore_state`
 
 ```python
 restore_state()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L55"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L58"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+## <kbd>class</kbd> `PersistentPlainTextEdit`
+
+
+
+
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L59"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `PersistentPlainTextEdit.__init__`
+
+```python
+__init__(name, *args, default='', changed=None, **kwargs)
+```
+
+
+
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L70"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `PersistentPlainTextEdit.restore_state`
+
+```python
+restore_state()
+```
+
+
+
+
+
+
+---
+
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L74"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentListWidget`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L56"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L75"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentListWidget.__init__`
 
 ```python
 __init__(name, items=[], default=[], changed=None, *args, **kwargs)
 ```
 
@@ -154,51 +194,51 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L73"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L92"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentListWidget.restore_state`
 
 ```python
 restore_state()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L70"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L89"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentListWidget.selected_items`
 
 ```python
 selected_items()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L81"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L100"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentTreeWidget`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L82"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L101"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTreeWidget.__init__`
 
 ```python
 __init__(
     name,
     items=[],
@@ -215,51 +255,51 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L100"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L119"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTreeWidget.restore_state`
 
 ```python
 restore_state()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L97"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L116"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTreeWidget.selected_items`
 
 ```python
 selected_items()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L108"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L127"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentComboBox`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L109"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L128"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentComboBox.__init__`
 
 ```python
 __init__(name, items=[], changed=None, *args, **kwargs)
 ```
 
@@ -268,37 +308,37 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L122"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L141"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentComboBox.restore_state`
 
 ```python
 restore_state()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L128"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L147"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentCheckableAction`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L129"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L148"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentCheckableAction.__init__`
 
 ```python
 __init__(name, *args, **kwargs)
 ```
 
@@ -307,15 +347,15 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L137"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="..\..\qtstrap\widgets\persistent_widgets.py#L156"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentCheckableAction.restore_state`
 
 ```python
 restore_state()
 ```
```

#### html2text {}

```diff
@@ -1,40 +1,47 @@
  [https://img.shields.io/badge/-source-cccccc?style=flat-square] # module
-`widgets.persistent_widgets` **Global Variables** --------------- - **PYQT6** -
-**PYQT5** - **PYSIDE2** - **PYSIDE6** --- [https://img.shields.io/badge/-
-source-cccccc?style=flat-square] ## class `PersistentCheckBox` [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`PersistentCheckBox.__init__` ```python __init__(name, changed=None, *args,
-**kwargs) ``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `PersistentCheckBox.restore_state` ```python restore_state()
-``` --- [https://img.shields.io/badge/-source-cccccc?style=flat-square] ##
-class `PersistentLineEdit` [https://img.shields.io/badge/-source-
-cccccc?style=flat-square] ### method `PersistentLineEdit.__init__` ```python
-__init__(name, *args, default='', changed=None, **kwargs) ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`PersistentLineEdit.restore_state` ```python restore_state() ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ## class
-`PersistentTextEdit` [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `PersistentTextEdit.__init__` ```python __init__(name,
-*args, default='', changed=None, **kwargs) ``` --- [https://img.shields.io/
-badge/-source-cccccc?style=flat-square] ### method
-`PersistentTextEdit.restore_state` ```python restore_state() ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ## class
-`PersistentListWidget` [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `PersistentListWidget.__init__` ```python __init__(name,
-items=[], default=[], changed=None, *args, **kwargs) ``` --- [https://
-img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`PersistentListWidget.restore_state` ```python restore_state() ``` --- [https:/
-/img.shields.io/badge/-source-cccccc?style=flat-square] ### method
-`PersistentListWidget.selected_items` ```python selected_items() ``` ---
+`widgets.persistent_widgets` **Global Variables** --------------- -
+**TYPE_CHECKING** - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** ---
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ## class
-`PersistentTreeWidget` [https://img.shields.io/badge/-source-cccccc?style=flat-
-square] ### method `PersistentTreeWidget.__init__` ```python __init__( name,
-items=[], index_column=0, default=[], changed=None, *args, **kwargs ) ``` ---
-[https://img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`PersistentCheckBox` [https://img.shields.io/badge/-source-cccccc?style=flat-
+square] ### method `PersistentCheckBox.__init__` ```python __init__(name,
+changed=None, *args, **kwargs) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `PersistentCheckBox.restore_state`
+```python restore_state() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ## class `PersistentLineEdit` [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`PersistentLineEdit.__init__` ```python __init__(name, *args, default='',
+changed=None, **kwargs) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `PersistentLineEdit.restore_state`
+```python restore_state() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ## class `PersistentTextEdit` [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`PersistentTextEdit.__init__` ```python __init__(name, *args, default='',
+changed=None, **kwargs) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `PersistentTextEdit.restore_state`
+```python restore_state() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ## class `PersistentPlainTextEdit` [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`PersistentPlainTextEdit.__init__` ```python __init__(name, *args, default='',
+changed=None, **kwargs) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `PersistentPlainTextEdit.restore_state`
+```python restore_state() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ## class `PersistentListWidget` [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`PersistentListWidget.__init__` ```python __init__(name, items=[], default=[],
+changed=None, *args, **kwargs) ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `PersistentListWidget.restore_state`
+```python restore_state() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ### method `PersistentListWidget.selected_items`
+```python selected_items() ``` --- [https://img.shields.io/badge/-source-
+cccccc?style=flat-square] ## class `PersistentTreeWidget` [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
+`PersistentTreeWidget.__init__` ```python __init__( name, items=[],
+index_column=0, default=[], changed=None, *args, **kwargs ) ``` --- [https://
+img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `PersistentTreeWidget.restore_state` ```python restore_state() ``` --- [https:/
 /img.shields.io/badge/-source-cccccc?style=flat-square] ### method
 `PersistentTreeWidget.selected_items` ```python selected_items() ``` ---
 [https://img.shields.io/badge/-source-cccccc?style=flat-square] ## class
 `PersistentComboBox` [https://img.shields.io/badge/-source-cccccc?style=flat-
 square] ### method `PersistentComboBox.__init__` ```python __init__(name,
 items=[], changed=None, *args, **kwargs) ``` --- [https://img.shields.io/badge/
```

### Comparing `qtstrap-0.4.1/docs/quickstart/baseapplication.md` & `qtstrap-0.4.2/docs/quickstart/baseapplication.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/quickstart/basemainwindow.md` & `qtstrap-0.4.2/docs/quickstart/basemainwindow.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/quickstart/context_layouts.md` & `qtstrap-0.4.2/docs/quickstart/context_layouts.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/quickstart/gettingstarted.md` & `qtstrap-0.4.2/docs/quickstart/gettingstarted.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/quickstart/installation.md` & `qtstrap-0.4.2/docs/quickstart/installation.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/base_application.md` & `qtstrap-0.4.2/docs/reference/base_application.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/base_window.md` & `qtstrap-0.4.2/docs/reference/base_window.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/options.md` & `qtstrap-0.4.2/docs/reference/options.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/toolbar.md` & `qtstrap-0.4.2/docs/reference/toolbar.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/utils.adapter.md` & `qtstrap-0.4.2/docs/reference/utils.adapter.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/utils.defer.md` & `qtstrap-0.4.2/docs/reference/utils.defer.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/utils.signals.md` & `qtstrap-0.4.2/docs/reference/utils.signals.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/utils.timestamp.md` & `qtstrap-0.4.2/docs/reference/utils.timestamp.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/utils.utils.md` & `qtstrap-0.4.2/docs/reference/utils.utils.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/widgets.buttons.md` & `qtstrap-0.4.2/docs/reference/widgets.buttons.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/widgets.labeledit.md` & `qtstrap-0.4.2/docs/reference/widgets.labeledit.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/widgets.layouts.md` & `qtstrap-0.4.2/docs/reference/widgets.layouts.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/widgets.line_widgets.md` & `qtstrap-0.4.2/docs/reference/widgets.line_widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/widgets.link_label.md` & `qtstrap-0.4.2/docs/reference/widgets.link_label.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/widgets.md` & `qtstrap-0.4.2/docs/reference/widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/widgets.persistent_tab_widget.md` & `qtstrap-0.4.2/docs/reference/widgets.persistent_tab_widget.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/reference/widgets.persistent_widgets.md` & `qtstrap-0.4.2/docs/reference/widgets.persistent_widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/screenshot1.png` & `qtstrap-0.4.2/docs/screenshot1.png`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/structure/makefile.md` & `qtstrap-0.4.2/docs/structure/makefile.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/structure/structure.md` & `qtstrap-0.4.2/docs/structure/structure.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/docs/test.md` & `qtstrap-0.4.2/docs/test.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/mkdocs.yml` & `qtstrap-0.4.2/mkdocs.yml`

 * *Files 17% similar despite different names*

```diff
@@ -8,20 +8,26 @@
     name: readthedocs
 plugins:
   - search
   - mermaid2
   - literate-nav
 
 nav:
-    - Overview:
-        - Home: index.md
-        - Quickstart: 
-            - Installation: quickstart/installation.md
-            - Getting Started: quickstart/gettingstarted.md
-            - BaseApplication: quickstart/baseapplication.md
-            - BaseMainWindow: quickstart/basemainwindow.md
-            - Context Layouts: quickstart/context_layouts.md
-        - Project Structure: 
-            - Project Structure: structure/structure.md
-            - Makefile: structure/makefile.md
-    - API Reference:
-      - api/*
+  - Overview:
+    - Home: index.md
+    - Quickstart: 
+      - Installation: quickstart/installation.md
+      - Getting Started: quickstart/gettingstarted.md
+      - BaseApplication: quickstart/baseapplication.md
+      - BaseMainWindow: quickstart/basemainwindow.md
+      - Context Layouts: quickstart/context_layouts.md
+    - Project Structure: 
+      - Project Structure: structure/structure.md
+      - Makefile: structure/makefile.md
+    - Extras: 
+      - Extras: extras/index.md
+      - Code Editor: extras/code_editor.md
+      - Command Palette: extras/command_palette.md
+      - Log Monitor: extras/log_monitor.md
+      - Styles: extras/styles.md
+  - API Reference:
+    - api/*
```

### Comparing `qtstrap-0.4.1/qtstrap/__init__.py` & `qtstrap-0.4.2/qtstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/__main__.py` & `qtstrap-0.4.2/qtstrap/__main__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/base_application.py` & `qtstrap-0.4.2/qtstrap/base_application.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/base_window.py` & `qtstrap-0.4.2/qtstrap/base_window.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/extras/code_editor/code_editor.py` & `qtstrap-0.4.2/qtstrap/extras/code_editor/code_editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
             '(': ')',
             '<': '>',
             '[': ']',
             '|': '|',
             '`': '`',
         }
 
+        self.comment_symbol = '//'
+
         set_font_options(self, {
             'setFamily': 'Courier',
             'setStyleHint': QFont.Monospace,
             'setFixedPitch': True,
         })
         
         self.installEventFilter(self)
@@ -179,22 +181,23 @@
 
         text = self.toPlainText()[start: end]
         text_lines = text.split('\n')
         first_line = text_lines[0]
         og_length = len(text)
         lines = []
         
-        add = not all([s[0] == '#' for s in text_lines if s])
+        comment_length = len(self.comment_symbol)
+        add = not all([s[:comment_length] == self.comment_symbol for s in text_lines if s])
 
         for line in text_lines:
             if line:
                 if add:
-                    line = '# ' + line
+                    line = f'{self.comment_symbol} ' + line
                 else:
-                    line = line.removeprefix('# ')
+                    line = line.removeprefix(f'{self.comment_symbol} ')
             lines.append(line)
 
         text = '\n'.join(lines)
         cur.insertText(text)
 
         final_end = og_end + len(text) - og_length
         final_start = og_start + len(lines[0]) - len(first_line)
@@ -265,15 +268,14 @@
 
         if direction == QTextCursor.Up:
             cur.setPosition(start)
             cur.movePosition(QTextCursor.Up)
             cur.movePosition(QTextCursor.EndOfLine, QTextCursor.KeepAnchor)
             cur.movePosition(QTextCursor.Right, QTextCursor.KeepAnchor)
             text = cur.selectedText()
-            print('move:', text)
             cur.setPosition(end)
             cur.movePosition(QTextCursor.Down)
             cur.movePosition(QTextCursor.StartOfLine)
             cur.insertText(text)
             cur.setPosition(start)
             cur.movePosition(QTextCursor.Up)
             cur.movePosition(QTextCursor.EndOfLine, QTextCursor.KeepAnchor)
@@ -283,15 +285,14 @@
             cur.setPosition(og_end - len(text), QTextCursor.KeepAnchor)
             
         if direction == QTextCursor.Down:
             cur.setPosition(end)
             cur.movePosition(QTextCursor.Down, QTextCursor.KeepAnchor)
             cur.movePosition(QTextCursor.EndOfLine, QTextCursor.KeepAnchor)
             text = cur.selectedText()
-            print('move:', text)
             cur.setPosition(start)
             cur.movePosition(QTextCursor.Up)
             cur.movePosition(QTextCursor.EndOfLine)
             cur.insertText(text)
             cur.setPosition(end + len(text))
             cur.movePosition(QTextCursor.Down)
             cur.movePosition(QTextCursor.EndOfLine, QTextCursor.KeepAnchor)
```

### Comparing `qtstrap-0.4.1/qtstrap/extras/code_editor/code_line.py` & `qtstrap-0.4.2/qtstrap/extras/code_editor/code_line.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/extras/code_editor/highlighters/python.py` & `qtstrap-0.4.2/qtstrap/extras/code_editor/highlighters/python.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/extras/command_palette/command_palette.py` & `qtstrap-0.4.2/qtstrap/extras/command_palette/command_palette.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,26 +231,28 @@
     def get_selection(self):
         index = self.list.currentIndex()
         return index.data(Qt.EditRole)
 
 
 @singleton
 class CommandPalette(QDialog):
-    def __init__(self, parent=None):
+    def __init__(self, parent=None, shortcut='Ctrl+Shift+P'):
         super().__init__(parent)
         self.setObjectName('CommandPalette')
         self.setWindowFlags(Qt.Tool | Qt.FramelessWindowHint | Qt.WindowStaysOnTopHint)
         self.setFocusPolicy(Qt.StrongFocus)
         
         set_font_options(self, {'setPointSize': 16})
         
         self.setMinimumWidth(700)
 
+        self.shortcut = shortcut
+
         self.action = QAction("Command Palette", self)
-        self.action.setShortcut('Ctrl+Shift+P')
+        self.action.setShortcut(self.shortcut)
         self.action.triggered.connect(self.palette)
 
         self.line = QLineEdit()
         # self.line.setStyleSheet("""
         #     QLineEdit {
         #         font-size: 16pt;
         #         border: 1px solid #0074D9;
@@ -272,31 +274,31 @@
         self.line.installEventFilter(self)
         self.callback = None
 
     def palette(self):
         self.open()
         self.command_completer.open()
 
-    def _open(self, cb=None, prompt=None, placeholder=None, completer=None, validator=None, mask=None):
+    def _open(self, cb=None, prompt=None, placeholder=None, choices=None, completer=None, validator=None, mask=None):
         self.callback = cb
 
         self.line.setText(prompt)
         self.line.setPlaceholderText(placeholder)
         self.line.setCompleter(completer)
         self.line.setValidator(validator)
         self.line.setInputMask(mask)
 
         self.command_completer.reset()
         self.center_on_parent()
         self.show()
         self.activateWindow()
         self.line.setFocus()
 
-    def open(self, cb=None, prompt=None, placeholder=None, completer=None, validator=None, mask=None):
-        QTimer.singleShot(0, lambda: self._open(cb, prompt, placeholder, completer, validator, mask))
+    def open(self, cb=None, prompt=None, placeholder=None, choices=None, completer=None, validator=None, mask=None):
+        QTimer.singleShot(0, lambda: self._open(cb, prompt, placeholder, choices, completer, validator, mask))
 
     def accept(self):
         if self.command_completer.active:
             name = self.command_completer.get_selection()
             self.dismiss()
             registry.execute(name)
         else:
```

### Comparing `qtstrap-0.4.1/qtstrap/extras/log_monitor/__init__.py` & `qtstrap-0.4.2/qtstrap/extras/log_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/extras/log_monitor/log_database_handler.py` & `qtstrap-0.4.2/qtstrap/extras/log_monitor/log_database_handler.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/extras/log_monitor/log_filter_controls.py` & `qtstrap-0.4.2/qtstrap/extras/log_monitor/log_filter_controls.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,14 +462,15 @@
         self.current_profile = self.settings['profiles'][profile_name]
         self.logger_filter.set_visible_loggers(self.current_profile['visible_loggers'])
         self.table.set_columns(self.current_profile.get('column_data', {}))
         self.update_filter()
 
     def columns_changed(self):
         self.current_profile['column_data'] = self.table.profile.column_data
+        self.table.set_columns(self.current_profile.get('column_data', {}))
         self.save_settings()
 
     def update_filter(self):
         text = self.text_filter.text()
         loggers = {item.full_name: item.get_levels() for _, item in self.logger_filter.loggers.items()}
         visible_loggers = self.logger_filter.visible_loggers
```

### Comparing `qtstrap-0.4.1/qtstrap/extras/log_monitor/log_profile.py` & `qtstrap-0.4.2/qtstrap/extras/log_monitor/log_profile.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/extras/log_monitor/log_table_view.py` & `qtstrap-0.4.2/qtstrap/extras/log_monitor/log_table_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
             try:
                 if index.column() == self.log_level_column:
                     level = super().data(index, Qt.DisplayRole)
                     return QColor(get_color(level[0]))
             except (IndexError, KeyError):
                 pass
             return None
+        elif role == Qt.ToolTipRole:                    # <- new lines
+            return super().data(index, Qt.DisplayRole)  # <- new lines
         else:
             return super().data(index, role)
 
 
 class LogTableView(QTableView):
     columns_changed = Signal()
```

### Comparing `qtstrap-0.4.1/qtstrap/extras/log_monitor/log_widget.py` & `qtstrap-0.4.2/qtstrap/extras/log_monitor/log_widget.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/extras/style/colors.py` & `qtstrap-0.4.2/qtstrap/extras/style/colors.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/extras/style/dark_palette.py` & `qtstrap-0.4.2/qtstrap/extras/style/dark_palette.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/extras/style/themes.py` & `qtstrap-0.4.2/qtstrap/extras/style/themes.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/options.py` & `qtstrap-0.4.2/qtstrap/options.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/qt.py` & `qtstrap-0.4.2/qtstrap/qt.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/template/Makefile` & `qtstrap-0.4.2/qtstrap/template/Makefile`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/template/app/main.py` & `qtstrap-0.4.2/qtstrap/template/app/main.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/template/app/resources/application.ico` & `qtstrap-0.4.2/qtstrap/template/app/resources/application.ico`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/template/app/resources/icon.svg` & `qtstrap-0.4.2/qtstrap/template/app/resources/icon.svg`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/template/bundle.spec` & `qtstrap-0.4.2/qtstrap/template/bundle.spec`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/template/installer.iss` & `qtstrap-0.4.2/qtstrap/template/installer.iss`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/utils/adapter.py` & `qtstrap-0.4.2/qtstrap/utils/adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-from qtstrap import QObject, SignalInstance
+from qtstrap import QObject
+
+
+try:
+    from qtstrap import SignalInstance
+except:
+    from qtstrap import pyqtBoundSignal as SignalInstance
 
 
 class Adapter(QObject):
     """ A signal adapter that helps create disposable connections between objects. 
     
     A signal-based interface can be defined using an Adapter.
```

### Comparing `qtstrap-0.4.1/qtstrap/utils/defer.py` & `qtstrap-0.4.2/qtstrap/utils/defer.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/utils/drag_and_drop.py` & `qtstrap-0.4.2/qtstrap/utils/drag_and_drop.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/utils/get_ip.py` & `qtstrap-0.4.2/qtstrap/utils/get_ip.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/utils/string_builder.py` & `qtstrap-0.4.2/qtstrap/utils/string_builder.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/utils/timestamp.py` & `qtstrap-0.4.2/qtstrap/utils/timestamp.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/utils/utils.py` & `qtstrap-0.4.2/qtstrap/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/widgets/__init__.py` & `qtstrap-0.4.2/qtstrap/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/widgets/buttons.py` & `qtstrap-0.4.2/qtstrap/widgets/buttons.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/widgets/labeledit.py` & `qtstrap-0.4.2/qtstrap/widgets/labeledit.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/widgets/layouts.py` & `qtstrap-0.4.2/qtstrap/widgets/layouts.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,18 @@
         if len(self._stack) > 0:
             layout = self._stack[len(self._stack) - 1]
         return layout
 
     def __call__(self):
         return self._layout
 
+    def __iadd__(self, item):
+        self.add(item)
+        return self
+
     def add(self, item, *args, **kwargs):
         if isinstance(item, QWidget):
             self._layout.addWidget(item, *args, **kwargs)
         elif isinstance(item, QLayout):
             self._layout.addLayout(item, *args, **kwargs)
         elif isinstance(item, list):
             for i in item:
@@ -152,14 +156,18 @@
 
         if margins:
             self.setContentsMargins(*margins)
 
         if orientation:
             self.setOrientation(orientation)
 
+    def __iadd__(self, item):
+        self.add(item)
+        return self
+
     def add(self, item, stretch=None):
         if isinstance(item, QWidget):
             self.addWidget(item)
             if stretch:
                 self.setStretchFactor(self.count()-1, stretch)
         elif isinstance(item, QLayout):
             self.addWidget(QWidget(self, layout=item))
@@ -214,14 +222,18 @@
             self.setContentsMargins(*margins)
 
         if orientation:
             if orientation in orientations:
                 orientation = orientations[orientation]
             self.setOrientation(orientation)
 
+    def __iadd__(self, item):
+        self.add(item)
+        return self
+
     def add(self, item, stretch=None):
         if isinstance(item, QWidget):
             self.widget().layout().addWidget(item)
             if stretch:
                 self.widget().layout().setStretchFactor(self.count()-1, stretch)
         elif isinstance(item, QLayout):
             self.addWidget(QWidget(self, layout=item))
```

### Comparing `qtstrap-0.4.1/qtstrap/widgets/line_widgets.py` & `qtstrap-0.4.2/qtstrap/widgets/line_widgets.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/widgets/link_label.py` & `qtstrap-0.4.2/qtstrap/widgets/link_label.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/widgets/persistent_tab_widget.py` & `qtstrap-0.4.2/qtstrap/widgets/persistent_tab_widget.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/widgets/persistent_widgets.py` & `qtstrap-0.4.2/qtstrap/widgets/persistent_widgets.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/widgets/toggle.py` & `qtstrap-0.4.2/qtstrap/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap/widgets/toolbar.py` & `qtstrap-0.4.2/qtstrap/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/qtstrap.egg-info/PKG-INFO` & `qtstrap-0.4.2/qtstrap.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtstrap
-Version: 0.4.1
+Version: 0.4.2
 Summary: Like Bootstrap, but qt-er.
 Home-page: https://github.com/qtstrap/qtstrap
 Author: David Kincaid
 Author-email: dlkincaid0@gmail.com
 License: MIT
 Project-URL: Documentation, https://qtstrap.github.io/qtstrap/
 Project-URL: Source, https://github.com/qtstrap/qtstrap
@@ -36,22 +36,60 @@
 
 # Features
 
 More complete docs are available [here](https://qtstrap.github.io/qtstrap/).
 
 * `qtstrap` command line tool to bootstrap new projects
 * crossplatform makefile with useful development commands
-* preconfigured pyinstaller spec file
-* preconfigured InnoSetup setup compiler script
+* preconfigured build system using PyInstaller and InnoSetup
 * custom Qt widgets with useful behaviors
 * Pythonic layout system using ContextLayouts
 * Some other stuff I haven't remembered yet
 
-# License
-This project is released under the MIT license.
+## Custom Widgets
+
+- `LabelEdit`
+- `HLine` and `VLine`
+- `LinkLabel`
+- Buttons:
+  - `StateButton`
+  - `IconToggleButton`
+  - `ConfirmToggleButton`
+  - `MenuButton`
+- Persistent Widgets (for rapid prototyping of saved data):
+  - `PersistentCheckableAction`
+  - `PersistentCheckBox`
+  - `PersistentComboBox`
+  - `PersistentLineEdit`
+  - `PersistentListWidget`
+  - `PersistentPlainTextEdit`
+  - `PersistentTabWidget`
+  - `PersistentTextEdit`
+  - `PersistentTreeWidget`
+
+## Utility Classes and Functions
+- `Adapter`
+- `TimeStamp`
+- `StringBuilder`
+- `call_later()`
+
+## decorators:
+- `@accepts_file_drops`
+- `@trace`
+- `@singleton`
+
+## context managers:
+- `Defer`
+- `SignalBlocker`
+
+## qtstrap.extras:
+  - `CommandPalette`, like VSCode or SublimeText
+  - Logging Subsystem: log to local database + log viewer widgets
+  - `CodeEditor`: Custom QTextEditor subclass customized for code editing
+
 
 # Dependencies
 
 * Python 3
 * PySide2 or PyQt5
 * Make(optional, but recommended)
```

### Comparing `qtstrap-0.4.1/qtstrap.egg-info/SOURCES.txt` & `qtstrap-0.4.2/qtstrap.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 requirements.txt
 requirements_build.txt
 requirements_test.txt
 run_tox_tests.py
 setup.cfg
 setup.py
 tox.ini
+.github/FUNDING.yml
 .github/workflows/main.yml
 docs/index.md
 docs/screenshot1.png
 docs/test.md
 docs/api/.pages
 docs/api/extras.code_editor.code_editor.md
 docs/api/extras.code_editor.code_line.md
@@ -31,33 +32,46 @@
 docs/api/extras.log_monitor.log_table_view.md
 docs/api/extras.log_monitor.log_widget.md
 docs/api/extras.log_monitor.md
 docs/api/extras.md
 docs/api/extras.style.colors.md
 docs/api/extras.style.dark_palette.md
 docs/api/extras.style.md
+docs/api/extras.style.themes.md
 docs/api/options.md
 docs/api/overview.md
 docs/api/settings.md
 docs/api/utils.adapter.md
+docs/api/utils.call_later.md
 docs/api/utils.decorators.md
 docs/api/utils.defer.md
+docs/api/utils.drag_and_drop.md
+docs/api/utils.get_ip.md
 docs/api/utils.md
 docs/api/utils.signals.md
 docs/api/utils.singleton.md
+docs/api/utils.string_builder.md
 docs/api/utils.timestamp.md
+docs/api/utils.trace.md
 docs/api/utils.utils.md
 docs/api/widgets.buttons.md
 docs/api/widgets.labeledit.md
 docs/api/widgets.layouts.md
 docs/api/widgets.line_widgets.md
 docs/api/widgets.link_label.md
 docs/api/widgets.md
 docs/api/widgets.persistent_tab_widget.md
 docs/api/widgets.persistent_widgets.md
+docs/api/widgets.toggle.md
+docs/api/widgets.toolbar.md
+docs/extras/code_editor.md
+docs/extras/command_palette.md
+docs/extras/index.md
+docs/extras/log_monitor.md
+docs/extras/styles.md
 docs/quickstart/baseapplication.md
 docs/quickstart/basemainwindow.md
 docs/quickstart/context_layouts.md
 docs/quickstart/gettingstarted.md
 docs/quickstart/installation.md
 docs/reference/base_application.md
 docs/reference/base_window.md
@@ -92,14 +106,15 @@
 qtstrap.egg-info/PKG-INFO
 qtstrap.egg-info/SOURCES.txt
 qtstrap.egg-info/dependency_links.txt
 qtstrap.egg-info/entry_points.txt
 qtstrap.egg-info/not-zip-safe
 qtstrap.egg-info/requires.txt
 qtstrap.egg-info/top_level.txt
+qtstrap/experimental/__init__.py
 qtstrap/extras/__init__.py
 qtstrap/extras/code_editor/__init__.py
 qtstrap/extras/code_editor/code_editor.py
 qtstrap/extras/code_editor/code_line.py
 qtstrap/extras/code_editor/highlighters/__init__.py
 qtstrap/extras/code_editor/highlighters/python.py
 qtstrap/extras/command_palette/__init__.py
@@ -110,14 +125,15 @@
 qtstrap/extras/log_monitor/log_profile.py
 qtstrap/extras/log_monitor/log_table_view.py
 qtstrap/extras/log_monitor/log_widget.py
 qtstrap/extras/style/__init__.py
 qtstrap/extras/style/colors.py
 qtstrap/extras/style/dark_palette.py
 qtstrap/extras/style/themes.py
+qtstrap/optional/__init__.py
 qtstrap/template/Makefile
 qtstrap/template/bundle.spec
 qtstrap/template/installer.iss
 qtstrap/template/requirements.txt
 qtstrap/template/app/main.py
 qtstrap/template/app/resources/application.ico
 qtstrap/template/app/resources/icon.svg
```

### Comparing `qtstrap-0.4.1/requirements.txt` & `qtstrap-0.4.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/requirements_build.txt` & `qtstrap-0.4.2/requirements_build.txt`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/requirements_test.txt` & `qtstrap-0.4.2/requirements_test.txt`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/setup.cfg` & `qtstrap-0.4.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7473 7472 6170 0d0a 7665 7273   = qtstrap..vers
-00000020: 696f 6e20 3d20 302e 342e 310d 0a64 6573  ion = 0.4.1..des
+00000020: 696f 6e20 3d20 302e 342e 320d 0a64 6573  ion = 0.4.2..des
 00000030: 6372 6970 7469 6f6e 203d 204c 696b 6520  cription = Like 
 00000040: 426f 6f74 7374 7261 702c 2062 7574 2071  Bootstrap, but q
 00000050: 742d 6572 2e0d 0a6c 6f6e 675f 6465 7363  t-er...long_desc
 00000060: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000070: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 00000080: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
 00000090: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
```

### Comparing `qtstrap-0.4.1/test/test_base_app.py` & `qtstrap-0.4.2/test/test_base_app.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/test/test_base_window.py` & `qtstrap-0.4.2/test/test_base_window.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/test/test_layouts.py` & `qtstrap-0.4.2/test/test_layouts.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.4.1/test/test_utils.py` & `qtstrap-0.4.2/test/test_utils.py`

 * *Files identical despite different names*


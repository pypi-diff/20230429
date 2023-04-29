# Comparing `tmp/bfactory-0.4.tar.gz` & `tmp/bfactory-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfactory-0.4.tar", last modified: Thu Apr 27 02:45:23 2023, max compression
+gzip compressed data, was "bfactory-0.4.1.tar", last modified: Sat Apr 29 02:20:50 2023, max compression
```

## Comparing `bfactory-0.4.tar` & `bfactory-0.4.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/
--rw-r--r--   0 blackbox  (1000) users      (985)     1063 2022-10-03 23:46:43.000000 bfactory-0.4/LICENSE
--rw-r--r--   0 blackbox  (1000) users      (985)      541 2023-04-27 02:45:23.808709 bfactory-0.4/PKG-INFO
--rw-r--r--   0 blackbox  (1000) users      (985)     1604 2022-10-03 23:46:43.000000 bfactory-0.4/README.md
--rw-r--r--   0 blackbox  (1000) users      (985)       87 2022-10-03 23:46:43.000000 bfactory-0.4/pyproject.toml
--rw-r--r--   0 blackbox  (1000) users      (985)      856 2023-04-27 02:45:23.812043 bfactory-0.4/setup.cfg
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-04 00:29:45.000000 bfactory-0.4/src/bfactory/__init__.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/config/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/config/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1251 2023-04-27 02:45:10.000000 bfactory-0.4/src/bfactory/config/settings.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/core/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/core/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)     3515 2022-11-10 04:08:56.000000 bfactory-0.4/src/bfactory/core/engine.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2130 2022-11-05 23:27:19.000000 bfactory-0.4/src/bfactory/core/tasks.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/core/templates/
--rw-r--r--   0 blackbox  (1000) users      (985)       85 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/core/templates/READ.ME
--rw-r--r--   0 blackbox  (1000) users      (985)      570 2022-10-04 00:02:46.000000 bfactory-0.4/src/bfactory/core/templates/admin.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/core/templates/helpers/
--rw-r--r--   0 blackbox  (1000) users      (985)     1179 2022-11-10 03:35:21.000000 bfactory-0.4/src/bfactory/core/templates/helpers/field.py
--rw-r--r--   0 blackbox  (1000) users      (985)      982 2022-11-10 03:37:52.000000 bfactory-0.4/src/bfactory/core/templates/helpers/field_serializer.py
--rw-r--r--   0 blackbox  (1000) users      (985)      341 2022-11-06 19:43:09.000000 bfactory-0.4/src/bfactory/core/templates/helpers/field_type_linting.py
--rw-r--r--   0 blackbox  (1000) users      (985)      624 2022-11-06 04:00:22.000000 bfactory-0.4/src/bfactory/core/templates/models.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2759 2022-10-04 00:02:40.000000 bfactory-0.4/src/bfactory/core/templates/myconf.py
--rw-r--r--   0 blackbox  (1000) users      (985)      599 2022-11-06 04:00:13.000000 bfactory-0.4/src/bfactory/core/templates/selectors.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1621 2022-11-29 20:30:05.000000 bfactory-0.4/src/bfactory/core/templates/services.py
--rw-r--r--   0 blackbox  (1000) users      (985)      570 2022-11-05 23:27:19.000000 bfactory-0.4/src/bfactory/core/templates/urls.py
--rw-r--r--   0 blackbox  (1000) users      (985)     4388 2022-11-10 03:54:52.000000 bfactory-0.4/src/bfactory/core/templates/views.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/inputs/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/inputs/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1550 2022-11-29 20:30:05.000000 bfactory-0.4/src/bfactory/inputs/arguments.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2534 2022-11-10 03:35:04.000000 bfactory-0.4/src/bfactory/inputs/manifest.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2698 2022-10-30 07:02:48.000000 bfactory-0.4/src/bfactory/inputs/manifest.schema.json
--rw-r--r--   0 blackbox  (1000) users      (985)      887 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/inputs/parse_manifest.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1363 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/inputs/validators.py
--rwxr-xr-x   0 blackbox  (1000) users      (985)     1066 2022-10-04 00:33:18.000000 bfactory-0.4/src/bfactory/main.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/startproject/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/startproject/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)      620 2022-10-04 00:19:42.000000 bfactory-0.4/src/bfactory/startproject/startproject.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/tests/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/tests/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)      743 2022-11-10 04:08:38.000000 bfactory-0.4/src/bfactory/tests/engine_tests.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1022 2022-11-29 20:30:05.000000 bfactory-0.4/src/bfactory/tests/manifest_test.json
--rw-r--r--   0 blackbox  (1000) users      (985)      675 2022-10-07 02:36:35.000000 bfactory-0.4/src/bfactory/tests/manifest_test.py
--rw-r--r--   0 blackbox  (1000) users      (985)      932 2022-10-04 00:31:46.000000 bfactory-0.4/src/bfactory/tests/run_tests.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/utils/
--rw-r--r--   0 blackbox  (1000) users      (985)      900 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/utils/crypto.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2442 2022-10-07 02:36:35.000000 bfactory-0.4/src/bfactory/utils/paths.py
--rw-r--r--   0 blackbox  (1000) users      (985)      450 2022-10-04 00:26:40.000000 bfactory-0.4/src/bfactory/utils/render.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory.egg-info/
--rw-r--r--   0 blackbox  (1000) users      (985)      541 2023-04-27 02:45:23.000000 bfactory-0.4/src/bfactory.egg-info/PKG-INFO
--rw-r--r--   0 blackbox  (1000) users      (985)     1481 2023-04-27 02:45:23.000000 bfactory-0.4/src/bfactory.egg-info/SOURCES.txt
--rw-r--r--   0 blackbox  (1000) users      (985)        1 2023-04-27 02:45:23.000000 bfactory-0.4/src/bfactory.egg-info/dependency_links.txt
--rw-r--r--   0 blackbox  (1000) users      (985)       48 2023-04-27 02:45:23.000000 bfactory-0.4/src/bfactory.egg-info/entry_points.txt
--rw-r--r--   0 blackbox  (1000) users      (985)       91 2023-04-27 02:45:23.000000 bfactory-0.4/src/bfactory.egg-info/requires.txt
--rw-r--r--   0 blackbox  (1000) users      (985)        9 2023-04-27 02:45:23.000000 bfactory-0.4/src/bfactory.egg-info/top_level.txt
--rwxr-xr-x   0 blackbox  (1000) users      (985)      197 2022-11-29 20:30:05.000000 bfactory-0.4/src/bfactory.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.612099 bfactory-0.4.1/
+-rw-r--r--   0 blackbox  (1000) users      (985)     1063 2022-10-03 23:46:43.000000 bfactory-0.4.1/LICENSE
+-rw-r--r--   0 blackbox  (1000) users      (985)      543 2023-04-29 02:20:50.612099 bfactory-0.4.1/PKG-INFO
+-rw-r--r--   0 blackbox  (1000) users      (985)     1604 2022-10-03 23:46:43.000000 bfactory-0.4.1/README.md
+-rw-r--r--   0 blackbox  (1000) users      (985)       87 2022-10-03 23:46:43.000000 bfactory-0.4.1/pyproject.toml
+-rw-r--r--   0 blackbox  (1000) users      (985)      856 2023-04-29 02:20:50.612099 bfactory-0.4.1/setup.cfg
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-04 00:29:45.000000 bfactory-0.4.1/src/bfactory/__init__.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/config/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/config/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1253 2023-04-29 02:18:07.000000 bfactory-0.4.1/src/bfactory/config/settings.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/core/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/core/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     3515 2022-11-10 04:08:56.000000 bfactory-0.4.1/src/bfactory/core/engine.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2130 2022-11-05 23:27:19.000000 bfactory-0.4.1/src/bfactory/core/tasks.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/core/templates/
+-rw-r--r--   0 blackbox  (1000) users      (985)       85 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/core/templates/READ.ME
+-rw-r--r--   0 blackbox  (1000) users      (985)      570 2022-10-04 00:02:46.000000 bfactory-0.4.1/src/bfactory/core/templates/admin.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/core/templates/helpers/
+-rw-r--r--   0 blackbox  (1000) users      (985)     1461 2023-04-29 00:28:37.000000 bfactory-0.4.1/src/bfactory/core/templates/helpers/field.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1260 2023-04-29 00:35:51.000000 bfactory-0.4.1/src/bfactory/core/templates/helpers/field_serializer.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      414 2023-04-29 00:35:02.000000 bfactory-0.4.1/src/bfactory/core/templates/helpers/field_type_linting.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      624 2022-11-06 04:00:22.000000 bfactory-0.4.1/src/bfactory/core/templates/models.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2759 2022-10-04 00:02:40.000000 bfactory-0.4.1/src/bfactory/core/templates/myconf.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      599 2023-04-29 00:34:58.000000 bfactory-0.4.1/src/bfactory/core/templates/selectors.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1621 2022-11-29 20:30:05.000000 bfactory-0.4.1/src/bfactory/core/templates/services.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      570 2022-11-05 23:27:19.000000 bfactory-0.4.1/src/bfactory/core/templates/urls.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     4388 2022-11-10 03:54:52.000000 bfactory-0.4.1/src/bfactory/core/templates/views.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/inputs/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/inputs/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1550 2022-11-29 20:30:05.000000 bfactory-0.4.1/src/bfactory/inputs/arguments.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2534 2022-11-10 03:35:04.000000 bfactory-0.4.1/src/bfactory/inputs/manifest.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2698 2022-10-30 07:02:48.000000 bfactory-0.4.1/src/bfactory/inputs/manifest.schema.json
+-rw-r--r--   0 blackbox  (1000) users      (985)      887 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/inputs/parse_manifest.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1363 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/inputs/validators.py
+-rwxr-xr-x   0 blackbox  (1000) users      (985)     1066 2022-10-04 00:33:18.000000 bfactory-0.4.1/src/bfactory/main.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/startproject/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/startproject/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      620 2022-10-04 00:19:42.000000 bfactory-0.4.1/src/bfactory/startproject/startproject.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/tests/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/tests/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      743 2022-11-10 04:08:38.000000 bfactory-0.4.1/src/bfactory/tests/engine_tests.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1022 2023-04-29 02:19:06.000000 bfactory-0.4.1/src/bfactory/tests/manifest_test.json
+-rw-r--r--   0 blackbox  (1000) users      (985)      675 2022-10-07 02:36:35.000000 bfactory-0.4.1/src/bfactory/tests/manifest_test.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      932 2022-10-04 00:31:46.000000 bfactory-0.4.1/src/bfactory/tests/run_tests.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.612099 bfactory-0.4.1/src/bfactory/utils/
+-rw-r--r--   0 blackbox  (1000) users      (985)      900 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/utils/crypto.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2442 2022-10-07 02:36:35.000000 bfactory-0.4.1/src/bfactory/utils/paths.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      450 2022-10-04 00:26:40.000000 bfactory-0.4.1/src/bfactory/utils/render.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory.egg-info/
+-rw-r--r--   0 blackbox  (1000) users      (985)      543 2023-04-29 02:20:50.000000 bfactory-0.4.1/src/bfactory.egg-info/PKG-INFO
+-rw-r--r--   0 blackbox  (1000) users      (985)     1481 2023-04-29 02:20:50.000000 bfactory-0.4.1/src/bfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)        1 2023-04-29 02:20:50.000000 bfactory-0.4.1/src/bfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)       48 2023-04-29 02:20:50.000000 bfactory-0.4.1/src/bfactory.egg-info/entry_points.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)       91 2023-04-29 02:20:50.000000 bfactory-0.4.1/src/bfactory.egg-info/requires.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)        9 2023-04-29 02:20:50.000000 bfactory-0.4.1/src/bfactory.egg-info/top_level.txt
+-rwxr-xr-x   0 blackbox  (1000) users      (985)      197 2022-11-29 20:30:05.000000 bfactory-0.4.1/src/bfactory.py
```

### Comparing `bfactory-0.4/LICENSE` & `bfactory-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/PKG-INFO` & `bfactory-0.4.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfactory
-Version: 0.4
+Version: 0.4.1
 Summary: Build an API from a manifest file
 Home-page: https://github.com/forkear/bfactory
 Author: Forkear
 Author-email: forkear@no-spam.org
 Project-URL: Documentation, https://github.com/forkear/bfactory/blob/main/README.md
 Project-URL: Source, https://github.com/forkear/bfactory
 Project-URL: Tracker, https://github.com/forkear/bfactory/issues
```

### Comparing `bfactory-0.4/README.md` & `bfactory-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/setup.cfg` & `bfactory-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/config/settings.py` & `bfactory-0.4.1/src/bfactory/config/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-__version__ = '0.4'
+__version__ = '0.4.1'
 
 TITLE_BANNER='''\
 
 ██████╗ ███████╗ █████╗  ██████╗████████╗ ██████╗ ██████╗ ██╗   ██╗
 ██╔══██╗██╔════╝██╔══██╗██╔════╝╚══██╔══╝██╔═══██╗██╔══██╗╚██╗ ██╔╝
 ██████╔╝█████╗  ███████║██║        ██║   ██║   ██║██████╔╝ ╚████╔╝ 
 ██╔══██╗██╔══╝  ██╔══██║██║        ██║   ██║   ██║██╔══██╗  ╚██╔╝
```

### Comparing `bfactory-0.4/src/bfactory/core/engine.py` & `bfactory-0.4.1/src/bfactory/core/engine.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/core/tasks.py` & `bfactory-0.4.1/src/bfactory/core/tasks.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/core/templates/admin.py` & `bfactory-0.4.1/src/bfactory/core/templates/admin.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/core/templates/helpers/field.py` & `bfactory-0.4.1/src/bfactory/core/templates/helpers/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 {%- if field.type == 'bool' -%}
     models.BooleanField({% if not field.req %} default=False {% endif %})
 {% endif %}
 {%- if field.type == 'user' or field.type == 'owner' -%}
     models.ForeignKey(User, related_name="{{model.name|lower}}_{{field.name|lower}}_user", on_delete=models.CASCADE{% if not field.req %}, null=True, blank=True{% endif %})
 {% endif %}
 {%- if field.type == 'int' -%}
+    models.IntegerField({% if not field.req %}null=True, blank=True{% endif %})
+{% endif %}
+{%- if field.type == 'float' -%}
+    models.DecimalField(max_digits=10, decimal_places=2{% if not field.req %}, null=True, blank=True{% endif %})
+{% endif %}
+{%- if field.type == 'pint' -%}
     models.PositiveIntegerField({% if not field.req %}null=True, blank=True{% endif %})
 {% endif %}
 {%- if field.type == 'fk' -%}
     models.ForeignKey("{{field.fk}}", related_name="{{model.name|lower}}_{{field.name|lower}}_{{field.fk|lower}}", on_delete=models.CASCADE{% if not field.req %},null=True, blank=True{% endif %})
 {% endif %}
 {%- if field.type == 'datetime' -%}
     models.DateTimeField({% if field.default == 'now' %}auto_now=True{% endif %}{% if not field.req %}, null=True, blank=True {% endif %})
```

### Comparing `bfactory-0.4/src/bfactory/core/templates/helpers/field_serializer.py` & `bfactory-0.4.1/src/bfactory/core/templates/helpers/field_serializer.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,19 +3,25 @@
 {% endif %}
 {%- if field.type == 'text'  -%}
     serializers.CharField({% if not field.req %} allow_blank=True {% endif %})
 {% endif %}
 {%- if field.type == 'bool' -%}
     serializers.BooleanField({% if not field.req %} default=False {% endif %})
 {% endif %}
-{%- if field.type == 'user' or field.type == 'owner' -%}
-    models.ForeignKey(User, on_delete=models.CASCADE{% if not field.req %}, null=True, blank=True{% endif %})
-{% endif %}
 {%- if field.type == 'int' -%}
-    models.PositiveIntegerField({% if not field.req %}null=True, blank=True{% endif %})
+    serializers.IntegerField({% if not field.req %}required=False{% endif %})
+{% endif %}
+{%- if field.type == 'pint' -%}
+    serializers.IntegerField(min_value=0{% if not field.req %}, required=False{% endif %})
 {% endif %}
 {%- if field.type == 'fk' -%}
     serializers.PrimaryKeyRelatedField(many=False, queryset={{field.fk}}.objects.all(), required={{field.req}} {% if not field.req %}, allow_null=True {% endif %})
 {% endif %}
 {%- if field.type == 'datetime' -%}
     serializers.DateTimeField()
+{% endif %}
+{%- if field.type == 'float' -%}
+    serializers.DecimalField(max_digits=10, decimal_places=2)
+{% endif %}
+{%- if field.type == 'user' or field.type == 'owner' -%}
+    serializers.PrimaryKeyRelatedField(many=False, queryset=User.objects.all(), required={{field.req}} {% if not field.req %}, allow_null=True {% endif %})
 {% endif %}
```

### Comparing `bfactory-0.4/src/bfactory/core/templates/models.py` & `bfactory-0.4.1/src/bfactory/core/templates/models.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/core/templates/myconf.py` & `bfactory-0.4.1/src/bfactory/core/templates/myconf.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/core/templates/selectors.py` & `bfactory-0.4.1/src/bfactory/core/templates/selectors.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/core/templates/services.py` & `bfactory-0.4.1/src/bfactory/core/templates/services.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/core/templates/urls.py` & `bfactory-0.4.1/src/bfactory/core/templates/urls.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/core/templates/views.py` & `bfactory-0.4.1/src/bfactory/core/templates/views.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/inputs/arguments.py` & `bfactory-0.4.1/src/bfactory/inputs/arguments.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/inputs/manifest.py` & `bfactory-0.4.1/src/bfactory/inputs/manifest.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/inputs/manifest.schema.json` & `bfactory-0.4.1/src/bfactory/inputs/manifest.schema.json`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/inputs/parse_manifest.py` & `bfactory-0.4.1/src/bfactory/inputs/parse_manifest.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/inputs/validators.py` & `bfactory-0.4.1/src/bfactory/inputs/validators.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/main.py` & `bfactory-0.4.1/src/bfactory/main.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/startproject/startproject.py` & `bfactory-0.4.1/src/bfactory/startproject/startproject.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/tests/engine_tests.py` & `bfactory-0.4.1/src/bfactory/tests/engine_tests.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/tests/manifest_test.json` & `bfactory-0.4.1/src/bfactory/tests/manifest_test.json`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/tests/manifest_test.py` & `bfactory-0.4.1/src/bfactory/tests/manifest_test.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/tests/run_tests.py` & `bfactory-0.4.1/src/bfactory/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/utils/crypto.py` & `bfactory-0.4.1/src/bfactory/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory/utils/paths.py` & `bfactory-0.4.1/src/bfactory/utils/paths.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4/src/bfactory.egg-info/PKG-INFO` & `bfactory-0.4.1/src/bfactory.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfactory
-Version: 0.4
+Version: 0.4.1
 Summary: Build an API from a manifest file
 Home-page: https://github.com/forkear/bfactory
 Author: Forkear
 Author-email: forkear@no-spam.org
 Project-URL: Documentation, https://github.com/forkear/bfactory/blob/main/README.md
 Project-URL: Source, https://github.com/forkear/bfactory
 Project-URL: Tracker, https://github.com/forkear/bfactory/issues
```

### Comparing `bfactory-0.4/src/bfactory.egg-info/SOURCES.txt` & `bfactory-0.4.1/src/bfactory.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/data-toolkit-1.4.6.tar.gz` & `tmp/data-toolkit-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-toolkit-1.4.6.tar", last modified: Tue Mar 28 09:51:06 2023, max compression
+gzip compressed data, was "data-toolkit-1.4.7.tar", last modified: Sat Apr 29 15:37:21 2023, max compression
```

## Comparing `data-toolkit-1.4.6.tar` & `data-toolkit-1.4.7.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-03-28 09:51:06.990603 data-toolkit-1.4.6/
--rw-r--r--   0 jlangr     (501) staff       (20)       58 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/CHANGELOG.md
--rw-r--r--   0 jlangr     (501) staff       (20)        1 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/LICENSE.md
--rw-r--r--   0 jlangr     (501) staff       (20)      130 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/MANIFEST.in
--rw-r--r--   0 jlangr     (501) staff       (20)     3592 2023-03-28 09:51:06.990683 data-toolkit-1.4.6/PKG-INFO
--rw-r--r--   0 jlangr     (501) staff       (20)     3259 2022-12-20 15:23:48.000000 data-toolkit-1.4.6/README.md
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-03-28 09:51:06.983353 data-toolkit-1.4.6/data_toolkit.egg-info/
--rw-r--r--   0 jlangr     (501) staff       (20)     3592 2023-03-28 09:51:06.000000 data-toolkit-1.4.6/data_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 jlangr     (501) staff       (20)     1087 2023-03-28 09:51:06.000000 data-toolkit-1.4.6/data_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 jlangr     (501) staff       (20)        1 2023-03-28 09:51:06.000000 data-toolkit-1.4.6/data_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 jlangr     (501) staff       (20)       36 2023-03-28 09:51:06.000000 data-toolkit-1.4.6/data_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 jlangr     (501) staff       (20)      112 2023-03-28 09:51:06.000000 data-toolkit-1.4.6/data_toolkit.egg-info/requires.txt
--rw-r--r--   0 jlangr     (501) staff       (20)        3 2023-03-28 09:51:06.000000 data-toolkit-1.4.6/data_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-03-28 09:51:06.983722 data-toolkit-1.4.6/dt/
--rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/__init__.py
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-03-28 09:51:06.984024 data-toolkit-1.4.6/dt/controllers/
--rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/controllers/__init__.py
--rw-r--r--   0 jlangr     (501) staff       (20)    33823 2023-03-28 09:24:00.000000 data-toolkit-1.4.6/dt/controllers/base.py
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-03-28 09:51:06.984614 data-toolkit-1.4.6/dt/core/
--rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/core/__init__.py
--rw-r--r--   0 jlangr     (501) staff       (20)     5741 2023-02-27 16:32:40.000000 data-toolkit-1.4.6/dt/core/data_diff.py
--rw-r--r--   0 jlangr     (501) staff       (20)       67 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/core/exc.py
--rw-r--r--   0 jlangr     (501) staff       (20)      176 2023-03-28 09:24:18.000000 data-toolkit-1.4.6/dt/core/version.py
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-03-28 09:51:06.989448 data-toolkit-1.4.6/dt/ext/
--rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/ext/__init__.py
--rw-r--r--   0 jlangr     (501) staff       (20)     8634 2023-03-28 09:50:55.000000 data-toolkit-1.4.6/dt/ext/asana.py
--rw-r--r--   0 jlangr     (501) staff       (20)     3759 2022-08-14 21:17:02.000000 data-toolkit-1.4.6/dt/ext/aws_ec2.py
--rw-r--r--   0 jlangr     (501) staff       (20)     8287 2023-01-07 23:59:43.000000 data-toolkit-1.4.6/dt/ext/aws_s3.py
--rw-r--r--   0 jlangr     (501) staff       (20)     3959 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/ext/aws_s3_list.py
--rw-r--r--   0 jlangr     (501) staff       (20)     7025 2022-09-04 16:24:11.000000 data-toolkit-1.4.6/dt/ext/aws_sg.py
--rw-r--r--   0 jlangr     (501) staff       (20)     2685 2022-12-22 21:21:09.000000 data-toolkit-1.4.6/dt/ext/codex.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1042 2023-02-27 16:33:26.000000 data-toolkit-1.4.6/dt/ext/config.py
--rw-r--r--   0 jlangr     (501) staff       (20)     4963 2023-03-24 10:20:24.000000 data-toolkit-1.4.6/dt/ext/fake_data.py
--rw-r--r--   0 jlangr     (501) staff       (20)     4100 2022-12-03 18:16:05.000000 data-toolkit-1.4.6/dt/ext/firelit.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1195 2023-02-27 16:32:40.000000 data-toolkit-1.4.6/dt/ext/gcp.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1354 2022-09-15 21:51:05.000000 data-toolkit-1.4.6/dt/ext/gdrive_dl.py
--rw-r--r--   0 jlangr     (501) staff       (20)     5627 2023-02-27 16:32:40.000000 data-toolkit-1.4.6/dt/ext/github.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1237 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/ext/gkeep.py
--rw-r--r--   0 jlangr     (501) staff       (20)     3914 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/ext/hist.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1080 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/ext/monitor.py
--rw-r--r--   0 jlangr     (501) staff       (20)     7769 2023-02-27 16:32:40.000000 data-toolkit-1.4.6/dt/ext/ms_outlook.py
--rw-r--r--   0 jlangr     (501) staff       (20)     3490 2022-12-20 15:23:48.000000 data-toolkit-1.4.6/dt/ext/notes.py
--rw-r--r--   0 jlangr     (501) staff       (20)    13933 2023-03-27 11:18:04.000000 data-toolkit-1.4.6/dt/ext/notions.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1334 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/ext/python_exec.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1619 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/ext/run.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1367 2022-08-14 21:17:00.000000 data-toolkit-1.4.6/dt/ext/sftp_conf.py
--rw-r--r--   0 jlangr     (501) staff       (20)     2212 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/ext/ssh_params.py
--rw-r--r--   0 jlangr     (501) staff       (20)     8758 2022-12-03 18:16:05.000000 data-toolkit-1.4.6/dt/ext/sshconf.py
--rw-r--r--   0 jlangr     (501) staff       (20)     3189 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/ext/tracking.py
--rw-r--r--   0 jlangr     (501) staff       (20)     2694 2022-08-14 21:17:02.000000 data-toolkit-1.4.6/dt/ext/tree.py
--rw-r--r--   0 jlangr     (501) staff       (20)     3808 2023-02-27 16:32:40.000000 data-toolkit-1.4.6/dt/ext/zshrc.txt
--rw-r--r--   0 jlangr     (501) staff       (20)      813 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/help.py
--rw-r--r--   0 jlangr     (501) staff       (20)     1855 2022-07-27 22:31:14.000000 data-toolkit-1.4.6/dt/main.py
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-03-28 09:51:06.989800 data-toolkit-1.4.6/dt/plugins/
--rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/plugins/__init__.py
--rw-r--r--   0 jlangr     (501) staff       (20)     6659 2022-08-14 21:28:36.000000 data-toolkit-1.4.6/dt/plugins/viz_utils.py
-drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-03-28 09:51:06.990435 data-toolkit-1.4.6/dt/templates/
--rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/templates/__init__.py
--rw-r--r--   0 jlangr     (501) staff       (20)       64 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/templates/command1.jinja2
--rw-r--r--   0 jlangr     (501) staff       (20)      458 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/dt/templates/sftp.json
--rw-r--r--   0 jlangr     (501) staff       (20)       99 2022-07-27 22:30:58.000000 data-toolkit-1.4.6/requirements-dev.txt
--rw-r--r--   0 jlangr     (501) staff       (20)       92 2022-09-08 17:42:10.000000 data-toolkit-1.4.6/requirements.txt
--rw-r--r--   0 jlangr     (501) staff       (20)       38 2023-03-28 09:51:06.990913 data-toolkit-1.4.6/setup.cfg
--rw-r--r--   0 jlangr     (501) staff       (20)     1130 2022-12-20 15:23:48.000000 data-toolkit-1.4.6/setup.py
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-29 15:37:21.561957 data-toolkit-1.4.7/
+-rw-r--r--   0 jlangr     (501) staff       (20)       58 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/CHANGELOG.md
+-rw-r--r--   0 jlangr     (501) staff       (20)        1 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/LICENSE.md
+-rw-r--r--   0 jlangr     (501) staff       (20)      130 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/MANIFEST.in
+-rw-r--r--   0 jlangr     (501) staff       (20)     3592 2023-04-29 15:37:21.562055 data-toolkit-1.4.7/PKG-INFO
+-rw-r--r--   0 jlangr     (501) staff       (20)     3259 2022-12-20 15:23:48.000000 data-toolkit-1.4.7/README.md
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-29 15:37:21.553863 data-toolkit-1.4.7/data_toolkit.egg-info/
+-rw-r--r--   0 jlangr     (501) staff       (20)     3592 2023-04-29 15:37:21.000000 data-toolkit-1.4.7/data_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 jlangr     (501) staff       (20)     1087 2023-04-29 15:37:21.000000 data-toolkit-1.4.7/data_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jlangr     (501) staff       (20)        1 2023-04-29 15:37:21.000000 data-toolkit-1.4.7/data_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jlangr     (501) staff       (20)       36 2023-04-29 15:37:21.000000 data-toolkit-1.4.7/data_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 jlangr     (501) staff       (20)      112 2023-04-29 15:37:21.000000 data-toolkit-1.4.7/data_toolkit.egg-info/requires.txt
+-rw-r--r--   0 jlangr     (501) staff       (20)        3 2023-04-29 15:37:21.000000 data-toolkit-1.4.7/data_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-29 15:37:21.554247 data-toolkit-1.4.7/dt/
+-rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/__init__.py
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-29 15:37:21.554560 data-toolkit-1.4.7/dt/controllers/
+-rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/controllers/__init__.py
+-rw-r--r--   0 jlangr     (501) staff       (20)    33827 2023-04-29 15:36:00.000000 data-toolkit-1.4.7/dt/controllers/base.py
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-29 15:37:21.555510 data-toolkit-1.4.7/dt/core/
+-rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/core/__init__.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     5741 2023-02-27 16:32:40.000000 data-toolkit-1.4.7/dt/core/data_diff.py
+-rw-r--r--   0 jlangr     (501) staff       (20)       67 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/core/exc.py
+-rw-r--r--   0 jlangr     (501) staff       (20)      176 2023-04-29 15:37:14.000000 data-toolkit-1.4.7/dt/core/version.py
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-29 15:37:21.560902 data-toolkit-1.4.7/dt/ext/
+-rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/ext/__init__.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     8852 2023-04-29 15:35:51.000000 data-toolkit-1.4.7/dt/ext/asana.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     3759 2022-08-14 21:17:02.000000 data-toolkit-1.4.7/dt/ext/aws_ec2.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     8287 2023-01-07 23:59:43.000000 data-toolkit-1.4.7/dt/ext/aws_s3.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     3959 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/ext/aws_s3_list.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     7025 2022-09-04 16:24:11.000000 data-toolkit-1.4.7/dt/ext/aws_sg.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     2685 2022-12-22 21:21:09.000000 data-toolkit-1.4.7/dt/ext/codex.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1042 2023-02-27 16:33:26.000000 data-toolkit-1.4.7/dt/ext/config.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     4963 2023-03-24 10:20:24.000000 data-toolkit-1.4.7/dt/ext/fake_data.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     4100 2022-12-03 18:16:05.000000 data-toolkit-1.4.7/dt/ext/firelit.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1195 2023-02-27 16:32:40.000000 data-toolkit-1.4.7/dt/ext/gcp.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1354 2022-09-15 21:51:05.000000 data-toolkit-1.4.7/dt/ext/gdrive_dl.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     5627 2023-02-27 16:32:40.000000 data-toolkit-1.4.7/dt/ext/github.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1237 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/ext/gkeep.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     3914 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/ext/hist.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1080 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/ext/monitor.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     7769 2023-02-27 16:32:40.000000 data-toolkit-1.4.7/dt/ext/ms_outlook.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     3490 2022-12-20 15:23:48.000000 data-toolkit-1.4.7/dt/ext/notes.py
+-rw-r--r--   0 jlangr     (501) staff       (20)    14061 2023-04-21 12:30:29.000000 data-toolkit-1.4.7/dt/ext/notions.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1334 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/ext/python_exec.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1619 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/ext/run.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1367 2022-08-14 21:17:00.000000 data-toolkit-1.4.7/dt/ext/sftp_conf.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     2212 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/ext/ssh_params.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     8758 2022-12-03 18:16:05.000000 data-toolkit-1.4.7/dt/ext/sshconf.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     3189 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/ext/tracking.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     2694 2022-08-14 21:17:02.000000 data-toolkit-1.4.7/dt/ext/tree.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     3808 2023-02-27 16:32:40.000000 data-toolkit-1.4.7/dt/ext/zshrc.txt
+-rw-r--r--   0 jlangr     (501) staff       (20)      813 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/help.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     1855 2022-07-27 22:31:14.000000 data-toolkit-1.4.7/dt/main.py
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-29 15:37:21.561163 data-toolkit-1.4.7/dt/plugins/
+-rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/plugins/__init__.py
+-rw-r--r--   0 jlangr     (501) staff       (20)     6659 2022-08-14 21:28:36.000000 data-toolkit-1.4.7/dt/plugins/viz_utils.py
+drwxr-xr-x   0 jlangr     (501) staff       (20)        0 2023-04-29 15:37:21.561764 data-toolkit-1.4.7/dt/templates/
+-rw-r--r--   0 jlangr     (501) staff       (20)        0 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/templates/__init__.py
+-rw-r--r--   0 jlangr     (501) staff       (20)       64 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/templates/command1.jinja2
+-rw-r--r--   0 jlangr     (501) staff       (20)      458 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/dt/templates/sftp.json
+-rw-r--r--   0 jlangr     (501) staff       (20)       99 2022-07-27 22:30:58.000000 data-toolkit-1.4.7/requirements-dev.txt
+-rw-r--r--   0 jlangr     (501) staff       (20)       92 2022-09-08 17:42:10.000000 data-toolkit-1.4.7/requirements.txt
+-rw-r--r--   0 jlangr     (501) staff       (20)       38 2023-04-29 15:37:21.562328 data-toolkit-1.4.7/setup.cfg
+-rw-r--r--   0 jlangr     (501) staff       (20)     1130 2022-12-20 15:23:48.000000 data-toolkit-1.4.7/setup.py
```

### Comparing `data-toolkit-1.4.6/PKG-INFO` & `data-toolkit-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-toolkit
-Version: 1.4.6
+Version: 1.4.7
 Summary: ML & data helper code!
 Home-page: https://github.com/jakublangr/data-toolkit/
 Author: Jakub Langr
 Author-email: james.langr@gmail.com
 License: (c) Jakub Langr
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `data-toolkit-1.4.6/README.md` & `data-toolkit-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/data_toolkit.egg-info/PKG-INFO` & `data-toolkit-1.4.7/data_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-toolkit
-Version: 1.4.6
+Version: 1.4.7
 Summary: ML & data helper code!
 Home-page: https://github.com/jakublangr/data-toolkit/
 Author: Jakub Langr
 Author-email: james.langr@gmail.com
 License: (c) Jakub Langr
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `data-toolkit-1.4.6/data_toolkit.egg-info/SOURCES.txt` & `data-toolkit-1.4.7/data_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/controllers/base.py` & `data-toolkit-1.4.7/dt/controllers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -787,15 +787,15 @@
                 "action": "store"
             }),
             (['-l'],{
                 "help": "Length of time in days this is expected to take",
                 "action": "store"
             }),
             (['-p'],{
-                "help" : "Project name. If not given, grabs IDG.",
+                "help" : "Project name. If not given, grabs saker.",
                 "action" : 'store'
             }),
             (['-i'],{
                 "help" : "Id of the finished task",
                 "action": "store"
             }),
             (['-ws'],{
@@ -807,15 +807,15 @@
                 "action": "store"
             })
         ]
     )
     def td(self):
         from ..ext.asana import add_todo, asana_list_todos, done_todo,  \
             fix_past_due, asana_list_workspaces
-        project = self.app.pargs.p or "IDG"
+        project = self.app.pargs.p or "saker"
 
         if self.app.pargs.action=='add':
             add_todo(self.app.pargs.t, self.app.pargs.l, self.app.pargs.ws, project)
         elif self.app.pargs.action=='ls':
             asana_list_todos(
                 self.app.pargs.p,
                 self.app.pargs.f,)
```

### Comparing `data-toolkit-1.4.6/dt/core/data_diff.py` & `data-toolkit-1.4.7/dt/core/data_diff.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/asana.py` & `data-toolkit-1.4.7/dt/ext/asana.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,18 @@
     if project_name not in asana_projects.keys():
         projects = list(client.projects.get_projects_for_workspace(workspace_id))
         if project_name == 0:
             # here project_name is id
             project_id = projects[int(project_name)]['gid']
         else:
             try:
-                project_id = [ w['gid'] for w in projects if w['name'] == project_name][0]
+                # filter s.t. project id that matches the project name
+                project_id = list(filter(lambda x: x['name'] == project_name, projects))[0]['gid']
+                import ipdb; ipdb.set_trace()
+                # project_id = [ w['gid'] for w in projects if w['name'] == project_name][0]
                 print(f"project_id of project name {project_name}: {project_id}")
             except IndexError:
                 print(f"Project {project_name} not found. But this could also be a bug.")
     else:
         project_id = asana_projects[project_name]
```

### Comparing `data-toolkit-1.4.6/dt/ext/aws_ec2.py` & `data-toolkit-1.4.7/dt/ext/aws_ec2.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/aws_s3.py` & `data-toolkit-1.4.7/dt/ext/aws_s3.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/aws_s3_list.py` & `data-toolkit-1.4.7/dt/ext/aws_s3_list.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/aws_sg.py` & `data-toolkit-1.4.7/dt/ext/aws_sg.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/codex.py` & `data-toolkit-1.4.7/dt/ext/codex.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/config.py` & `data-toolkit-1.4.7/dt/ext/config.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/fake_data.py` & `data-toolkit-1.4.7/dt/ext/fake_data.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/firelit.py` & `data-toolkit-1.4.7/dt/ext/firelit.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/gcp.py` & `data-toolkit-1.4.7/dt/ext/gcp.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/gdrive_dl.py` & `data-toolkit-1.4.7/dt/ext/gdrive_dl.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/github.py` & `data-toolkit-1.4.7/dt/ext/github.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/gkeep.py` & `data-toolkit-1.4.7/dt/ext/gkeep.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/hist.py` & `data-toolkit-1.4.7/dt/ext/hist.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/monitor.py` & `data-toolkit-1.4.7/dt/ext/monitor.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/ms_outlook.py` & `data-toolkit-1.4.7/dt/ext/ms_outlook.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/notes.py` & `data-toolkit-1.4.7/dt/ext/notes.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/notions.py` & `data-toolkit-1.4.7/dt/ext/notions.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,30 +189,35 @@
             'Account Rejection by Bank': 1,
         },
         'Account Activation by Bank': {
             'Account Activation by Bank': 1,
         },
     }
     
+    
     for comp,idx in enumerate(companies):
         num_steps = fake.pyint(min_value=1, max_value=25)
         start_time = fake.date_time_between(start_date="-1y", end_date="now")
          
         path = []
         comments = []
     
         current_stage = 'Account Opening Request'
         transition_time = start_time
         
         
         # use the transition graph to generate a path to take the number of (unique) steps as define above
         for i in range(num_steps):
             transition_probs = transition_graph[current_stage]
-             
-            transition_time = fake.date_time_between(start_date=transition_time, end_date="now")
+            
+            # make min difference 6 hours 
+            next_time = timedelta(hours=6) + transition_time
+            
+            
+            transition_time = fake.date_time_between(start_date=next_time, end_date="now")
             rand = fake.pyfloat(min_value=0, max_value=1)
             # loop through the transitions and determine if the random number falls within the range for that transition
             for stage, prob in transition_probs.items():
                 data = {
                             "id": idx,
                             "company_id": comp,
                             "stage": current_stage,
```

### Comparing `data-toolkit-1.4.6/dt/ext/python_exec.py` & `data-toolkit-1.4.7/dt/ext/python_exec.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/run.py` & `data-toolkit-1.4.7/dt/ext/run.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/sftp_conf.py` & `data-toolkit-1.4.7/dt/ext/sftp_conf.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/ssh_params.py` & `data-toolkit-1.4.7/dt/ext/ssh_params.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/sshconf.py` & `data-toolkit-1.4.7/dt/ext/sshconf.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/tracking.py` & `data-toolkit-1.4.7/dt/ext/tracking.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/tree.py` & `data-toolkit-1.4.7/dt/ext/tree.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/ext/zshrc.txt` & `data-toolkit-1.4.7/dt/ext/zshrc.txt`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/help.py` & `data-toolkit-1.4.7/dt/help.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/main.py` & `data-toolkit-1.4.7/dt/main.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/dt/plugins/viz_utils.py` & `data-toolkit-1.4.7/dt/plugins/viz_utils.py`

 * *Files identical despite different names*

### Comparing `data-toolkit-1.4.6/setup.py` & `data-toolkit-1.4.7/setup.py`

 * *Files identical despite different names*


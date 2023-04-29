# Comparing `tmp/cliboa-2.3.1b0.tar.gz` & `tmp/cliboa-2.3.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliboa-2.3.1b0.tar", last modified: Fri Apr 28 09:16:51 2023, max compression
+gzip compressed data, was "cliboa-2.3.2b0.tar", last modified: Sat Apr 29 13:20:43 2023, max compression
```

## Comparing `cliboa-2.3.1b0.tar` & `cliboa-2.3.2b0.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.738918 cliboa-2.3.1b0/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5408 2023-04-28 09:16:51.738918 cliboa-2.3.1b0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4669 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.730918 cliboa-2.3.1b0/cliboa/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.730918 cliboa-2.3.1b0/cliboa/adapter/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/aws.py
--rw-r--r--   0 root         (0) root         (0)     1011 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/azure.py
--rw-r--r--   0 root         (0) root         (0)     3145 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/ftp.py
--rw-r--r--   0 root         (0) root         (0)     3243 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/gcp.py
--rw-r--r--   0 root         (0) root         (0)      562 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/mysql.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/postgres.py
--rw-r--r--   0 root         (0) root         (0)     3649 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/rdbms.py
--rw-r--r--   0 root         (0) root         (0)     4011 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/sftp.py
--rw-r--r--   0 root         (0) root         (0)     8565 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/sqlite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.730918 cliboa-2.3.1b0/cliboa/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6292 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/cli/cliboadmin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.730918 cliboa-2.3.1b0/cliboa/common/
--rw-r--r--   0 root         (0) root         (0)     1482 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/common/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.730918 cliboa-2.3.1b0/cliboa/conf/
--rw-r--r--   0 root         (0) root         (0)     1333 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)       58 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/conf/cliboa.ini
--rw-r--r--   0 root         (0) root         (0)     1429 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/conf/default_environment.py
--rw-r--r--   0 root         (0) root         (0)      360 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/conf/logging.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.730918 cliboa-2.3.1b0/cliboa/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2537 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/factory.py
--rw-r--r--   0 root         (0) root         (0)     7381 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/file_parser.py
--rw-r--r--   0 root         (0) root         (0)     3152 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/listener.py
--rw-r--r--   0 root         (0) root         (0)    12553 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/manager.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/scenario_queue.py
--rw-r--r--   0 root         (0) root         (0)     1848 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/step_queue.py
--rw-r--r--   0 root         (0) root         (0)     4406 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/strategy.py
--rw-r--r--   0 root         (0) root         (0)     6369 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/validator.py
--rw-r--r--   0 root         (0) root         (0)     2955 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/worker.py
--rw-r--r--   0 root         (0) root         (0)     3031 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.734918 cliboa-2.3.1b0/cliboa/scenario/
--rw-r--r--   0 root         (0) root         (0)     2253 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1732 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/aws.py
--rw-r--r--   0 root         (0) root         (0)     1718 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/azure.py
--rw-r--r--   0 root         (0) root         (0)     4554 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.734918 cliboa-2.3.1b0/cliboa/scenario/extract/
--rw-r--r--   0 root         (0) root         (0)     6328 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/aws.py
--rw-r--r--   0 root         (0) root         (0)     2402 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/azure.py
--rw-r--r--   0 root         (0) root         (0)     1470 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/file.py
--rw-r--r--   0 root         (0) root         (0)     3143 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/ftp.py
--rw-r--r--   0 root         (0) root         (0)    10166 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/gcp.py
--rw-r--r--   0 root         (0) root         (0)     3729 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/http.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/mysql.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/postgres.py
--rw-r--r--   0 root         (0) root         (0)     5575 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/sftp.py
--rw-r--r--   0 root         (0) root         (0)     1973 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/sqlite.py
--rw-r--r--   0 root         (0) root         (0)      308 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extras.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/ftp.py
--rw-r--r--   0 root         (0) root         (0)     3090 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/gcp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.734918 cliboa-2.3.1b0/cliboa/scenario/load/
--rw-r--r--   0 root         (0) root         (0)     2442 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/aws.py
--rw-r--r--   0 root         (0) root         (0)     2516 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/azure.py
--rw-r--r--   0 root         (0) root         (0)     1291 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/file.py
--rw-r--r--   0 root         (0) root         (0)     9340 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/gcp.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/mysql.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/postgres.py
--rw-r--r--   0 root         (0) root         (0)     2518 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/sftp.py
--rw-r--r--   0 root         (0) root         (0)     4178 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     6319 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/rdbms.py
--rw-r--r--   0 root         (0) root         (0)     2144 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/sample_step.py
--rw-r--r--   0 root         (0) root         (0)     2846 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/sftp.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/sqlite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.734918 cliboa-2.3.1b0/cliboa/scenario/transform/
--rw-r--r--   0 root         (0) root         (0)     3267 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/transform/aes.py
--rw-r--r--   0 root         (0) root         (0)    30540 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/transform/csv.py
--rw-r--r--   0 root         (0) root         (0)    21683 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/transform/file.py
--rw-r--r--   0 root         (0) root         (0)     5130 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/transform/gpg.py
--rw-r--r--   0 root         (0) root         (0)     3721 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/transform/json.py
--rw-r--r--   0 root         (0) root         (0)     1894 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/transform/system.py
--rw-r--r--   0 root         (0) root         (0)     2498 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.734918 cliboa-2.3.1b0/cliboa/template/
--rw-r--r--   0 root         (0) root         (0)     1214 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/Pipfile.above36
--rw-r--r--   0 root         (0) root         (0)     1238 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/Pipfile.above37
--rw-r--r--   0 root         (0) root         (0)     1237 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/Pipfile.above38
--rw-r--r--   0 root         (0) root         (0)     1237 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/Pipfile.above39
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.734918 cliboa-2.3.1b0/cliboa/template/bin/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/bin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1005 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/bin/clibomanager.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/pyproject.above37.toml
--rw-r--r--   0 root         (0) root         (0)     1282 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/pyproject.above38.toml
--rw-r--r--   0 root         (0) root         (0)     1282 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/pyproject.above39.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.738918 cliboa-2.3.1b0/cliboa/util/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2444 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/cache.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/class_util.py
--rw-r--r--   0 root         (0) root         (0)       78 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/constant.py
--rw-r--r--   0 root         (0) root         (0)     4240 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/csv.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/date.py
--rw-r--r--   0 root         (0) root         (0)     1723 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/exception.py
--rw-r--r--   0 root         (0) root         (0)     2975 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/file.py
--rw-r--r--   0 root         (0) root         (0)     4240 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/ftp_util.py
--rw-r--r--   0 root         (0) root         (0)     2598 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/gpg.py
--rw-r--r--   0 root         (0) root         (0)     1255 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/helper.py
--rw-r--r--   0 root         (0) root         (0)     3621 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/http.py
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/lisboa_log.py
--rw-r--r--   0 root         (0) root         (0)      747 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/parallel_with_config.py
--rw-r--r--   0 root         (0) root         (0)     1942 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/rdbms_util.py
--rw-r--r--   0 root         (0) root         (0)     9191 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/sftp.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.730918 cliboa-2.3.1b0/cliboa.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5408 2023-04-28 09:16:51.000000 cliboa-2.3.1b0/cliboa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2708 2023-04-28 09:16:51.000000 cliboa-2.3.1b0/cliboa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 09:16:51.000000 cliboa-2.3.1b0/cliboa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-28 09:16:51.000000 cliboa-2.3.1b0/cliboa.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 09:16:51.000000 cliboa-2.3.1b0/cliboa.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      344 2023-04-28 09:16:51.738918 cliboa-2.3.1b0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.739488 cliboa-2.3.2b0/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5408 2023-04-29 13:20:43.739488 cliboa-2.3.2b0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4669 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.727488 cliboa-2.3.2b0/cliboa/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.731488 cliboa-2.3.2b0/cliboa/adapter/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/adapter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/adapter/aws.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/adapter/azure.py
+-rw-r--r--   0 root         (0) root         (0)     3145 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/adapter/ftp.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/adapter/gcp.py
+-rw-r--r--   0 root         (0) root         (0)      562 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/adapter/mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/adapter/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/adapter/rdbms.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/adapter/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     8565 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/adapter/sqlite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.731488 cliboa-2.3.2b0/cliboa/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6292 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/cli/cliboadmin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.731488 cliboa-2.3.2b0/cliboa/common/
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/common/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.731488 cliboa-2.3.2b0/cliboa/conf/
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       58 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/conf/cliboa.ini
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/conf/default_environment.py
+-rw-r--r--   0 root         (0) root         (0)      360 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/conf/logging.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.731488 cliboa-2.3.2b0/cliboa/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/core/factory.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/core/file_parser.py
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/core/listener.py
+-rw-r--r--   0 root         (0) root         (0)    12553 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/core/manager.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/core/scenario_queue.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/core/step_queue.py
+-rw-r--r--   0 root         (0) root         (0)     4406 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/core/strategy.py
+-rw-r--r--   0 root         (0) root         (0)     6369 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/core/validator.py
+-rw-r--r--   0 root         (0) root         (0)     2955 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/core/worker.py
+-rw-r--r--   0 root         (0) root         (0)     3031 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.731488 cliboa-2.3.2b0/cliboa/scenario/
+-rw-r--r--   0 root         (0) root         (0)     2253 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/aws.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/azure.py
+-rw-r--r--   0 root         (0) root         (0)     4554 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.735488 cliboa-2.3.2b0/cliboa/scenario/extract/
+-rw-r--r--   0 root         (0) root         (0)     6328 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/extract/aws.py
+-rw-r--r--   0 root         (0) root         (0)     2402 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/extract/azure.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/extract/file.py
+-rw-r--r--   0 root         (0) root         (0)     3143 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/extract/ftp.py
+-rw-r--r--   0 root         (0) root         (0)    10166 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/extract/gcp.py
+-rw-r--r--   0 root         (0) root         (0)     3729 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/extract/http.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/extract/mysql.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/extract/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     5575 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/extract/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/extract/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/extras.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/ftp.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/gcp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.735488 cliboa-2.3.2b0/cliboa/scenario/load/
+-rw-r--r--   0 root         (0) root         (0)     2442 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/load/aws.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/load/azure.py
+-rw-r--r--   0 root         (0) root         (0)     1291 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/load/file.py
+-rw-r--r--   0 root         (0) root         (0)     9340 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/load/gcp.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/load/mysql.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/load/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     2518 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/load/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     4178 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/load/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     6319 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/rdbms.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/sample_step.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/sqlite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.735488 cliboa-2.3.2b0/cliboa/scenario/transform/
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/transform/aes.py
+-rw-r--r--   0 root         (0) root         (0)    30540 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/transform/csv.py
+-rw-r--r--   0 root         (0) root         (0)    21683 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/transform/file.py
+-rw-r--r--   0 root         (0) root         (0)     5130 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/transform/gpg.py
+-rw-r--r--   0 root         (0) root         (0)     3721 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/transform/json.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/transform/system.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/scenario/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.735488 cliboa-2.3.2b0/cliboa/template/
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/template/Pipfile.above36
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/template/Pipfile.above37
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/template/Pipfile.above38
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/template/Pipfile.above39
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/template/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.735488 cliboa-2.3.2b0/cliboa/template/bin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/template/bin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/template/bin/clibomanager.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/template/pyproject.above37.toml
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/template/pyproject.above38.toml
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/template/pyproject.above39.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.739488 cliboa-2.3.2b0/cliboa/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/cache.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/class_util.py
+-rw-r--r--   0 root         (0) root         (0)       78 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/constant.py
+-rw-r--r--   0 root         (0) root         (0)     4240 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/csv.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/date.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/exception.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/file.py
+-rw-r--r--   0 root         (0) root         (0)     4240 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/ftp_util.py
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/gpg.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/helper.py
+-rw-r--r--   0 root         (0) root         (0)     3621 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/http.py
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/lisboa_log.py
+-rw-r--r--   0 root         (0) root         (0)      747 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/parallel_with_config.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/rdbms_util.py
+-rw-r--r--   0 root         (0) root         (0)     9191 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/cliboa/util/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:20:43.727488 cliboa-2.3.2b0/cliboa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5408 2023-04-29 13:20:43.000000 cliboa-2.3.2b0/cliboa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-04-29 13:20:43.000000 cliboa-2.3.2b0/cliboa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 13:20:43.000000 cliboa-2.3.2b0/cliboa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-29 13:20:43.000000 cliboa-2.3.2b0/cliboa.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-29 13:20:43.000000 cliboa-2.3.2b0/cliboa.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      344 2023-04-29 13:20:43.739488 cliboa-2.3.2b0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2640 2023-04-29 13:20:39.000000 cliboa-2.3.2b0/setup.py
```

### Comparing `cliboa-2.3.1b0/LICENSE` & `cliboa-2.3.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/PKG-INFO` & `cliboa-2.3.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliboa
-Version: 2.3.1b0
+Version: 2.3.2b0
 Summary: application framework for ETL(ELT) processing
 Home-page: https://github.com/BrainPad/cliboa
 Author: BrainPad
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cliboa-2.3.1b0/README.md` & `cliboa-2.3.2b0/README.md`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/adapter/aws.py` & `cliboa-2.3.2b0/cliboa/adapter/aws.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/adapter/azure.py` & `cliboa-2.3.2b0/cliboa/adapter/azure.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/adapter/ftp.py` & `cliboa-2.3.2b0/cliboa/adapter/ftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/adapter/gcp.py` & `cliboa-2.3.2b0/cliboa/adapter/gcp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/adapter/mysql.py` & `cliboa-2.3.2b0/cliboa/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/adapter/postgres.py` & `cliboa-2.3.2b0/cliboa/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/adapter/rdbms.py` & `cliboa-2.3.2b0/cliboa/adapter/rdbms.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/adapter/sftp.py` & `cliboa-2.3.2b0/cliboa/adapter/sftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/adapter/sqlite.py` & `cliboa-2.3.2b0/cliboa/adapter/sqlite.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/cli/cliboadmin.py` & `cliboa-2.3.2b0/cliboa/cli/cliboadmin.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/common/environment.py` & `cliboa-2.3.2b0/cliboa/common/environment.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/conf/__init__.py` & `cliboa-2.3.2b0/cliboa/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/conf/default_environment.py` & `cliboa-2.3.2b0/cliboa/conf/default_environment.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/core/factory.py` & `cliboa-2.3.2b0/cliboa/core/factory.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/core/file_parser.py` & `cliboa-2.3.2b0/cliboa/core/file_parser.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/core/listener.py` & `cliboa-2.3.2b0/cliboa/core/listener.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/core/manager.py` & `cliboa-2.3.2b0/cliboa/core/manager.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/core/scenario_queue.py` & `cliboa-2.3.2b0/cliboa/core/scenario_queue.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/core/step_queue.py` & `cliboa-2.3.2b0/cliboa/core/step_queue.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/core/strategy.py` & `cliboa-2.3.2b0/cliboa/core/strategy.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/core/validator.py` & `cliboa-2.3.2b0/cliboa/core/validator.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/core/worker.py` & `cliboa-2.3.2b0/cliboa/core/worker.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/interface.py` & `cliboa-2.3.2b0/cliboa/interface.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/__init__.py` & `cliboa-2.3.2b0/cliboa/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/aws.py` & `cliboa-2.3.2b0/cliboa/scenario/aws.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/azure.py` & `cliboa-2.3.2b0/cliboa/scenario/azure.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/base.py` & `cliboa-2.3.2b0/cliboa/scenario/base.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/extract/aws.py` & `cliboa-2.3.2b0/cliboa/scenario/extract/aws.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/extract/azure.py` & `cliboa-2.3.2b0/cliboa/scenario/extract/azure.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/extract/file.py` & `cliboa-2.3.2b0/cliboa/scenario/extract/file.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/extract/ftp.py` & `cliboa-2.3.2b0/cliboa/scenario/extract/ftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/extract/gcp.py` & `cliboa-2.3.2b0/cliboa/scenario/extract/gcp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/extract/http.py` & `cliboa-2.3.2b0/cliboa/scenario/extract/http.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/extract/mysql.py` & `cliboa-2.3.2b0/cliboa/scenario/extract/mysql.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/extract/postgres.py` & `cliboa-2.3.2b0/cliboa/scenario/extract/postgres.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/extract/sftp.py` & `cliboa-2.3.2b0/cliboa/scenario/extract/sftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/extract/sqlite.py` & `cliboa-2.3.2b0/cliboa/scenario/extract/sqlite.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/ftp.py` & `cliboa-2.3.2b0/cliboa/scenario/ftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/gcp.py` & `cliboa-2.3.2b0/cliboa/scenario/gcp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/load/aws.py` & `cliboa-2.3.2b0/cliboa/scenario/load/aws.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/load/azure.py` & `cliboa-2.3.2b0/cliboa/scenario/load/azure.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/load/file.py` & `cliboa-2.3.2b0/cliboa/scenario/load/file.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/load/gcp.py` & `cliboa-2.3.2b0/cliboa/scenario/load/gcp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/load/mysql.py` & `cliboa-2.3.2b0/cliboa/scenario/load/mysql.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/load/postgres.py` & `cliboa-2.3.2b0/cliboa/scenario/load/postgres.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/load/sftp.py` & `cliboa-2.3.2b0/cliboa/scenario/load/sftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/load/sqlite.py` & `cliboa-2.3.2b0/cliboa/scenario/load/sqlite.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/rdbms.py` & `cliboa-2.3.2b0/cliboa/scenario/rdbms.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/sample_step.py` & `cliboa-2.3.2b0/cliboa/scenario/sample_step.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/sftp.py` & `cliboa-2.3.2b0/cliboa/scenario/sftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/sqlite.py` & `cliboa-2.3.2b0/cliboa/scenario/sqlite.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/transform/aes.py` & `cliboa-2.3.2b0/cliboa/scenario/transform/aes.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/transform/csv.py` & `cliboa-2.3.2b0/cliboa/scenario/transform/csv.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/transform/file.py` & `cliboa-2.3.2b0/cliboa/scenario/transform/file.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/transform/gpg.py` & `cliboa-2.3.2b0/cliboa/scenario/transform/gpg.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/transform/json.py` & `cliboa-2.3.2b0/cliboa/scenario/transform/json.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/transform/system.py` & `cliboa-2.3.2b0/cliboa/scenario/transform/system.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/scenario/validator.py` & `cliboa-2.3.2b0/cliboa/scenario/validator.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/template/Pipfile.above36` & `cliboa-2.3.2b0/cliboa/template/Pipfile.above36`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/template/Pipfile.above37` & `cliboa-2.3.2b0/cliboa/template/Pipfile.above37`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/template/Pipfile.above38` & `cliboa-2.3.2b0/cliboa/template/Pipfile.above38`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/template/Pipfile.above39` & `cliboa-2.3.2b0/cliboa/template/Pipfile.above39`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/template/bin/clibomanager.py` & `cliboa-2.3.2b0/cliboa/template/bin/clibomanager.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/template/pyproject.above37.toml` & `cliboa-2.3.2b0/cliboa/template/pyproject.above37.toml`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/template/pyproject.above38.toml` & `cliboa-2.3.2b0/cliboa/template/pyproject.above38.toml`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/template/pyproject.above39.toml` & `cliboa-2.3.2b0/cliboa/template/pyproject.above39.toml`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/util/cache.py` & `cliboa-2.3.2b0/cliboa/util/cache.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/util/class_util.py` & `cliboa-2.3.2b0/cliboa/util/class_util.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/util/csv.py` & `cliboa-2.3.2b0/cliboa/util/csv.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/util/date.py` & `cliboa-2.3.2b0/cliboa/util/date.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/util/exception.py` & `cliboa-2.3.2b0/cliboa/util/exception.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/util/file.py` & `cliboa-2.3.2b0/cliboa/util/file.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/util/ftp_util.py` & `cliboa-2.3.2b0/cliboa/util/ftp_util.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/util/gpg.py` & `cliboa-2.3.2b0/cliboa/util/gpg.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/util/helper.py` & `cliboa-2.3.2b0/cliboa/util/helper.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/util/http.py` & `cliboa-2.3.2b0/cliboa/util/http.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/util/parallel_with_config.py` & `cliboa-2.3.2b0/cliboa/util/parallel_with_config.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/util/rdbms_util.py` & `cliboa-2.3.2b0/cliboa/util/rdbms_util.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/util/sftp.py` & `cliboa-2.3.2b0/cliboa/util/sftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa/util/string.py` & `cliboa-2.3.2b0/cliboa/util/string.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/cliboa.egg-info/PKG-INFO` & `cliboa-2.3.2b0/cliboa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliboa
-Version: 2.3.1b0
+Version: 2.3.2b0
 Summary: application framework for ETL(ELT) processing
 Home-page: https://github.com/BrainPad/cliboa
 Author: BrainPad
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cliboa-2.3.1b0/cliboa.egg-info/SOURCES.txt` & `cliboa-2.3.2b0/cliboa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.1b0/setup.py` & `cliboa-2.3.2b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def read(filename):
     with open(path.join(path.dirname(__file__), filename), encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="cliboa",
-    version="2.3.1b0",
+    version="2.3.2b0",
     description="application framework for ETL(ELT) processing",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/BrainPad/cliboa",  # Optional
     author="BrainPad",
     # author_email='brainpad.co.jp',
     classifiers=[
```


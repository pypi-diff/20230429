# Comparing `tmp/zenutils-0.3.9.tar.gz` & `tmp/zenutils-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenutils-0.3.9.tar", last modified: Sat Oct 22 13:01:51 2022, max compression
+gzip compressed data, was "zenutils-0.4.8.tar", last modified: Sat Apr 29 03:02:08 2023, max compression
```

## Comparing `zenutils-0.3.9.tar` & `zenutils-0.4.8.tar`

### file list

```diff
@@ -1,65 +1,78 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-22 13:01:51.246810 zenutils-0.3.9/
--rw-r--r--   0 test       (501) staff       (20)     1067 2022-06-16 09:27:11.000000 zenutils-0.3.9/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      198 2022-06-17 11:16:41.000000 zenutils-0.3.9/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)    20457 2022-10-22 13:01:51.246563 zenutils-0.3.9/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)    19856 2022-10-22 12:38:16.000000 zenutils-0.3.9/README.md
--rw-r--r--   0 test       (501) staff       (20)       16 2022-06-17 10:49:49.000000 zenutils-0.3.9/requirements.py32.txt
--rw-r--r--   0 test       (501) staff       (20)        0 2022-10-22 13:01:50.000000 zenutils-0.3.9/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2022-10-22 13:01:51.246871 zenutils-0.3.9/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1617 2022-10-22 12:38:22.000000 zenutils-0.3.9/setup.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-22 13:01:51.241927 zenutils-0.3.9/zenutils/
--rw-r--r--   0 test       (501) staff       (20)      184 2022-06-19 12:22:31.000000 zenutils-0.3.9/zenutils/__init__.py
--rw-r--r--   0 test       (501) staff       (20)      602 2022-06-18 15:33:41.000000 zenutils-0.3.9/zenutils/base64utils.py
--rw-r--r--   0 test       (501) staff       (20)      308 2022-06-21 01:33:03.000000 zenutils-0.3.9/zenutils/baseutils.py
--rw-r--r--   0 test       (501) staff       (20)     3835 2022-09-02 15:28:21.000000 zenutils-0.3.9/zenutils/cacheutils.py
--rw-r--r--   0 test       (501) staff       (20)    16879 2022-06-21 06:14:08.000000 zenutils-0.3.9/zenutils/cipherutils.py
--rw-r--r--   0 test       (501) staff       (20)    13435 2022-08-09 12:44:33.000000 zenutils-0.3.9/zenutils/dictutils.py
--rw-r--r--   0 test       (501) staff       (20)    23236 2022-09-20 04:32:52.000000 zenutils-0.3.9/zenutils/fsutils.py
--rw-r--r--   0 test       (501) staff       (20)    12866 2022-10-18 06:15:35.000000 zenutils-0.3.9/zenutils/funcutils.py
--rw-r--r--   0 test       (501) staff       (20)    25718 2022-09-23 16:30:41.000000 zenutils-0.3.9/zenutils/hashutils.py
--rw-r--r--   0 test       (501) staff       (20)     3531 2022-06-19 11:53:27.000000 zenutils-0.3.9/zenutils/httputils.py
--rw-r--r--   0 test       (501) staff       (20)     9081 2022-08-14 02:47:51.000000 zenutils-0.3.9/zenutils/jsonutils.py
--rw-r--r--   0 test       (501) staff       (20)     8771 2022-09-23 15:38:47.000000 zenutils-0.3.9/zenutils/listutils.py
--rw-r--r--   0 test       (501) staff       (20)     7149 2022-09-20 14:26:52.000000 zenutils-0.3.9/zenutils/logutils.py
--rw-r--r--   0 test       (501) staff       (20)    18115 2022-06-19 14:11:01.000000 zenutils-0.3.9/zenutils/nameutils.py
--rw-r--r--   0 test       (501) staff       (20)     5499 2022-09-23 17:23:36.000000 zenutils-0.3.9/zenutils/numericutils.py
--rw-r--r--   0 test       (501) staff       (20)    10682 2022-09-28 07:15:34.000000 zenutils-0.3.9/zenutils/randomutils.py
--rw-r--r--   0 test       (501) staff       (20)     5562 2022-10-18 04:53:37.000000 zenutils-0.3.9/zenutils/sixutils.py
--rw-r--r--   0 test       (501) staff       (20)    31350 2022-06-21 07:26:11.000000 zenutils-0.3.9/zenutils/strutils.py
--rw-r--r--   0 test       (501) staff       (20)     7656 2022-10-22 12:36:18.000000 zenutils-0.3.9/zenutils/sysutils.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-22 13:01:51.246029 zenutils-0.3.9/zenutils/tests/
--rw-r--r--   0 test       (501) staff       (20)      171 2022-06-17 06:56:58.000000 zenutils-0.3.9/zenutils/tests/__init__.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-22 13:01:51.246285 zenutils-0.3.9/zenutils/tests/assets/
--rw-r--r--   0 test       (501) staff       (20)        0 2022-06-19 08:45:08.000000 zenutils-0.3.9/zenutils/tests/assets/a.txt
--rw-r--r--   0 test       (501) staff       (20)      823 2022-06-21 07:48:43.000000 zenutils-0.3.9/zenutils/tests/assets/p1.jpeg
--rw-r--r--   0 test       (501) staff       (20)      143 2022-09-23 14:14:23.000000 zenutils-0.3.9/zenutils/tests/t08_01.py
--rw-r--r--   0 test       (501) staff       (20)      481 2022-06-21 01:34:38.000000 zenutils-0.3.9/zenutils/tests/test_baseutils.py
--rw-r--r--   0 test       (501) staff       (20)     1734 2022-09-02 15:28:07.000000 zenutils-0.3.9/zenutils/tests/test_cacheutils.py
--rw-r--r--   0 test       (501) staff       (20)    15419 2022-06-21 03:54:40.000000 zenutils-0.3.9/zenutils/tests/test_cipherutils.py
--rw-r--r--   0 test       (501) staff       (20)     9329 2022-08-09 06:57:09.000000 zenutils-0.3.9/zenutils/tests/test_dictutils.py
--rw-r--r--   0 test       (501) staff       (20)     7281 2022-09-20 04:29:06.000000 zenutils-0.3.9/zenutils/tests/test_fsutils.py
--rw-r--r--   0 test       (501) staff       (20)     6765 2022-09-23 14:27:53.000000 zenutils-0.3.9/zenutils/tests/test_funcutils.py
--rw-r--r--   0 test       (501) staff       (20)     5879 2022-08-28 09:03:36.000000 zenutils-0.3.9/zenutils/tests/test_hashutils.py
--rw-r--r--   0 test       (501) staff       (20)     2818 2022-08-28 08:48:38.000000 zenutils-0.3.9/zenutils/tests/test_httputils.py
--rw-r--r--   0 test       (501) staff       (20)      807 2022-08-25 16:35:30.000000 zenutils-0.3.9/zenutils/tests/test_import_all.py
--rw-r--r--   0 test       (501) staff       (20)     1821 2022-06-21 06:30:06.000000 zenutils-0.3.9/zenutils/tests/test_jsonutils.py
--rw-r--r--   0 test       (501) staff       (20)    10045 2022-06-19 14:09:18.000000 zenutils-0.3.9/zenutils/tests/test_listutils.py
--rw-r--r--   0 test       (501) staff       (20)     1051 2022-06-21 01:39:50.000000 zenutils-0.3.9/zenutils/tests/test_logutils.py
--rw-r--r--   0 test       (501) staff       (20)      980 2022-06-19 14:09:25.000000 zenutils-0.3.9/zenutils/tests/test_nameutils.py
--rw-r--r--   0 test       (501) staff       (20)    13987 2022-09-23 17:25:31.000000 zenutils-0.3.9/zenutils/tests/test_numericutils.py
--rw-r--r--   0 test       (501) staff       (20)    54463 2022-09-28 07:22:41.000000 zenutils-0.3.9/zenutils/tests/test_randomutils.py
--rw-r--r--   0 test       (501) staff       (20)     4304 2022-10-18 04:33:14.000000 zenutils-0.3.9/zenutils/tests/test_sixutils.py
--rw-r--r--   0 test       (501) staff       (20)    27083 2022-06-21 07:36:31.000000 zenutils-0.3.9/zenutils/tests/test_strutils.py
--rw-r--r--   0 test       (501) staff       (20)     2056 2022-08-16 15:10:43.000000 zenutils-0.3.9/zenutils/tests/test_sysutils.py
--rw-r--r--   0 test       (501) staff       (20)     4540 2022-06-20 13:23:51.000000 zenutils-0.3.9/zenutils/tests/test_threadutils.py
--rw-r--r--   0 test       (501) staff       (20)     3151 2022-08-05 14:11:47.000000 zenutils-0.3.9/zenutils/tests/test_treeutils.py
--rw-r--r--   0 test       (501) staff       (20)     5116 2022-06-19 14:09:58.000000 zenutils-0.3.9/zenutils/tests/test_typingutils.py
--rw-r--r--   0 test       (501) staff       (20)    20792 2022-08-03 06:49:45.000000 zenutils-0.3.9/zenutils/threadutils.py
--rw-r--r--   0 test       (501) staff       (20)     4029 2022-08-05 14:09:17.000000 zenutils-0.3.9/zenutils/treeutils.py
--rw-r--r--   0 test       (501) staff       (20)     7917 2022-06-21 01:35:25.000000 zenutils-0.3.9/zenutils/typingutils.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-22 13:01:51.242579 zenutils-0.3.9/zenutils.egg-info/
--rw-r--r--   0 test       (501) staff       (20)    20457 2022-10-22 13:01:51.000000 zenutils-0.3.9/zenutils.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     1537 2022-10-22 13:01:51.000000 zenutils-0.3.9/zenutils.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2022-10-22 13:01:51.000000 zenutils-0.3.9/zenutils.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2022-10-22 13:01:50.000000 zenutils-0.3.9/zenutils.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)        9 2022-10-22 13:01:51.000000 zenutils-0.3.9/zenutils.egg-info/top_level.txt
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-29 03:02:08.273943 zenutils-0.4.8/
+-rw-r--r--   0 test       (501) staff       (20)     1067 2023-03-09 12:54:10.000000 zenutils-0.4.8/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      198 2022-06-17 11:16:41.000000 zenutils-0.4.8/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)    22941 2023-04-29 03:02:08.273795 zenutils-0.4.8/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)    22379 2023-04-29 03:01:59.000000 zenutils-0.4.8/README.md
+-rw-r--r--   0 test       (501) staff       (20)       16 2022-06-17 10:49:49.000000 zenutils-0.4.8/requirements.py32.txt
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-04-29 03:02:07.000000 zenutils-0.4.8/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2023-04-29 03:02:08.273978 zenutils-0.4.8/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1664 2023-04-29 03:02:04.000000 zenutils-0.4.8/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-29 03:02:08.269200 zenutils-0.4.8/zenutils/
+-rw-r--r--   0 test       (501) staff       (20)      218 2023-04-19 02:53:36.000000 zenutils-0.4.8/zenutils/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      664 2023-04-20 03:01:50.000000 zenutils-0.4.8/zenutils/base64utils.py
+-rw-r--r--   0 test       (501) staff       (20)      370 2023-04-28 16:14:26.000000 zenutils-0.4.8/zenutils/baseutils.py
+-rw-r--r--   0 test       (501) staff       (20)     4917 2023-04-20 02:52:09.000000 zenutils-0.4.8/zenutils/cacheutils.py
+-rw-r--r--   0 test       (501) staff       (20)    17069 2023-04-20 02:52:47.000000 zenutils-0.4.8/zenutils/cipherutils.py
+-rw-r--r--   0 test       (501) staff       (20)      881 2023-04-20 02:52:57.000000 zenutils-0.4.8/zenutils/dateutils.py
+-rw-r--r--   0 test       (501) staff       (20)    14746 2023-04-29 02:37:41.000000 zenutils-0.4.8/zenutils/dictutils.py
+-rw-r--r--   0 test       (501) staff       (20)    27016 2023-04-29 02:27:06.000000 zenutils-0.4.8/zenutils/errorutils.py
+-rw-r--r--   0 test       (501) staff       (20)    23276 2023-04-20 02:53:46.000000 zenutils-0.4.8/zenutils/fsutils.py
+-rw-r--r--   0 test       (501) staff       (20)    17947 2023-04-28 16:06:17.000000 zenutils-0.4.8/zenutils/funcutils.py
+-rw-r--r--   0 test       (501) staff       (20)    26607 2023-04-28 16:13:15.000000 zenutils-0.4.8/zenutils/hashutils.py
+-rw-r--r--   0 test       (501) staff       (20)     3579 2023-04-20 02:54:41.000000 zenutils-0.4.8/zenutils/httputils.py
+-rw-r--r--   0 test       (501) staff       (20)     2650 2023-04-20 02:54:51.000000 zenutils-0.4.8/zenutils/importutils.py
+-rw-r--r--   0 test       (501) staff       (20)     9113 2023-04-20 02:56:33.000000 zenutils-0.4.8/zenutils/jsonutils.py
+-rw-r--r--   0 test       (501) staff       (20)     8815 2023-04-20 02:56:43.000000 zenutils-0.4.8/zenutils/listutils.py
+-rw-r--r--   0 test       (501) staff       (20)     7310 2023-04-20 02:56:51.000000 zenutils-0.4.8/zenutils/logutils.py
+-rw-r--r--   0 test       (501) staff       (20)    23173 2023-04-20 02:57:01.000000 zenutils-0.4.8/zenutils/nameutils.py
+-rw-r--r--   0 test       (501) staff       (20)     5553 2023-04-20 02:57:09.000000 zenutils-0.4.8/zenutils/numericutils.py
+-rw-r--r--   0 test       (501) staff       (20)     2285 2023-04-20 02:57:21.000000 zenutils-0.4.8/zenutils/packutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1594 2023-04-20 02:57:30.000000 zenutils-0.4.8/zenutils/perfutils.py
+-rw-r--r--   0 test       (501) staff       (20)    11099 2023-04-20 02:57:38.000000 zenutils-0.4.8/zenutils/randomutils.py
+-rw-r--r--   0 test       (501) staff       (20)     6555 2023-04-24 12:39:02.000000 zenutils-0.4.8/zenutils/serviceutils.py
+-rw-r--r--   0 test       (501) staff       (20)     5603 2023-04-20 02:58:07.000000 zenutils-0.4.8/zenutils/sixutils.py
+-rw-r--r--   0 test       (501) staff       (20)     6448 2023-04-20 02:58:25.000000 zenutils-0.4.8/zenutils/socketserverutils.py
+-rw-r--r--   0 test       (501) staff       (20)    31798 2023-04-24 11:43:46.000000 zenutils-0.4.8/zenutils/strutils.py
+-rw-r--r--   0 test       (501) staff       (20)     7857 2023-04-20 02:58:48.000000 zenutils-0.4.8/zenutils/sysutils.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-29 03:02:08.273357 zenutils-0.4.8/zenutils/tests/
+-rw-r--r--   0 test       (501) staff       (20)      171 2022-06-17 06:56:58.000000 zenutils-0.4.8/zenutils/tests/__init__.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-29 03:02:08.273615 zenutils-0.4.8/zenutils/tests/assets/
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-06-19 08:45:08.000000 zenutils-0.4.8/zenutils/tests/assets/a.txt
+-rw-r--r--   0 test       (501) staff       (20)      823 2022-06-21 07:48:43.000000 zenutils-0.4.8/zenutils/tests/assets/p1.jpeg
+-rw-r--r--   0 test       (501) staff       (20)      143 2022-09-23 14:14:23.000000 zenutils-0.4.8/zenutils/tests/t08_01.py
+-rw-r--r--   0 test       (501) staff       (20)      481 2022-06-21 01:34:38.000000 zenutils-0.4.8/zenutils/tests/test_baseutils.py
+-rw-r--r--   0 test       (501) staff       (20)     2194 2023-04-20 02:25:44.000000 zenutils-0.4.8/zenutils/tests/test_cacheutils.py
+-rw-r--r--   0 test       (501) staff       (20)    15419 2022-06-21 03:54:40.000000 zenutils-0.4.8/zenutils/tests/test_cipherutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1246 2022-11-29 02:04:49.000000 zenutils-0.4.8/zenutils/tests/test_dateutils.py
+-rw-r--r--   0 test       (501) staff       (20)    10883 2023-04-29 02:40:02.000000 zenutils-0.4.8/zenutils/tests/test_dictutils.py
+-rw-r--r--   0 test       (501) staff       (20)     4573 2022-11-23 12:36:21.000000 zenutils-0.4.8/zenutils/tests/test_errorutils.py
+-rw-r--r--   0 test       (501) staff       (20)     7281 2022-09-20 04:29:06.000000 zenutils-0.4.8/zenutils/tests/test_fsutils.py
+-rw-r--r--   0 test       (501) staff       (20)     8677 2023-04-28 16:03:25.000000 zenutils-0.4.8/zenutils/tests/test_funcutils.py
+-rw-r--r--   0 test       (501) staff       (20)     6123 2023-04-29 00:46:11.000000 zenutils-0.4.8/zenutils/tests/test_hashutils.py
+-rw-r--r--   0 test       (501) staff       (20)     2818 2022-08-28 08:48:38.000000 zenutils-0.4.8/zenutils/tests/test_httputils.py
+-rw-r--r--   0 test       (501) staff       (20)     1020 2022-11-23 06:59:43.000000 zenutils-0.4.8/zenutils/tests/test_import_all.py
+-rw-r--r--   0 test       (501) staff       (20)     2502 2022-11-23 08:06:56.000000 zenutils-0.4.8/zenutils/tests/test_importutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1821 2022-06-21 06:30:06.000000 zenutils-0.4.8/zenutils/tests/test_jsonutils.py
+-rw-r--r--   0 test       (501) staff       (20)    10045 2022-06-19 14:09:18.000000 zenutils-0.4.8/zenutils/tests/test_listutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1051 2022-06-21 01:39:50.000000 zenutils-0.4.8/zenutils/tests/test_logutils.py
+-rw-r--r--   0 test       (501) staff       (20)      980 2022-06-19 14:09:25.000000 zenutils-0.4.8/zenutils/tests/test_nameutils.py
+-rw-r--r--   0 test       (501) staff       (20)    13971 2022-11-20 03:51:51.000000 zenutils-0.4.8/zenutils/tests/test_numericutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1187 2022-11-20 04:12:31.000000 zenutils-0.4.8/zenutils/tests/test_packutils.py
+-rw-r--r--   0 test       (501) staff       (20)    54463 2022-09-28 07:22:41.000000 zenutils-0.4.8/zenutils/tests/test_randomutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1746 2022-11-20 03:15:03.000000 zenutils-0.4.8/zenutils/tests/test_serviceutils.py
+-rw-r--r--   0 test       (501) staff       (20)     4304 2022-10-18 04:33:14.000000 zenutils-0.4.8/zenutils/tests/test_sixutils.py
+-rw-r--r--   0 test       (501) staff       (20)    27083 2022-06-21 07:36:31.000000 zenutils-0.4.8/zenutils/tests/test_strutils.py
+-rw-r--r--   0 test       (501) staff       (20)     2056 2022-08-16 15:10:43.000000 zenutils-0.4.8/zenutils/tests/test_sysutils.py
+-rw-r--r--   0 test       (501) staff       (20)     6447 2023-04-27 15:34:56.000000 zenutils-0.4.8/zenutils/tests/test_threadutils.py
+-rw-r--r--   0 test       (501) staff       (20)     3151 2022-08-05 14:11:47.000000 zenutils-0.4.8/zenutils/tests/test_treeutils.py
+-rw-r--r--   0 test       (501) staff       (20)     5116 2022-06-19 14:09:58.000000 zenutils-0.4.8/zenutils/tests/test_typingutils.py
+-rw-r--r--   0 test       (501) staff       (20)    27192 2023-04-25 06:15:12.000000 zenutils-0.4.8/zenutils/threadutils.py
+-rw-r--r--   0 test       (501) staff       (20)     4299 2023-04-20 03:01:07.000000 zenutils-0.4.8/zenutils/treeutils.py
+-rw-r--r--   0 test       (501) staff       (20)     8202 2023-04-20 03:01:17.000000 zenutils-0.4.8/zenutils/typingutils.py
+-rw-r--r--   0 test       (501) staff       (20)     3054 2023-04-20 03:17:04.000000 zenutils-0.4.8/zenutils/xmlrpcutils.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-29 03:02:08.269775 zenutils-0.4.8/zenutils.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)    22941 2023-04-29 03:02:08.000000 zenutils-0.4.8/zenutils.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     1900 2023-04-29 03:02:08.000000 zenutils-0.4.8/zenutils.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-04-29 03:02:08.000000 zenutils-0.4.8/zenutils.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-04-29 03:02:08.000000 zenutils-0.4.8/zenutils.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)        9 2023-04-29 03:02:08.000000 zenutils-0.4.8/zenutils.egg-info/top_level.txt
```

### Comparing `zenutils-0.3.9/LICENSE` & `zenutils-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/setup.py` & `zenutils-0.4.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 
 import os
 from io import open
 from setuptools import setup
 from setuptools import find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-with open(os.path.join(here, 'README.md'), "r", encoding="utf-8") as fobj:
+with open(os.path.join(here, "README.md"), "r", encoding="utf-8") as fobj:
     long_description = fobj.read()
 
 requires = []
-with open(os.path.join(here, 'requirements.txt'), "r", encoding="utf-8") as fobj:
+with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires += [x.strip() for x in fobj.readlines() if x.strip()]
 if os.sys.version_info.major == 3 and os.sys.version_info.minor <= 2:
-    with open(os.path.join(here, 'requirements.py32.txt'), "r", encoding="utf-8") as fobj:
+    with open(
+        os.path.join(here, "requirements.py32.txt"), "r", encoding="utf-8"
+    ) as fobj:
         requires += [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="zenutils",
-    version="0.3.9",
+    version="0.4.8",
     description="Collection of simple utils.",
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     author="zencore",
     author_email="dobetter@zencore.cn",
     license="MIT",
     license_files=("LICENSE",),
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
     ],
     keywords=["zenutils"],
     install_requires=requires,
     packages=find_packages("."),
     zip_safe=False,
     include_package_data=True,
 )
```

### Comparing `zenutils-0.3.9/zenutils/base64utils.py` & `zenutils-0.4.8/zenutils/base64utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
-import base64
+"""BASE64相关工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
+import base64
+
 __all__ = [] + base64.__all__
 
 from base64 import *
 
 _globals = globals()
 
 if not "encodebytes" in _globals and "encodestring" in _globals:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.3.9/zenutils/cacheutils.py` & `zenutils-0.4.8/zenutils/cacheutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""缓存相关工具。
+"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 import functools
 
 __all__ = [
     "get_cached_value",
     "cache",
 ]
 
+
 def get_cached_value(holder_object, cache_key, getter, *args, **kwargs):
     """Get cached value from an holder_object and set the cache value at the first request.
 
     @Returns:
         (Any): The cahced value or the getter returned value.
-    
+
     @Parameters:
         holder_object(Any): The holder object which holds the cache property.
         cache_key(str): The cache property which will attach to the holder object.
         getter(Callable): The callable object which will be called if there is no cache value.
         *args(Any): Place holder parameters which will be used by getter.
         **kwargs(Any): Keyword parameters which will be used by getter.
 
@@ -28,23 +39,23 @@
         value = get_cached_value(request, "cache_key_for_get_user_info", services.get_user_info, token=token)
     """
     cache_key = force_text(cache_key)
     if not hasattr(holder_object, cache_key):
         setattr(holder_object, cache_key, getter(*args, **kwargs))
     return getattr(holder_object, cache_key)
 
+
 def cache(holder_object=None, cache_key=None):
     """
+    @param holder_object Any: The holder object which holds the cache property.
+    @param cache_key str: The cache property which will attach to the holder object.
+
     @Notice:
         If your only give one parameter, then the parameter will be treated as cache_key.
 
-    @Parameters:
-        holder_object(Any): The holder object which holds the cache property.
-        cache_key(str): The cache property which will attach to the holder object.
-
     @Example:
         a = Object()
         @cacheutils.cache(a, "_num")
         def getNum():
             return random.randint(0, 10)
         v1 = getNum()
         v2 = getNum()
@@ -87,21 +98,54 @@
             # 这样以来在inner函数中就没有对holder_object变量的任何修改
             # 这时在inner函数中就可以取出宿主函数变量holder_object
             if (holder_object is None) and (cache_key is None):
                 holder_object_inner = args[0]
                 cache_key_inner = args[1]
                 args = args[2:]
             elif holder_object is None:
-                holder_object_inner = args[0] 
+                holder_object_inner = args[0]
                 cache_key_inner = cache_key
                 args = args[1:]
             else:
                 holder_object_inner = holder_object
                 cache_key_inner = cache_key
             if hasattr(holder_object_inner, cache_key_inner):
                 return getattr(holder_object_inner, cache_key_inner)
             else:
                 result = func(*args, **kwargs)
                 setattr(holder_object_inner, cache_key_inner, result)
                 return result
+
         return inner
+
     return outer
+
+
+class ReqIdCache(object):
+    """用于reqid的缓存。
+
+    基本思路是分批保存，分批清理。
+    """
+
+    def __init__(self, bucket_size=100 * 10000, bucket_cout=10):
+        self.bucket_size = bucket_size
+        self.bucket_count = bucket_cout
+        self.buckets = []
+        for _ in range(self.bucket_count):
+            self.buckets.append(set())
+        self.current_bucket = 0
+
+    def add(self, reqid):
+        """将新的reqid添加到缓存池中。"""
+        if len(self.buckets[self.current_bucket]) >= self.bucket_size:
+            # 循环使用n个缓存池。
+            self.current_bucket += 1
+            self.current_bucket = self.current_bucket % self.bucket_count
+            self.buckets[self.current_bucket] = set()
+        self.buckets[self.current_bucket].add(reqid)
+
+    def exists(self, reqid):
+        """判断当前reqid是否在缓存池中。"""
+        for i in range(self.bucket_count):
+            if reqid in self.buckets[i]:
+                return True
+        return False
```

### Comparing `zenutils-0.3.9/zenutils/cipherutils.py` & `zenutils-0.4.8/zenutils/cipherutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""加解密工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 __all__ = [
     "DecryptFailed",
     "EncoderBase",
     "RawDataEncoder",
     "HexlifyEncoder",
@@ -20,92 +29,99 @@
     "S12Cipher",
 ]
 
 import json
 import binascii
 import string
 
+
 class DecryptFailed(RuntimeError):
     pass
 
-class EncoderBase(object):
 
+class EncoderBase(object):
     def encode(self, data):
         raise NotImplementedError()
 
     def decode(self, data):
         raise NotImplementedError()
 
-class RawDataEncoder(EncoderBase):
 
+class RawDataEncoder(EncoderBase):
     def encode(self, data):
         return data
-    
+
     def decode(self, data):
         return data
 
-class HexlifyEncoder(EncoderBase):
 
+class HexlifyEncoder(EncoderBase):
     def encode(self, data):
         if data is None:
             return None
         return binascii.hexlify(data).decode()
 
     def decode(self, data):
         if data is None:
             return None
         return binascii.unhexlify(data.encode("utf-8"))
 
-class Base64Encoder(EncoderBase):
 
+class Base64Encoder(EncoderBase):
     def encode(self, data):
         from zenutils import strutils
         from zenutils import base64utils
+
         if data is None:
             return None
         data = force_bytes(data)
         return strutils.join_lines(strutils.force_text(base64utils.encodebytes(data)))
 
     def decode(self, data):
         from zenutils import strutils
         from zenutils import base64utils
+
         if data is None:
             return None
         data = strutils.force_bytes(data)
         return base64utils.decodebytes(data)
 
-class SafeBase64Encoder(EncoderBase):
 
+class SafeBase64Encoder(EncoderBase):
     def encode(self, data):
         from zenutils import strutils
         from zenutils import base64utils
+
         if data is None:
             return None
         data = force_bytes(data)
-        return strutils.join_lines(strutils.force_text(base64utils.urlsafe_b64encode(data)))
+        return strutils.join_lines(
+            strutils.force_text(base64utils.urlsafe_b64encode(data))
+        )
 
     def decode(self, data):
         from zenutils import strutils
         from zenutils import base64utils
+
         if data is None:
             return None
         data = force_bytes(data)
         return base64utils.urlsafe_b64decode(data)
 
+
 class Utf8Encoder(EncoderBase):
-    
     def encode(self, data):
         """Turn utf8 decodable bytes to string.
 
         @Returns:
             (str): The result string.
-        
+
         @Parameters:
             data(bytes): Utf8 decodable bytes.
-        
+
         @Example:
             encoder = Utf8Encoder()
             data1 = "测试".encode("utf-8")
             data2 = encoder.encode(data1)
             data3 = encoder.decode(data2)
             assert data1 == data3
             assert data2 = "测试"
@@ -115,39 +131,40 @@
         return data.decode("utf-8")
 
     def decode(self, data):
         """Turn utf8 encodable str to utf8 encoded bytes.
 
         @Returns:
             (bytes): The result bytes.
-        
+
         @Parameters:
             data(str): Utf8 encodable str.
-        
+
         @Example:
             encoder = Utf8Encoder()
             data1 = "测试".encode("utf-8")
             data2 = encoder.encode(data1)
             data3 = encoder.decode(data2)
             assert data1 == data3
             assert data2 = "测试"
         """
         if not data:
             return None
         return data.encode("utf-8")
 
-class _SimpleCipher(object):
 
+class _SimpleCipher(object):
     def __init__(self, encrypt, decrypt):
         self.encrypt = encrypt
         self.decrypt = decrypt
 
+
 class CipherBase(object):
-    """params: password, result_encoder, force_text, text_encoding, cipher_core, encrypt, decrypt, encrypt_kwargs, decrypt_kwargs
-    """
+    """params: password, result_encoder, force_text, text_encoding, cipher_core, encrypt, decrypt, encrypt_kwargs, decrypt_kwargs"""
+
     default_encrypt_force_bytes = True
     default_decrypt_force_bytes = True
     default_encrypt_kwargs = {}
     default_decrypt_kwargs = {}
     default_result_encoder = None
     default_force_text = None
     default_text_encoding = None
@@ -164,62 +181,82 @@
             "text_encoding": self.default_text_encoding,
             "cipher_core": self.default_cipher_core,
         }
         if hasattr(self, "defaults"):
             defaults.update(getattr(self, "defaults"))
         return defaults
 
-    def __init__(self, 
-            password=None,
-            encrypt_force_bytes=None,
-            decrypt_force_bytes=None,
-            encrypt_kwargs=None,
-            decrypt_kwargs=None,
-            result_encoder=None,
-            force_text=None,
-            text_encoding=None,
-            cipher_core=None,
-            encrypt=None,
-            decrypt=None,
-            kwargs=None, **extra_kwargs):
+    def __init__(
+        self,
+        password=None,
+        encrypt_force_bytes=None,
+        decrypt_force_bytes=None,
+        encrypt_kwargs=None,
+        decrypt_kwargs=None,
+        result_encoder=None,
+        force_text=None,
+        text_encoding=None,
+        cipher_core=None,
+        encrypt=None,
+        decrypt=None,
+        kwargs=None,
+        **extra_kwargs
+    ):
         from zenutils import listutils
         from zenutils import funcutils
+
         kwargs = kwargs or {}
         defaults = self.get_defaults()
         self.password = password
-        self.encrypt_force_bytes = listutils.first(encrypt_force_bytes, defaults["encrypt_force_bytes"], True)
-        self.decrypt_force_bytes = listutils.first(decrypt_force_bytes, defaults["decrypt_force_bytes"], True)
-        self.result_encoder = listutils.first(result_encoder, defaults["result_encoder"], RawDataEncoder())
+        self.encrypt_force_bytes = listutils.first(
+            encrypt_force_bytes, defaults["encrypt_force_bytes"], True
+        )
+        self.decrypt_force_bytes = listutils.first(
+            decrypt_force_bytes, defaults["decrypt_force_bytes"], True
+        )
+        self.result_encoder = listutils.first(
+            result_encoder, defaults["result_encoder"], RawDataEncoder()
+        )
         self.force_text = listutils.first(force_text, defaults["force_text"], False)
-        self.text_encoding = listutils.first(text_encoding, defaults["text_encoding"], "utf-8")
+        self.text_encoding = listutils.first(
+            text_encoding, defaults["text_encoding"], "utf-8"
+        )
         self.cipher_core = listutils.first(cipher_core, defaults["cipher_core"], None)
-        self.encrypt_kwargs = listutils.first(encrypt_kwargs, defaults["encrypt_kwargs"], {})
-        self.decrypt_kwargs = listutils.first(decrypt_kwargs, defaults["decrypt_kwargs"], {})
+        self.encrypt_kwargs = listutils.first(
+            encrypt_kwargs, defaults["encrypt_kwargs"], {}
+        )
+        self.decrypt_kwargs = listutils.first(
+            decrypt_kwargs, defaults["decrypt_kwargs"], {}
+        )
         for key, value in kwargs.items():
             self.encrypt_kwargs.setdefault(key, value)
             self.decrypt_kwargs.setdefault(key, value)
         self.kwargs = extra_kwargs
         self.cipher_instance = None
         if self.cipher_core:
-            self.cipher_instance = funcutils.call_with_inject(self.cipher_core, self.kwargs)
+            self.cipher_instance = funcutils.call_with_inject(
+                self.cipher_core, self.kwargs
+            )
         else:
             if encrypt or decrypt:
                 self.cipher_instance = _SimpleCipher(encrypt, decrypt)
 
     def encrypt(self, data, **kwargs):
         from zenutils import strutils
+
         if data is None:
             return None
         if self.encrypt_force_bytes:
             data = strutils.force_bytes(data, self.text_encoding)
         encrypted_data = self.do_encrypt(data, **kwargs)
         return self.result_encoder.encode(encrypted_data)
 
     def decrypt(self, text, **kwargs):
         from zenutils import strutils
+
         if text is None:
             return None
         data = self.result_encoder.decode(text)
         if self.decrypt_force_bytes:
             data = strutils.force_bytes(data, self.text_encoding)
         decrypted_data = self.do_decrypt(data, **kwargs)
         if self.force_text:
@@ -241,14 +278,15 @@
             context = {}
             context.update(self.decrypt_kwargs)
             context.update(kwargs)
             return self.cipher_instance.decrypt(data, context)
         else:
             return NotImplementedError("NO decrypt method...")
 
+
 class IvCipher(CipherBase):
     """Int value encryption and decryption cipher.
 
     Example:
 
     In [38]: from fastutils import cipherutils
 
@@ -264,31 +302,34 @@
     4 205
     5 253
     6 294
     7 339
     8 364
     9 447
     """
+
     default_encrypt_force_bytes = False
     default_decrypt_force_bytes = False
 
     def __init__(self, password, **kwargs):
         self.password = password
         self.iv_params = self.get_iv_params()
         super(IvCipher, self).__init__(passowrd=password, **kwargs)
 
     def get_iv_params(self):
         from zenutils import randomutils
+
         gen = randomutils.Random(self.password)
         n = gen.randint(1024, 9999)
         iv = [gen.randint(1, 100) for _ in range(n)]
         return n, iv
 
     def do_encrypt(self, number, **kwargs):
         from zenutils import strutils
+
         number = strutils.force_int(number)
         flag = False
         if number < 0:
             number = -1 * number
             flag = True
         n, iv = self.iv_params
         s = sum(iv)
@@ -297,14 +338,15 @@
         r = a * s + sum(iv[:b])
         if flag:
             r = -1 * r
         return r
 
     def do_decrypt(self, number, **kwargs):
         from zenutils import strutils
+
         number = strutils.force_int(number)
         flag = False
         if number < 0:
             number = -1 * number
             flag = True
         n, iv = self.iv_params
         s = sum(iv)
@@ -320,14 +362,15 @@
                     break
             if t != number:
                 raise DecryptFailed("iv_decrypt failed: number={}".format(number))
         if flag:
             r = -1 * r
         return r
 
+
 class IvfCipher(IvCipher):
     """Float value encryption and decryption cipher.
 
     Example:
 
     In [41]: from fastutils import cipherutils
 
@@ -344,24 +387,25 @@
     4 +0000000000020016127691 <class 'str'>
     5 +0000000000025020160338 <class 'str'>
     6 +0000000000030024191109 <class 'str'>
     7 +0000000000035028221552 <class 'str'>
     8 +0000000000040032254031 <class 'str'>
     9 +0000000000045036286491 <class 'str'>
     """
+
     def __init__(self, password, int_digits=12, float_digits=4, **kwargs):
         """password is required.
         int_digits is the max length of int part value. Add 0 padding to left.
         float_digits is the max length of float part value. Add 0 padding to right.
         """
         self.int_digits = int_digits
         self.float_digits = float_digits
         self.module = 10 ** (float_digits * 2)
         self.max_value_length = float_digits * 2 + self.int_digits + 2
-        self.max = 10 ** self.max_value_length - 1
+        self.max = 10**self.max_value_length - 1
         self.value_template = "{:0%dd}" % self.max_value_length
         super(IvfCipher, self).__init__(password=password, **kwargs)
 
     def do_encrypt(self, number, **kwargs):
         number = int(number * self.module)
         number = super(IvfCipher, self).do_encrypt(number)
         if number >= 0:
@@ -379,81 +423,87 @@
         if self.float_digits == 0:
             number = int(number)
         if sign == "*":
             return -1 * number
         else:
             return number
 
+
 class MappingCipher(CipherBase):
     """Turn every byte to another value.
 
     0 -> b'randseed01'
     1 -> b'randseed02'
     ... -> ...
     255 -> b'randseed03'
 
     """
+
     def __init__(self, password=None, **kwargs):
         from zenutils import randomutils
+
         super(MappingCipher, self).__init__(password=password, **kwargs)
         self.password = password
         self.seeds = self.try_to_load_seeds(password)
         if not self.seeds:
             self.randomGenerator = randomutils.Random(password)
             self.seeds = self.get_seeds()
         self.encrypt_mapping = self.get_encrypt_mapping()
         self.decrypt_mapping = self.get_decrypt_mapping()
 
     def get_seeds(self):
         raise NotImplementedError()
 
     def get_encrypt_mapping(self):
         from zenutils import numericutils
+
         mapping = {}
         for i in range(256):
             mapping[numericutils.int2bytes(i)] = self.seeds[i]
         return mapping
-    
+
     def get_decrypt_mapping(self):
         from zenutils import numericutils
+
         mapping = {}
         for i in range(256):
             mapping[self.seeds[i]] = numericutils.int2bytes(i)
         return mapping
-    
+
     def do_encrypt(self, data, **kwargs):
         if data is None:
             return None
         data = bytes_to_array(data)
         empty = b""
         result = empty.join([self.encrypt_mapping[c] for c in data])
         return result
-    
+
     def do_decrypt(self, data, **kwargs):
         if data is None:
             return None
         result = b""
         data_length = len(data)
         max_seed_length = max([len(x) for x in self.decrypt_mapping.keys()])
         start = 0
         while start < data_length:
             found = False
-            for seed_length in range(1, max_seed_length+1):
-                seed = data[start: start+seed_length]
+            for seed_length in range(1, max_seed_length + 1):
+                seed = data[start : start + seed_length]
                 if seed in self.decrypt_mapping:
                     result += self.decrypt_mapping[seed]
                     start += seed_length
                     found = True
                     break
             if not found:
                 raise DecryptFailed()
         return result
 
     def dumps(self):
         from zenutils import strutils
+
         seeds = [binascii.hexlify(x).decode() for x in self.seeds]
         data = strutils.force_bytes(json.dumps(seeds))
         data = strutils.force_text(binascii.hexlify(data))
         return data
 
     @classmethod
     def loads(cls, data):
@@ -472,49 +522,53 @@
             return None
 
     @classmethod
     def password_to_key(cls, password):
         cipher = cls(password=password)
         return cipher.dumps()
 
+
 class S1Cipher(MappingCipher):
     """Turn every byte to another byte randomly by the password.
 
     b'\x00' -> b'\x8f'
     b'\x01' -> b'\x8d'
     ...
     b'\xff' -> b'\xd8'
     """
 
     def get_seeds(self):
         from zenutils import numericutils
+
         seeds = list(range(256))
         self.randomGenerator.shuffle(seeds)
         return [numericutils.int2bytes(x) for x in seeds]
 
+
 class S2Cipher(MappingCipher):
     """Turn every byte to two ascii_lowercase str randomly by the password.
 
     b'\x00' -> "si"
     b'\x01' -> "xs"
     ...
     b'\xff' -> "xy"
     """
 
     def get_seeds(self):
         letters = string.ascii_lowercase
         seeds = set()
         for a in letters:
             for b in letters:
-                seeds.add(a+b)
+                seeds.add(a + b)
         seeds = list(seeds)
         self.randomGenerator.shuffle(seeds)
         seeds = [x.encode() for x in seeds[:256]]
         return seeds
 
+
 class S12Cipher(MappingCipher):
     """Turn every byte to two random bytes that keeps the order.
 
     b'\x00' -> b"\x01\x0d"
     b'\x01' -> b"\x01\x1a"
     ...
     b'\xff' -> b"\xef\xcc"
```

### Comparing `zenutils-0.3.9/zenutils/dictutils.py` & `zenutils-0.4.8/zenutils/dictutils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""字典类型工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
-from zenutils.baseutils import Null
 
 __all__ = [
+    "fix_object",
+    "to_object",
     "Object",
     "deep_merge",
     "select",
     "touch",
     "attrgetorset",
     "attrset",
     "update",
     "ignore_none_item",
     "change",
     "changes",
     "prefix_key",
     "diff",
-    "fix_object",
-    "to_object",
+    "HttpHeadersDict",
 ]
 
+from zenutils.baseutils import Null
+from functools import partial
+
 
 def fix_object(data):
     if isinstance(data, dict):
         keys = list(data.keys())
         for key in keys:
             data[key] = to_object(data[key])
     elif isinstance(data, list):
@@ -32,14 +44,15 @@
             data[index] = to_object(data[index])
     elif isinstance(data, set):
         data2 = list(data)
         data.clear()
         for item in data2:
             data.add(to_object(item))
 
+
 def to_object(data):
     if isinstance(data, Object):
         return data
     elif isinstance(data, dict):
         result = Object()
         for key, value in data.items():
             if isinstance(value, dict):
@@ -59,36 +72,43 @@
     elif isinstance(data, tuple):
         data = list(data)
         for index in range(len(data)):
             data[index] = to_object(data[index])
         return tuple(data)
     return data
 
+
 class Object(dict):
     """Dict object allow use dot path selector.
 
     Example:
 
     In [32]: from zenutils import dictutils
-    
+
     In [33]: config = dictutils.Object()
 
     In [34]: config.listen = ('0.0.0.0', 6379)
 
     In [35]: config.listen
     Out[35]: ('0.0.0.0', 6379)
 
     In [36]: config['listen']
     Out[36]: ('0.0.0.0', 6379)
 
     In [39]: config['debug'] = True
 
     In [40]: config.debug
     Out[40]: True
+
+    注意：
+
+    1. dictutils.Object([1, 2, 3])将报错。初始化数据的顶层必须为dict类型。
+    2. dictutils.Object({"a": [1, 2, 3]})是允许的。
     """
+
     def __init__(self, *args, **kwargs):
         super(Object, self).__init__(*args, **kwargs)
         fix_object(self)
         for key, value in self.items():
             setattr(self, key, value)
 
     def __setitem__(self, key, value):
@@ -136,18 +156,37 @@
     def clear(self):
         keys = list(super(Object, self).keys())
         result = super(Object, self).clear()
         for key in keys:
             if hasattr(self, key):
                 delattr(self, key)
         return result
-    
+
     def copy(self):
         return Object(super(Object, self).copy())
 
+    def select(self, path, default_value=None):
+        data = self
+        paths = path.split(".")
+        for path in paths:
+            if isinstance(data, dict) and path in data:
+                data = data[path]
+            elif (
+                isinstance(data, (list, tuple))
+                and path.isdigit()
+                and int(path) < len(data)
+            ):
+                data = data[int(path)]
+            elif hasattr(data, path):
+                data = getattr(data, path)
+            else:
+                return default_value
+        return data
+
+
 def deep_merge(target, data):
     """Merge the second dict into the first one deeply. Always returns the first dict reference.
 
     Example:
 
     In [14]: from zenutils import dictutils
 
@@ -164,15 +203,16 @@
         value1 = target.get(key2, None)
         if isinstance(value1, dict) and isinstance(value2, dict):
             deep_merge(value1, value2)
         else:
             target[key2] = value2
     return target
 
-def select(data, path, default_value= None):
+
+def select(data, path, default_value=None, slient=True):
     """Get field value in dot sperated path.
 
     Example:
 
     In [6]: from zenutils import dictutils
 
     In [7]: data = {
@@ -183,38 +223,55 @@
     ...: }
     ...: }
 
     In [8]: dictutils.select(data, "a.b.c")
     Out[8]: 'abc'
 
     """
-    paths = path.split(".")
-    for path in paths:
-        if isinstance(data, dict) and path in data:
-            data = data[path]
-        elif isinstance(data, (list, tuple)) and path.isdigit() and int(path) < len(data):
-            data = data[int(path)]
-        elif hasattr(data, path):
-            data = getattr(data, path)
+
+    def _(value, slient, path):
+        if slient:
+            return value
         else:
-            return default_value
-    return data
+            raise KeyError(path)
+
+    default = partial(_, default_value, slient, path)
+    names = path.split(".")
+    node = data
+    for name in names:
+        if isinstance(node, dict):
+            try:
+                node = node[name]
+            except:
+                return default()
+        elif isinstance(node, list) and name.isdigit():
+            try:
+                node = node[int(name)]
+            except:
+                return default()
+        elif hasattr(node, name):
+            node = getattr(node, name)
+        else:
+            return default()
+    return node
+
 
 def touch(data, path, default_value):
     """Make sure data has the path.
     If data has the path, return the orignal value.
     If data NOT has the path, create a new path, and set to default_value, returns the default value.
     """
     result = select(data, path, Null)
     if result == Null:
         update(data, path, default_value)
         return default_value
     else:
         return result
 
+
 def attrgetorset(data, key, default_value):
     """Get or set attr to data directly, and the key is a one level key.
     If data contains the key, get the original value.
     If data NOT contains the key, set the key to the default value.
     """
     if isinstance(data, dict):
         if not key in data:
@@ -228,14 +285,15 @@
             data[key] = default_value
         return data[key]
     else:
         if not hasattr(data, key):
             setattr(data, key, default_value)
         return getattr(data, key)
 
+
 def attrset(data, key, value):
     """Set attr to data directory, and the key is a one level key.
     If data contains the key, overrdie the original value with the new value.
     If data NOT contains the key, add a new key to the new value.
     """
     if isinstance(data, dict):
         data[key] = value
@@ -244,14 +302,15 @@
         if key >= len(data):
             for _ in range(key + 1 - len(data)):
                 data.append(None)
         data[key] = value
     else:
         setattr(data, key, value)
 
+
 def update(data, path, value):
     """Set attr to data, and the key is a dot-seperated-path.
 
     If data contains the key, override the original value with the new value.
     If data NOT contains the key, add a new key to the new value.
 
 
@@ -270,14 +329,15 @@
             else:
                 next_empty_value = {}
         data = attrgetorset(data, path, next_empty_value)
     path = paths[-1]
     attrset(data, path, value)
     return old_data
 
+
 def ignore_none_item(data):
     """Returns a new dict that only contains empty-value field.
 
     None, empty list, empty dict: are treat as empty values.
     0, empty string, False: are NOT empty values.
 
     Example:
@@ -302,57 +362,83 @@
             continue
         if not value:
             if isinstance(value, (list, dict)):
                 continue
         result[key] = value
     return result
 
-def change(object_instance, data_dict, object_key, dict_key=None, do_update=True, ignore_empty_value=False):
-    """Update property value of object_instance, using the value from data_dict. If value changed, return True. If value is equals, return False.
-    """
+
+def change(
+    object_instance,
+    data_dict,
+    object_key,
+    dict_key=None,
+    do_update=True,
+    ignore_empty_value=False,
+):
+    """Update property value of object_instance, using the value from data_dict. If value changed, return True. If value is equals, return False."""
     dict_key = dict_key or object_key
     if isinstance(object_instance, dict):
         object_value = object_instance.get(object_key, None)
     else:
         object_value = getattr(object_instance, object_key, None)
     if isinstance(data_dict, dict):
         dict_value = data_dict.get(dict_key, None)
     else:
         dict_value = getattr(data_dict, dict_key, None)
-    if (object_value == dict_value) or (ignore_empty_value and (object_value == "" or object_value == None) and (dict_value == "" or dict_value == None)):
+    if (object_value == dict_value) or (
+        ignore_empty_value
+        and (object_value == "" or object_value == None)
+        and (dict_value == "" or dict_value == None)
+    ):
         return False
     else:
         if do_update:
             if isinstance(object_instance, dict):
                 object_instance[object_key] = dict_value
             else:
                 setattr(object_instance, object_key, dict_value)
         return True
 
-def changes(object_instance, data_dict, keys, return_changed_keys=False, do_update=True, ignore_empty_value=False):
-    """Update property values of object_instance, using the value form data_dict. If any property changed, return True. If values are equal, return False. keys is a list of string or string pair.
-    """
+
+def changes(
+    object_instance,
+    data_dict,
+    keys,
+    return_changed_keys=False,
+    do_update=True,
+    ignore_empty_value=False,
+):
+    """Update property values of object_instance, using the value form data_dict. If any property changed, return True. If values are equal, return False. keys is a list of string or string pair."""
     result = False
     changed_keys = []
     for key in keys:
         if isinstance(key, (tuple, set, list)) and len(key) > 1:
             object_key = key[0]
             dict_key = key[1]
         else:
             object_key = key
             dict_key = None
-        changed = change(object_instance, data_dict, object_key, dict_key, do_update=do_update, ignore_empty_value=ignore_empty_value)
+        changed = change(
+            object_instance,
+            data_dict,
+            object_key,
+            dict_key,
+            do_update=do_update,
+            ignore_empty_value=ignore_empty_value,
+        )
         if changed:
             changed_keys.append(object_key)
             result = True
     if return_changed_keys:
         return result, changed_keys
     else:
         return result
 
+
 def prefix_key(data, prefix):
     """Add a prefix for all keys.
 
     Example:
 
     In [41]: from zenutils import dictutils
 
@@ -362,35 +448,35 @@
     """
     data2 = {}
     for key, value in data.items():
         key = prefix + key.capitalize()
         data2[key] = value
     return data2
 
+
 def diff(object_instance1, object_instance2):
-    """Find keys that changed. Returns: created_keys, updated_keys, deleted_keys
-    """
+    """Find keys that changed. Returns: created_keys, updated_keys, deleted_keys"""
     deleted_keys = []
     updated_keys = []
     created_keys = []
 
     keys1 = set(object_instance1.keys())
     keys2 = set(object_instance2.keys())
 
     deleted_keys = list(keys1 - keys2)
     created_keys = list(keys2 - keys1)
     both_keys = keys1.intersection(keys2)
     for key in both_keys:
         if object_instance1[key] != object_instance2[key]:
             updated_keys.append(key)
-    
+
     return created_keys, updated_keys, deleted_keys
 
-class HttpHeadersDict(object):
 
+class HttpHeadersDict(object):
     def __init__(self, data=None):
         self.data = []
         if isinstance(data, dict):
             for key, value in data.items():
                 self.data.append((key, value))
         elif isinstance(data, list):
             for key, value in data:
@@ -407,44 +493,43 @@
     def add_header(self, name, value):
         name = name.title()
         self.data.append((name, value))
         return True
 
     def delete_header(self, name):
         name = name.title()
-        for index in range(len(self.data)-1, -1, -1):
+        for index in range(len(self.data) - 1, -1, -1):
             if self.data[index][0] == name:
                 del self.data[index]
                 return True
         return False
 
     def replace_header(self, name, value):
         name = name.title()
         delete_flag = False
         new_flag = True
-        for index in range(len(self.data)-1, -1, -1):
+        for index in range(len(self.data) - 1, -1, -1):
             if self.data[index][0] == name:
                 if delete_flag:
                     del self.data[index]
                 else:
                     self.data[index] = (name, value)
                     delete_flag = True
                     new_flag = False
         if new_flag:
             self.data.append((name, value))
         return True
 
     def get(self, name):
         name = name.title()
-        for index in range(len(self.data)-1, -1, -1):
+        for index in range(len(self.data) - 1, -1, -1):
             if self.data[index][0] == name:
                 return self.data[index][1]
         return None
 
     def getlist(self, name):
         name = name.title()
         values = []
         for index in range(len(self.data)):
             if self.data[index][0] == name:
                 values.append(self.data[index][1])
         return values
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.3.9/zenutils/fsutils.py` & `zenutils-0.4.8/zenutils/fsutils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""文件工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 __all__ = [
     "mkdir",
     "rm",
     "filecopy",
     "treecopy",
@@ -42,54 +51,56 @@
 import datetime
 from uuid import uuid4
 from io import open
 
 try:
     FileExistsError
 except NameError:
-    FileExistsError = OSError # required by python 2.7
+    FileExistsError = OSError  # required by python 2.7
+
 
 def mkdir(folder):
     """Create a folder if it's not exists.
 
     @Returns:
-        (bool): True means the folder exists or created. 
+        (bool): True means the folder exists or created.
                 False means create the folder failed, or there is already a file take the folder's name.
 
     @Parameters:
         folder(str): The folder's name.
-    
+
     @Examples:
         assert fsutils.mkdir("a") is True
         assert fsutils.touch("b")
         assert fsutils.mkdir("b") is False
     """
     folder = os.path.abspath(folder)
     if not os.path.exists(folder):
         try:
             try:
                 os.makedirs(folder, exist_ok=True)
-            except TypeError: # fix for py2 that doesn't known the exist_ok parameter
+            except TypeError:  # fix for py2 that doesn't known the exist_ok parameter
                 os.makedirs(folder)
         except FileExistsError:
             pass
     return os.path.exists(folder) and os.path.isdir(folder)
 
+
 def rm(filename):
-    """Make sure a file or a directory has been deleted.
-    """
+    """Make sure a file or a directory has been deleted."""
     if os.path.exists(filename):
         if os.path.isfile(filename):
             os.unlink(filename)
         else:
             shutil.rmtree(filename, ignore_errors=True, onerror=None)
         return not os.path.exists(filename)
     else:
         return True
 
+
 def filecopy(src, dst, dst_is_a_folder=None):
     """Copy a file from src to dst. If dst_is_a_folder=True, then copy the src file to the dst folder and keeps the same name.
 
     Exmaples:
 
         filecopy("a.txt", "b.txt") # copy a.txt to file b.txt.
         filecopy("a.txt", "b") # copy a.txt to file b.
@@ -99,115 +110,140 @@
     if dst_is_a_folder is None:
         if os.path.exists(dst) and os.path.isdir(dst):
             dst_is_a_folder = True
         else:
             dst_is_a_folder = False
     elif dst_is_a_folder is False:
         if os.path.exists(dst) and os.path.isdir(dst):
-            raise ValueError("There is already a folder named: {dst}, you can NOT copy to it with dst_is_a_folder flag is True...".format(
-                dst=dst,
-            ))
+            raise ValueError(
+                "There is already a folder named: {dst}, you can NOT copy to it with dst_is_a_folder flag is True...".format(
+                    dst=dst,
+                )
+            )
     if dst_is_a_folder:
         src_name = os.path.basename(src)
         dst = os.path.join(dst, src_name)
     shutil.copy2(src, dst)
 
+
 def treecopy(src, dst, keep_src_folder_name=True):
-    """Copy a folder from src to dst. If keep_src_folder_name=True, copy the src folder to the dst folder and keeps the same name.
-    """
+    """Copy a folder from src to dst. If keep_src_folder_name=True, copy the src folder to the dst folder and keeps the same name."""
     if keep_src_folder_name:
         src_name = os.path.basename(src)
         dst = os.path.join(dst, src_name)
     shutil.copytree(src, dst)
 
+
 def copy(src, dst, keep_src_folder_name=True, dst_is_a_folder=False):
     if os.path.exists(src):
         if os.path.isfile(src):
             filecopy(src, dst, dst_is_a_folder)
         else:
             treecopy(src, dst, keep_src_folder_name)
 
+
 def pathjoin(path1, path2):
-    """Concat two paths.
-    """
+    """Concat two paths."""
     return os.path.abspath(os.path.join(path1, path2))
 
+
 def readfile(filename, binary=False, encoding="utf-8", default=None):
-    """Read content from file. Return default value if the file not exists.
-    """
+    """Read content from file. Return default value if the file not exists."""
     if not os.path.exists(filename):
         return default
     if binary:
         with open(filename, "rb") as fobj:
             return fobj.read()
     else:
         with open(filename, "r", encoding=encoding) as fobj:
             return fobj.read()
 
+
 def write(filename, data, encoding="utf-8"):
-    """Write content data to file.
-    """
+    """Write content data to file."""
     folder = os.path.dirname(filename)
     mkdir(folder)
     if isinstance(data, bytes):
         with open(filename, "wb") as fobj:
             fobj.write(data)
     else:
         with open(filename, "w", encoding=encoding) as fobj:
             fobj.write(data)
 
+
 def get_swap_filename(filename, prefix=".", suffix=".swap", add_random_suffix=True):
-    """Get a swap filename.
-    """
+    """Get a swap filename."""
     from zenutils import strutils
 
     folder, filename = os.path.split(filename)
     final_filename = ""
     if prefix:
         final_filename += prefix
     final_filename += filename
     if suffix:
         final_filename += suffix
     if add_random_suffix:
         final_filename += "." + strutils.random_string(8)
     return os.path.join(folder, final_filename)
 
-def safe_write(filename, data, encoding="utf-8", swap_prefix=".", swap_suffix=".swap", swap_add_random_suffix=True):
-    """Write content to a swap file and then rename it to the target filename.
-    """
-    swap_filename = get_swap_filename(filename, prefix=swap_prefix, suffix=swap_suffix, add_random_suffix=swap_add_random_suffix)
+
+def safe_write(
+    filename,
+    data,
+    encoding="utf-8",
+    swap_prefix=".",
+    swap_suffix=".swap",
+    swap_add_random_suffix=True,
+):
+    """Write content to a swap file and then rename it to the target filename."""
+    swap_filename = get_swap_filename(
+        filename,
+        prefix=swap_prefix,
+        suffix=swap_suffix,
+        add_random_suffix=swap_add_random_suffix,
+    )
     write(swap_filename, data, encoding)
     rename(swap_filename, filename)
 
+
 def get_temp_workspace(prefix="", makedir=True):
     """Create a temp folder and return it's path.
 
     @todo: the new workspace folder should be deleted after use.
     """
     folder_name = prefix + str(uuid4())
     path = os.path.abspath(os.path.join(tempfile.gettempdir(), folder_name))
     if makedir:
         mkdir(path)
     return path
 
+
 def rename(filepath, name):
-    """Only change filename or directory name, but CAN not change the path, e.g. /a/b.txt -> /a/c.txt is ok, /a/b.txt -> /b/b.txt is NOT ok.
-    """
+    """Only change filename or directory name, but CAN not change the path, e.g. /a/b.txt -> /a/c.txt is ok, /a/b.txt -> /b/b.txt is NOT ok."""
     name = os.path.basename(name)
     folder = os.path.dirname(filepath)
     dst = os.path.abspath(os.path.join(folder, name))
     os.rename(filepath, dst)
     return dst
 
+
 def move(src, dst):
-    """Move a file or a folder to another place.
-    """
+    """Move a file or a folder to another place."""
     os.rename(src, dst)
 
-def file_content_replace(filename, original, replacement, binary=False, encoding="utf-8", ignore_errors=True, **kwargs):
+
+def file_content_replace(
+    filename,
+    original,
+    replacement,
+    binary=False,
+    encoding="utf-8",
+    ignore_errors=True,
+    **kwargs
+):
     """Repleace file content.
 
     filename: The file to be replace. If filename is a folder name, then all files under the folder will be replaced.
     original: String to be replace. The string will be removed from the file.
     replacement: String used to do replace. The string will be appear in the file.
     """
     file_replaced = []
@@ -237,75 +273,79 @@
                 except Exception as error:
                     file_failed[path] = error
                     if not ignore_errors:
                         raise error
 
     return file_replaced, file_failed
 
+
 def touch(filename):
-    """Make sure a file exists
-    """
+    """Make sure a file exists"""
     if os.path.exists(filename):
         os.utime(filename, (time.time(), time.time()))
     else:
         with open(filename, "wb") as _:
             pass
     return os.stat(filename)
 
+
 def expand(filename):
     """Expand user and expand vars.
 
     @Returns:
         (str): Returns expended filename.
-    
+
     @Parameters:
         filename(str): The filename template to be expanded.
-    
+
     @Examples:
         asserts fsutils.expand("~/a.txt") == "/Users/test/a.txt"
     """
     return os.path.abspath(os.path.expandvars(os.path.expanduser(filename)))
 
+
 def expands(*filenames):
     """Expand user and expand vars for the given filenames.
 
     @Returns:
         (list of string): Returns expended filenames.
-    
+
     @Parameters:
         *filenames(str, multiple): Filenames.
-    
+
     @Example:
         assert fsutils.expends("~/a.txt") == ["/Users/test/a.txt"]
     """
     results = []
     for filename in filenames:
         results.append(expand(filename))
     return results
 
+
 def first_exists_file(*filenames, **kwargs):
     """Return the first exists file's abspath. If none file exists, return None.
 
     @Returns:
         (str): The first exists file's abspath.
-    
+
     @Parameters:
         *filenames(str, multiple): Filenames.
         default(str or None, keyword parameter): The default filename if all the given filenames is not exists.
-    
+
     @Examples:
         assert first_exists_file("a.txt", "b.txt", "c.txt", default="failback.txt") == "failback.txt"
     """
     default = kwargs.get("default", None)
     for filename in filenames:
         filename = expand(filename)
         if os.path.exists(filename):
             return os.path.abspath(filename)
     return default
 
+
 def get_application_config_paths(appname, name="config", suffix="yml"):
     return expands(
         "./{0}-{1}.{2}".format(appname, name, suffix),
         "./conf/{0}-{1}.{2}".format(appname, name, suffix),
         "./etc/{0}-{1}.{2}".format(appname, name, suffix),
         "~/.{0}/{1}.{2}".format(appname, name, suffix),
         "~/{0}/{1}.{2}".format(appname, name, suffix),
@@ -313,31 +353,33 @@
         "./conf/{0}.{1}".format(name, suffix),
         "./etc/{0}.{1}".format(name, suffix),
         "~/{0}.{1}".format(name, suffix),
         "~/.{0}.{1}".format(name, suffix),
         "{0}.{1}".format(name, suffix),
     )
 
+
 def get_application_config_filepath(appname, name="config", suffix="yml"):
     """Get application config filepath by search these places:
-        ./{appname}-{name}.{suffix}
-        ./conf/{appname}-{name}.{suffix}
-        ./etc/{appname}-{name}.{suffix}
-        ~/.{appname}/{name}.{suffix}
-        ~/{appname}/{name}.{suffix}
-        ./{name}.{suffix}
-        ./conf/{name}.{suffix}
-        ./etc/{name}.{suffix}
-        ~/{name}.{suffix}
-        ~/.{name}.{suffix}
-        {name}.{suffix}
+    ./{appname}-{name}.{suffix}
+    ./conf/{appname}-{name}.{suffix}
+    ./etc/{appname}-{name}.{suffix}
+    ~/.{appname}/{name}.{suffix}
+    ~/{appname}/{name}.{suffix}
+    ./{name}.{suffix}
+    ./conf/{name}.{suffix}
+    ./etc/{name}.{suffix}
+    ~/{name}.{suffix}
+    ~/.{name}.{suffix}
+    {name}.{suffix}
     """
     paths = get_application_config_paths(appname, name, suffix)
     return first_exists_file(*paths)
 
+
 def info(filename):
     """Get file information.
 
     In [1]: from zenutils import fsutils
 
     In [2]: fsutils.info('README.md')
     Out[2]:
@@ -357,27 +399,29 @@
         "abspath": os.path.abspath(filename),
         "size": stat.st_size,
         "atime": datetime.datetime.fromtimestamp(stat.st_atime),
         "ctime": datetime.datetime.fromtimestamp(stat.st_ctime),
         "mode": stat.st_mode,
     }
 
+
 size_unit_names = [
     "B",
     "KB",
     "MB",
     "GB",
     "TB",
     "PB",
     "EB",
     "ZB",
     "YB",
 ]
 
-size_unit_upper_limit = [1024 ** (index+1) for index, _ in enumerate(size_unit_names)]
+size_unit_upper_limit = [1024 ** (index + 1) for index, _ in enumerate(size_unit_names)]
+
 
 def get_size_deviation(unit_name):
     """Get the deviation of 1000-based-size and 1024-based-size.
 
     In [37]: from zenutils import fsutils
 
     In [38]: for unit_name in fsutils.size_unit_names:
@@ -392,24 +436,25 @@
     EB => 0.13263826201159645
     ZB => 0.15296705274569966
     YB => 0.17281938744697234       # 1000-based-size is 17.281938744697234 % less than 1024-based-size.
 
     """
     unit_name = unit_name.upper()
     x = size_unit_names.index(unit_name)
-    return 1 - (1000 ** x) / (1024 ** x)
+    return 1 - (1000**x) / (1024**x)
+
 
 def get_unit_size(unit_name, kb_size=1024):
-    """base is the size of KB, choices are 1000 or 1024.
-    """
+    """base is the size of KB, choices are 1000 or 1024."""
     unit_name = unit_name.upper()
     if not unit_name.endswith("B"):
         unit_name += "B"
     return kb_size ** size_unit_names.index(unit_name)
 
+
 def get_size_display(size_in_bytes, gap=""):
     """Turn size in bytes to human readable display.
 
     In [35]: from zenutils import fsutils
 
     In [36]: for i in range(30):
         ...:     value = 10**i
@@ -449,19 +494,20 @@
     final_index = 0
     final_upper_limit = 1
     for index, upper_limit in enumerate(size_unit_upper_limit[:-1]):
         if upper_limit > size_in_bytes:
             break
         final_index = index + 1
         final_upper_limit = upper_limit
-    display = "{0:.2f}".format(size_in_bytes/final_upper_limit)
-    if size_in_bytes%final_upper_limit == 0:
+    display = "{0:.2f}".format(size_in_bytes / final_upper_limit)
+    if size_in_bytes % final_upper_limit == 0:
         display = display.rstrip("0").rstrip(".")
     return display + gap + size_unit_names[final_index]
 
+
 class TemporaryFile(object):
     """Temporary file manager class.
 
     In [9]: from zenutils import fsutils
 
     In [10]: filepath = None
         ...: with fsutils.TemporaryFile() as fman:
@@ -481,45 +527,50 @@
 
     In [12]: os.path.exists(filepath) # out of the with block, the temporary file is deleted
     Out[12]: False
 
     In [13]: filepath
     Out[13]: 'C:\\\\Users\\\\\test\\\\AppData\\\\Local\\\\Temp\\\\639f49cf-e3be-42b6-923b-1c5c37c024fb'
     """
-    def __init__(self, content=None, encoding="utf-8", workspace=None, filename_prefix="", filename_suffix="", touch_file=True):
+
+    def __init__(
+        self,
+        content=None,
+        encoding="utf-8",
+        workspace=None,
+        filename_prefix="",
+        filename_suffix="",
+        touch_file=True,
+    ):
         self.workspace = workspace or tempfile.gettempdir()
         mkdir(self.workspace)
         self.filename = filename_prefix + str(uuid4()) + filename_suffix
         self.filepath = os.path.join(self.workspace, self.filename)
         if content:
             write(self.filepath, content, encoding)
         elif touch_file:
             touch(self.filepath)
         self.fobj = None
 
     def __enter__(self):
-        """Start of the with scope.
-        """
+        """Start of the with scope."""
         return self
-    
+
     def __exit__(self, type, value, traceback):
-        """End of the with scope.
-        """
+        """End of the with scope."""
         self.close()
         self.delete()
 
     def __del__(self):
-        """When the TemporaryFile instance is deleting, close the file handler and delete the file first.
-        """
+        """When the TemporaryFile instance is deleting, close the file handler and delete the file first."""
         self.close()
         self.delete()
 
     def delete(self):
-        """Delete the temporary file. Will be automatically called when the TemporaryFile instance deleting.
-        """
+        """Delete the temporary file. Will be automatically called when the TemporaryFile instance deleting."""
         if self.filepath and os.path.exists(self.filepath):
             os.unlink(self.filepath)
 
     def open(self, *args, **kwargs):
         """Open or Reopen the file and get it's file handler.
 
         Example:
@@ -538,48 +589,47 @@
 
         """
         self.close()
         self.fobj = open(self.filepath, *args, **kwargs)
         return self
 
     def close(self):
-        """Close the file handler. Will be automatically called when the TemporaryFile instance deleting.
-        """
+        """Close the file handler. Will be automatically called when the TemporaryFile instance deleting."""
         if self.fobj:
             self.fobj.close()
             self.fobj = None
 
     @property
     def buffer(self):
         return self.fobj.buffer
 
     @property
     def closed(self):
         return self.fobj.closed
-    
+
     def detach(self, *args, **kwargs):
         return self.fobj.detach(*args, **kwargs)
 
     @property
     def encoding(self):
         return self.fobj.encoding
-    
+
     @property
     def errors(self):
         return self.fobj.errors
-    
+
     def fileno(self, *args, **kwargs):
         return self.fobj.fileno(*args, **kwargs)
-    
+
     def flush(self, *args, **kwargs):
         return self.fobj.flush(*args, **kwargs)
-    
+
     def isatty(self, *args, **kwargs):
         return self.fobj.isatty(*args, **kwargs)
-    
+
     @property
     def line_buffering(self):
         return self.fobj.line_buffering
 
     @property
     def mode(self):
         return self.fobj.mode
@@ -587,57 +637,58 @@
     @property
     def name(self):
         return self.fobj.name
 
     @property
     def newlines(self):
         return self.fobj.newlines
-    
+
     def read(self, *args, **kwargs):
         return self.fobj.read(*args, **kwargs)
-    
+
     def readable(self, *args, **kwargs):
         return self.fobj.readable(*args, **kwargs)
-    
+
     def readline(self, *args, **kwargs):
         return self.fobj.readline(*args, **kwargs)
-    
+
     def readlines(self, *args, **kwargs):
         return self.readlines(*args, **kwargs)
-    
+
     def reconfigure(self, *args, **kwargs):
         return self.fobj.reconfigure(*args, **kwargs)
-    
+
     def seek(self, *args, **kwargs):
         return self.fobj.seek(*args, **kwargs)
-    
+
     def seekable(self, *args, **kwargs):
         return self.fobj.seekable(*args, **kwargs)
 
     def truncate(self, *args, **kwargs):
         return self.fobj.truncate(*args, **kwargs)
-    
+
     def writable(self, *args, **kwargs):
         return self.fobj.writable(*args, **kwargs)
-    
+
     def write(self, *args, **kwargs):
         return self.fobj.write(*args, **kwargs)
-    
+
     @property
     def write_through(self):
         return self.fobj.write_through
-    
+
     def writelines(self, *args, **kwargs):
         return self.fobj.writelines(*args, **kwargs)
 
+
 NT_FILENAME_CHAR_REPLACEMENTS = {
     "<": "_",
     ">": "_",
     ":": "_",
-    "\"": "'",
+    '"': "'",
     "/": "_",
     "\\": "_",
     "|": "_",
     "*": "_",
     "?": "_",
     "\x00": "",
     "\x01": "",
@@ -670,26 +721,26 @@
     "\x1C": "",
     "\x1D": "",
     "\x1E": "",
     "\x1F": "",
 }
 POSIX_FILENAME_CHAR_REPLACEMENTS = {
     "/": "_",
-    "'": '\"',
+    "'": '"',
     "\x00": "",
 }
 DARWIN_FILENAME_CHAR_REPLACEMENTS = {
     ":": "_",
 }
 ALL_PLATFORM_FILENAME_CHAR_REPLACEMENTS = {
     "<": "_",
     ">": "_",
     ":": "_",
-    "\"": "_",
-    "'": '_',
+    '"': "_",
+    "'": "_",
     "/": "_",
     "\\": "_",
     "|": "_",
     "*": "_",
     "?": "_",
     "\x00": "",
     "\x01": "",
@@ -724,15 +775,15 @@
     "\x1E": "",
     "\x1F": "",
 }
 NT_FILENAME_RESERVED = [
     "CON",
     "PRN",
     "AUX",
-    "NUL", 
+    "NUL",
     "COM1",
     "COM2",
     "COM3",
     "COM4",
     "COM5",
     "COM6",
     "COM7",
@@ -744,23 +795,24 @@
     "LPT4",
     "LPT5",
     "LPT6",
     "LPT7",
     "LPT8",
     "LPT9",
 ]
-NT_FILENAME_RESERVED = ["^"+x+"(\\..*)?$" for x in NT_FILENAME_RESERVED]
+NT_FILENAME_RESERVED = ["^" + x + "(\\..*)?$" for x in NT_FILENAME_RESERVED]
 
 for _key in NT_FILENAME_CHAR_REPLACEMENTS:
     assert _key in ALL_PLATFORM_FILENAME_CHAR_REPLACEMENTS
 for _key in POSIX_FILENAME_CHAR_REPLACEMENTS:
     assert _key in ALL_PLATFORM_FILENAME_CHAR_REPLACEMENTS
 for _key in DARWIN_FILENAME_CHAR_REPLACEMENTS:
     assert _key in ALL_PLATFORM_FILENAME_CHAR_REPLACEMENTS
 
+
 def get_safe_filename(filename, for_all_platform=True):
     """Replace bad chars in filename and return the filename safe for create a file.
 
     The filename MUST be a basename of a filename, MUST NOT include any dir name.
 
     @Examples:
         assert get_safe_filename("a<b.txt") == "a_b.txt"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.3.9/zenutils/hashutils.py` & `zenutils-0.4.8/zenutils/hashutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""哈希工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils import strutils
 from zenutils import base64utils
 from zenutils.sixutils import *
 
 import os
 import binascii
 
@@ -62,210 +71,225 @@
 for _method_name in hashlib.algorithms_available:
     _method_name_lower = _method_name.lower()
     _method_name_lower = _method_name_lower.replace("-", "_")
     algorithms_available.add(_method_name_lower)
     algorithms_name_mapping[_method_name_lower] = _method_name
 DEFAULT_HASH_METHOD = "sm3"
 DEFAULT_PASSWORD_HASH_METHOD = "ssm3"
-DEFAULT_BUFFER_SIZE = 1024*1024
+DEFAULT_BUFFER_SIZE = 1024 * 1024
+
 
 # ##################################################################################
 # RESULT ENCODER AREA
 # ##################################################################################
 class ResultEncoderBase(object):
-
     @classmethod
     def encode(cls, result):
         raise NotImplementedError()
 
     classmethod
+
     def decode(cls, result):
         raise NotImplementedError()
 
-class DigestResultEncoder(ResultEncoderBase):
 
+class DigestResultEncoder(ResultEncoderBase):
     @classmethod
     def encode(cls, result):
         return result
 
     classmethod
+
     def decode(cls, result):
         return result
 
-class Base64ResultEncoder(ResultEncoderBase):
 
+class Base64ResultEncoder(ResultEncoderBase):
     @classmethod
     def encode(cls, result):
         return strutils.join_lines(TEXT(base64utils.encodebytes(result)))
 
     classmethod
+
     def decode(cls, result):
         return base64utils.decodebytes(BYTES(result))
 
-class HexlifyResultEncoder(ResultEncoderBase):
 
+class HexlifyResultEncoder(ResultEncoderBase):
     @classmethod
     def encode(cls, result):
         return TEXT(binascii.hexlify(result))
 
     @classmethod
     def decode(cls, result):
         return binascii.unhexlify(BYTES(result))
 
+
 DEFAULT_RESULT_ENCODER = HexlifyResultEncoder
 
 # ##################################################################################
 # HASH METHOD LOADER BASE AREA
 # ##################################################################################
 HASH_METHOD_LOADERS = {}
 
+
 def setup_hash_method_loader(name, loader):
     algorithms_available.add(name)
     HASH_METHOD_LOADERS[name] = loader
 
+
 def new(method, *args, **kwargs):
-    """New hash generator instance.
-    """
+    """New hash generator instance."""
     method = method.lower().strip()
     if method in HASH_METHOD_LOADERS:
         return method_load(method)(*args, **kwargs)
     else:
         method = algorithms_name_mapping.get(method, method)
         return hashlib.new(method, *args, **kwargs)
 
+
 def method_load(method):
     """Get hash generator class by method name.
 
     @Returns:
         (hash generator class)
-    
+
     @Parameters:
         method(str, bytes, hash generator class): Hash generator class name.
     """
     if isinstance(method, (BYTES_TYPE, STR_TYPE)):
         method = force_text(method)
         loader = HASH_METHOD_LOADERS.get(method, None)
         if loader:
             return loader()
         else:
-            return lambda : new(method)
+            return lambda: new(method)
     else:
         return method
 
+
 def is_the_same_hash_method(method1, method2):
-    """Use a random buffer hash code to test if the method1 and method2 are the same hash method.
-    """
+    """Use a random buffer hash code to test if the method1 and method2 are the same hash method."""
     buffer = os.urandom(1024)
     gen1 = method1()
     gen2 = method2()
     gen1.update(buffer)
     gen2.update(buffer)
     return gen1.digest() == gen1.digest()
 
+
 # ##################################################################################
 # HASH METHOD LOADER REGISTER AREA
 # ##################################################################################
 _hashlib_has_sm3_flag = None
+
+
 def get_sm3_class():
     """
     load sm3 class from sm3utils.
     zenutils is not deps on sm3utils, so you need to install sm3utils by yourself.
     """
     global _hashlib_has_sm3_flag
     if _hashlib_has_sm3_flag is None:
         try:
             hashlib.new("sm3")
             _hashlib_has_sm3_flag = True
         except:
             _hashlib_has_sm3_flag = False
     if _hashlib_has_sm3_flag:
-        return lambda : hashlib.new("sm3")
+        return lambda: hashlib.new("sm3")
     else:
         try:
             from sm3utils import sm3
         except ImportError:
             msg = "Sm3 in not avaiable in hashlib of your python installation. We need a third party library sm3utils, which is not a part of zenutils. You need to installed sm3utils by yourself, or put it into your project's requirements.txt."
-            logger.error()
+            logger.error(msg)
             raise RuntimeError(msg)
         return sm3
 
+
 def get_sha_class():
     """
     alias sha1 as sha
     """
-    return lambda : hashlib.new("sha1")
+    return lambda: hashlib.new("sha1")
+
 
 def get_xxh128_class():
     try:
         from xxhash import xxh128
     except ImportError:
         msg = "xxh128 hash requires library xxhash, which is not a part of zenutils. You need to installed xxhash by yourself, or put it into your project's requirements.txt."
         logger.error(msg)
         raise RuntimeError(msg)
     return xxh128
 
+
 def get_xxh64_class():
     try:
         from xxhash import xxh64
     except ImportError:
         msg = "xxh64 hash requires library xxhash, which is not a part of zenutils. You need to installed xxhash by yourself, or put it into your project's requirements.txt."
         logger.error(msg)
         raise RuntimeError(msg)
     return xxh64
 
+
 def get_xxh32_class():
     try:
         from xxhash import xxh32
     except ImportError:
         msg = "xxh32 hash requires library xxhash, which is not a part of zenutils. You need to installed xxhash by yourself, or put it into your project's requirements.txt."
         logger.error(msg)
         raise RuntimeError(msg)
     return xxh32
 
+
 setup_hash_method_loader("sha", get_sha_class)
 setup_hash_method_loader("sm3", get_sm3_class)
 setup_hash_method_loader("xxh128", get_xxh128_class)
 setup_hash_method_loader("xxh64", get_xxh64_class)
 setup_hash_method_loader("xxh32", get_xxh32_class)
 
+
 # ##################################################################################
 # PBKDF2 HMAC HANDLER AERA
 # ##################################################################################
-
 def _pbkdf2_hmac(hash_name, password, salt, iterations, dklen=None):
     """Password based key derivation function 2 (PKCS #5 v2.0)
 
     This Python implementations based on the hmac module about as fast
     as OpenSSL's PKCS5_PBKDF2_HMAC for short passwords and much faster
     for long passwords.
-    """    
+    """
     from zenutils import numericutils
+
     _trans_5C = numericutils.ints2bytes((x ^ 0x5C) for x in range(256))
     _trans_36 = numericutils.ints2bytes((x ^ 0x36) for x in range(256))
 
     if not isinstance(hash_name, STR_TYPE):
         msg = "hash_name {value} requires {required_type} type but got {real_type} type...".format(
-            value = hash_name,
-            required_type = STR_TYPE,
-            real_type = type(hash_name),
+            value=hash_name,
+            required_type=STR_TYPE,
+            real_type=type(hash_name),
         )
         raise TypeError(msg)
 
     if not isinstance(password, (bytes, bytearray)):
         password = bytes(memoryview(password))
     if not isinstance(salt, (bytes, bytearray)):
         salt = bytes(memoryview(salt))
 
     # Fast inline HMAC implementation
     inner = new(hash_name)
     outer = new(hash_name)
-    blocksize = getattr(inner, 'block_size', 64)
+    blocksize = getattr(inner, "block_size", 64)
     if len(password) > blocksize:
         password = new(hash_name, password).digest()
-    password = password + b'\x00' * (blocksize - len(password))
+    password = password + b"\x00" * (blocksize - len(password))
     inner.update(password.translate(_trans_36))
     outer.update(password.translate(_trans_5C))
 
     def prf(msg, inner=inner, outer=outer):
         # PBKDF2_HMAC uses the password as key. We can re-use the same
         # digest objects and just update copies to skip initialization.
         icpy = inner.copy()
@@ -277,57 +301,57 @@
     if iterations < 1:
         raise ValueError(iterations)
     if dklen is None:
         dklen = outer.digest_size
     if dklen < 1:
         raise ValueError(dklen)
 
-    dkey = b''
+    dkey = b""
     loop = 1
     from_bytes = numericutils.from_bytes
     while len(dkey) < dklen:
         # prev = prf(salt + loop.to_bytes(4, 'big'))
-        prev = prf(salt + numericutils.int2bytes(loop, 4, 'big'))
+        prev = prf(salt + numericutils.int2bytes(loop, 4, "big"))
         # endianness doesn't matter here as long to / from use the same
-        rkey = from_bytes(prev, 'big')
+        rkey = from_bytes(prev, "big")
         for i in range(iterations - 1):
             prev = prf(prev)
             # rkey = rkey ^ prev
-            rkey ^= from_bytes(prev, 'big')
+            rkey ^= from_bytes(prev, "big")
         loop += 1
         # dkey += rkey.to_bytes(inner.digest_size, 'big')
-        dkey += numericutils.int2bytes(rkey, inner.digest_size, 'big')
+        dkey += numericutils.int2bytes(rkey, inner.digest_size, "big")
     return dkey[:dklen]
 
+
+# ##################################################################################
 #
 # FIX hashlib.pbkdf2_hmac missing problem for old python
 #
 # But because hashlib.pbkdf2_hmac is not support extra hash method
 # So better not use hashlib.pbkdf2_hmac directly
 # You can use pbkdf2_hmac to work with your self define hash method
 # Firstly you have to register your self define hash method with setup_hash_method_loader
-# 
-try:
-    # OpenSSL's PKCS5_PBKDF2_HMAC requires OpenSSL 1.0+ with HMAC and SHA
-    from hashlib import pbkdf2_hmac
-except ImportError:
-    hashlib.pbkdf2_hmac = _pbkdf2_hmac
-
+#
+# ##################################################################################
 def pbkdf2_hmac(hash_name, password, salt, iterations, dklen=None):
-    """If method supported by hashlib, returns hashlib.pbkdf2_hmac, or else returns self defined _pbkdf2_hmac.
-    """
+    """If method supported by hashlib, returns hashlib.pbkdf2_hmac, or else returns self defined _pbkdf2_hmac."""
     try:
         return hashlib.pbkdf2_hmac(hash_name, password, salt, iterations, dklen)
+    except AttributeError:
+        return _pbkdf2_hmac(hash_name, password, salt, iterations, dklen)
     except ValueError:
         return _pbkdf2_hmac(hash_name, password, salt, iterations, dklen)
 
+
 # ##################################################################################
 # BASE HASH CALC AREA
 # ##################################################################################
 
+
 def get_file_hash_result(filename, **kwargs):
     method = kwargs.get("method", DEFAULT_HASH_METHOD)
     buffer_size = kwargs.get("buffer_size", DEFAULT_BUFFER_SIZE)
     result_encoder = kwargs.get("result_encoder", DEFAULT_RESULT_ENCODER)
     method = method_load(method)
     gen = method()
     with open(filename, "rb") as fobj:
@@ -335,46 +359,57 @@
             buffer = fobj.read(buffer_size)
             if not buffer:
                 break
             gen.update(buffer)
     digest = gen.digest()
     return result_encoder.encode(digest)
 
+
 def get_hash_result(*args, **kwargs):
     method = kwargs.get("method", DEFAULT_HASH_METHOD)
     result_encoder = kwargs.get("result_encoder", DEFAULT_RESULT_ENCODER)
     gen_class = method_load(method)
     gen = gen_class()
     for arg in args:
         gen.update(force_bytes(arg))
     digest = gen.digest()
     return result_encoder.encode(digest)
 
+
 def get_salted_hash_base64(*args, **kwargs):
     from zenutils import strutils
     from zenutils import base64utils
+
     method = kwargs.get("method", "md5")
     salt_length = kwargs.get("salt_length", 4)
     salt = kwargs.get("salt", None)
     if salt is None:
         salt = strutils.random_string(length=salt_length)
     gen_class = method_load(method)
     gen = gen_class()
     for arg in args:
         gen.update(force_bytes(arg))
     gen.update(force_bytes(salt))
     data = gen.digest() + force_bytes(salt)
     result = force_text(base64utils.encodebytes(data))
     return strutils.join_lines(result)
 
+
 # ##################################################################################
 # PBKDF2 HMAC CALC AREA
 # ##################################################################################
 
-def get_pbkdf2_hmac(text, salt=None, iterations=2048, hash_name=DEFAULT_HASH_METHOD, seperator_between_pbkdf2_and_method="_"):
+
+def get_pbkdf2_hmac(
+    text,
+    salt=None,
+    iterations=2048,
+    hash_name=DEFAULT_HASH_METHOD,
+    seperator_between_pbkdf2_and_method="_",
+):
     from zenutils import strutils
     from zenutils import base64utils
 
     if salt is None:
         salt = strutils.random_string(16, choices=string.ascii_letters)
     text = force_bytes(text)
     salt = force_bytes(salt)
@@ -383,54 +418,66 @@
         seperator=seperator_between_pbkdf2_and_method,
         hash_name=TEXT(hash_name),
         iterations=iterations,
         salt=TEXT(salt),
         data=strutils.join_lines(TEXT(base64utils.encodebytes(data))),
     )
 
+
 def validate_pbkdf2_hmac(password, text):
     text = force_text(text)
     matches = re.findall("pbkdf2([_:])(.+)\\$(\\d+)\\$(.+)\\$(.+)", text)
     if len(matches) != 1:
         return False
     sep, hash_name, iterations, salt, _ = matches[0]
     if not iterations.isdigit():
         return False
     else:
         iterations = int(iterations)
-    data = get_pbkdf2_hmac(password, salt=salt, iterations=iterations, hash_name=hash_name, seperator_between_pbkdf2_and_method=sep)
+    data = get_pbkdf2_hmac(
+        password,
+        salt=salt,
+        iterations=iterations,
+        hash_name=hash_name,
+        seperator_between_pbkdf2_and_method=sep,
+    )
     if data == text:
         return True
     else:
         return False
 
+
 # ##################################################################################
 # PASSWORD HASH AREA
 # ##################################################################################
 PASSWORD_HASH_METHODS = {}
 
+
 class PasswordHashMethodNotSupportError(Exception):
     pass
 
-class PasswordHashMethodBase(object):
 
+class PasswordHashMethodBase(object):
     def get_password_hash(self, password):
         pass
 
     def validate_password_hash(self, password_hash_data, password):
         pass
 
+
 def register_password_hash_method(name, password_hash_method_instance):
     PASSWORD_HASH_METHODS[name] = password_hash_method_instance
 
+
 def get_password_hash_methods():
     methods = list(PASSWORD_HASH_METHODS.keys())
     methods.sort()
     return methods
 
+
 def get_password_hash(password, method=DEFAULT_PASSWORD_HASH_METHOD):
     """
     4 kind password hash format supported:
 
     1. Simple hash with method prefix. e.g. {SHA1}w0mcJylzCn+AfvuGdqkty2+KP48=
     2. Salted hash with method prefix. e.g. {SSHA}qWgORjfMmQJPipkl0KtdvQ6rGcppdVBIZGtGcQ==
     3. Pbkdf2 hmac hash. e.g. 'pbkdf2_sha256$2048$TdisEdeyNKNltWAj$eLzCMpQjSDIh9GFMjJCzhBPexrfeQfoLYypbHtTH6V8='
@@ -439,225 +486,314 @@
     method = method.upper()
     password_hash_method = PASSWORD_HASH_METHODS.get(method, None)
     if password_hash_method:
         return password_hash_method.get_password_hash(password)
     else:
         raise PasswordHashMethodNotSupportError()
 
+
 def validate_password_hash(password_hash_data, password):
     for _, method in PASSWORD_HASH_METHODS.items():
         result = method.validate_password_hash(password_hash_data, password)
         if result in [True, False]:
             return result
     return False
 
-class Pbkdf2PasswordHashBase(PasswordHashMethodBase):
 
+class Pbkdf2PasswordHashBase(PasswordHashMethodBase):
     seperator_between_pbkdf2_and_method = "_"
     method = DEFAULT_HASH_METHOD
     prefix = "pbkdf2_{method}$".format(method=DEFAULT_HASH_METHOD)
 
     def get_password_hash(self, password):
-        return get_pbkdf2_hmac(password, hash_name=self.method, seperator_between_pbkdf2_and_method=self.seperator_between_pbkdf2_and_method)
+        return get_pbkdf2_hmac(
+            password,
+            hash_name=self.method,
+            seperator_between_pbkdf2_and_method=self.seperator_between_pbkdf2_and_method,
+        )
 
     def validate_password_hash(self, password_hash_data, password):
         if not hasattr(self, "prefix"):
             return None
         if not password_hash_data.startswith(self.prefix):
             return None
         return validate_pbkdf2_hmac(password, password_hash_data)
 
+
 def register_pbkdf2_password_hash(method, prefix, seperator, class_name_suffix=""):
-    class_name = "".join([x.title() for x in [method, "pbkdf2", "password", "hash", class_name_suffix]])
-    globals()[class_name] = create_new_class(class_name, (Pbkdf2PasswordHashBase,), {
-        "seperator_between_pbkdf2_and_method": seperator,
-        "method": method,
-        "prefix": prefix,
-    })
+    class_name = "".join(
+        [x.title() for x in [method, "pbkdf2", "password", "hash", class_name_suffix]]
+    )
+    globals()[class_name] = create_new_class(
+        class_name,
+        (Pbkdf2PasswordHashBase,),
+        {
+            "seperator_between_pbkdf2_and_method": seperator,
+            "method": method,
+            "prefix": prefix,
+        },
+    )
     return globals()[class_name]
 
+
 class SimplePasswordHashBase(PasswordHashMethodBase):
-    
     method = DEFAULT_PASSWORD_HASH_METHOD
     prefix = "{{{method}}}".format(method=DEFAULT_PASSWORD_HASH_METHOD.upper())
 
     def get_password_hash(self, password):
         return self.prefix + get_hash_base64(password, method=self.method)
 
     def validate_password_hash(self, password_hash_data, password):
         if not hasattr(self, "prefix"):
             return None
         if not password_hash_data.startswith(self.prefix):
             return None
         new_password_hash_data = self.get_password_hash(password)
         return new_password_hash_data == password_hash_data
 
+
 def register_simple_password_hash(method, prefix, class_name_suffix=""):
-    class_name = "".join([x.title() for x in [method, "simple", "password", "hash", class_name_suffix]])
-    globals()[class_name] = create_new_class(class_name, (SimplePasswordHashBase,), {
-        "method": method,
-        "prefix": prefix,
-    })
+    class_name = "".join(
+        [x.title() for x in [method, "simple", "password", "hash", class_name_suffix]]
+    )
+    globals()[class_name] = create_new_class(
+        class_name,
+        (SimplePasswordHashBase,),
+        {
+            "method": method,
+            "prefix": prefix,
+        },
+    )
     return globals()[class_name]
 
-class SimpleSaltPasswordHashBase(PasswordHashMethodBase):
 
+class SimpleSaltPasswordHashBase(PasswordHashMethodBase):
     method = DEFAULT_PASSWORD_HASH_METHOD
     prefix = "{{{method}}}".format(method=DEFAULT_PASSWORD_HASH_METHOD.upper())
     hash_size = 0
     salt_length = 8
 
     def get_hash_size(self):
         if self.hash_size == 0:
             gen_class = method_load(self.method)
             self.hash_size = gen_class().digest_size
         return self.hash_size
 
     def get_password_hash(self, password, salt_length=None, salt=None):
         if salt_length is None:
             salt_length = self.salt_length
-        return self.prefix + get_salted_hash_base64(password, salt_length=salt_length, salt=salt, method=self.method)
+        return self.prefix + get_salted_hash_base64(
+            password, salt_length=salt_length, salt=salt, method=self.method
+        )
 
     def validate_password_hash(self, password_hash_data, password):
         if not hasattr(self, "prefix"):
             return None
         if not password_hash_data.startswith(self.prefix):
             return None
-        salt = base64utils.decodebytes(force_bytes(password_hash_data[len(self.prefix):]))[self.get_hash_size():]
+        salt = base64utils.decodebytes(
+            force_bytes(password_hash_data[len(self.prefix) :])
+        )[self.get_hash_size() :]
         new_password_hash_data = self.get_password_hash(password, salt=salt)
         return new_password_hash_data == password_hash_data
 
-def register_simple_salt_password_hash(method, prefix, hash_size=0, salt_length=8, class_name_suffix=""):
-    class_name = "".join([x.title() for x in [method, "simple", "salt", "password", "hash", class_name_suffix]])
-    globals()[class_name] = create_new_class(class_name, (SimpleSaltPasswordHashBase,), {
-        "method": method,
-        "prefix": prefix,
-        "hash_size": hash_size,
-        "salt_length": salt_length,
-    })
+
+def register_simple_salt_password_hash(
+    method, prefix, hash_size=0, salt_length=8, class_name_suffix=""
+):
+    class_name = "".join(
+        [
+            x.title()
+            for x in [method, "simple", "salt", "password", "hash", class_name_suffix]
+        ]
+    )
+    globals()[class_name] = create_new_class(
+        class_name,
+        (SimpleSaltPasswordHashBase,),
+        {
+            "method": method,
+            "prefix": prefix,
+            "hash_size": hash_size,
+            "salt_length": salt_length,
+        },
+    )
     return globals()[class_name]
 
-class HexlifyPasswordHashBase(PasswordHashMethodBase):
 
+class HexlifyPasswordHashBase(PasswordHashMethodBase):
     length = 40
     method = DEFAULT_HASH_METHOD
 
     def get_length(self):
         if self.length == 0:
             gen_class = method_load(self.method)
             self.length = 2 * gen_class().digest_size
         return self.length
 
     def get_password_hash(self, password):
         return get_hash_hexdigest(password, method=self.method)
-    
+
     def validate_password_hash(self, password_hash_data, password):
         from zenutils import strutils
+
         if not strutils.is_unhexlifiable(password_hash_data):
             return None
         if len(password_hash_data) != self.get_length():
             return None
         new_password_hash_data = self.get_password_hash(password)
         if new_password_hash_data == password_hash_data:
             return True
         else:
             return None
 
+
 def register_hexlify_password_hash(method, length=0, class_name_suffix=""):
-    class_name = "".join([x.title() for x in [method, "hexlify", "password", "hash", class_name_suffix]])
-    globals()[class_name] = create_new_class(class_name, (HexlifyPasswordHashBase,), {
-        "method": method,
-        "length": length,
-    })
+    class_name = "".join(
+        [x.title() for x in [method, "hexlify", "password", "hash", class_name_suffix]]
+    )
+    globals()[class_name] = create_new_class(
+        class_name,
+        (HexlifyPasswordHashBase,),
+        {
+            "method": method,
+            "length": length,
+        },
+    )
     return globals()[class_name]
 
+
 # ##################################################################################
 # HASH CALC METHOD ALIAS AREA
 # ##################################################################################
-get_file_hash = functools.partial(get_file_hash_result, result_encoder=HexlifyResultEncoder)
-get_file_hash_hexdigest = functools.partial(get_file_hash_result, result_encoder=HexlifyResultEncoder)
-get_file_hash_base64 = functools.partial(get_file_hash_result, result_encoder=Base64ResultEncoder)
+get_file_hash = functools.partial(
+    get_file_hash_result, result_encoder=HexlifyResultEncoder
+)
+get_file_hash_hexdigest = functools.partial(
+    get_file_hash_result, result_encoder=HexlifyResultEncoder
+)
+get_file_hash_base64 = functools.partial(
+    get_file_hash_result, result_encoder=Base64ResultEncoder
+)
 get_hash = functools.partial(get_hash_result, result_encoder=HexlifyResultEncoder)
-get_hash_hexdigest = functools.partial(get_hash_result, result_encoder=HexlifyResultEncoder)
+get_hash_hexdigest = functools.partial(
+    get_hash_result, result_encoder=HexlifyResultEncoder
+)
 get_hash_base64 = functools.partial(get_hash_result, result_encoder=Base64ResultEncoder)
 
-_not_simple_hash_algorithms = set([
-    "shake_128",
-    "shake_256",
-])
+_not_simple_hash_algorithms = set(
+    [
+        "shake_128",
+        "shake_256",
+    ]
+)
 for method in algorithms_available:
     if method in _not_simple_hash_algorithms:
         continue
     # ##################################################################################
     # STRING HASH CALC METHOD ALIAS
     # ##################################################################################
     name = "get_{method}_digest".format(method=method)
-    globals()[name] = functools.partial(get_hash_result, method=method, result_encoder=DigestResultEncoder)
+    globals()[name] = functools.partial(
+        get_hash_result, method=method, result_encoder=DigestResultEncoder
+    )
     __all__.append(name)
 
     name = "get_{method}".format(method=method)
-    globals()[name] = functools.partial(get_hash_result, method=method, result_encoder=HexlifyResultEncoder)
+    globals()[name] = functools.partial(
+        get_hash_result, method=method, result_encoder=HexlifyResultEncoder
+    )
     __all__.append(name)
 
     name = "get_{method}_hexdigest".format(method=method)
-    globals()[name] = functools.partial(get_hash_result, method=method, result_encoder=HexlifyResultEncoder)
+    globals()[name] = functools.partial(
+        get_hash_result, method=method, result_encoder=HexlifyResultEncoder
+    )
     __all__.append(name)
 
     name = "get_{method}_base64".format(method=method)
-    globals()[name] = functools.partial(get_hash_result, method=method, result_encoder=Base64ResultEncoder)
+    globals()[name] = functools.partial(
+        get_hash_result, method=method, result_encoder=Base64ResultEncoder
+    )
     __all__.append(name)
 
-
     # ##################################################################################
     # FILE HASH CALC METHOD ALIAS
     # ##################################################################################
     name = "get_file_{method}_digest".format(method=method)
-    globals()[name] = functools.partial(get_file_hash_result, method=method, result_encoder=DigestResultEncoder)
+    globals()[name] = functools.partial(
+        get_file_hash_result, method=method, result_encoder=DigestResultEncoder
+    )
     __all__.append(name)
 
     name = "get_file_{method}".format(method=method)
-    globals()[name] = functools.partial(get_file_hash_result, method=method, result_encoder=HexlifyResultEncoder)
+    globals()[name] = functools.partial(
+        get_file_hash_result, method=method, result_encoder=HexlifyResultEncoder
+    )
     __all__.append(name)
 
     name = "get_file_{method}_hexdigest".format(method=method)
-    globals()[name] = functools.partial(get_file_hash_result, method=method, result_encoder=HexlifyResultEncoder)
+    globals()[name] = functools.partial(
+        get_file_hash_result, method=method, result_encoder=HexlifyResultEncoder
+    )
     __all__.append(name)
 
     name = "get_file_{method}_base64".format(method=method)
-    globals()[name] = functools.partial(get_file_hash_result, method=method, result_encoder=Base64ResultEncoder)
+    globals()[name] = functools.partial(
+        get_file_hash_result, method=method, result_encoder=Base64ResultEncoder
+    )
     __all__.append(name)
 
     # ##################################################################################
     # PBKDF2 METHOD ALIAS
     # ##################################################################################
     name = "get_pbkdf2_{method}".format(method=method)
     globals()[name] = functools.partial(get_pbkdf2_hmac, hash_name=method)
     __all__.append(name)
 
     name = "validate_pbkdf2_{method}".format(method=method)
     globals()[name] = validate_pbkdf2_hmac
     __all__.append(name)
 
     password_hash_method_name = "PBKDF2_{method}".format(method=method.upper())
-    password_hash_method_class = register_pbkdf2_password_hash(method, "pbkdf2_{method}$".format(method=method), "_", class_name_suffix="")
-    register_password_hash_method(password_hash_method_name, password_hash_method_class())
+    password_hash_method_class = register_pbkdf2_password_hash(
+        method, "pbkdf2_{method}$".format(method=method), "_", class_name_suffix=""
+    )
+    register_password_hash_method(
+        password_hash_method_name, password_hash_method_class()
+    )
     __all__.append(password_hash_method_class.__name__)
 
     password_hash_method_name = "PBKDF2:{method}".format(method=method.upper())
-    password_hash_method_class = register_pbkdf2_password_hash(method, "pbkdf2:{method}$".format(method=method), ":", class_name_suffix="Colon")
-    register_password_hash_method(password_hash_method_name, password_hash_method_class())
+    password_hash_method_class = register_pbkdf2_password_hash(
+        method, "pbkdf2:{method}$".format(method=method), ":", class_name_suffix="Colon"
+    )
+    register_password_hash_method(
+        password_hash_method_name, password_hash_method_class()
+    )
     __all__.append(password_hash_method_class.__name__)
 
     password_hash_method_name = "S{method}".format(method=method.upper())
-    password_hash_method_class = register_simple_salt_password_hash(method, "{{S{method}}}".format(method=method.upper()), class_name_suffix="")
-    register_password_hash_method(password_hash_method_name, password_hash_method_class())
+    password_hash_method_class = register_simple_salt_password_hash(
+        method, "{{S{method}}}".format(method=method.upper()), class_name_suffix=""
+    )
+    register_password_hash_method(
+        password_hash_method_name, password_hash_method_class()
+    )
     __all__.append(password_hash_method_class.__name__)
 
     password_hash_method_name = "{method}".format(method=method.upper())
-    password_hash_method_class = register_simple_password_hash(method, "{{{method}}}".format(method=method.upper()), class_name_suffix="")
-    register_password_hash_method(password_hash_method_name, password_hash_method_class())
+    password_hash_method_class = register_simple_password_hash(
+        method, "{{{method}}}".format(method=method.upper()), class_name_suffix=""
+    )
+    register_password_hash_method(
+        password_hash_method_name, password_hash_method_class()
+    )
     __all__.append(password_hash_method_class.__name__)
 
     password_hash_method_name = "{method}HEX".format(method=method.upper())
-    password_hash_method_class = register_hexlify_password_hash(method, class_name_suffix="")
-    register_password_hash_method(password_hash_method_name, password_hash_method_class())
+    password_hash_method_class = register_hexlify_password_hash(
+        method, class_name_suffix=""
+    )
+    register_password_hash_method(
+        password_hash_method_name, password_hash_method_class()
+    )
     __all__.append(password_hash_method_class.__name__)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.3.9/zenutils/httputils.py` & `zenutils-0.4.8/zenutils/httputils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,103 +1,119 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""HTTP请求工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 __all__ = [
     "urlparse",
     "get_urlinfo",
     "get_url_filename",
     "get_url_save_path",
     "get_sitename",
     "download",
 ]
 
 import os
+
 try:
     from urllib.parse import urlparse
     from urllib.parse import ParseResult
 except ImportError:
-    from urlparse import urlparse # fix for python2.7
+    from urlparse import urlparse  # fix for python2.7
     from urlparse import ParseResult
 
 default_download_chunk_size = 4096
 
+
 def get_urlinfo(url):
     """Parse url.
 
     @Returns:
         (ParseResult): The url informations.
-    
+
     @Parameters:
         url(str): The string of the url.
     """
     if isinstance(url, ParseResult):
         info = url
     else:
         info = urlparse(url)
     return info
 
+
 def get_url_filename(url, info=None):
     """Get the filename that maybe used to save the content of the url.
 
     @Returns:
         (str): The final filename.
-    
+
     @Parameters:
         url(str): The url to be saved.
         info(ParseResult, optional): Info will be used if it is provided.
                                      If not provided, get the info from the url by call get_urlinfo().
     """
     info = info or get_urlinfo(url)
     path = info.path
     filename = os.path.split(path)[1]
     if not filename:
         filename = "index.html"
     return filename
 
+
 def get_url_save_path(url, save_root, info=None):
     info = info or get_urlinfo(url)
     filename = get_url_filename(url, info)
     path = info.path.split(info.path)[0]
-    filepath = os.path.abspath(os.path.join(save_root, "."+path+"/", filename))
+    filepath = os.path.abspath(os.path.join(save_root, "." + path + "/", filename))
     return filepath
 
+
 def get_sitename(url):
     """Get the hostname of the url.
 
     @Returns:
         (str): The hostname of the url.
-    
+
     @Paramters:
         url(str): The url string.
     """
     info = get_urlinfo(url)
     return info.hostname
 
+
 def download_py2(url, filename):
-    """Download implement for py2.
-    """
+    """Download implement for py2."""
     import urllib2
+
     response = urllib2.urlopen(url)
     size = 0
     with open(filename, "wb") as fobj:
         while True:
             chunk = response.read(default_download_chunk_size)
             if len(chunk) > 0:
                 size += len(chunk)
                 fobj.write(chunk)
             else:
                 break
     return size
 
+
 def download_py3(url, filename):
-    """Download implement for py3.
-    """
+    """Download implement for py3."""
     import http.client
+
     info = get_urlinfo(url)
     if info.scheme == "https":
         conn = http.client.HTTPSConnection(info.hostname, info.port or 443)
     else:
         conn = http.client.HTTPConnection(info.hostname, info.port or 80)
     path = info.path
     if info.query:
@@ -111,20 +127,21 @@
             if len(chunk) > 0:
                 size += len(chunk)
                 fobj.write(chunk)
             else:
                 break
     return size
 
+
 def download(url, filename):
     """Simple http get request. Use to download a file from url and save it to a file.
 
     @Returns:
         (int): Content read size.
-    
+
     @Paramters:
         url(str): The url to be downloaded.
         filename(str): The filename to be used in saving downloaded file.
     """
     if PY2:
         return download_py2(url, filename)
     else:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.3.9/zenutils/jsonutils.py` & `zenutils-0.4.8/zenutils/jsonutils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""JSON工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 __all__ = [
     "register_global_encoder",
     "make_simple_json_encoder",
     "SimpleJsonEncoder",
     "simple_json_dumps",
@@ -19,25 +28,26 @@
 from functools import partial
 
 from zenutils.sixutils import BASESTRING_TYPES
 
 default_simple_json_encoder_base = json.encoder.JSONEncoder
 default_error_code = 1
 
-class JsonEncodeLibrary(object):
 
+class JsonEncodeLibrary(object):
     def __init__(self, base_class=default_simple_json_encoder_base):
         self.base_class = base_class
         self.encoders = {}
         self.__encoder = None
 
     def get_encoder(self):
         this = self
         if this.__encoder is not None:
             return this.__encoder
+
         class SimpleJsonEncoderBase(this.base_class):
             def default(self, o):
                 for t, encoder in this.encoders.items():
                     try:
                         isinstance_flag = isinstance(o, t)
                     except:
                         isinstance_flag = False
@@ -46,119 +56,140 @@
                     try:
                         issubclass_flag = issubclass(o, t)
                     except:
                         issubclass_flag = False
                     if issubclass_flag:
                         return encoder(o)
                 return super(SimpleJsonEncoder, self).default(o)
+
         if PY2:
             import json
             import json.encoder
+
             _default_encode_basestring = json.encoder.encode_basestring
             _default_encode_basestring_ascii = json.encoder.encode_basestring_ascii
+
             def _encode_basestring(s):
                 try:
                     s = force_text(s)
                 except:
                     s = encode_bytes(s)
                 return _default_encode_basestring(s)
+
             def _encode_basestring_ascii(s):
                 try:
                     s = force_text(s)
                 except:
                     s = encode_bytes(s)
                 return _default_encode_basestring_ascii(s)
+
             class SimpleJsonEncoder(SimpleJsonEncoderBase):
                 def encode(self, o):
                     json.encoder.encode_basestring = _encode_basestring
                     json.encoder.encode_basestring_ascii = _encode_basestring_ascii
                     result = super(SimpleJsonEncoder, self).encode(o)
                     json.encoder.encode_basestring = _default_encode_basestring
-                    json.encoder.encode_basestring_ascii = _default_encode_basestring_ascii     
+                    json.encoder.encode_basestring_ascii = (
+                        _default_encode_basestring_ascii
+                    )
                     return result
+
         else:
+
             class SimpleJsonEncoder(SimpleJsonEncoderBase):
                 pass
+
         this.__encoder = SimpleJsonEncoder
         setattr(this.__encoder, "library", this)
         return this.__encoder
 
     def register(self, type, encode):
         self.encoders[type] = encode
 
     def unregister(self, type):
         if type in self.encoders:
             del self.encoders[type]
 
+
 DATETIME_ISO_FORMAT = "isoformat"
 DATETIME_FORMAT = DATETIME_ISO_FORMAT
 
+
 def set_datetime_format(format=DATETIME_ISO_FORMAT):
     global DATETIME_FORMAT
     DATETIME_FORMAT = format
 
+
 def encode_datetime(value):
     if DATETIME_FORMAT == DATETIME_ISO_FORMAT:
         return value.isoformat()
     else:
         return value.strftime(DATETIME_FORMAT)
 
+
 def encode_bytes(value):
     return binascii.hexlify(value).decode()
 
+
 def encode_basestring(value):
     if isinstance(value, BYTES_TYPE):
         return encode_bytes(value)
     else:
         return value
 
+
 def encode_decimal(value):
     return float(value)
 
+
 def encode_complex(value):
     return [value.real, value.imag]
 
+
 def encode_uuid(value):
     return str(value)
 
+
 def encode_image(image):
     from zenutils import base64utils
+
     buffer = BytesIO()
     image.save(buffer, format="png")
     return """data:image/{format};base64,{data}""".format(
         format=format,
         data=force_text(base64utils.encodebytes(buffer.getvalue())),
-        )
+    )
+
 
 def encode_exception(error):
     from zenutils import strutils
     from zenutils import funcutils
+
     if error.args:
         try:
             code = strutils.force_int(error.args[0])
             message = " ".join(error.args[1:])
             return {
                 "code": code,
                 "message": message,
             }
         except:
             message = " ".join(error.args)
             if message:
-                return {
-                    "code": default_error_code,
-                    "message": message
-                }
+                return {"code": default_error_code, "message": message}
     return {
         "code": default_error_code,
         "message": funcutils.get_class_name(error),
     }
 
+
 def encode_bizerror(error):
     return error.json
 
+
 def encode_django_model(django_model):
     from django.core import serializers
 
     try:
         isinstance_flag = isinstance(django_model, Model)
     except:
         isinstance_flag = False
@@ -173,133 +204,148 @@
         text = serializers.serialize("json", [django_model])
         results = json.loads(text)
         obj = results[0]["fields"]
         obj[pk_name] = results[0]["pk"]
         return obj
     return None
 
+
 def encode_django_queryset(django_queryset):
     from django.core import serializers
-    
+
     pk_name = django_queryset.model._meta.pk.name
     text = serializers.serialize("json", django_queryset)
     results = json.loads(text)
     data = []
     for result in results:
         obj = result["fields"]
         obj[pk_name] = result["pk"]
         data.append(obj)
     return data
 
+
 def encode_django_query(django_query):
     return str(django_query)
 
+
 GLOBAL_ENCODERS = {}
 
+
 def register_global_encoder(type, encoder):
     """Register a new encoder type to the global-encoder-collections.
 
     @Returns:
         (None): Nothing.
-    
+
     @Paramters:
         type(Any type): The type has a custom encode callback.
         encoder(Callable): A callable object that
                             takes one parameter which is to be json serialized
                             and returns the system serializable value.
-    
+
 
     @Example:
         class Model(object):
             def __init__(self):
                 self.name = ""
                 self.age = 0
-            
+
             def json(self):
                 return {
                     "name": self.name,
                     "age": self.age,
                 }
-        
+
         def model_encoder(o):
             return o.json()
-        
+
         register_global_encoder(Model, model_encoder)
     """
     if isinstance(type, (list, tuple, set)):
         types = type
     else:
         types = [type]
     for type in types:
         GLOBAL_ENCODERS[type] = encoder
 
+
 def register_simple_encoders(library):
     """Copy the encoders in the global-encoder-collections to a new encoder library instance.
 
     @Returns:
         (None): Nothing.
-    
+
     @Parameters:
         library(JsonEncodeLibrary): An instance of JsonEncodeLibrary.
     """
     for type, encoder in GLOBAL_ENCODERS.items():
         library.register(type, encoder)
 
-register_global_encoder((datetime.datetime, datetime.date, datetime.time), encode_datetime)
+
+register_global_encoder(
+    (datetime.datetime, datetime.date, datetime.time), encode_datetime
+)
 register_global_encoder(decimal.Decimal, encode_decimal)
 register_global_encoder(complex, encode_complex)
 register_global_encoder(uuid.UUID, encode_uuid)
 register_global_encoder(BASESTRING_TYPES, encode_basestring)
 
 
 try:
     from zenutils import dictutils
+
     register_global_encoder(dictutils.HttpHeadersDict, lambda x: x.data)
 except Exception:
     pass
 
 try:
     from zenutils import funcutils
+
     for exception_class in funcutils.get_all_builtin_exceptions():
         register_global_encoder(exception_class, encode_exception)
 except Exception:
     pass
 
 try:
     from PIL.Image import Image
+
     register_global_encoder(Image, encode_image)
 except ImportError:
     pass
 
 try:
     from django.db.models import Model
+
     register_global_encoder(Model, encode_django_model)
 except ImportError:
     pass
 
 try:
     from bizerror import BizErrorBase
+
     register_global_encoder(BizErrorBase, encode_bizerror)
 except ImportError:
     pass
 
 try:
     from django.db.models import QuerySet
+
     register_global_encoder(QuerySet, encode_django_queryset)
 except ImportError:
     pass
 
 try:
     from django.db.models.sql.query import Query
+
     register_global_encoder(Query, encode_django_query)
 except ImportError:
     pass
 
 
 def make_simple_json_encoder(base_class=default_simple_json_encoder_base):
     library = JsonEncodeLibrary(base_class)
     register_simple_encoders(library)
     return library.get_encoder()
 
+
 SimpleJsonEncoder = make_simple_json_encoder()
 simple_json_dumps = partial(json.dumps, cls=SimpleJsonEncoder)
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.3.9/zenutils/listutils.py` & `zenutils-0.4.8/zenutils/listutils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""列表工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 __all__ = [
     "pad",
     "chunk",
     "clean_none",
     "ignore_none_element",
@@ -25,48 +34,51 @@
 
 def pad(thelist, size, padding):
     if len(thelist) < size:
         for _ in range(size - len(thelist)):
             thelist.append(padding)
     return thelist
 
+
 def chunk(thelist, size, with_padding=False, padding=None):
     data = []
     start = 0
     while True:
         if len(thelist) < size:
             if with_padding:
                 pad(thelist, size, padding)
             data.append(thelist)
             break
-        data.append(thelist[start:start+size])
-        thelist = thelist[start+size:]
+        data.append(thelist[start : start + size])
+        thelist = thelist[start + size :]
         if not thelist:
             break
     return data
 
+
 def clean_none(thelist):
-    """Remove None or empty element in thelist.
-    """
+    """Remove None or empty element in thelist."""
     return [element for element in thelist if element]
 
+
 ignore_none_element = clean_none
 
+
 def unique(thelist):
-    """Remove duplicated elements from the list.
-    """
+    """Remove duplicated elements from the list."""
     result = []
     for element in thelist:
         if not element in result:
             result.append(element)
     return result
 
+
 def replace(thelist, map, inplace=False):
     """Replace element in thelist, the map is collection of {old_value: new_value}.
-    
+
     inplace == True, will effect the original list.
     inplace == False, will create a new list to return.
     """
     if inplace:
         for index in range(len(thelist)):
             value = thelist[index]
             if value in map:
@@ -79,50 +91,51 @@
             value = thelist[index]
             if value in map:
                 newlist.append(map[value])
             else:
                 newlist.append(value)
         return newlist
 
+
 def append_new(thelist, value):
-    """Append new value and only new value to the list.
-    """
+    """Append new value and only new value to the list."""
     if not value in thelist:
         thelist.append(value)
     return value
 
+
 def group(thelist):
-    """Count every element in thelist. e.g. ["a", "b", "c", "a", "b", "b"] => {"a": 2, "b": 3, "c": 1}.
-    """
+    """Count every element in thelist. e.g. ["a", "b", "c", "a", "b", "b"] => {"a": 2, "b": 3, "c": 1}."""
     info = {}
     for x in thelist:
         if x in info:
             info[x] += 1
         else:
             info[x] = 1
     return info
 
+
 def compare(old_set, new_set):
-    """Compare old_set and new_set, return set_new, set_delete, set_update.
-    """
+    """Compare old_set and new_set, return set_new, set_delete, set_update."""
     old_set = set(old_set)
     new_set = set(new_set)
 
     set_new = new_set - old_set
     set_delete = old_set - new_set
     set_update = old_set.intersection(new_set)
 
     return set_new, set_delete, set_update
 
+
 def first(*thelist, **options):
     """Return first non-none value. check is a callable function that returns the real value.
 
     @Returns:
         (any): The first non-None value in thelist. If there is No non-None value in thelist, returns the default value which is default to None.
-    
+
     @Parameters:
         thelist(any, multiple): The list to be searched.
         check(Callable[any, Optional[None, any]]]): The callable function used the check the value is a non-None value of not.
         default(any): The default value.
 
     @Usage:
         thelist = [None, "OK"]
@@ -147,25 +160,27 @@
     if check is None:
         check = lambda x: x
     for value in thelist:
         if check(value) != None:
             return value
     return default
 
+
 class CyclicDependencyError(ValueError):
     pass
 
+
 def topological_sort(*thelists):
     mapping = {}
     for thelist in thelists:
         for element in thelist:
             if not element in mapping:
                 mapping[element] = set()
         for index in range(1, len(thelist)):
-            prev = thelist[index-1]
+            prev = thelist[index - 1]
             current = thelist[index]
             mapping[current].add(prev)
     result = []
     while True:
         oks = []
         for k in list(mapping.keys()):
             v = mapping[k]
@@ -180,35 +195,38 @@
                 for k, v in mapping.items():
                     if ok in v:
                         v.remove(ok)
     if mapping:
         raise CyclicDependencyError()
     return result
 
+
 def topological_test(thelist, tester):
     last_index = -1
     for element in tester:
         index = thelist.index(element)
         if index < last_index:
             return False
         last_index = index
     return True
 
+
 def is_ordered(thelist, reverse=False):
     if reverse:
         for index in range(1, len(thelist)):
-            if thelist[index] > thelist[index-1]:
+            if thelist[index] > thelist[index - 1]:
                 return False
         return True
     else:
         for index in range(1, len(thelist)):
-            if thelist[index] < thelist[index-1]:
+            if thelist[index] < thelist[index - 1]:
                 return False
         return True
 
+
 def list2dict(thelist, fields):
     """Turn list to dict, using keys in fields.
 
     Examples:
 
     In [1]: from zenutils import listutils
 
@@ -221,15 +239,15 @@
     In [4]: listutils.list2dict([1,2,3], ['a', 'b', 'c', 'd'])
     Out[4]: {'a': 1, 'b': 2, 'c': 3, 'd': None}
     """
     result = {}
     thelistlength = len(thelist)
     field_infos = []
     for field in fields:
-        field_info = None            
+        field_info = None
         if isinstance(field, (tuple, list)):
             field_name = field[0]
             if len(field) >= 2:
                 field_default = field[1]
             field_info = (field_name, field_default)
         else:
             field_info = (field, None)
@@ -237,66 +255,78 @@
     for index, field_info in enumerate(field_infos):
         if index < thelistlength:
             result[field_info[0]] = thelist[index]
         else:
             result[field_info[0]] = field_info[1]
     return result
 
-def compare_execute(old_data, new_data, create_callback, delete_callback, change_callback, old_key, new_key=None):
+
+def compare_execute(
+    old_data,
+    new_data,
+    create_callback,
+    delete_callback,
+    change_callback,
+    old_key,
+    new_key=None,
+):
     """Compare two list, find elements to create/delete/change, and do callbacks.
-    
+
     Returns elements of: (created, deleted, changed).
     """
     new_key = new_key or old_key
 
     old_mapping = {}
     new_mapping = {}
 
     for data in old_data:
         key = old_key(data)
         old_mapping[key] = data
-    
+
     for data in new_data:
         key = new_key(data)
         new_mapping[key] = data
-    
+
     old_keys = set(list(old_mapping.keys()))
     new_keys = set(list(new_mapping.keys()))
 
     create_keys = new_keys - old_keys
     change_keys = new_keys.intersection(old_keys)
     delete_keys = old_keys - new_keys
 
     created = []
     if create_callback:
         for key in create_keys:
             data = new_mapping[key]
             result = create_callback(key, data)
             if not result is None:
                 created.append(result)
-        
+
     changed = []
     if change_callback:
         for key in change_keys:
             instance = old_mapping[key]
             data = new_mapping[key]
             result = change_callback(key, instance, data)
             if not result is None:
                 changed.append(result)
-    
+
     deleted = []
     if delete_callback:
         for key in delete_keys:
             instance = old_mapping[key]
             result = delete_callback(key, instance)
             if not result is None:
                 deleted.append(result)
-    
+
     return created, deleted, changed
 
+
 # ##################################################################
 # Removed to anotehr module
 # ##################################################################
 
+
 def int_list_to_bytes(*args, **kwargs):
     from zenutils import numericutils
+
     return numericutils.ints2bytes(*args, **kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.3.9/zenutils/logutils.py` & `zenutils-0.4.8/zenutils/logutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""日志工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 """
 Make logging setup easy. Default logging settings:
 
 ```
 logging_config = {
@@ -96,14 +105,15 @@
 import os
 from logging.config import dictConfig
 from logging import StreamHandler
 from logging.handlers import TimedRotatingFileHandler
 
 file_handler_backupCount = 30
 
+
 def get_console_handler(formatter="default", loglevel="DEBUG", handler_class=None):
     from zenutils import funcutils
 
     """Make a console handler settings.
     """
     handler_class = handler_class or StreamHandler
     default_params = {
@@ -112,43 +122,48 @@
     }
     params = funcutils.get_inject_params(handler_class, default_params)
     params["class"] = ".".join([handler_class.__module__, handler_class.__name__])
     params["formatter"] = formatter
     params["level"] = loglevel
     return params
 
-def get_file_handler(filename, formatter="default", loglevel="DEBUG", handler_class=None):
-    """Make a file handler settings.
-    """
+
+def get_file_handler(
+    filename, formatter="default", loglevel="DEBUG", handler_class=None
+):
+    """Make a file handler settings."""
     from zenutils import funcutils
 
     handler_class = handler_class or TimedRotatingFileHandler
-    default_params =  {
+    default_params = {
         "level": loglevel,
         "filename": filename,
         "when": "midnight",
         "interval": 1,
         "backupCount": file_handler_backupCount,
         "formatter": formatter,
         "encoding": "utf-8",
     }
     params = funcutils.get_inject_params(handler_class, default_params)
     params["class"] = ".".join([handler_class.__module__, handler_class.__name__])
     params["formatter"] = formatter
     params["level"] = loglevel
     return params
 
+
 def get_simple_config(
-        logfile=None,
-        loglevel=None,
-        logfmt=None,
-        loggers=None,
-        logging=None,
-        console_handler_class=None,
-        file_handler_class=None, **kwargs):
+    logfile=None,
+    loglevel=None,
+    logfmt=None,
+    loggers=None,
+    logging=None,
+    console_handler_class=None,
+    file_handler_class=None,
+    **kwargs
+):
     """Make simple logging settings.
 
     logfile default to app.log.
     loglevel choices are: DEBUG/INFO/WARNING/ERROR. default to INFO.
     logfmt choices are: default/message_only/json. default to default.
     Use logger parameter to override the default settings' logger sections.
     Use logging parameter to override the whole settings.
@@ -163,59 +178,70 @@
             "default": {
                 "format": "{asctime} {levelname} {module} {funcName} {process} {thread} {message}",
             },
         })
     """
     from zenutils import dictutils
     from zenutils import fsutils
+
     loggers = loggers or {}
     config = logging or {}
-    logfile = logfile or config.get("logfile", "./logs/app.log") # default log file to `pwd`/logs/app.log
+    logfile = logfile or config.get(
+        "logfile", "./logs/app.log"
+    )  # default log file to `pwd`/logs/app.log
     loglevel = loglevel or config.get("loglevel", "INFO")
     logfmt = logfmt or config.get("logfmt", "default")
     # make sure log folder exists...
     logfolder = os.path.abspath(os.path.dirname(logfile))
     fsutils.mkdir(logfolder)
     # default logging template
     logging_config = {
         "version": 1,
         "disable_existing_loggers": False,
         "formatters": {
             "default": {
-                "format": "{asctime} {levelname} {pathname} {lineno} {module} {funcName} {process} {thread} {message}",
-                "style": "{"
+                "format": "%(asctime)s %(levelname)s %(pathname)s %(lineno)s %(module)s %(funcName)s %(process)s %(thread)s %(message)s",
             },
             "simple": {
-                "format": "{asctime} {levelname} {message}",
-                "style": "{"
+                "format": "%(asctime)s %(levelname)s %(message)s",
             },
             "message_only": {
-                "format": "{message}",
-                "style": "{",
+                "format": "%(message)s",
             },
         },
         "handlers": {
-            "default_console": get_console_handler("default", "DEBUG", handler_class=console_handler_class),
-            "default_file": get_file_handler(logfile, "default", "DEBUG", handler_class=file_handler_class),
-            "simple_console": get_console_handler("simple", "DEBUG", handler_class=console_handler_class),
-            "simple_file": get_file_handler(logfile, "simple", "DEBUG", handler_class=file_handler_class),
-            "message_only_console": get_console_handler("message_only", "DEBUG", handler_class=console_handler_class),
-            "message_only_file": get_file_handler(logfile, "message_only", "DEBUG", handler_class=file_handler_class),
-        },
-        "loggers": {
+            "default_console": get_console_handler(
+                "default", "DEBUG", handler_class=console_handler_class
+            ),
+            "default_file": get_file_handler(
+                logfile, "default", "DEBUG", handler_class=file_handler_class
+            ),
+            "simple_console": get_console_handler(
+                "simple", "DEBUG", handler_class=console_handler_class
+            ),
+            "simple_file": get_file_handler(
+                logfile, "simple", "DEBUG", handler_class=file_handler_class
+            ),
+            "message_only_console": get_console_handler(
+                "message_only", "DEBUG", handler_class=console_handler_class
+            ),
+            "message_only_file": get_file_handler(
+                logfile, "message_only", "DEBUG", handler_class=file_handler_class
+            ),
         },
+        "loggers": {},
         "root": {
-            "handlers": [logfmt+"_file", logfmt+"_console"],
+            "handlers": [logfmt + "_file", logfmt + "_console"],
             "level": loglevel,
             "propagate": True,
-        }
+        },
     }
     dictutils.deep_merge(logging_config, config)
     dictutils.deep_merge(logging_config, {"loggers": loggers})
     dictutils.deep_merge(logging_config, kwargs)
     return logging_config
 
+
 def setup(*args, **kwargs):
-    """Using get_simple_config to get the logging settings and enable them. Parameters are the same with get_simple_config function.
-    """
+    """Using get_simple_config to get the logging settings and enable them. Parameters are the same with get_simple_config function."""
     config = get_simple_config(*args, **kwargs)
     dictConfig(config)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.3.9/zenutils/numericutils.py` & `zenutils-0.4.8/zenutils/numericutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""数值工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 __all__ = [
     "binary_decompose",
     "decimal_change_base",
     "get_float_part",
     "float_split",
@@ -15,95 +24,104 @@
     "is_infinity",
     "from_bytes",
     "bytes2ints",
     "ints2bytes",
     "int2bytes",
 ]
 
+
 def binary_decompose(value):
     values = set()
     binary_string = bin(value)[2:]
     length = len(binary_string) - 1
     for c in binary_string:
         if c == "1":
             values.add(2**length)
         length -= 1
     return values
 
-def decimal_change_base(number, base=16, characters="0123456789abcdefghijklmnopqrstuvwxyz"):
+
+def decimal_change_base(
+    number, base=16, characters="0123456789abcdefghijklmnopqrstuvwxyz"
+):
     digits = []
     while number:
-        digits.append( number % base )
+        digits.append(number % base)
         number //= base
     digits.reverse()
     if not digits:
         digits.append(0)
     if characters:
         return "".join([characters[x] for x in digits])
     else:
         return digits
 
+
 def get_float_part(value, precision=7):
     value = abs(value)
-    mod = 10 ** precision
+    mod = 10**precision
     value_all = int(value * mod)
     value_int = int(value) * mod
     value_float = value_all - value_int
     return value_float
 
+
 def float_split(value, precision=7):
     if value >= 0:
         sign = 1
     else:
         sign = -1
     value = abs(value)
     int_value = int(value)
     float_value = get_float_part(value, precision)
     return sign, int_value, float_value
 
 
-infinity = float("inf") # Positive infinity
-_infinity = float("-inf") # Negative infinity
+infinity = float("inf")  # Positive infinity
+_infinity = float("-inf")  # Negative infinity
 
 pinfinity = infinity
 ninfinity = _infinity
 
+
 def is_infinity(value):
     """Check if the value is infinity value or not.
 
     @Returns:
         (bool): True means the value is infinity. False means the value is NOT infinity.
 
     @Parameters:
         value(float): The value to be checked.
     """
-    if type(value) == float and (str(value) in ["inf", "-inf"] or value in [infinity, _infinity]):
+    if type(value) == float and (
+        str(value) in ["inf", "-inf"] or value in [infinity, _infinity]
+    ):
         return True
     else:
         return False
 
+
 def from_bytes(data, byteorder="big", signed=False):
-    """int.from_bytes entrypoint.
-    """
+    """int.from_bytes entrypoint."""
     if hasattr(int, "from_bytes"):
         return int.from_bytes(data, byteorder, signed=signed)
     else:
         return _from_bytes(data, byteorder, signed=signed)
 
+
 def _from_bytes(data, byteorder="big", signed=False):
-    """int.from_bytes backport.
-    """
+    """int.from_bytes backport."""
     # int.from_bytes(...) for python2.7
     import struct
     from zenutils import strutils
 
     # length == 0
     if not data:
         return 0
-    
+
     # length == 1
     if len(data) < 2:
         if signed:
             formatter = "b"
         else:
             formatter = "B"
         return struct.unpack(formatter, data)[0]
@@ -131,37 +149,39 @@
         result = struct.unpack(formatter.lower(), data[0])[0]
     for idx, chunk in enumerate(data[1:]):
         if idx == len(data[1:]) - 1:
             delta = last_delta
         result = result * delta + struct.unpack(formatter, chunk)[0]
     return result
 
+
 def bytes2ints(data):
     """Turn bytes to int arrary.
 
     @Returns:
         (list of int): int array.
-    
+
     @Parameters:
         data(bytes): The bytes data.
-    
+
     @Examples:
         assert strutils.bytes2ints(b'hello') == [104, 101, 108, 108, 111]
     """
     if PY2:
         return [ord(x) for x in data]
     else:
         return list(data)
 
+
 def ints2bytes(ints):
     return b"".join([int2bytes(x) for x in ints])
 
+
 def int2bytes(value, length=0, byteorder="big", signed=False):
-    """int.to_bytes. Auto detect the samllest length.
-    """
+    """int.to_bytes. Auto detect the samllest length."""
     if length == 0:
         if signed:
             c = -128
             length = 1
             while c > value:
                 c *= 256
                 length += 1
@@ -177,17 +197,17 @@
                 result = b"\xff"
             else:
                 result = b"\x00"
         return result
     else:
         return _int2bytes(value, length, byteorder, signed=signed)
 
+
 def _int2bytes(value, length=0, byteorder="big", signed=False):
-    """int.to_bytes
-    """
+    """int.to_bytes"""
     if length == 0:
         if signed:
             c = -128
             length = 1
             while c > value:
                 c *= 256
                 length += 1
@@ -206,14 +226,14 @@
             bs.append(value % 256)
             value = value // 256
     if signed:
         pad = 255
     else:
         pad = 0
     if length:
-        bs += [pad] * (length-len(bs))
+        bs += [pad] * (length - len(bs))
     if not bs:
         bs.append(pad)
     if byteorder == "big":
         bs.reverse()
     result = b"".join([bchar(x) for x in bs])
     return result
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.3.9/zenutils/randomutils.py` & `zenutils-0.4.8/zenutils/randomutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""随机数工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 __all__ = [
     "choices",
     "get_password_seed32",
     "Random",
     "Lcg31Random",
@@ -22,74 +31,75 @@
 import getpass
 import os
 import threading
 import hashlib
 import struct
 import functools
 
-if not hasattr(time, "perf_counter"): # fix for py2.7
+if not hasattr(time, "perf_counter"):  # fix for py2.7
     time.perf_counter = time.clock
 
-DEFAULT_MODULUS = (2 ** 30 - 123) * 0.91 # always NOT change this
-DEFAULT_MULTIPLIER = (2 ** 29 - 456) * 0.93 # always NOT change this
-DEFAULT_INCREMENT = (2 ** 28 - 789) * 0.95 # always NOT change this
+DEFAULT_MODULUS = (2**30 - 123) * 0.91  # always NOT change this
+DEFAULT_MULTIPLIER = (2**29 - 456) * 0.93  # always NOT change this
+DEFAULT_INCREMENT = (2**28 - 789) * 0.95  # always NOT change this
 
-LCG31_RANDOM_DEFAULT_MODULUS = 2 ** 31
+LCG31_RANDOM_DEFAULT_MODULUS = 2**31
 LCG31_RANDOM_DEFAULT_MULTIPLIER = 1103515245
 LCG31_RANDOM_DEFAULT_INCREMENT = 12345
 
 
 def get_password_seed32(passowrd=None):
     """Turn password to int32 seed value.
 
     password can be None, str, bytes, int, long typed.
     """
-    modulus=2**32
+    modulus = 2**32
     if passowrd is None:
         return int(time.time()) % modulus
     if isinstance(passowrd, NUMERIC_TYPES):
         return int(passowrd) % modulus
     if isinstance(passowrd, float):
         return int(passowrd) % modulus
     if isinstance(passowrd, STR_TYPE):
         passowrd = passowrd.encode("utf-8")
     if isinstance(passowrd, BYTES_TYPE):
         from zlib import crc32
+
         return crc32(passowrd) % modulus
     else:
-        msg = "Random seed type must be in (str, bytes, int, long, float), but {} got.".format(type(passowrd))
+        msg = "Random seed type must be in (str, bytes, int, long, float), but {} got.".format(
+            type(passowrd)
+        )
         raise ValueError(msg)
 
 
 class RandomBase(object):
-    """Pseudo-random generator base.
-    """
+    """Pseudo-random generator base."""
+
     def __init__(self, seed=None, **kwrags):
         self.seed = self.get_seed(seed, **kwrags)
 
     @classmethod
     def get_seed(cls, seed, **kwargs):
         return get_password_seed32(seed)
 
     def random(self):
-        """return a float number in [0, 1).
-        """
+        """return a float number in [0, 1)."""
         raise NotImplementedError()
 
-    def randint(self, a, b = None):
-        """If a<b, then return int number in [a, b). If a>b, then return int number in [b, a).
-        """
+    def randint(self, a, b=None):
+        """If a<b, then return int number in [a, b). If a>b, then return int number in [b, a)."""
         if b is None:
             return int(self.random() * a)
         else:
             if a > b:
                 a, b = b, a
             return int(self.random() * (b - a) + a)
 
-    def get_bytes(self, length = 1):
+    def get_bytes(self, length=1):
         return bytes(bytearray([self.randint(256) for _ in range(length)]))
 
     def choice(self, seq):
         index = self.randint(len(seq))
         return seq[index]
 
     def choices(self, population, k=1):
@@ -107,14 +117,15 @@
             q = self.randint(length)
             if p == q:
                 q += self.randint(length)
                 q %= length
             thelist[p], thelist[q] = thelist[q], thelist[p]
         return thelist
 
+
 class Random(RandomBase):
     """Pseudo-random number generator. Linear congruential generator.
 
     ## randomness testing
 
     import os
     import random
@@ -184,50 +195,62 @@
     randomutils.Random(2)=80
     randomutils.Random(3)=53
     randomutils.Random(4)=98189
     randomutils.Random(5)=1097420
     randomutils.Random(6)=10117127       # not so good, about 5,000,000 ~ 10,000,000
 
     """
-    def __init__(self, seed=None, a=DEFAULT_MULTIPLIER, c=DEFAULT_INCREMENT, m=DEFAULT_MODULUS):
+
+    def __init__(
+        self, seed=None, a=DEFAULT_MULTIPLIER, c=DEFAULT_INCREMENT, m=DEFAULT_MODULUS
+    ):
         self.seed = self.get_seed(seed)
         self.a = a
         self.c = c
         self.m = m
 
     @classmethod
     def get_seed(cls, seed):
         from zenutils import numericutils
+
         if seed is None:
             return time.time()
         if isinstance(seed, STR_TYPE):
             seed = seed.encode("utf-8")
         if isinstance(seed, BYTES_TYPE):
             seed = numericutils.from_bytes(hashlib.sha512(seed).digest(), "big")
         if isinstance(seed, NUMERIC_TYPES):
             return seed
         else:
-            msg = "Random seed type must be in (str, bytes, int, long, float), but {} got.".format(type(seed))
+            msg = "Random seed type must be in (str, bytes, int, long, float), but {} got.".format(
+                type(seed)
+            )
             raise ValueError(msg)
 
     def random(self):
-        """return a float number in [0, 1).
-        """
+        """return a float number in [0, 1)."""
         r = (self.a * self.seed + self.c) % self.m
         p = r / self.m
         self.seed = r
         return p
 
+
 class Lcg31Random(RandomBase):
     """Linear congruential generator.
 
     Using modulus=2**31, multiplier=1103515245, increment=12345
     """
 
-    def __init__(self, seed=None, a=LCG31_RANDOM_DEFAULT_MULTIPLIER, c=LCG31_RANDOM_DEFAULT_INCREMENT, m=LCG31_RANDOM_DEFAULT_MODULUS):
+    def __init__(
+        self,
+        seed=None,
+        a=LCG31_RANDOM_DEFAULT_MULTIPLIER,
+        c=LCG31_RANDOM_DEFAULT_INCREMENT,
+        m=LCG31_RANDOM_DEFAULT_MODULUS,
+    ):
         self.a = a
         self.c = c
         self.m = m
         self.seed = self.get_seed(seed)
 
     @classmethod
     def get_seed(cls, seed):
@@ -235,16 +258,16 @@
 
     def random(self):
         r = (self.a * self.seed + self.c) % self.m
         p = r / self.m
         self.seed = r
         return p
 
-class HashPrng(RandomBase):
 
+class HashPrng(RandomBase):
     BASE_BYTES = 4
     BASE = 256**BASE_BYTES
 
     def __init__(self, seed=None, method=hashlib.sha512):
         self.seed = self.get_seed(seed, method)
         self.generator = method(self.seed)
         self.digests = []
@@ -260,91 +283,116 @@
     def random(self):
         if not self.digests:
             self.round += 1
             self.generator.update(force_bytes(self.round))
             self.generator.update(self.seed)
             digest_data = self.generator.digest()
             digest_count = len(digest_data) // 4
-            self.digests = list(struct.unpack(">" + ("I"*digest_count), digest_data))
+            self.digests = list(struct.unpack(">" + ("I" * digest_count), digest_data))
         digest = self.digests.pop()
         result = 1.0 * digest / self.BASE
         return result
 
+
 def get_random_space_size(generator, length):
     data = set()
     while True:
         seed = generator.get_bytes(length)
         if seed in data:
             return len(data)
         data.add(seed)
 
 
 class UuidGenerator(object):
-    """UUID generator, using machine based counter, so that it will NOT generate conflict UUIDs.
-    """
+    """UUID generator, using machine based counter, so that it will NOT generate conflict UUIDs."""
+
     def __init__(self, namespace=None):
         from zenutils import sysutils
         from zenutils import strutils
 
         self.namespace = strutils.force_text(namespace or "default")
         self.seed1 = strutils.force_text(uuid.uuid1())
         self.seed4 = strutils.force_text(uuid.uuid4())
         self.hostname = strutils.force_text(socket.gethostname())
         self.node = strutils.force_text(uuid.getnode())
         self.user = strutils.force_text(getpass.getuser())
         self.pid = strutils.force_text(os.getpid())
         self.tid = strutils.force_text(sysutils.get_current_thread_id())
         self.counter = 0
         self.counter_lock = threading.Lock()
-        self.domain_template = ".".join(["{ts1}", "{ts2}", "{counter}", self.tid, self.pid, self.user, self.node, self.hostname, self.seed4, self.seed1, self.namespace])
+        self.domain_template = ".".join(
+            [
+                "{ts1}",
+                "{ts2}",
+                "{counter}",
+                self.tid,
+                self.pid,
+                self.user,
+                self.node,
+                self.hostname,
+                self.seed4,
+                self.seed1,
+                self.namespace,
+            ]
+        )
         self.ts0 = time.perf_counter()
 
     def next(self, n=1):
         from zenutils import strutils
+
         if n < 1:
             return []
         with self.counter_lock:
             counter_start = self.counter
             self.counter += n
             counter_end = self.counter
         uuids = []
         for counter in range(counter_start, counter_end):
             ts1 = int(time.time() * 1000000)
             ts2 = int(time.perf_counter() * 1000000000)
             domain = self.domain_template.format(ts1=ts1, ts2=ts2, counter=counter)
-            new_uuid = uuid.UUID(bytes=hashlib.md5(uuid.NAMESPACE_DNS.bytes + strutils.force_bytes(domain)).digest())
+            new_uuid = uuid.UUID(
+                bytes=hashlib.md5(
+                    uuid.NAMESPACE_DNS.bytes + strutils.force_bytes(domain)
+                ).digest()
+            )
             uuids.append(new_uuid)
         if n == 1:
             return uuids[0]
         else:
             return uuids
 
+
 uuidgen = UuidGenerator()
 
+
 def uuid1():
     return uuidgen.next()
 
+
 uuid3 = uuid4 = uuid5 = uuid1
 
+
 def choices(thelist, k):
     """Randomly select k elements from thelist. Element can be selected multiple times.
 
     @Returns:
         (list): Returns selected k elements.
-    
+
     @Parameters:
         thelist(list of Any): The list where the elements select from.
         k(int): Select K times.
-    
+
     @Examples:
         randomutils.choices([1,2,3], 2) --> Result may [1, 1], [1, 2], [1,3], [2, 1], [2, 2]...
         randomutils.choices('hello', 2) --> Result may ['h', 'e'], ['h', 'o']...
     """
     return [random.choice(thelist) for _ in range(k)]
 
+
 Md5Prng = functools.partial(HashPrng, method=hashlib.md5)
 ShaPrng = functools.partial(HashPrng, method=hashlib.sha1)
 Sha1Prng = functools.partial(HashPrng, method=hashlib.sha1)
 Sha224Prng = functools.partial(HashPrng, method=hashlib.sha224)
 Sha256Prng = functools.partial(HashPrng, method=hashlib.sha256)
 Sha384Prng = functools.partial(HashPrng, method=hashlib.sha384)
 Sha512Prng = functools.partial(HashPrng, method=hashlib.sha512)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.3.9/zenutils/sixutils.py` & `zenutils-0.4.8/zenutils/sixutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""PYTHON2/3兼容性处理工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 
 __all__ = [
     "PY2",
     "PY3",
     "STR_TYPE",
     "BYTES_TYPE",
     "BASESTRING_TYPES",
@@ -28,27 +37,28 @@
 default_encoding = "utf-8"
 
 INT_TO_BYTES = {}
 if sys.version_info.major == 2:
     range = xrange
     PY2 = True
     PY3 = False
-    BASESTRING_TYPES = (basestring,str,unicode)
+    BASESTRING_TYPES = (basestring, str, unicode)
     STR_TYPE = unicode
     BYTES_TYPE = str
     for i in range(256):
         INT_TO_BYTES[i] = chr(i)
     NUMERIC_TYPES = (int, long, float)
     InterruptedError = KeyboardInterrupt
     __all__.append("InterruptedError")
 
     def create_new_class(name, bases, dict, **kwargs):
         if isinstance(name, unicode):
             name = name.encode("utf-8")
         return type(name, bases, dict, **kwargs)
+
 else:
     PY2 = False
     PY3 = True
     BASESTRING_TYPES = (str, bytes)
     STR_TYPE = str
     BYTES_TYPE = bytes
     for i in range(256):
@@ -56,24 +66,25 @@
     NUMERIC_TYPES = (int, float)
     create_new_class = type
 
 if sys.version_info.major == 3 and sys.version_info.minor in [0, 1, 2]:
     InterruptedError = KeyboardInterrupt
     __all__.append("InterruptedError")
 
+
 def force_bytes(value, encoding=None):
     """Turn all things to bytes. If the original value is bytes, try to decode with encoding given or default encodings utf-8 and gb18030.
 
     @Returns:
         (str): Returns a str value.
-    
+
     @Parameters:
         value(str or bytes or any): The value to be transformed.
         encoding(str or list[str], optional): The encoding method will be used to decode.
-    
+
     @Example:
         assert sixutils.force_bytes(b'hello') == b'hello'
         assert sixutils.force_bytes('测试'.encode('utf-8')) == '测试'
         assert sixutils.force_bytes('hello') == b'hello'
         assert sixutils.force_bytes(1234) == b'1234'
         assert sixutils.force_bytes([1,2,3]) == b"[1, 2, 3]"
     """
@@ -86,20 +97,21 @@
     encoding = encoding or default_encoding
     if isinstance(value, STR_TYPE):
         return value.encode(encoding)
     else:
         value = STR_TYPE(value)
         return value.encode(encoding)
 
+
 def force_text(value, encoding=None):
     """Turn all things to text. If the original value is bytes, try to decode with encoding given or default encodings utf-8 and gb18030.
 
     @Returns:
         (str): Returns a str value.
-    
+
     @Parameters:
         value(str or bytes or any): The value to be transformed.
         encoding(str or list[str], optional): The encoding method will be used to decode.
 
     @Example:
         assert sixutils.force_text(b'hello') == 'hello'
         assert sixutils.force_text('测试'.encode('utf-8')) == '测试'
@@ -127,68 +139,71 @@
             return value.decode(encoding)
         except UnicodeDecodeError as error:
             last_error = error
     if last_error:
         last_error.encoding = " or ".join(encodings)
         raise last_error
 
+
 def bytes_to_array(data):
     """Turn bytes into list of bytes char.
 
     @Returns:
         (list of bytes char): Returns the list of the bytes char.
-    
+
     @Parameters:
         data(str or bytes): The data to be splitted.
-    
+
     @Example:
         sixutils.bytes_to_array(b"hello") == [b"h", b"e", b"l", b"l", b"o"]
     """
     data = force_bytes(data)
     if PY2:
         return list(data)
     else:
-        return [data[idx:idx+1] for idx in range(len(data))]
+        return [data[idx : idx + 1] for idx in range(len(data))]
+
 
 def bstr_to_array(data):
     """Get char array of the given data.
 
     Returns:
         (list of char): The char array of the given daa.
-    
+
     @Parameters:
         data(str or bytes): The data will be split into chars.
-    
+
     @Examples:
         assert sixutils.bstr_to_array("hello") == ["h", "e", "l", "l", "o"]
         assert sixutils.bstr_to_array(b"hello") == [b"h", b"e", b"l", b"l", b"o"]
     """
     if isinstance(data, BYTES_TYPE):
         return bytes_to_array(data)
     else:
         return list(data)
 
+
 def bchar(value):
     """Similar as chr(value) by returns bytes char. The value is in [0, 255].
 
     @Returns:
         (bytes char): One length bytes.
-    
+
     @Parameters:
         value(int): The int value between [0, 255].
-    
+
     @Example:
         assert bchar(0) == b'\\x00';
         assert bchar(1) == b'\\x01';
         assert bchar(255) == b'\\xff'.
     """
     return INT_TO_BYTES[value]
 
+
 def TEXT(value):
-    """Alias for force_text.
-    """
+    """Alias for force_text."""
     return force_text(value)
 
+
 def BYTES(value):
-    """Alias for force_bytes.
-    """
+    """Alias for force_bytes."""
     return force_bytes(value)
```

### Comparing `zenutils-0.3.9/zenutils/strutils.py` & `zenutils-0.4.8/zenutils/strutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""字符串工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 """
 String operate functions.
 """
 
 __all__ = [
+    "StrUtils",
     "HEXLIFY_CHARS",
     "URLSAFEB64_CHARS",
     "BASE64_CHARS",
     "SHI",
     "BAI",
     "QIAN",
     "WAN",
     "YI",
     "default_encodings",
     "default_encoding",
     "default_random_string_choices",
     "default_cn_yuan",
+    "simple_cn_yuan",
     "default_cn_digits",
     "default_cn_places",
     "default_cn_negative",
     "default_cn_float_places",
     "random_string",
     "char_force_to_int",
     "force_int",
@@ -88,64 +99,48 @@
 import uuid
 from decimal import Decimal
 from io import BytesIO
 from io import open
 from .sixutils import *
 
 HEXLIFY_CHARS = TEXT("0123456789abcdefABCDEF")
-URLSAFEB64_CHARS = TEXT("-0123456789=ABCDEFGHIJKLMNOPQRSTUVWXYZ_abcdefghijklmnopqrstuvwxyz\r\n")
-BASE64_CHARS = TEXT("+/0123456789=ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz\r\n")
+URLSAFEB64_CHARS = TEXT(
+    "-0123456789=ABCDEFGHIJKLMNOPQRSTUVWXYZ_abcdefghijklmnopqrstuvwxyz\r\n"
+)
+BASE64_CHARS = TEXT(
+    "+/0123456789=ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz\r\n"
+)
 
 SHI = 10
 BAI = SHI * 10
 QIAN = BAI * 10
 WAN = QIAN * 10
 YI = WAN * WAN
 
 default_encodings = ["utf8", "gb18030"]
 default_encoding = "utf-8"
 default_random_string_choices = TEXT(string.ascii_letters)
 default_cn_yuan = TEXT("圆")
+simple_cn_yuan = TEXT("元")
 default_cn_digits = TEXT("零壹贰叁肆伍陆柒捌玖")
 default_cn_places = TEXT("拾佰仟万亿")
 default_cn_negative = TEXT("负")
 default_cn_float_places = TEXT("角分厘毫丝忽微")
 
 
-def random_string(length, choices=default_random_string_choices):
-    """Generates a random string of specified length using specified characters.
-
-    In [3]: strutils.random_string(8)
-    Out[3]: 'wJhsaYVq'
-
-    In [4]: strutils.random_string(32)
-    Out[4]: 'JtYNblzfEFYdgwcTjNiorwucrlHuIeTQ'
-
-    In [5]: import string
-
-    In [8]: strutils.random_string(32, choices=string.ascii_letters+string.punctuation)
-    Out[8]: "]ivN^F]v#jPraNLC:F?<}:!'}aox=lKY"
-
-    In [9]: strutils.random_string(32, choices=string.ascii_letters+string.punctuation)
-    Out[9]: 'Flx,TOkDV_g&CsHq#l`RZ:(J#eVxENYJ'
-    """
-    from zenutils import randomutils
-    empty = force_type_to("", choices)
-    choices = bstr_to_array(choices)
-    return empty.join(randomutils.choices(choices, k=length))
-
 def char_force_to_int(char):
     if callable(char):
         char = char()
     if char is None:
         return None
     if isinstance(char, int):
         return char
     return ord(char)
 
+
 def force_int(value):
     if callable(value):
         value = value()
     if value is None:
         return None
     if isinstance(value, int):
         return value
@@ -154,28 +149,30 @@
     if isinstance(value, Decimal):
         return int(value)
     value = force_text(value)
     if "." in value:
         return int(float(value))
     return int(value)
 
+
 def force_float(value):
     if callable(value):
         value = value()
     if value is None:
         return None
     if isinstance(value, float):
         return value
     if isinstance(value, int):
         return float(value)
     if isinstance(value, Decimal):
         return float(value)
     value = force_text(value)
     return float(value)
 
+
 def force_numberic(value):
     if callable(value):
         value = value()
     if value is None:
         return None
     if isinstance(value, (int, float, Decimal)):
         return value
@@ -183,54 +180,56 @@
         value = value.decode(default_encoding)
     value = str(value)
     if "." in value:
         return float(value)
     else:
         return int(value)
 
+
 def wholestrip(text):
-    """Remove all white spaces in text. White spaces are ' \\t\\n\\r\\x0b\\x0c\\u3000'. 
-    
-    Note: 
-    
-    It's NOT only trim the left and right white characters, 
+    """Remove all white spaces in text. White spaces are ' \\t\\n\\r\\x0b\\x0c\\u3000'.
+
+    Note:
+
+    It's NOT only trim the left and right white characters,
     but also remove white characters in the middle of the text.
     """
     if text is None:
         return None
     for space in string.whitespace + "\u3000":
         text = text.replace(space, "")
     return text
 
+
 def simplesplit(text, sep=None, maxsplit=None):
     """Simple split. Same as str.split(xxx). Make it behave the same both in py2 and py3.
 
     @Returns:
         (list of str, list fof bytes): Return a list of the words in the string, using sep as the delimiter string.
-    
+
     @Parameters:
         text(str or bytes): The text to be splitted.
         sep(str or bytes):  The delimiter according which to split the string.
                             None (the default value) means split according to any whitespace,
                             and discard empty strings from the result.
         maxsplit(int):      Maximum number of splits to do.
-                            -1 means no limit. 
+                            -1 means no limit.
                             None means using system default which is -1.
     """
     sep = force_type_to(sep, text)
     if maxsplit:
         return text.split(sep, maxsplit)
     elif sep:
         return text.split(sep)
     else:
         return text.split()
 
+
 def split2(text, seps=None):
-    """Split string into two parts.
-    """
+    """Split string into two parts."""
     if text is None:
         return None
     if not seps:
         ss = simplesplit(text, maxsplit=1)
     else:
         if not isinstance(seps, (list, set, tuple)):
             seps = [seps]
@@ -247,17 +246,17 @@
         ss = simplesplit(text, sep=min_sep, maxsplit=1)
     if len(ss) == 0:
         ss.append("")
     if len(ss) == 1:
         ss.append("")
     return ss
 
+
 def split(text, seps, strip=False):
-    """Split string with a list of sperators. seps is a list of string, all sep in the seps are treated as delimiter.
-    """
+    """Split string with a list of sperators. seps is a list of string, all sep in the seps are treated as delimiter."""
     if not text:
         return []
     if not isinstance(seps, (list, set, tuple)):
         seps = [seps]
     results = [text]
     for sep in seps:
         row = []
@@ -267,115 +266,120 @@
     if strip:
         row = []
         for value in results:
             row.append(value.strip())
         results = row
     return results
 
+
 def force_type_to(src, dst):
     """Change src's type to the type of the dst.
 
     @Returns:
         (str or bytes): If dst is in bytes type, turns src's type to types, and returns changed value.
                         If dst is in str type, turns src's type to str, and returns changed value.
                         If dst is in other types, just returns the src value.
-    
+
     @Parameters:
         src(str or bytes): The src data.
         target(str or bytes): The dst data, which type will be copied.
 
     """
     if isinstance(dst, STR_TYPE):
         return force_text(src)
     elif isinstance(dst, BYTES_TYPE):
         return force_bytes(src)
     else:
         return src
 
+
 def str_composed_by(text, choices):
     """Test if text is composed by chars in the choices.
 
     @Returns:
         (bool): If all char in text is also in choices, returns True.
                 If one char in text is NOT in choices, returns False.
-    
+
     @Parameters:
         text(str or bytes): The text to be tested.
         choices(str, bytes, list of str char, list of bytes char): The good char set.
     """
     text = force_type_to(text, choices)
     text_set = set(text)
     choices_set = set(choices)
-    if text_set - choices_set: # text has char not in choices, so just returns False
+    if text_set - choices_set:  # text has char not in choices, so just returns False
         return False
     else:
         return True
 
+
 is_str_composed_by_the_choices = str_composed_by
 
+
 def is_hex_digits(text):
-    """Test if all chars in text is hex digits.
-    """
+    """Test if all chars in text is hex digits."""
     if not text:
         return False
     return str_composed_by(text, HEXLIFY_CHARS)
 
+
 def join_lines(text):
-    """Join multi-lines into single line.
-    """
+    """Join multi-lines into single line."""
     empty = force_type_to("", text)
     return empty.join(text.splitlines())
 
+
 def is_urlsafeb64_decodable(text):
-    """Test if the text can be decoded by urlsafeb64 method.
-    """
+    """Test if the text can be decoded by urlsafeb64 method."""
     text = wholestrip(text)
     if not text:
         return False
     if len(text) % 4 != 0:
         return False
     text = join_lines(text)
     return str_composed_by(text, URLSAFEB64_CHARS)
 
+
 def is_base64_decodable(text):
-    """Test  if the text can be decoded by base64 method.
-    """
+    """Test  if the text can be decoded by base64 method."""
     text = wholestrip(text)
     if not text:
         return False
     if len(text) % 4 != 0:
         return False
     text = join_lines(text)
     return str_composed_by(text, BASE64_CHARS)
 
+
 def is_unhexlifiable(text):
-    """Test if the text can be decoded by unhexlify method.
-    """
+    """Test if the text can be decoded by unhexlify method."""
     text = wholestrip(text)
     if not text:
         return False
     if len(text) % 2 != 0:
         return False
     return str_composed_by(text, HEXLIFY_CHARS)
 
+
 def text_display_length(text, unicode_display_length=2, encoding=None):
-    """Get text display length.
-    """
+    """Get text display length."""
     text = force_text(text, encoding)
     length = 0
     for c in text:
         if ord(c) <= 128:
             length += 1
         else:
             length += unicode_display_length
     return length
 
-def text_display_shorten(text, max_length, unicode_display_length=2, suffix="...", encoding=None):
-    """Shorten text to fix the max display length.
-    """
+
+def text_display_shorten(
+    text, max_length, unicode_display_length=2, suffix="...", encoding=None
+):
+    """Shorten text to fix the max display length."""
     text = force_text(text, encoding)
     if max_length < len(suffix):
         max_length = len(suffix)
     tlen = text_display_length(text, unicode_display_length=unicode_display_length)
     if tlen <= max_length:
         return text
     result = ""
@@ -392,29 +396,31 @@
             result += c
             break
         else:
             break
     result += suffix
     return result
 
+
 def smart_get_binary_data(text):
     """Smart get bytes form the given data.
 
     @Returns:
         (bytes): The parsed bytes data.
-    
+
     @Paramters:
         text(text or bytes): If text is bytes typed, just returns it's value.
                              If text is str typed, try to parse it.
                              First try to unhexlify it.
                              Second try to do urlsafe_b64decode it.
                              Third try to do base64.decodebytes on it.
                              Forth try to encode it as utf8(default_encoding).
     """
     from zenutils import base64utils
+
     if isinstance(text, STR_TYPE):
         if is_unhexlifiable(text):
             text = force_bytes(text)
             return binascii.unhexlify(text)
         elif is_urlsafeb64_decodable(text):
             text = force_bytes(text)
             return base64utils.urlsafe_b64decode(text)
@@ -424,14 +430,15 @@
         else:
             return force_bytes(text)
     elif isinstance(text, BYTES_TYPE):
         return text
     else:
         raise TypeError()
 
+
 def is_chinese_character(c):
     """
     Block                                   Range       Comment
     CJK Unified Ideographs                  4E00-9FFF   Common
     CJK Unified Ideographs Extension A      3400-4DBF   Rare
     CJK Unified Ideographs Extension B      20000-2A6DF Rare, historic
     CJK Unified Ideographs Extension C      2A700–2B73F Rare, historic
@@ -451,70 +458,75 @@
         return True
     if 0x2B740 <= c <= 0x2B81F:
         return True
     if 0x2B820 <= c <= 0x2CEAF:
         return True
     if 0xF900 <= c <= 0xFAFF:
         return True
-    if 0x2F800 <=c <= 0x2FA1F:
+    if 0x2F800 <= c <= 0x2FA1F:
         return True
     return False
 
+
 def binarify(data):
     """Turn bytes into binary string. Similar to binascii.hexlify(), but using binary instread hex.
-    
+
     Examples:
 
     In [11]: strutils.binarify(b'0')
     Out[11]: '00110000'
 
     In [12]: strutils.binarify(b'a')
     Out[12]: '01100001'
 
     In [13]: strutils.binarify(b'hello')
     Out[13]: '0110100001100101011011000110110001101111'
     """
     data = bytes_to_array(data)
     return "".join(["{:08b}".format(ord(x)) for x in data])
 
+
 def unbinarify(text):
     if not text:
         return b""
     text = force_text(text)
     from zenutils import listutils
+
     return b"".join([bchar(int(x, 2)) for x in listutils.chunk(text, 8)])
 
+
 def substrings(value, lengths=None):
     value = value or ""
     subs = set()
     if lengths is None:
         lengths = list(range(len(value)))
     elif isinstance(lengths, int):
         lengths = [lengths]
     for length in lengths:
         for start in range(len(value) - length + 1):
-            sub = value[start: start + length]
+            sub = value[start : start + length]
             subs.add(sub)
     return subs
 
+
 def combinations2(values, length):
-    """同combinations，使用了itertools.product实现，简化了实现逻辑。但性能仅为combinations的一半。仅供参考。
-    """
+    """同combinations，使用了itertools.product实现，简化了实现逻辑。但性能仅为combinations的一半。仅供参考。"""
     results = set()
     min_length = min([len(x) for x in values])
     repeat = int(math.ceil(length / min_length * 2))
     for vs in itertools.product(values, repeat=repeat):
         line = "".join(vs)
         line_length = len(line)
         max_start_index = line_length - length
-        for index in range(max_start_index+1):
-            word = line[index:index+length]
+        for index in range(max_start_index + 1):
+            word = line[index : index + length]
             results.add(word)
     return results
 
+
 def combinations(values, length):
     """取values中各字符串的任意连接（可重复取），在组成的新字符串中，取任意指定长度子串所形成的集合。
 
     例如：
 
     In [96]: strutils.combinations(['abc', 'xyz'], 5)
     Out[96]:
@@ -535,15 +547,15 @@
     'zxyza',
     'zxyzx'}
 
     """
     values = list(values)
     min_length = min([len(x) for x in values])
     max_length = max([len(x) for x in values])
-    repeat = int(math.ceil((length*1.0 - min_length)/min_length))
+    repeat = int(math.ceil((length * 1.0 - min_length) / min_length))
     repeat_incr = False
     if length <= min_length:
         repeat_incr = True
     if length % min_length == 2 and length % max_length == 2:
         repeat_incr = True
     if length % min_length == 0 and length % max_length == 0:
         repeat_incr = True
@@ -569,28 +581,44 @@
             good_words.add(x)
     result_words = set()
     for word in good_words:
         for subword in substrings(word, length):
             result_words.add(subword)
     return result_words
 
-def captital_number(value, yuan=default_cn_yuan, digits=default_cn_digits, places=default_cn_places, negative=default_cn_float_places, float_places=default_cn_float_places):
+
+def captital_number(
+    value,
+    yuan=default_cn_yuan,
+    digits=default_cn_digits,
+    places=default_cn_places,
+    negative=default_cn_float_places,
+    float_places=default_cn_float_places,
+):
     from zenutils.numericutils import float_split
 
     sign, int_part, float_part = float_split(value, precision=7)
 
     def parse4(value):
         qian = value // QIAN
         value = value % QIAN
         bai = value // BAI
         value = value % BAI
         shi = value // SHI
         value = value % SHI
         ge = value
-        return digits[qian] + places[2] + digits[bai] + places[1] + digits[shi] + places[0] + digits[ge]
+        return (
+            digits[qian]
+            + places[2]
+            + digits[bai]
+            + places[1]
+            + digits[shi]
+            + places[0]
+            + digits[ge]
+        )
 
     def parse8(value):
         high = value // WAN
         low = value % WAN
         return parse4(high) + places[3] + parse4(low)
 
     def parse(value):
@@ -599,15 +627,15 @@
             yis.append(value % YI)
             value //= YI
         yis.reverse()
         return places[4].join([parse8(x) for x in yis])
 
     def remove0(value_string):
         z0 = digits[0]
-        z00 = digits[0] +  digits[0]
+        z00 = digits[0] + digits[0]
         for place in places:
             value_string = value_string.replace(digits[0] + place, digits[0])
         while z00 in value_string:
             value_string = value_string.replace(z00, z0)
         if value_string.startswith(z0):
             value_string = value_string[1:]
         if value_string.endswith(z0):
@@ -635,36 +663,44 @@
 
     result = int_string + yuan + float_string
     if sign < 0:
         result = negative + result
 
     return result
 
+
 def clean(value, keep_chars):
     """Clean the string value and only keep characters in keep_chars.
 
     @Returns:
-        (str or bytes): Cleaned new value which it's chars are all in keep_chars.  
+        (str or bytes): Cleaned new value which it's chars are all in keep_chars.
 
     @Parameters:
         value(str or bytes): The string to be cleaned.
         keep_chars(str or bytes): The good characters will be kept.
-    
+
     @Note:
         The two parameters' type must be the same.
     """
     if not isinstance(keep_chars, set):
         keep_chars = set(bstr_to_array(keep_chars))
     empty = force_type_to("", value)
     vs = [x for x in bstr_to_array(value) if x in keep_chars]
     return empty.join(vs)
 
-do_clean = clean # Alias of clean
 
-def camel(value, clean=False, keep_chars=string.ascii_letters + string.digits, lower_first=False):
+do_clean = clean  # Alias of clean
+
+
+def camel(
+    value,
+    clean=False,
+    keep_chars=string.ascii_letters + string.digits,
+    lower_first=False,
+):
     if value is None:
         return None
     words = []
     word_chars = set(string.ascii_letters)
     word = ""
     non_word = ""
     for c in value:
@@ -689,106 +725,113 @@
         result = "".join(words)
     if len(result) < 1:
         return result
     if lower_first:
         result = result[0].lower() + result[1:]
     return result
 
+
 def no_mapping(value):
     return value
 
+
 def none_to_empty_string(value):
     """Turn None to empty string.
 
     @Returns:
         (Any): If value is None, returns empty string, or else returns value itself.
-    
+
     @Parameters:
         value(Any): The value to be transformed.
     """
     if value is None:
         return ""
     else:
         return value
 
+
 def strip_string(value):
     """If value is str, then do string strip, or else returns the value itself.
 
     @Returns:
         (Any): strip value.
 
     @Parameters:
         value(Any): The value to be strip. Only str/bytes typed value will be stripped.
     """
     if isinstance(value, (STR_TYPE, BYTES_TYPE)):
         return value.strip()
     else:
         return value
 
+
 def format_with_mapping(template, mapping, *args, **kwargs):
     def trans(value):
         if callable(mapping):
             return mapping(value)
         else:
             return mapping.get(value, value)
+
     new_args = []
     new_kwargs = {}
-    names = re.findall('{([^}:]*)', template)
+    names = re.findall("{([^}:]*)", template)
     counter = 0
     for index in range(len(names)):
         if names[index] == "":
             names[index] = counter
             counter += 1
         elif names[index].isdigit():
             names[index] = int(names[index])
     ps_args = [x for x in names if isinstance(x, int)]
     if ps_args:
         max_args_index = max(ps_args)
-        for index in range(max_args_index+1):
+        for index in range(max_args_index + 1):
             if index in names:
                 value = trans(args[index])
             else:
                 value = None
             new_args.append(value)
     for key, value in kwargs.items():
         if key in names:
             value = trans(kwargs[key])
         new_kwargs[key] = value
     return template.format(*new_args, **new_kwargs)
 
+
 default_quotes = [
-    '"""', # quote left and quote right are the same
+    '"""',  # quote left and quote right are the same
     "'''",
     '"',
     "'",
     "`",
-    ('“', '”'), # quote left and quote right are NOT the same
+    ("“", "”"),  # quote left and quote right are NOT the same
     ("‘", "’"),
     ("『", "』"),
     ("「", "」"),
     ("﹁", "﹂"),
     ("﹃", "﹄"),
     ("｢", "｣"),
-    ]
+]
+
 
 def unquote(value, quotes=None):
-    """Trim one level quote. If not quoted, do nothing.
-    """
+    """Trim one level quote. If not quoted, do nothing."""
     quotes = quotes or default_quotes
     for quote_pair in quotes:
         if isinstance(quote_pair, STR_TYPE):
             quote_pair = (quote_pair, quote_pair)
         if value.startswith(quote_pair[0]) and value.endswith(quote_pair[1]):
-            return value[len(quote_pair[0]):-1*len(quote_pair[1])]
+            return value[len(quote_pair[0]) : -1 * len(quote_pair[1])]
     return value
 
+
 def is_uuid(value, allow_bad_characters=False):
     """Test if the value is UUID typed or UUID liked str.
-    
-    If allow_bad_characters=True, 
+
+    If allow_bad_characters=True,
     treat c1fd56f3-bd79-42ed-a45c-d711c4032bag liked string as UUID,
     even it contains NON hex character(the last character g is NOT a hex digist).
     """
     if isinstance(value, uuid.UUID):
         return True
 
     if isinstance(value, (tuple, list)):
@@ -803,15 +846,15 @@
             _ = uuid.UUID(int=value)
             return True
         except ValueError:
             return False
 
     def broken_uuid_check(value):
         value = force_text(value).lower()
-        pattern = '^[a-zA-Z0-9]{8}-?[a-zA-Z0-9]{4}-?[a-zA-Z0-9]{4}-?[a-zA-Z0-9]{4}-?[a-zA-Z0-9]{12}$'
+        pattern = "^[a-zA-Z0-9]{8}-?[a-zA-Z0-9]{4}-?[a-zA-Z0-9]{4}-?[a-zA-Z0-9]{4}-?[a-zA-Z0-9]{12}$"
         if not re.match(pattern, value):
             return False
         ok_chars = set("0123456789abcdef-")
         bad_chars = 0
         for c in value:
             if not c in ok_chars:
                 bad_chars += 1
@@ -839,38 +882,45 @@
             except ValueError:
                 if allow_bad_characters:
                     return broken_uuid_check(value)
                 return False
 
     return False
 
+
 def stringlist_append(string_value, new_element, separator=",", allow_duplicate=True):
     elements = split(string_value, [separator], strip=True)
     if allow_duplicate or (not new_element in elements):
         elements.append(new_element)
     return separator.join(elements)
 
+
 def html_element_css_append(classes, new_class_name):
-    return stringlist_append(classes, new_class_name, separator=" ", allow_duplicate=False)
+    return stringlist_append(
+        classes, new_class_name, separator=" ", allow_duplicate=False
+    )
+
 
 def remove_prefix(thestring, prefix):
     if thestring.startswith(prefix):
-        return thestring[len(prefix):]
+        return thestring[len(prefix) :]
     else:
         return thestring
 
+
 def remove_suffix(thestring, suffix):
     if thestring.endswith(suffix):
         if len(suffix):
-            return thestring[:-len(suffix)]
+            return thestring[: -len(suffix)]
         else:
             return thestring
     else:
         return thestring
 
+
 def encodable(value, encoding=default_encoding):
     """Test if the string value can be encoded by special encoding.
 
     Examples:
 
     In [11]: strutils.encodable('hello') # ascii letters can be encoded by utf-8 encoding.
     Out[11]: True
@@ -884,14 +934,15 @@
     """
     try:
         value.encode(encoding)
         return True
     except UnicodeEncodeError:
         return False
 
+
 def decodable(value, encoding=default_encoding):
     """Test if the bytes value can be decoded by special encoding.
 
     Examples:
 
     In [2]: strutils.decodable('测试'.encode('gbk')) # string encoded by gbk can not be decoded by utf-8
     Out[2]: False
@@ -902,14 +953,15 @@
     """
     try:
         value.decode(encoding)
         return True
     except UnicodeDecodeError:
         return False
 
+
 def chunk(value, size):
     """Split string value into chunks. Chunk size must be greater than 0.
 
     Examples:
 
     In [33]: strutils.chunk('hello', 3)
     Out[33]: ['hel', 'lo']
@@ -925,21 +977,22 @@
         raise ValueError("chunk size must be greater than 0...")
     if value is None:
         return []
     chunks = []
     length = len(value)
     start = 0
     while start < length:
-        chunks.append(value[start:start+size])
+        chunks.append(value[start : start + size])
         start += size
     return chunks
 
+
 def get_all_substrings(value):
     """Get all substrings of the value.
-    
+
     Examples:
 
     In [4]: strutils.get_all_substrings('a')
     Out[4]: {'a'}
 
     In [5]: strutils.get_all_substrings('ab')
     Out[5]: {'a', 'ab', 'b'}
@@ -947,15 +1000,15 @@
     In [6]: strutils.get_all_substrings('abc')
     Out[6]: {'a', 'ab', 'abc', 'b', 'bc', 'c'}
 
     In [7]: strutils.get_all_substrings('abcd')
     Out[7]: {'a', 'ab', 'abc', 'abcd', 'b', 'bc', 'bcd', 'c', 'cd', 'd'}
 
     In [8]: strutils.get_all_substrings('abcde')
-    Out[8]: 
+    Out[8]:
     {'a',
     'ab',
     'abc',
     'abcd',
     'abcde',
     'b',
     'bc',
@@ -967,19 +1020,20 @@
     'd',
     'de',
     'e'}
     """
     substrings = set()
     for length in range(len(value)):
         length += 1
-        for index in range(len(value)-length+1):
-            substring = value[index:index+length]
+        for index in range(len(value) - length + 1):
+            substring = value[index : index + length]
             substrings.add(substring)
     return substrings
 
+
 def reverse(value):
     """Reverse a string.
 
     @Returns:
         (str): Returns the reversed string.
 
     @Parameters:
@@ -992,25 +1046,28 @@
     if value is None:
         return None
     empty = force_type_to("", value)
     chars = bstr_to_array(value)
     chars.reverse()
     return empty.join(chars)
 
-def get_image_bytes(image, format= "png"):
+
+def get_image_bytes(image, format="png"):
     """Save PIL image into bytes buffer instread of a disk file.
 
     @Returns:
         (bytes): The image content bytes.
-    
+
     @Parameters:
         image(Image, or filename of image, or image bytes): The image to be load content bytes.
         format(str, default to 'png'): If the image is an instance of PIL.Imgae, it need an format the save the image content.
     """
-    if isinstance(image, BYTES_TYPE) and len(image) >= 44: # the 1x1 webp image takes only 44 bytes
+    if (
+        isinstance(image, BYTES_TYPE) and len(image) >= 44
+    ):  # the 1x1 webp image takes only 44 bytes
         try:
             # try to open the image, it maybe a filename bytes.
             with open(image, "rb") as fobj:
                 pass
         except:
             return image
     if isinstance(image, BASESTRING_TYPES):
@@ -1019,62 +1076,101 @@
             return fobj.read()
     else:
         # image is PIL.Image object
         buffer = BytesIO()
         image.save(buffer, format=format)
         return buffer.getvalue()
 
-def get_base64image(image, format= "png"):
+
+def get_base64image(image, format="png"):
     """Turn image binary content into base64 encoded string, so that it can be used in image <img src="xxx" /> directly.
 
     @Returns:
         (str): The image src url string.
-    
+
     @Parameters:
         image(Image, or filename of the image, or the image bytes): The image to be transformed.
         format(str, default to 'png'). Format should match the content the image. Can be png, or jpeg, or gif.
     """
     from zenutils import base64utils
+
     image = get_image_bytes(image)
     return """data:image/{format};base64,{data}""".format(
         format=format,
         data=force_text(base64utils.encodebytes(image)),
-        )
+    )
+
 
 def parse_base64image(image):
     """Parse base64 encoded image string.
 
     @Returns:
         (format, image_bytes)
-    
+
     @Paramters:
         image(str): base64 encoded image string that can be used in html image tag's src property.
 
     """
     from zenutils import base64utils
+
     image = force_text(image)
     header, data = simplesplit(image, ",", maxsplit=1)
     format = re.findall("data:image/(.*);base64", header)[0]
     data = force_bytes(data)
     return format, base64utils.decodebytes(data)
 
+
 # ##################################################################
 # Removed to anotehr module
 # ##################################################################
 
+
 def bytes2ints(*args, **kwargs):
-    """See detail to zenutils.numericutils.bytes2ints.
-    """
+    """See detail to zenutils.numericutils.bytes2ints."""
     from zenutils import numericutils
+
     return numericutils.bytes2ints(*args, **kwargs)
 
+
 def ints2bytes(*args, **kwargs):
-    """See detail to zenutils.numericutils.ints2bytes.
-    """
+    """See detail to zenutils.numericutils.ints2bytes."""
     from zenutils import numericutils
+
     return numericutils.ints2bytes(*args, **kwargs)
 
+
 def int2bytes(*args, **kwargs):
-    """See tail to zenutils.numericutils.int2bytes.
-    """
+    """See tail to zenutils.numericutils.int2bytes."""
     from zenutils import numericutils
+
     return numericutils.int2bytes(*args, **kwargs)
+
+
+class StrUtils(object):
+    """字符串工具类。"""
+
+    @staticmethod
+    def random_string(length, choices=default_random_string_choices):
+        """Generates a random string of specified length using specified characters.
+
+        In [3]: strutils.random_string(8)
+        Out[3]: 'wJhsaYVq'
+
+        In [4]: strutils.random_string(32)
+        Out[4]: 'JtYNblzfEFYdgwcTjNiorwucrlHuIeTQ'
+
+        In [5]: import string
+
+        In [8]: strutils.random_string(32, choices=string.ascii_letters+string.punctuation)
+        Out[8]: "]ivN^F]v#jPraNLC:F?<}:!'}aox=lKY"
+
+        In [9]: strutils.random_string(32, choices=string.ascii_letters+string.punctuation)
+        Out[9]: 'Flx,TOkDV_g&CsHq#l`RZ:(J#eVxENYJ'
+        """
+        from zenutils import randomutils
+
+        empty = force_type_to("", choices)
+        choices = bstr_to_array(choices)
+        return empty.join(randomutils.choices(choices, k=length))
+
+
+random_string = StrUtils.random_string
```

### Comparing `zenutils-0.3.9/zenutils/sysutils.py` & `zenutils-0.4.8/zenutils/sysutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""操作系统工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 __all__ = [
     "get_current_thread_id",
     "get_worker_id",
     "get_random_script_name",
     "execute_script",
@@ -16,45 +25,50 @@
 import os
 import uuid
 import time
 import signal
 import socket
 import subprocess
 import threading
+
 try:
     import queue
 except ImportError:
-    import Queue as queue # fix for py2.7
+    import Queue as queue  # fix for py2.7
 
 
 def get_current_thread_id():
     """Get current thread id.
 
     @Returns:
         (int): Current thread's id.
-    
+
     @Parameters:
 
     """
     return threading.current_thread().ident
 
+
 def get_worker_id(prefix=None):
     """Get a unique name for a worker. The name template is `{prefix}:{hostname}:{process-id}:{thread-id}`.
 
     In [32]: from fastutils import sysutils
 
     In [33]: sysutils.get_worker_id('testapp')
     Out[33]: 'testapp:DESKTOP-MO5DJHQ:1896:9192'
     """
-    worker_inner_id = "{}:{}:{}".format(socket.gethostname(), os.getpid(), get_current_thread_id())
+    worker_inner_id = "{}:{}:{}".format(
+        socket.gethostname(), os.getpid(), get_current_thread_id()
+    )
     if prefix:
         return prefix + ":" + worker_inner_id
     else:
         return worker_inner_id
 
+
 def get_random_script_name(suffix=None):
     """Generate a random script name. For windows add .bat suffix.
 
     In [1]: import os
 
     In [2]: os.name
     Out[2]: 'nt'
@@ -68,18 +82,19 @@
         if os.name == "nt":
             suffix = ".bat"
         else:
             suffix = ""
     name = str(uuid.uuid4())
     return name + suffix
 
+
 class NonBlockReader(object):
     """
-    When we read from a stream, 
-    but not sure if it will block or not-block, 
+    When we read from a stream,
+    but not sure if it will block or not-block,
     so we read it from a new thread that will not block the main thread.
 
     Mostly you need to close the stream after your read,
     so that the created thread can got the read failed exception and end itself.
     """
 
     def __init__(self, stream, wait_time=1, autostart=True):
@@ -126,48 +141,61 @@
                 break
             results.append(line)
         return results
 
     def read(self):
         return "\n".join(self.readlines())
 
+
 def default_timeout_kill(pid, sig=signal.SIGINT):
     """Kill the process.
 
     @Returns:
         (None): Nothing.
-    
+
     @Parameters:
         pid(int): The process's pid to be killed.
         sig(SIGNAL, default to signal.SIGINT): The SIGNAL to be send to the process.
     """
     os.kill(pid, sig)
 
+
 def psutil_timeout_kill(pid, sig=signal.SIGINT):
     """Kill the process and it's all subprocesses. psutil is required which may not be installed whiling installing zenutils.
 
     @Retruns:
         (None): Nothing.
-    
+
     @Parameters:
         pid(int): The process's pid to be killed.
         sig(SIGNAL, default to signal.SIGINT): The SIGNAL to be send to the process and it's all subprocesses.
     """
     import psutil
+
     mainp = psutil.Process(pid)
     for subp in mainp.children(recursive=True):
         os.kill(subp.pid, sig)
     os.kill(mainp.pid, sig)
 
-def execute_script(script, workspace=None, script_name=None, timeout=0, timeout_kill=None, timeout_kill_wait=1, non_block_read_timeout=2, delete_script=True):
+
+def execute_script(
+    script,
+    workspace=None,
+    script_name=None,
+    timeout=0,
+    timeout_kill=None,
+    timeout_kill_wait=1,
+    non_block_read_timeout=2,
+    delete_script=True,
+):
     """Execute a shell script under special workspace.
 
     @Returns:
         (int, str, str): Returns script exitcode, std output and std error.
-    
+
     @Parameters:
         script(str): Script source code.
         workspace(str, optional): Workspace path. If not given, a random template folder will be used.
         script_name(str, optional): A name used for creating the temporary script file. If not given, a random name will be used.
         timeout(int, optional): Script run time limit. 0 means no time limit.
         kill_sig(SIGNAL): Send the signal to the subprocess if it's running time is exceeded.
         kill_wait(int): Wait for some seconds after send kill signal to the subprocess.
@@ -177,22 +205,30 @@
     """
     from zenutils import fsutils
     from zenutils import strutils
 
     workspace = workspace or fsutils.get_temp_workspace()
     if not os.path.exists(workspace):
         os.makedirs(workspace, exist_ok=True)
-    
+
     script_name = script_name or get_random_script_name()
     script_path = os.path.join(workspace, script_name)
     fsutils.write(script_path, script)
     os.chmod(script_path, 0o755)
 
     normally_finished_flag = False
-    p = subprocess.Popen(script_path, stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=workspace, shell=True, universal_newlines=True, bufsize=0)
+    p = subprocess.Popen(
+        script_path,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        cwd=workspace,
+        shell=True,
+        universal_newlines=True,
+        bufsize=0,
+    )
     if timeout > 0:
         try:
             p.wait(timeout)
             normally_finished_flag = True
         except subprocess.TimeoutExpired:
             timeout_kill = timeout_kill or default_timeout_kill
             try:
@@ -220,31 +256,35 @@
         code, stdout, stderr = p.returncode, p.stdout.read(), p.stderr.read()
         stdout = strutils.force_text(stdout)
         stderr = strutils.force_text(stderr)
         result = code, stdout, stderr
     else:
         stdout_reader = NonBlockReader(p.stdout, wait_time=non_block_read_timeout)
         stderr_reader = NonBlockReader(p.stderr, wait_time=non_block_read_timeout)
-        result = p.returncode, force_text(stdout_reader.read()), force_text(stderr_reader.read())
+        result = (
+            p.returncode,
+            force_text(stdout_reader.read()),
+            force_text(stderr_reader.read()),
+        )
         try:
             p.stdout.close()
             p.stderr.close()
         except Exception:
             pass
-    
+
     if delete_script:
         try:
             os.unlink(script_path)
         except Exception:
             pass
     return result
 
+
 def get_node_ip():
-    """get node's main ip address.
-    """
+    """get node's main ip address."""
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     s.settimeout(0)
     try:
         # doesn't even have to be reachable
         s.connect(("10.254.254.254", 1))
         ip = s.getsockname()[0]
     except Exception:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.3.9/zenutils/tests/assets/p1.jpeg` & `zenutils-0.4.8/zenutils/tests/assets/p1.jpeg`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/zenutils/tests/test_cacheutils.py` & `zenutils-0.4.8/zenutils/tests/test_cacheutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 from zenutils import cacheutils
 
 import random
 import unittest
 
 _test_cacheutils_counter = 0
 
+
 class Object(object):
     pass
 
-class TestCacheUtils(unittest.TestCase):
 
+class TestCacheUtils(unittest.TestCase):
     def test01(self):
         a = Object()
+
         def hi():
             return "hi"
+
         assert cacheutils.get_cached_value(a, "hi", hi) == "hi"
 
     def test02(self):
         global _test_cacheutils_counter
         _test_cacheutils_counter = 0
         a = Object()
+
         def counter():
             global _test_cacheutils_counter
             _test_cacheutils_counter += 1
             return _test_cacheutils_counter
+
         assert cacheutils.get_cached_value(a, "counter", counter) == 1
         assert cacheutils.get_cached_value(a, "counter", counter) == 1
 
     def test03(self):
         a = Object()
+
         @cacheutils.cache(a, "_num")
         def getNum():
             return random.randint(1, 10)
+
         v1 = getNum()
         v2 = getNum()
         v3 = getNum()
         assert v1
         assert v1 == v2 == v3
 
     def test04(self):
@@ -54,13 +69,28 @@
         assert v1
         assert v1 == v2 == v3
 
     def test5(self):
         @cacheutils.cache()
         def getNum():
             return random.randint(1, 10)
+
         a = Object()
         v1 = getNum(a, "_num")
         v2 = getNum(a, "_num")
         v3 = getNum(a, "_num")
         assert v1
         assert v1 == v2 == v3
+
+    def test6(self):
+        db = cacheutils.ReqIdCache(10)
+        assert db.exists(1) is False
+        assert db.exists("2") is False
+        # 插入1后
+        db.add("1")
+        # 判断1存在
+        assert db.exists("1")
+        # 插入1000个值，将已插入的1溢出
+        for i in range(100):
+            db.add(i)
+        # 重新判断发现1已经不存在
+        assert db.exists("1") is False
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.3.9/zenutils/tests/test_cipherutils.py` & `zenutils-0.4.8/zenutils/tests/test_cipherutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/zenutils/tests/test_dictutils.py` & `zenutils-0.4.8/zenutils/tests/test_dictutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 import json
 
 import unittest
 from zenutils import dictutils
 
+
 class TestDictUtils(unittest.TestCase):
     def test01(self):
         data1 = {
             "a": {
                 "b": {
                     "c": "c",
                 }
@@ -23,22 +32,20 @@
                     "d": "d",
                 }
             }
         }
         dictutils.deep_merge(data1, data2)
         assert data1["a"]["b"]["c"] == "c"
         assert data1["a"]["b"]["d"] == "d"
-    
+
     def test02(self):
         data1 = {
             "a": "a",
         }
-        data2 = {
-            "a": [1, 2, 3]
-        }
+        data2 = {"a": [1, 2, 3]}
         dictutils.deep_merge(data1, data2)
         assert data1["a"] == [1, 2, 3]
 
     def test03(self):
         data = {
             "a": {
                 "b": {
@@ -51,31 +58,19 @@
         assert dictutils.select(data, "a.b.c") == "c"
 
     def test04(self):
         data = [1, 2, 3]
         assert dictutils.select(data, "0") == 1
 
     def test05(self):
-        data = {
-            "a": [{
-                "b": {
-                    "c": "c"
-                }
-            }]
-        }
+        data = {"a": [{"b": {"c": "c"}}]}
         assert dictutils.select(data, "a.0.b.c") == "c"
 
     def test06(self):
-        data = {
-            "a": [{
-                "b": {
-                    "c": "c"
-                }
-            }]
-        }
+        data = {"a": [{"b": {"c": "c"}}]}
         assert dictutils.select(data, "a.1") is None
 
     def test07(self):
         data = {}
         dictutils.update(data, "a.b.c.d", "d")
         assert dictutils.select(data, "a.b.c.d") == "d"
 
@@ -88,35 +83,39 @@
         data = {}
         dictutils.update(data, "a.1.c.d", "d")
         assert data["a"][0] is None
         assert dictutils.select(data, "a.1.c.d") == "d"
 
     def test10(self):
         data = {
-            "a": [{
-                "c": {
-                    "d": "d",
+            "a": [
+                {
+                    "c": {
+                        "d": "d",
+                    }
                 }
-            }]
+            ]
         }
         dictutils.update(data, "a.0.c.d", "e")
         assert dictutils.select(data, "a.0.c.d") == "e"
 
     def test11(self):
         data = []
         dictutils.update(data, "5", "e")
         assert dictutils.select(data, "5") == "e"
 
     def test12(self):
         data = {
-            "a": [{
-                "b": {
-                    "c": "c",
+            "a": [
+                {
+                    "b": {
+                        "c": "c",
+                    }
                 }
-            }]
+            ]
         }
         dictutils.update(data, "a.0.b.d", "d")
         assert dictutils.select(data, "a.0.b.c") == "c"
         assert dictutils.select(data, "a.0.b.d") == "d"
 
     def test13(self):
         data1 = {
@@ -138,30 +137,30 @@
     def test14(self):
         data1 = {"a": True, "b": "b", "c": 1234}
         data2 = dictutils.to_object(data1)
         assert data2.a == True
         assert data2.b == "b"
         assert data2.c == 1234
 
-        data3 = {"a": {"a": [1,2,3], "b-c": {"a-a": "a-a"}}}
+        data3 = {"a": {"a": [1, 2, 3], "b-c": {"a-a": "a-a"}}}
         data4 = dictutils.to_object(data3)
-        assert data4.a.a == [1,2,3]
+        assert data4.a.a == [1, 2, 3]
         assert data4.a["b-c"]["a-a"] == "a-a"
 
         text4 = json.dumps(data4, sort_keys=True)
         text3 = json.dumps(data3, sort_keys=True)
         assert text3 == text4
 
     def test15(self):
         data1 = dictutils.to_object({"a": "a", "b": "b"})
         data2 = {"a": "a", "b": "c"}
         assert dictutils.change(data1, data2, "a") == False
         assert dictutils.change(data1, data2, "b") == True
         assert data1.b == "c"
-    
+
     def test16(self):
         data1 = dictutils.to_object({"a": "a", "b": "b"})
         data1["a"] = "b"
         assert data1.a == "b"
         data1.b = "c"
         assert data1["b"] == "c"
         data1.c = "d"
@@ -199,16 +198,16 @@
         data2 = dictutils.to_object(data1)
         dictutils.update(data2, "a.b.c", "a.b.c")
         assert data2.a.b.c == "a.b.c"
 
     def test21(self):
         data = dictutils.Object()
         data.a = {}
-        data['a']['b'] = 'a.b'
-        assert data.a.b == 'a.b'
+        data["a"]["b"] = "a.b"
+        assert data.a.b == "a.b"
 
     def test22(self):
         data = dictutils.Object({"a": {"b": "a.b"}})
         assert data.a.b == "a.b"
 
     def test23(self):
         data1 = {}
@@ -225,14 +224,15 @@
         data2 = dictutils.prefix_key(data1, "department")
         assert data2["departmentId"] == data1["id"]
         assert data2["departmentName"] == data1["name"]
 
     def test25(self):
         class A(object):
             pass
+
         data1 = A()
         dictutils.update(data1, "a.b.c.d", "a.b.c.d")
         assert dictutils.select(data1, "a.b.c.d") == "a.b.c.d"
 
     def test26(self):
         a = {
             "a": "a",
@@ -254,68 +254,66 @@
         assert a.a == "a"
         assert a.b.c == "c"
         assert a.b.d[0].e == "e"
 
     def test28(self):
         a = dictutils.Object()
         b = dictutils.Object()
-        b.a = 'a'
-        b.b = {
-            "c": "c"
-        }
+        b.a = "a"
+        b.b = {"c": "c"}
         a.update(b)
         assert a.a == "a"
         assert a.b.c == "c"
 
     def test29(self):
         a = dictutils.Object()
         b = dictutils.Object()
-        a.a = 'a'
-        b.a = 'b'
+        a.a = "a"
+        b.a = "b"
         a.update(b)
-        b.a = 'c'
-        assert a.a == 'b'
-        assert b.a == 'c'
+        b.a = "c"
+        assert a.a == "b"
+        assert b.a == "c"
 
     def test30(self):
         a = dictutils.Object()
-        a.setdefault('a', 'a')
-        assert a.a == 'a'
+        a.setdefault("a", "a")
+        assert a.a == "a"
 
     def test31(self):
-        a = dictutils.Object(a='a')
-        assert a.pop('a') == 'a'
-        assert a.pop('a', 'b') == 'b'
+        a = dictutils.Object(a="a")
+        assert a.pop("a") == "a"
+        assert a.pop("a", "b") == "b"
 
     def test32(self):
-        a = dictutils.Object(a='a')
+        a = dictutils.Object(a="a")
         a.clear()
-        assert not 'a' in a
+        assert not "a" in a
 
     def test33(self):
-        a = dictutils.Object(a='a')
+        a = dictutils.Object(a="a")
         b = a.copy()
-        assert b.a == 'a'
+        assert b.a == "a"
 
     def test34(self):
-        a = dictutils.Object(a='b')
+        a = dictutils.Object(a="b")
         k, v = a.popitem()
-        assert k == 'a'
-        assert v == 'b'
-        assert not 'a' in a
-        assert hasattr(a, 'a') is False
+        assert k == "a"
+        assert v == "b"
+        assert not "a" in a
+        assert hasattr(a, "a") is False
 
     def test35(self):
         a = dictutils.Object()
-        a.a = [1,2,3, {'a': 'a'}]
-        assert a.a[3].a == 'a'
+        a.a = [1, 2, 3, {"a": "a"}]
+        assert a.a[3].a == "a"
 
     def test36(self):
         a = dictutils.Object()
-        a.a = [1,2,3]
+        a.a = [1, 2, 3]
         a.a.append({"a": "a"})
         assert type(a.a[3]) == dict
         a.fix()
         assert a.a[3].a == "a"
 
     def test37(self):
         headers = dictutils.HttpHeadersDict()
@@ -341,7 +339,63 @@
         assert headers.getlist("a") == ["c"]
 
     def test40(self):
         headers = dictutils.HttpHeadersDict()
         assert headers.create_header("a", "a")
         assert headers.create_header("a", "b") is False
         assert headers.getlist("a") == ["a"]
+
+    def test41(self):
+        config = dictutils.Object()
+        assert config.select("server.listen", "0.0.0.0") == "0.0.0.0"
+        assert config.select("server.port", 8080) == 8080
+
+    def test42(self):
+        config = dictutils.Object(
+            {
+                "daemon": True,
+            }
+        )
+        assert config.select("server.listen", "0.0.0.0") == "0.0.0.0"
+        assert config.select("server.port", 8080) == 8080
+        assert config.select("daemon", False) == True
+
+    def test43(self):
+        cfg1 = {"a": {"b": "b"}}
+        cfg2 = {"a": {"c": "c", "d": [{"e": "e"}]}}
+        dictutils.deep_merge(cfg1, cfg2)
+        assert cfg1["a"]["b"] == "b"
+        assert cfg1["a"]["c"] == "c"
+
+    def test44(self):
+        data1 = {"a": [1, 2, {"b": "b"}]}
+        data2 = dictutils.Object(data1)
+        assert data2.select("a.2.b") == "b"
+
+    def test45(self):
+        data = dictutils.Object({"a": [1, 2, 3]})
+        assert data["a"][0] == 1
+
+    def test46(self):
+        data = dictutils.Object(
+            {
+                "a": (1, 2, 3),
+                "b": set([1, 2, 3]),
+            }
+        )
+        assert data.select("a.0") == 1
+        assert data.select("a.1") == 2
+        assert data.select("a.2") == 3
+        assert data.select("b") == set([3, 2, 1])
+
+    def test47(self):
+        data = dictutils.Object({"a": 1})
+        with self.assertRaises(KeyError):
+            dictutils.select(data, "b", slient=False)
+
+    def test48(self):
+        class A(object):
+            pass
+
+        data = A()
+        with self.assertRaises(KeyError):
+            dictutils.select(data, "hello", slient=False)
```

### Comparing `zenutils-0.3.9/zenutils/tests/test_fsutils.py` & `zenutils-0.4.8/zenutils/tests/test_fsutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/zenutils/tests/test_funcutils.py` & `zenutils-0.4.8/zenutils/tests/test_funcutils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 import os
 import sys
 import uuid
 import random
 import unittest
 from zenutils import funcutils
 
 
 class TestFuncUtils(unittest.TestCase):
     def test01(self):
         def s(a, b):
             return a + b
+
         data = {
             "a": 1,
             "b": 2,
             "c": 3,
         }
         params = funcutils.get_inject_params(s, data)
         assert params["a"] == 1
@@ -26,91 +35,100 @@
 
         result = funcutils.call_with_inject(s, data)
         assert result == 3
 
     def test02(self):
         def s(a, b=2):
             return a + b
+
         data = {
             "a": 1,
             "c": 3,
         }
         params = funcutils.get_inject_params(s, data)
         assert params["a"] == 1
         assert params["b"] == 2
 
         result = funcutils.call_with_inject(s, data)
         assert result == 3
 
     def test03(self):
         def s(a, b=2):
             return a + b
+
         data = {
             "a": 1,
             "c": 2,
         }
         params = funcutils.get_inject_params(s, data)
         assert params["a"] == 1
         assert params["b"] == 2
 
         result = funcutils.call_with_inject(s, data)
         assert result == 3
 
     def test04(self):
         def hi(msg="hi"):
             pass
+
         assert funcutils.get_default_values(hi)["msg"] == "hi"
-    
+
         def add(a=0, b=0):
             pass
+
         data = funcutils.get_default_values(add)
         assert data["a"] == 0
         assert data["b"] == 0
 
         def sub(a, b):
             pass
+
         data = funcutils.get_default_values(sub)
         assert data == {}
 
         def multi(a, b=1):
             pass
+
         data = funcutils.get_default_values(multi)
         assert data["b"] == 1
         assert not "a" in data
 
     def test05(self):
         def incr(value):
             return value + 1
+
         def decr(value):
             return value - 2
-        
+
         assert funcutils.chain(incr, decr)(3) == 2
         assert funcutils.chain(incr, decr)(0) == -1
-    
 
         def incr(value, *args, **kwargs):
             incr_delta = kwargs.get("incr_delta", 0)
             return value + incr_delta
+
         def decr(value, *args, **kwargs):
             decr_delta = kwargs.get("decr_delta", 0)
             return value - decr_delta
+
         extra_kwargs = {
             "incr_delta": 1,
             "decr_delta": 2,
         }
         assert funcutils.chain(incr, decr)(3, extra_kwargs=extra_kwargs) == 2
         assert funcutils.chain(incr, decr)(0, extra_kwargs=extra_kwargs) == -1
 
     def test06(self):
-
         class Summer(object):
             def __init__(self):
                 self.total = 0
+
             def add(self):
                 self.total += 1
+
             def add2(self):
                 self.total += 2
 
         summer = Summer()
         add3 = funcutils.BunchCallable(summer.add, summer.add2)
         add3()
         assert summer.total == 3
@@ -121,26 +139,24 @@
 
         add6 = funcutils.BunchCallable(add4, summer.add2)
         add6()
         assert summer.total == 13
 
     def test07(self):
         class Bar(object):
-
             _bar = 1
 
             @funcutils.classproperty
             def bar(cls):
                 return cls._bar
 
             @bar.setter
             def bar(cls, value):
                 cls._bar = value
 
-
         # test instance instantiation
         foo = Bar()
         assert foo.bar == 1
 
         baz = Bar()
         assert baz.bar == 1
 
@@ -160,24 +176,26 @@
         assert funcutils.is_a_class(str) is True
         assert funcutils.is_a_class(type(str)) is True
         assert funcutils.is_a_class("hello") is False
         assert funcutils.is_a_class(b"hello") is False
 
         class A(object):
             pass
+
         assert funcutils.is_a_class(A) is True
         assert funcutils.is_a_class(A()) is False
 
-        B = create_new_class('B', (), {})
+        B = create_new_class("B", (), {})
         assert funcutils.is_a_class(B) is True
 
     def test08_01(self):
         if sys.version_info.major == 3 and sys.version_info.minor >= 3:
             sys.path.append(os.path.dirname(__file__))
             from t08_01 import C
+
             assert funcutils.is_a_class(C) is True
             assert funcutils.is_a_class(C()) is False
 
     def test09(self):
         es = funcutils.get_all_builtin_exceptions()
         assert Exception in es
         assert TypeError in es
@@ -196,48 +214,129 @@
         assert "BaseException" in builtins
         assert "Exception" in builtins
         assert "RuntimeError" in builtins
 
     def test11(self):
         assert funcutils.get_class_name(Exception) == "Exception"
         assert funcutils.get_class_name(Exception()) == "Exception"
+
         class A(object):
             pass
+
         assert funcutils.get_class_name(A) == "A"
         assert funcutils.get_class_name(A()) == "A"
 
     def test12(self):
-        """多次随机，确保总是能得到正确值。
-        """
+        """多次随机，确保总是能得到正确值。"""
+
         @funcutils.retry(limit=100)
         def say_hello(name):
             if random.randint(0, 10) < 5:
                 raise Exception()
             return "hello, " + name
 
         assert say_hello("test") == "hello, test"
 
     def test13(self):
-        """重试超过limit后，将抛出最后一次的异常。
-        """
+        """重试超过limit后，将抛出最后一次的异常。"""
+
         @funcutils.retry()
         def say_hello(name):
             raise Exception()
-        
+
         with self.assertRaises(Exception):
             say_hello("test")
 
     def test14(self):
-        """如果要求遇到SayHelloException直接抛出异常，则遇到SayHelloException不会进行重试
-        """
+        """如果要求遇到SayHelloException直接抛出异常，则遇到SayHelloException不会进行重试"""
+
         class SayHelloException(Exception):
             pass
 
         @funcutils.retry(raise_exceptions=[SayHelloException], is_retry=True)
         def ping(is_retry=False):
             if is_retry:
                 return "pong"
             raise SayHelloException()
 
         with self.assertRaises(SayHelloException):
             assert ping()
 
+    def test15(self):
+        from zenutils import dictutils
+
+        class A(object):
+            def __init__(self):
+                self.data = dictutils.Object(
+                    {
+                        "a": "a",
+                        "b": {
+                            "c": "c",
+                        },
+                    }
+                )
+
+            def __getattr__(self, name):
+                return funcutils.ChainableProxy(name, self._get_data)
+
+            def _get_data(self, path):
+                return self.data.select(path)
+
+        a = A()
+        assert a.a() == "a"
+        assert a.b.c() == "c"
+
+    def test16(self):
+        class A(object):
+            def __getattr__(self, name):
+                return funcutils.ChainableProxy(name, self._execute)
+
+            def _execute(self, path):
+                return getattr(self, "do_" + path)()
+
+            def do_ping(self):
+                return "pong"
+
+        a = A()
+        assert a.ping() == "pong"
+
+    def test17(self):
+        def a():
+            """
+            hello world
+            """
+
+        assert funcutils.get_method_help(a).strip() == "hello world"
+
+    def test18(self):
+        def a():
+            pass
+
+        a.__help_text__ = "hello world"
+        assert funcutils.get_method_help(a).strip() == "hello world"
+
+    def test19(self):
+        def a():
+            pass
+
+        a.__help__ = "hello world"
+        assert funcutils.get_method_help(a).strip() == "hello world"
+
+    def test20(self):
+        def a():
+            """
+            @signature {{{
+                [
+                    ["str"]
+                ]
+            }}}
+            """
+            return "a"
+
+        assert funcutils.get_method_signature(a) == [["str"]]
+
+    def test21(self):
+        def a():
+            return "a"
+
+        a.__signature__ = [["str"]]
+        assert funcutils.get_method_signature(a) == [["str"]]
```

### Comparing `zenutils-0.3.9/zenutils/tests/test_hashutils.py` & `zenutils-0.4.8/zenutils/tests/test_hashutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from sys import prefix
 from zenutils.sixutils import *
 
 import os
 import uuid
 import random
 import unittest
 
 from zenutils import hashutils
 from zenutils import strutils
 
-class TestHashUtils(unittest.TestCase):
 
+class TestHashUtils(unittest.TestCase):
     def test01(self):
         text = hashutils.get_md5()
         assert text == "d41d8cd98f00b204e9800998ecf8427e"
 
     def test02(self):
         text = hashutils.get_md5(b"a")
         assert text == "0cc175b9c0f1b6a831c399e269772661"
@@ -29,27 +37,37 @@
     def test04(self):
         text = hashutils.get_md5("a", "b", 1)
         assert text == "68b6a776378decbb4a79cda89087c4ce"
 
     def test05(self):
         text = hashutils.get_sha1("a", 1, True)
         assert text == "3251aeb0f68984b60d7cb2ed7f2505bee819a7c7"
-    
+
     def test06(self):
         text = hashutils.get_sha1_base64("a", 1, True, 0.01)
         assert text == "yrZxIUBkyZ03qTIMbYORcBdnFRc="
 
     def test07(self):
-        text = hashutils.get_pbkdf2_hmac("testpassword", salt="bPBMORgAZP53", iterations=150000, hash_name="sha256")
-        assert text == "pbkdf2_sha256$150000$bPBMORgAZP53$yPCstMcQYC9Rgn0h2mT0egPjUdW5T7WUiViib9Sn0dM="
+        text = hashutils.get_pbkdf2_hmac(
+            "testpassword", salt="bPBMORgAZP53", iterations=150000, hash_name="sha256"
+        )
+        assert (
+            text
+            == "pbkdf2_sha256$150000$bPBMORgAZP53$yPCstMcQYC9Rgn0h2mT0egPjUdW5T7WUiViib9Sn0dM="
+        )
 
     def test08(self):
-        text = hashutils.get_pbkdf2_sha256("testpassword", salt="bPBMORgAZP53", iterations=150000)
-        assert text == "pbkdf2_sha256$150000$bPBMORgAZP53$yPCstMcQYC9Rgn0h2mT0egPjUdW5T7WUiViib9Sn0dM="
-  
+        text = hashutils.get_pbkdf2_sha256(
+            "testpassword", salt="bPBMORgAZP53", iterations=150000
+        )
+        assert (
+            text
+            == "pbkdf2_sha256$150000$bPBMORgAZP53$yPCstMcQYC9Rgn0h2mT0egPjUdW5T7WUiViib9Sn0dM="
+        )
+
     def test09(self):
         text = hashutils.get_pbkdf2_sha256("just a test")
         assert hashutils.validate_pbkdf2_sha256("just a test", text)
 
     def test10(self):
         text = hashutils.get_pbkdf2_md5("just a test")
         assert hashutils.validate_pbkdf2_md5("just a test", text)
@@ -60,21 +78,25 @@
         text = hashutils.get_pbkdf2_md5(b"just a test")
         assert hashutils.validate_pbkdf2_md5("just a test", text)
 
         text = hashutils.get_pbkdf2_md5("just a test")
         assert hashutils.validate_pbkdf2_md5(b"just a test", text)
 
     def test11(self):
-        assert "5vNnRsy6QsKIrPkG5ja7J46ut+g=" == hashutils.get_sha1_base64(b"just a test")
-        assert "5vNnRsy6QsKIrPkG5ja7J46ut+g=" == hashutils.get_sha1_base64("just a test")
+        assert "5vNnRsy6QsKIrPkG5ja7J46ut+g=" == hashutils.get_sha1_base64(
+            b"just a test"
+        )
+        assert "5vNnRsy6QsKIrPkG5ja7J46ut+g=" == hashutils.get_sha1_base64(
+            "just a test"
+        )
 
     def test12(self):
         filename = "{0}.txt".format(str(uuid.uuid4()))
         try:
-            length = random.randint(0, 1024*1024*16)
+            length = random.randint(0, 1024 * 1024 * 16)
             stream = os.urandom(length)
             with open(filename, "wb") as fobj:
                 fobj.write(stream)
             code1 = hashutils.get_file_md5(filename)
             code2 = hashutils.get_md5(stream)
             assert code1 == code2
 
@@ -82,17 +104,23 @@
             code4 = hashutils.get_sha1(stream)
             assert code3 == code4
         finally:
             if os.path.exists(filename):
                 os.unlink(filename)
 
     def test13(self):
-        assert hashutils.is_the_same_hash_method(hashutils.method_load("md5"), hashutils.method_load(b"md5"))
-        assert hashutils.is_the_same_hash_method(hashutils.method_load("sha1"), hashutils.method_load(b"sha1"))
-        assert hashutils.is_the_same_hash_method(hashutils.method_load("sha256"), hashutils.method_load(b"sha256"))
+        assert hashutils.is_the_same_hash_method(
+            hashutils.method_load("md5"), hashutils.method_load(b"md5")
+        )
+        assert hashutils.is_the_same_hash_method(
+            hashutils.method_load("sha1"), hashutils.method_load(b"sha1")
+        )
+        assert hashutils.is_the_same_hash_method(
+            hashutils.method_load("sha256"), hashutils.method_load(b"sha256")
+        )
 
     def test14(self):
         methods = [
             "MD5",
             "SHA",
             "SHA1",
             "SHA224",
@@ -127,15 +155,15 @@
             if not method.startswith("SH"):
                 continue
             data1 = strutils.random_string(12)
             data2 = hashutils.get_password_hash(data1, method=method)
             result = hashutils.validate_password_hash(data2, data1)
             print(method, data1, data2, result)
             assert result
-    
+
     def test17(self):
         """
         检查哈希结果前缀是否存在冲突。
         """
         prefixes = []
         for _, method in hashutils.PASSWORD_HASH_METHODS.items():
             if not hasattr(method, "prefix"):
@@ -149,20 +177,19 @@
 
             prefixes.append(prefix)
 
     def test18(self):
         data1 = strutils.random_string(8)
         data2 = hashutils.get_password_hash(data1, "sm3")
         assert data2
-    
+
     def test19(self):
         for method in hashutils.get_password_hash_methods():
             print(method)
             data1 = strutils.random_string(8)
             data2 = hashutils.get_password_hash(data1, method)
             print(method, data1, data2)
             result = hashutils.validate_password_hash(data2, data1)
             print(method, data1, data2, result)
             assert data1
             assert data2
             assert result
-
```

### Comparing `zenutils-0.3.9/zenutils/tests/test_httputils.py` & `zenutils-0.4.8/zenutils/tests/test_httputils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/zenutils/tests/test_import_all.py` & `zenutils-0.4.8/zenutils/tests/test_import_all.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 
 import unittest
 
 from zenutils.base64utils import *
 from zenutils.baseutils import *
 from zenutils.cacheutils import *
 from zenutils.cipherutils import *
+from zenutils.errorutils import *
 from zenutils.dictutils import *
 from zenutils.fsutils import *
 from zenutils.funcutils import *
 from zenutils.hashutils import *
 from zenutils.httputils import *
+from zenutils.importutils import *
 from zenutils.jsonutils import *
 from zenutils.listutils import *
 from zenutils.logutils import *
 from zenutils.nameutils import *
 from zenutils.numericutils import *
+from zenutils.packutils import *
+from zenutils.perfutils import *
 from zenutils.randomutils import *
+from zenutils.serviceutils import *
 from zenutils.sixutils import *
+from zenutils.socketserverutils import *
 from zenutils.strutils import *
 from zenutils.sysutils import *
 from zenutils.threadutils import *
 from zenutils.treeutils import *
 from zenutils.typingutils import *
 
+
 class TestImportAll(unittest.TestCase):
     
     def test01(self):
         assert True
```

### Comparing `zenutils-0.3.9/zenutils/tests/test_jsonutils.py` & `zenutils-0.4.8/zenutils/tests/test_jsonutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/zenutils/tests/test_listutils.py` & `zenutils-0.4.8/zenutils/tests/test_listutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/zenutils/tests/test_logutils.py` & `zenutils-0.4.8/zenutils/tests/test_logutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/zenutils/tests/test_nameutils.py` & `zenutils-0.4.8/zenutils/tests/test_nameutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/zenutils/tests/test_numericutils.py` & `zenutils-0.4.8/zenutils/tests/test_numericutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
 from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
-import numbers
 from zenutils.sixutils import *
 
 import os
 import random
 import unittest
 from zenutils import numericutils
```

### Comparing `zenutils-0.3.9/zenutils/tests/test_randomutils.py` & `zenutils-0.4.8/zenutils/tests/test_randomutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/zenutils/tests/test_sixutils.py` & `zenutils-0.4.8/zenutils/tests/test_sixutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/zenutils/tests/test_strutils.py` & `zenutils-0.4.8/zenutils/tests/test_strutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/zenutils/tests/test_sysutils.py` & `zenutils-0.4.8/zenutils/tests/test_sysutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/zenutils/tests/test_threadutils.py` & `zenutils-0.4.8/zenutils/tests/test_threadutils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,58 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 
-
 import time
 import unittest
 import threading
+import random
+
 try:
     from queue import Queue
     from queue import Empty
 except ImportError:
     from Queue import Queue
     from Queue import Empty
 
 
 from zenutils import threadutils
 
-class TestThreadUtils(unittest.TestCase):
 
-    def test01(self):
+class TestThreadUtils(unittest.TestCase):
+    def test1(self):
         numbers = []
         meta = {
             "max_number": 10**9,
             "number": 1,
         }
+
         def get_numbers(ma, ns):
             if ma["number"] <= meta["max_number"]:
                 ns.append(meta["number"])
                 ma["number"] += 1
-        service = threadutils.Service(service_loop=get_numbers, service_loop_kwargs={
-            "ma": meta,
-            "ns": numbers,
-        }, service_loop_interval=0)
+
+        service = threadutils.Service(
+            service_loop=get_numbers,
+            service_loop_kwargs={
+                "ma": meta,
+                "ns": numbers,
+            },
+            service_loop_interval=0,
+        )
         service.start()
         len0 = len(numbers)
         time.sleep(5)
         len1 = len(numbers)
         assert len1 > len0
         service.stop()
         len11 = len(numbers)
@@ -53,76 +68,87 @@
         assert service.terminated_time
         assert service.service_thread.is_alive() == False
         len3 = len(numbers)
         time.sleep(5)
         len4 = len(numbers)
         assert len4 == len3
         s1 = sum(numbers)
-        s2 = (len(numbers)+1)*len(numbers)/2
+        s2 = (len(numbers) + 1) * len(numbers) / 2
         assert s1 == s2
 
-    def test02(self):
+    def test2(self):
         number_counter = threadutils.Counter()
         number_queue = Queue()
 
         class NumberPut(threadutils.SimpleProducer):
             def __init__(self, number_counter, **kwargs):
                 self.number_counter = number_counter
                 super(NumberPut, self).__init__(**kwargs)
-    
+
             def produce(self):
                 return [self.number_counter.incr()]
-    
+
         class NumberGet(threadutils.SimpleConsumer):
             def __init__(self, number_queue, **kwargs):
                 self.number_queue = number_queue
                 super(NumberGet, self).__init__(**kwargs)
-            
+
             def consume(self, task):
                 self.number_queue.put(task)
 
         server = threadutils.SimpleProducerConsumerServer(
             producer_class=NumberPut,
             consumer_class=NumberGet,
-            producer_class_init_kwargs={"number_counter": number_counter, "service_loop_interval": 0},
-            consumer_class_init_kwargs={"number_queue": number_queue, "service_loop_interval": 0},
+            producer_class_init_kwargs={
+                "number_counter": number_counter,
+                "service_loop_interval": 0,
+            },
+            consumer_class_init_kwargs={
+                "number_queue": number_queue,
+                "service_loop_interval": 0,
+            },
             queue_size=0,
-            )
+        )
         server.start()
         time.sleep(5)
         server.stop()
         assert number_counter.value == number_queue.qsize()
 
-    def test03(self):
+    def test3(self):
         number_counter = threadutils.Counter()
         number_queue = Queue()
+
         def NumberPut(number_counter):
             return [number_counter.incr()]
+
         def NumberGet(task, number_queue):
             number_queue.put(task)
+
         server = threadutils.SimpleProducerConsumerServer(
             produce=NumberPut,
             produce_kwargs={"number_counter": number_counter},
             consume=NumberGet,
             consume_kwargs={"number_queue": number_queue},
             service_loop_interval=0,
             queue_size=0,
-            )
+        )
         server.start()
         time.sleep(5)
         server.stop()
         assert number_counter.value == number_queue.qsize()
- 
-    def test04(self):
+
+    def test4(self):
         number_counter = threadutils.Counter()
         number_queue = Queue()
+
         def number_generate(size):
             for i in range(size):
                 value = number_counter.incr()
                 number_queue.put(value)
+
         tsnum = 10
         tsize = 10000
         ts = []
         for _ in range(tsnum):
             t = threading.Thread(target=number_generate, args=[tsize])
             t.start()
             ts.append(t)
@@ -132,17 +158,85 @@
         while True:
             try:
                 ns.add(number_queue.get(block=False))
             except Empty:
                 break
         assert len(ns) == tsnum * tsize
 
-    def test05(self):
+    def test5(self):
         c = threadutils.Counter()
         c.incr()
         assert c.value == 1
         c.incr()
         assert c.value == 2
         c.decr()
         assert c.value == 1
         c.decr()
         assert c.value == 0
+
+    def test6(self):
+        q = threadutils.ConcurrentLimitJobQueue(2)
+        assert q.acquire()
+        assert q.acquire()
+        assert q.acquire(timeout=1) is False
+        q.put(1)
+        q.put(2)
+        assert q.get()
+        assert q.get()
+        assert q.get(timeout=1) is None
+        q.release()
+        assert q.acquire()
+        assert q.acquire(timeout=1) is False
+        q.release()
+        q.release()
+        assert q.acquire()
+        assert q.acquire()
+        assert q.acquire(timeout=1) is False
+
+    def test7(self):
+        jq = threadutils.JobQueue()
+
+        t1 = threading.Thread(target=jq.serve_forever)
+        t1.start()
+
+        t2 = threading.Thread(target=jq.serve_forever)
+        t2.start()
+
+        def echo(msg):
+            return msg
+
+        for i in range(1024):
+            msg = "hello world {}".format(i)
+            assert jq.execute(echo, args=[msg]) == msg
+
+        assert jq.stop()
+        t1.join()
+        t2.join()
+
+    def test8(self):
+        ct = threadutils.WorkerCounter()
+        ct.incr()
+        ct.incr()
+        assert ct.wait(1) is False
+        ct.decr()
+        ct.decr()
+        assert ct.wait(1)
+
+    def test9(self):
+        ct = threadutils.WorkerCounter()
+        values = threadutils.Counter()
+
+        def worker(ct, values):
+            ct.incr()
+            time.sleep(random.randint(10, 30) / 10.0)
+            values.incr()
+            ct.decr()
+
+        t1 = threading.Thread(target=worker, args=[ct, values])
+        t1.start()
+        t2 = threading.Thread(target=worker, args=[ct, values])
+        t2.start()
+        t3 = threading.Thread(target=worker, args=[ct, values])
+        t3.start()
+
+        ct.wait()
+        assert values.value == 3
```

### Comparing `zenutils-0.3.9/zenutils/tests/test_treeutils.py` & `zenutils-0.4.8/zenutils/tests/test_treeutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/zenutils/tests/test_typingutils.py` & `zenutils-0.4.8/zenutils/tests/test_typingutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.9/zenutils/threadutils.py` & `zenutils-0.4.8/zenutils/funcutils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,512 +1,639 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""魔法工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
-__all__ = [
-    "Counter",
-    "StartOnTerminatedService",
-    "ServiceStop",
-    "ServiceTerminate",
-    "LoopIdle",
-    "Service",
-    "SimpleProducer",
-    "SimpleConsumer",
-    "SimpleServer",
-    "SimpleProducerConsumerServer",
-]
-
+import re
 import time
+import json
+import functools
 import logging
-import threading
+
 try:
-    from queue import Queue
-    from queue import Empty
-    from queue import Full
+    from inspect import signature
+    from inspect import isclass
+    import inspect
 except ImportError:
-    from Queue import Queue
-    from Queue import Empty
-    from Queue import Full
+    from inspect2 import signature  # required by python 2.7 and python 3.2
+    from inspect2 import isclass
+    import inspect2 as inspect
+
+__all__ = [
+    "inspect",
+    "signature",
+    "isclass",
+    "get_default_values",
+    "get_inject_params",
+    "call_with_inject",
+    "mcall_with_inject",
+    "classproperty",
+    "chain",
+    "BunchCallable",
+    "try_again_on_error",
+    "get_builtins_dict",
+    "get_all_builtin_exceptions",
+    "get_class_name",
+    "ChainableProxy",
+    "is_a_class",
+    "get_method_help",
+    "get_method_signature",
+]
 
 logger = logging.getLogger(__name__)
 
-class Counter(object):
-    """Thread safe counter.
+
+def get_default_values(func):
+    """Get function parameters default value.
+
+    In [1]: from zenutils import funcutils
+
+    In [2]: def hi(name, msg="hi, {name}"):
+    ...:     print(msg.format(name=name))
+    ...:
+
+    In [3]: funcutils.get_default_values(hi)
+    Out[3]: {'msg': 'hi, {name}'}
+    """
+    data = {}
+    parameters = signature(func).parameters
+    for name, parameter in parameters.items():
+        if parameter.default != parameter.empty:
+            data[name] = parameter.default
+    return data
+
+
+def get_inject_params(func, data, raise_on_missing_field=True):
+    """Get all params that required by calling the func from data.
+
+    In [1]: from zenutils import funcutils
+
+    In [2]: def hi(name, msg="hi, {name}"):
+    ...:     print(msg.format(name=name))
+    ...:
+
+    In [3]: params = funcutils.get_inject_params(hi, data)
+
+    In [4]: params
+    Out[4]: {'name': 'Cissie', 'msg': 'hi, {name}'}
+
+    In [5]: hi(**params)
+    hi, Cissie
+
     """
-    def __init__(self, init_value=0):
-        self.lock = threading.Lock()
-        self.value = init_value
-    
-    def incr(self, delta=1):
-        with self.lock:
-            self.value += delta
-            return self.value
-
-    def decr(self, delta=1):
-        with self.lock:
-            self.value -= delta
-            return self.value
-
-class StartOnTerminatedService(RuntimeError):
-    pass
-
-class ServiceStop(RuntimeError):
-    pass
-
-class ServiceTerminate(RuntimeError):
-    pass
-
-class LoopIdle(RuntimeError):
-    pass
-
-class Service(object):
-    default_service_loop_interval = 1
-    default_sleep_interval_in_joining = 1
-    default_sleep_interval_after_stopped = 1
-
-    def __init__(self, service_loop=None, service_loop_args=None, service_loop_kwargs=None, service_loop_interval=None, sleep_interval_in_joining=None, sleep_interval_after_stopped=None, server=None, service_name=None, on_loop_error=None, on_loop_idle=None, on_loop_finished=None, **kwargs):
-        self.service_start_lock = threading.Lock()
-        self.service_thread = None
-
-        self.started = None
-        self.started_time = None
-        self.terminate_flag = False
-        self.terminate_time = None
-        self.terminated = False
-        self.terminated_time = None
-        self.stop_flag = None
-        self.stop_time = None
-        self.stopped = None
-        self.stopped_time = None
-    
-        self.is_running = False
-
-        self.service_loop_callback = service_loop
-        self.service_loop_args = service_loop_args or []
-        self.service_loop_kwargs = service_loop_kwargs or {}
-        if service_loop_interval is None:
-            self.service_loop_interval = self.default_service_loop_interval
+    from zenutils import typingutils
+
+    params = {}
+    parameters = signature(func).parameters
+    for name, parameter in parameters.items():
+        if parameter.kind == 2:  # 无法处理*args这样的占位参数，忽略他们
+            continue
+        if parameter.default is parameter.empty:
+            # no default value, this parameter is required
+            if not name in data:
+                if raise_on_missing_field:
+                    raise KeyError("Missing parameter: {name}".format(name=name))
+                else:
+                    continue
+            value = data[name]
         else:
-            self.service_loop_interval = service_loop_interval
-        self.sleep_interval_in_joining = sleep_interval_in_joining or self.default_sleep_interval_in_joining
-        self.sleep_interval_after_stopped = sleep_interval_after_stopped or self.default_sleep_interval_after_stopped
-        self.server = server
-        self.service_name = service_name or self.service_loop_callback.__name__
-        self.on_loop_error_callback = on_loop_error
-        self.on_loop_idle_callback = on_loop_idle
-        self.on_loop_finished_callback = on_loop_finished
+            value = data.get(name, parameter.default)
+        if not parameter.annotation is parameter.empty:
+            value = typingutils.smart_cast(parameter.annotation, value, field_name=name)
+        params[name] = value
+    return params
+
+
+def call_with_inject(func, data):
+    """Call a func with parameters auto inject."""
+    raise_on_missing_field = True
+    args = data.get("_inject_args", []) or []  # 获取位置参数
+    if len(args):
+        raise_on_missing_field = False  # 如果已经有位置参数，无法正确判断是否有字段缺失的情况，则在获取关键字参数时就不再抛出异常
+    kwargs = get_inject_params(
+        func, data, raise_on_missing_field=raise_on_missing_field
+    )
+    try:
+        return func(*args, **kwargs)
+    except Exception as error:
+        logger.debug(
+            "call_with_inject failed: args={args}, kwargs={kwargs}, error_message={error}".format(
+                args=args, kwargs=kwargs, error=error
+            )
+        )
+        raise error
+
+
+def mcall_with_inject(funcs, data):
+    if not isinstance(funcs, (list, set, tuple)):
+        funcs = [funcs]
+    results = []
+    for func in funcs:
+        params = get_inject_params(func, data)
+        result = func(**params)
+        results.append(result)
+    return results
+
+
+class ClassPropertyDescriptor(object):
+    def __init__(self, fget, fset=None):
+        self.fget = fget
+        self.fset = fset
+
+    def __get__(self, obj, klass=None):
+        if klass is None:
+            klass = type(obj)
+        return self.fget.__get__(obj, klass)()
+
+    def __set__(self, obj, value):
+        if not self.fset:
+            raise AttributeError("can't set attribute")
+        type_ = type(obj)
+        return self.fset.__get__(obj, type_)(value)
+
+    def setter(self, func):
+        if not isinstance(func, (classmethod, staticmethod)):
+            func = classmethod(func)
+        self.fset = func
+        return self
+
+
+def classproperty(func):
+    """classproperty decorator.
+
+    class Bar(object):
+
+        _bar = 1
+
+        @classproperty
+        def bar(cls):
+            return cls._bar
+
+        @bar.setter
+        def bar(cls, value):
+            cls._bar = value
+
+
+    # test instance instantiation
+    foo = Bar()
+    assert foo.bar == 1
+
+    baz = Bar()
+    assert baz.bar == 1
+
+    # test static variable
+    baz.bar = 5
+    assert foo.bar == 5
+
+    # test setting variable on the class
+    Bar.bar = 50
+    assert baz.bar == 50
+    assert foo.bar == 50
+    """
+    if not isinstance(func, (classmethod, staticmethod)):
+        func = classmethod(func)
 
-    def start(self):
-        """Create the service thread and start the service loop.
-        """
-        if self.terminated:
-            raise StartOnTerminatedService()
-        self.start_time = time.time()
-        self.stop_flag = False
-        self.stop_time = None
-        self.stopped = False
-        self.stopped_time = None
-        with self.service_start_lock:
-            if not self.started:
-                self.service_thread = threading.Thread(target=self.main)
-                self.service_thread.daemon = True
-                self.service_thread.start()
-                self.started = True
-                self.started_time = time.time()
+    return ClassPropertyDescriptor(func)
 
-    def stop(self, wait=True, wait_timeout=-1):
-        """Stop the service loop, but keep the service thread, so that it can be resumed.
-        """
-        self.stop_flag = True
-        self.stop_time = time.time()
-        return self.join(wait, wait_timeout)
 
-    def terminate(self, wait=True, wait_timeout=-1):
-        """Stop the service loop and exit the service thread. It can not be resumed.
-        """
-        self.terminate_flag = True
-        self.terminate_time = time.time()
-        return self.stop(wait, wait_timeout)
+class chain(object):
+    """ """
 
-    def join(self, wait=True, wait_timeout=-1):
-        """Return True means service stopped, False means not stopped and timeout, None means no waiting...
+    def __init__(self, *args):
+        self.funcs = args
+
+    def __call__(self, init_result, extra_args=None, extra_kwargs=None):
+        extra_args = extra_args or []
+        extra_kwargs = extra_kwargs or {}
+        result = init_result
+        for func in self.funcs:
+            if func and callable(func):
+                result = func(result, *extra_args, **extra_kwargs)
+        return result
+
+
+class BunchCallable(object):
+    def __init__(self, *args, **kwargs):
+        """BunchCallable init.
+
+        @Returns:
+            (None)
+
+        @Parameters:
+            args(Any, multiple):
+            return_callback_results(bool, optional, default to False):
         """
-        if not wait:
-            if not self.is_running:
-                return True
+        return_callback_results = kwargs.get("return_callback_results", False)
+        self.return_callback_results = return_callback_results
+        self.funcs = []
+        for func in args:
+            if isinstance(func, self.__class__):
+                self.funcs += func.funcs
             else:
-                None # no waiting, so we don't know it's stopped or not
-        stime = time.time()
-        while self.is_running:
-            if wait_timeout >= 0 and time.time() - stime >= wait_timeout:
-                return False
-            time.sleep(self.sleep_interval_in_joining)
-        return True
+                self.funcs.append(func)
 
-    def main(self):
-        """
-        The main control process of the service,
-        calling the service_loop process,
-        dealing with the stop and terminate events and handling the exceptions.
-        """
-        while not self.terminate_flag:
-            if self.stop_flag:
-                self.is_running = False
-                if self.stopped_time is None:
-                    self.stopped_time = time.time()
-                self.stopped = True
-                time.sleep(self.sleep_interval_after_stopped)
-                continue
-            self.is_running = True
-            try:
+    def __call__(self, *args, **kwargs):
+        results = []
+        for func in self.funcs:
+            if func and callable(func):
+                result = func(*args, **kwargs)
+            else:
+                result = None
+            results.append(result)
+        if self.return_callback_results:
+            return results
+        else:
+            return None
+
+
+def try_again_on_error(
+    sleep=5, limit=0, callback=None, callback_args=None, callback_kwargs=None
+):
+    def outter_wrapper(func):
+        def wrapper(*args, **kwargs):
+            counter = 0
+            while True:
+                counter += 1
                 try:
-                    self.service_loop()
-                except LoopIdle:
-                    self.on_loop_idle()
-                except ServiceStop:
-                    self.stop(wait=False)
+                    return func(*args, **kwargs)
                 except InterruptedError:
-                    self.terminate(wait=False)
-                except ServiceTerminate:
-                    self.terminate(wait=False)
+                    logger.info("exit on got InterruptedError...")
+                    break
                 except Exception as error:
-                    self.on_loop_error(error)
-                finally:
-                    self.on_loop_finished()
-            except ServiceStop:
-                self.stop(wait=False)
-            except InterruptedError:
-                self.terminate(wait=False)
-            except ServiceTerminate:
-                self.terminate(wait=False)
-            except Exception as error:
-                logger.exception("service main process got unknown error: {0}".format(str(error)))
-            if (not self.terminated) and self.service_loop_interval:
-                time.sleep(self.service_loop_interval)
-        self.terminated_time = time.time()
-        self.terminated = True
-        self.is_running = False
-
-    def service_loop(self):
-        logger.debug("calling service_loop...")
-        if self.service_loop_callback and callable(self.service_loop_callback):
-            logger.debug("calling service_loop_callback...")
-            self.service_loop_callback(*self.service_loop_args, **self.service_loop_kwargs)
-            logger.debug("call service_loop_callback finished.")
-        logger.debug("call service_loop finished.")
-
-    def on_loop_idle(self):
-        logger.debug("calling service on_loop_idle...")
-        if self.on_loop_idle_callback and callable(self.on_loop_idle_callback):
-            try:
-                logger.debug("calling on_loop_idle_callback...")
-                self.on_loop_idle_callback()
-                logger.debug("call on_loop_idle_callback finished.")
-            except Exception as error:
-                logger.exception("calling on_loop_idle_callback failed: {0}".format(str(error)))
-        logger.debug("call service on_loop_idle finished.")
-
-    def on_loop_error(self, error):
-        logger.debug("calling serice on_loop_error: {0}".format(str(error)))
-        if self.on_loop_error_callback and callable(self.on_loop_error_callback):
+                    logger.exception("got unknown exception: {0}".format(str(error)))
+                    if callback:
+                        logger.info(
+                            "call callback function {0} with params {1} {2}".format(
+                                str(callback), str(callback_args), str(callback_kwargs)
+                            )
+                        )
+                        local_callback_args = callback_args or []
+                        local_callback_kwargs = callback_kwargs or {}
+                        callback(*local_callback_args, **local_callback_kwargs)
+                    time.sleep(sleep)
+                if limit and counter >= limit:
+                    break
+
+        return functools.wraps(func)(wrapper)
+
+    return outter_wrapper
+
+
+def get_builtins_dict():
+    """Get builtins data as dict typed.
+
+    @Returns:
+        (dict): All data in builtins.
+
+    """
+    data = {}
+    if PY2:  # no updates anymore...
+        # keys are __builtins__ of python 2.7.18
+        keys = [
+            "ArithmeticError",
+            "AssertionError",
+            "AttributeError",
+            "BaseException",
+            "BufferError",
+            "BytesWarning",
+            "DeprecationWarning",
+            "EOFError",
+            "Ellipsis",
+            "EnvironmentError",
+            "Exception",
+            "False",
+            "FloatingPointError",
+            "FutureWarning",
+            "GeneratorExit",
+            "IOError",
+            "ImportError",
+            "ImportWarning",
+            "IndentationError",
+            "IndexError",
+            "KeyError",
+            "KeyboardInterrupt",
+            "LookupError",
+            "MemoryError",
+            "NameError",
+            "None",
+            "NotImplemented",
+            "NotImplementedError",
+            "OSError",
+            "OverflowError",
+            "PendingDeprecationWarning",
+            "ReferenceError",
+            "RuntimeError",
+            "RuntimeWarning",
+            "StandardError",
+            "StopIteration",
+            "SyntaxError",
+            "SyntaxWarning",
+            "SystemError",
+            "SystemExit",
+            "TabError",
+            "True",
+            "TypeError",
+            "UnboundLocalError",
+            "UnicodeDecodeError",
+            "UnicodeEncodeError",
+            "UnicodeError",
+            "UnicodeTranslateError",
+            "UnicodeWarning",
+            "UserWarning",
+            "ValueError",
+            "Warning",
+            "ZeroDivisionError",
+            "__debug__",
+            "__doc__",
+            "__import__",
+            "__name__",
+            "__package__",
+            "abs",
+            "all",
+            "any",
+            "apply",
+            "basestring",
+            "bin",
+            "bool",
+            "buffer",
+            "bytearray",
+            "bytes",
+            "callable",
+            "chr",
+            "classmethod",
+            "cmp",
+            "coerce",
+            "compile",
+            "complex",
+            "copyright",
+            "credits",
+            "delattr",
+            "dict",
+            "dir",
+            "divmod",
+            "enumerate",
+            "eval",
+            "execfile",
+            "exit",
+            "file",
+            "filter",
+            "float",
+            "format",
+            "frozenset",
+            "getattr",
+            "globals",
+            "hasattr",
+            "hash",
+            "help",
+            "hex",
+            "id",
+            "input",
+            "int",
+            "intern",
+            "isinstance",
+            "issubclass",
+            "iter",
+            "len",
+            "license",
+            "list",
+            "locals",
+            "long",
+            "map",
+            "max",
+            "memoryview",
+            "min",
+            "next",
+            "object",
+            "oct",
+            "open",
+            "ord",
+            "pow",
+            "print",
+            "property",
+            "quit",
+            "range",
+            "raw_input",
+            "reduce",
+            "reload",
+            "repr",
+            "reversed",
+            "round",
+            "set",
+            "setattr",
+            "slice",
+            "sorted",
+            "staticmethod",
+            "str",
+            "sum",
+            "super",
+            "tuple",
+            "type",
+            "unichr",
+            "unicode",
+            "vars",
+            "xrange",
+            "zip",
+        ]
+        for key in keys:
             try:
-                logger.debug("calling on_loop_error_callback...")
-                self.on_loop_error_callback(error)
-                logger.debug("call on_loop_error_callback finished.")
-            except Exception as error:
-                logger.exception("call on_loop_error_callback failed: {0}".format(str(error)))
-        logger.debug("call service on_loop_error finished.")
-
-    def on_loop_finished(self):
-        logger.debug("calling service on_loop_finished...")
-        if self.on_loop_finished_callback and callable(self.on_loop_finished_callback):
+                data[key] = eval(key)
+            except:
+                pass
+    else:
+        import builtins
+
+        for key in dir(builtins):
+            data[key] = getattr(builtins, key)
+    return data
+
+
+def get_all_builtin_exceptions():
+    """Get all builtin exceptions."""
+
+    def get_exceptions(scope):
+        klasses = set()
+        for key, value in scope.items():
+            if key.startswith("_"):
+                continue
             try:
-                logger.debug("calling on_loop_finished_callback...")
-                self.on_loop_finished_callback()
-                logger.debug("call on_loop_finished_callback finished.")
-            except Exception as error:
-                logger.exception("call on on_loop_finished_callback failed: {0}".format(str(error)))
-        logger.debug("call service on_loop_finished finished.")
-
-class SimpleProducer(Service):
-    is_producer = True
-    is_consumer = False
-    default_task_queue_put_timeout = 1
-
-    def __init__(self, task_queue, produce=None, produce_args=None, produce_kwargs=None, task_queue_put_timeout=None, **kwargs):
-        self.task_queue = task_queue
-        self.produce_callback = produce
-        self.produce_callback_args = produce_args or []
-        self.produce_callback_kwargs = produce_kwargs or {}
-        if task_queue_put_timeout is None:
-            self.task_queue_put_timeout = self.default_task_queue_put_timeout
-        else:
-            self.task_queue_put_timeout = task_queue_put_timeout
-        self.produced_counter = Counter()
-        super(SimpleProducer, self).__init__(**kwargs)
+                if issubclass(value, BaseException):
+                    klasses.add(value)
+            except (
+                TypeError
+            ):  # some value can NOT be used in issubclass(xxx), just ignore it...
+                pass
+        return klasses
+
+    es1 = get_exceptions(get_builtins_dict())
+    es2 = get_exceptions(globals())
+    es3 = get_exceptions(locals())
+    return es1.union(es2).union(es3)
 
-    def service_loop(self):
-        """SimpleProducer service_loop is making tasks and putting the tasks into task queue.
-        """
-        logger.debug("SimpleProducer doing service_loop, and making tasks...")
-        tasks = self.produce()
-        logger.debug("SimpleProducer made tasks: {0}".format(tasks))
-        if tasks:
-            delta = len(tasks)
-            logger.debug("SimpleProducer icnring produced_counter, value += {0}".format(delta))
-            self.produced_counter.incr(delta)
-        logger.debug("SimpleProducer putting tasks into task queue...")
-        for task in tasks:
-            while True:
+
+def get_class_name(klass, with_module=False):
+    """Get a class's name.
+
+    @Returns:
+        (str): The name of the klass.
+
+    @Parameters:
+        klass(Any): A class or
+    """
+    if not is_a_class(klass):
+        klass = klass.__class__
+    if with_module:
+        return klass.__module__ + "." + klass.__name__
+    else:
+        return klass.__name__
+
+
+def retry(sleep=0, limit=3, exceptions=None, raise_exceptions=None, **kwargs):
+    """Retry function on errors.
+
+    @Parameters:
+        sleep(int, default to 0):
+            Sleep seconds after retry failed. 0 or less means no sleep.
+        limit(int, default to 3):
+            max try times.
+        exceptions(list of exception types, default to [Exception] means all kind of exceptions):
+            only retry on these errors, otherwise raise immediately.
+        raise_exceptions(list of exception types, default to []):
+            raise immediately for these exceptions.
+        **kwargs:
+            Update key parameters while doing retry.
+
+    @Example:
+        @retry(sleep=5, limit=3)
+        def download(url, filename):
+            response = requests.get(url)
+            with open(filename, "wb") as fobj:
+                fobj.write(response.content)
+        download("http://zencore.cn/example.zip", "example.zip")
+    """
+    if isinstance(raise_exceptions, (list, set)):
+        raise_exceptions = tuple(list(raise_exceptions))
+    if isinstance(exceptions, (list, set)):
+        exceptions = tuple(list(exceptions))
+
+    def outter_wrapper(func):
+        def wrapper(*func_args, **func_kwargs):
+            last_error = None
+            for i in range(limit):
+                break_flag = None
                 try:
-                    logger.debug("SimpleProducer putting task into task_queue: {0}".format(task))
-                    self.task_queue.put(task, timeout=self.task_queue_put_timeout)
-                    logger.debug("SimpleProducer put task done, task: {0}".format(task))
-                    break
-                except Full:
-                    logger.debug("SimpleProducer put task into task_queue failed because the task_queue is full, try again, task: {}".format(task))
-                    pass
-
-    def produce(self):
-        logger.debug("SimpleProducer is making tasks and calling the produce_callback...")
-        if self.produce_callback and callable(self.produce_callback):
-            logger.debug("SimpleProducer is calling produce_callback: args={0} kwargs={1}".format(self.produce_callback_args, self.produce_callback_kwargs))
-            tasks = self.produce_callback(*self.produce_callback_args, **self.produce_callback_kwargs)
-            logger.debug("SimpleProducer call SimpleProducer finished.")
-        else:
-            logger.debug("SimpleProducer has NO produce_callback, return empty tasks...")
-            tasks = []
-        logger.debug("SimpleProducer call produce_callback done, tasks: {0}".format(tasks))
-        return tasks
-
-class SimpleConsumer(Service):
-    is_producer = False
-    is_consumer = True
-    default_task_queue_get_timeout = 1
-
-    def __init__(self, task_queue, consume=None, consume_args=None, consume_kwargs=None, task_queue_get_timeout=None, **kwargs):
-        self.task_queue = task_queue
-        self.consume_callback = consume
-        self.consume_callback_args = consume_args or []
-        self.consume_callback_kwargs = consume_kwargs or {}
-        if task_queue_get_timeout is None:
-            self.task_queue_get_timeout = self.default_task_queue_get_timeout
-        else:
-            self.task_queue_get_timeout = task_queue_get_timeout
-        self.consumed_counter = Counter()
-        super(SimpleConsumer, self).__init__(**kwargs)
+                    if i > 0:
+                        func_kwargs.update(**kwargs)
+                        logger.warning(
+                            "retry again on {func} with last_error={last_error}...".format(
+                                func=func, last_error=last_error
+                            )
+                        )
+                    return func(*func_args, **func_kwargs)
+                except InterruptedError as error:  # 中断异常，则不再重试
+                    last_error = error
+                    break_flag = True
+                except Exception as error:
+                    last_error = error
+                    if raise_exceptions:  # 遇到这些异常，则不再重试，其它都应该重试
+                        if isinstance(error, raise_exceptions):
+                            break_flag = True
+                        else:
+                            break_flag = False
+                    else:  # 遇到这些异常，则重试，其它都不再重试
+                        retry_exceptions = exceptions or Exception
+                        if isinstance(error, retry_exceptions):
+                            break_flag = False
+                        else:
+                            break_flag = True
+                if break_flag is True:
+                    raise last_error
+                if sleep > 0:
+                    time.sleep(sleep)
+            raise last_error
+
+        return functools.wraps(func)(wrapper)
+
+    return outter_wrapper
+
+
+class ChainableProxy(object):
+    """Use in creating a server proxy.
+
+    class ServerProxy(object):
+
+        def __getattr__(self, name):
+            return ChainableProxy(name, self._proxy_callback)
+
+        def _proxy_callback(self, path, *args, **kwargs):
+            return self.remote_exeucte(path, *args, **kwargs)
+
+    server = ServerProxy(...)
+    server.debug.ping()
+    server.myapp.my_remote_call(...)
+    """
 
-    def service_loop(self):
-        """SimpleConsume service_loop is getting tasks from the task_queue, and handling the tasks.
-        """
-        logger.debug("SimpleConsume doing service_loop, and getting task from task_queue...")
-        try:
-            task = self.task_queue.get(timeout=self.task_queue_get_timeout)
-            logger.debug("SimpleConsume got a task: {}".format(task))
-        except Empty:
-            logger.debug("SimpleConsume got NO task...")
-            raise LoopIdle()
-        logger.debug("SimpleConsume icnring consumed_counter, value += 1")
-        self.consumed_counter.incr()
-        logger.debug("SimpleConsume handling the task: {}".format(task))
-        try:
-            result = self.consume(task)
-        except Exception as error:
-            logger.exception("SimpleConsume handling the task and got failed: {0}".format(str(error)))
-            raise error
-        logger.debug("SimpleConsume handled the task, result={0}".format(result))
-
-    def consume(self, task):
-        logger.debug("SimpleConsumer is handling the task: {0}".format(task))
-        if self.consume_callback and callable(self.consume_callback):
-            logger.debug("SimpleConsumer is calling consume_callback: args={0} kwargs={1}".format(self.consume_callback_args, self.consume_callback_kwargs))
-            result = self.consume_callback(task, *self.consume_callback_args, **self.consume_callback_kwargs)
-            logger.debug("SimpleConsumer call consume_callback finished.")
-        else:
-            result = None
-        logger.debug("SimpleConsumer call consume_callback done, result: {0}".format(result))
-        return result
+    def __init__(self, path, proxy_callback, proxy_callback_extra_data=None):
+        self.path = path
+        self.proxy_callback = proxy_callback
+        self.proxy_callback_extra_data = proxy_callback_extra_data or {}
+
+    def __getattr__(self, name):
+        return ChainableProxy(
+            ".".join([self.path, name]),
+            self.proxy_callback,
+            self.proxy_callback_extra_data,
+        )
+
+    def __call__(self, *args, **kwargs):
+        args = args or tuple([])
+        args = tuple([self.path]) + args
+        kwargs = kwargs or {}
+        for key, value in self.proxy_callback_extra_data.items():
+            kwargs.setdefault(key, value)
+        return self.proxy_callback(*args, **kwargs)
 
-class SimpleServer(object):
 
-    def __init__(self, workers=None, **kwargs):
-        workers = workers or []
-        self.workers = [] + workers
-        self.start_lock = threading.Lock()
-        self.started = None
-        self.started_time = None
-        self.stop_flag = None
-        self.stop_time = None
-        self.terminate_flag = False
-        self.terminate_time = None
-
-    def add_worker(self, worker):
-        self.workers.append(worker)
-
-    @property
-    def is_runing(self):
-        for worker in self.workers:
-            if worker.is_running:
-                return True
-        return False
-
-    @property
-    def stopped(self):
-        for worker in self.workers:
-            if not worker.stopped:
-                return False
-        return True
-
-    @property
-    def stopped_time(self):
-        latest_time = None
-        for worker in self.workers:
-            if latest_time is None:
-                latest_time = worker.stopped_time
-            if worker.stopped_time > latest_time:
-                latest_time = worker.stopped_time
-        return latest_time
-
-    @property
-    def terminated(self):
-        for worker in self.workers:
-            if not worker.terminated:
-                return False
-        return True
-
-    @property
-    def terminated_time(self):
-        latest_time = None
-        for worker in self.workers:
-            if latest_time is None:
-                latest_time = worker.terminated_time
-            if worker.terminated_time > latest_time:
-                latest_time = worker.terminated_time
-        return latest_time
-
-    def start(self):
-        logger.debug("SimpleServer starting...")
-        with self.start_lock:
-            self.stop_flag = False
-            self.stop_time = None
-            for worker in self.workers:
-                logger.info("SimpleServer starting worker: {0}".format(worker.service_name))
-                worker.start()
-            if not self.started:
-                self.started = True
-                self.started_time = time.time()
-
-    def stop(self, wait=True, wait_timeout=-1):
-        logger.debug("SimpleServer stopping...")
-        self.stop_flag = True
-        self.stop_time = time.time()
-        results = []
-        for worker in self.workers:
-            result = worker.stop(wait, wait_timeout)
-            results.append(result)
-        for result in results:
-            if result is None:
-                logger.debug("SimpleServer stopping result=None")
-                return None
-            if result is False:
-                logger.debug("SimpleServer stopping result=False")
-                return False
-        logger.debug("SimpleServer stopping result=True")
-        return True
-
-    def terminate(self, wait=True, wait_timeout=-1):
-        logger.debug("SimpleServer terminating...")
-        self.terminate_flag = True
-        self.terminate_time = time.time()
-        results = []
-        for worker in self.workers:
-            result = worker.terminate(wait, wait_timeout)
-        for result in results:
-            if result is None:
-                logger.debug("SimpleServer terminating result=None")
-                return None
-            if result is False:
-                logger.debug("SimpleServer terminating result=False")
-                return False
-        logger.debug("SimpleServer terminating result=True")
-        return True
+### alias to keep old compatiable
+is_a_class = isclass
 
-    def join(self, wait=True, wait_timeout=-1):
-        logger.debug("SimpleServer joining...")
-        results = []
-        for worker in self.workers:
-            result = worker.join(wait, wait_timeout)
-        for result in results:
-            if result is None:
-                logger.debug("SimpleServer joining result=None")
-                return None
-            if result is False:
-                logger.debug("SimpleServer joining result=False")
-                return False
-        logger.debug("SimpleServer joining result=True")
-        return True
-
-    @classmethod
-    def serve(cls, **kwargs):
-        server = cls(**kwargs)
-        server.start()
-        return server
-
-class SimpleProducerConsumerServer(SimpleServer):
-    default_queue_size = 200
-    default_producer_class = SimpleProducer
-    default_consumer_class = SimpleConsumer
-    default_producer_number = 1
-    default_consumer_number = 1
-
-    def __init__(self, producer_class=None, consumer_class=None, producer_number=None, consumer_number=None, queue_size=None, server=None, service_name=None, **kwargs):
-        self.producer_class = producer_class or self.default_producer_class
-        self.consumer_class = consumer_class or self.default_consumer_class
-        self.producer_number = producer_number or self.default_producer_number
-        self.consumer_number = consumer_number or self.default_consumer_number
-        self.kwargs = kwargs
-        self.queue_size = queue_size or self.default_queue_size
-        self.server = server
-        self.service_name = service_name or self.__class__.__name__
-        self.task_queue = Queue(self.queue_size)
-        self.producers = self.create_producers()
-        self.consumers = self.create_consumers()
-        super(SimpleProducerConsumerServer, self).__init__(self.producers + self.consumers)
-
-    def create_producers(self):
-        logger.info("SimpleProducerConsumerServer creating producers...")
-        producers = []
-        for index in range(self.producer_number):
-            service_name = self.service_name + ":producer#{0}".format(index)
-            logger.info("SimpleProducerConsumerServer creating producer: {0}".format(service_name))
-            args = self.kwargs.get("producer_class_init_args", [])
-            kwargs = {
-                "task_queue": self.task_queue,
-                "server": self,
-                "service_name": service_name,
-            }
-            kwargs.update(self.kwargs.get("producer_class_init_kwargs", {}))
-            kwargs.update(self.kwargs)
-            producer = self.producer_class(*args, **kwargs)
-            producers.append(producer)
-        logger.info("SimpleProducerConsumerServer creating producers done")
-        return producers
-    
-    def create_consumers(self):
-        logger.info("SimpleProducerConsumerServer creating consumers...")
-        consumers = []
-        for index in range(self.consumer_number):
-            service_name = self.service_name + ":consumer#{0}".format(index)
-            logger.info("SimpleProducerConsumerServer creating consumer: {0}".format(service_name))
-            args = self.kwargs.get("consumer_class_init_args", [])
-            kwargs = {
-                "task_queue": self.task_queue,
-                "server": self,
-                "service_name": service_name,
-            }
-            kwargs.update(self.kwargs.get("consumer_class_init_kwargs", {}))
-            kwargs.update(self.kwargs)
-            consumer = self.consumer_class(*args, **kwargs)
-            consumers.append(consumer)
-        logger.info("SimpleProducerConsumerServer creating consumers done")
-        return consumers
+
+def get_method_help(func):
+    """
+    获取函数的帮助信息。一般用于rpc提示。
+    """
+    if hasattr(func, "__help_text__"):
+        return getattr(func, "__help_text__")
+    if hasattr(func, "__help__"):
+        return getattr(func, "__help__")
+    if hasattr(func, "__doc__"):
+        return getattr(func, "__doc__")
+    return ""
+
+
+def get_method_signature(func):
+    """
+    获取函数的参数和返回值信息。一般用于rpc提示。
+    """
+    if hasattr(func, "__signature__"):
+        return getattr(func, "__signature__")
+    help_text = get_method_help(func)
+    if help_text:
+        sigs = [
+            x.strip()
+            for x in re.findall(
+                "@signature \\{\\{\\{(.*)\\}\\}\\}",
+                help_text,
+                re.MULTILINE | re.IGNORECASE | re.DOTALL,
+            )
+        ]
+        if sigs:
+            return json.loads(sigs[0])
+    return []
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.3.9/zenutils/treeutils.py` & `zenutils-0.4.8/zenutils/treeutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,97 +1,134 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""树结构工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 __all__ = [
     "build_tree",
     "tree_walk",
     "print_tree_callback",
     "print_tree",
     "SimpleRouterTree",
 ]
 
-def build_tree(thelist, pk_attr="id", parent_attr="parent_id", children_attr="children"):
-    """Tree node is a dict with pk_attr, parent_attr and children_attr fields: {"id": 2, "parent_id": 1, "children": []}.
-    """
+
+def build_tree(
+    thelist, pk_attr="id", parent_attr="parent_id", children_attr="children"
+):
+    """Tree node is a dict with pk_attr, parent_attr and children_attr fields: {"id": 2, "parent_id": 1, "children": []}."""
     from zenutils import dictutils
+
     roots = []
     nodes = {}
     for node in thelist:
         dictutils.touch(node, children_attr, [])
         node_id = dictutils.select(node, pk_attr)
         nodes[node_id] = node
     for node in thelist:
         parent_id = dictutils.select(node, parent_attr)
         if (not parent_id) or (not parent_id in nodes):
             roots.append(node)
         else:
             dictutils.select(nodes[parent_id], children_attr).append(node)
     return roots
 
-def tree_walk(tree, callback, children_attr="children", callback_args=None, callback_kwargs=None, depth=0, parent=None):
+
+def tree_walk(
+    tree,
+    callback,
+    children_attr="children",
+    callback_args=None,
+    callback_kwargs=None,
+    depth=0,
+    parent=None,
+):
     from zenutils import dictutils
 
     callback_args = callback_args or ()
     callback_kwargs = callback_kwargs or {}
 
     for node in tree:
         callback(node, tree, depth, parent, *callback_args, **callback_kwargs)
         children = dictutils.select(node, children_attr, [])
         if children:
-            tree_walk(children, callback, children_attr, callback_args, callback_kwargs, depth+1, node)
+            tree_walk(
+                children,
+                callback,
+                children_attr,
+                callback_args,
+                callback_kwargs,
+                depth + 1,
+                node,
+            )
+
 
 def print_tree_callback(node, tree, depth, parent, *args, **kwargs):
     from zenutils import dictutils
+
     title_attr = kwargs.get("title_attr", "title")
     indent_string = kwargs.get("indent_string", "    ")
     print(indent_string * depth + dictutils.select(node, title_attr))
 
-def print_tree(tree, title_attr="title", children_attr="children", indent_string="     "):
-    tree_walk(tree, print_tree_callback, children_attr, (), {"title_attr": title_attr, "indent_string": indent_string})
+
+def print_tree(
+    tree, title_attr="title", children_attr="children", indent_string="     "
+):
+    tree_walk(
+        tree,
+        print_tree_callback,
+        children_attr,
+        (),
+        {"title_attr": title_attr, "indent_string": indent_string},
+    )
+
 
 class SimpleRouterTree(object):
-    """简单的路由索引和搜索树。
-    """
+    """简单的路由索引和搜索树。"""
 
     def __init__(self):
         self.data = {}
         self.paths = {}
-    
+
     def index(self, path, data):
-        """索引
-        """
+        """索引"""
         cp = self.data
         for c in path:
             if not c in cp:
                 cp[c] = {}
             cp = cp[c]
         cp["_data"] = data
         cp["_path"] = path
         self.paths[path] = cp
         return cp
 
     def get(self, path):
-        """精确匹配
-        """
+        """精确匹配"""
         cp = self.data
         for c in path:
             if c in cp:
                 cp = cp[c]
             else:
                 return None
         if not "_data" in cp:
             return None
         else:
             return cp["_data"]
 
     def get_best_match(self, path):
-        """最长匹配
-        """
+        """最长匹配"""
         best_match = None
         best_path = None
         cp = self.data
         for c in path:
             if "_data" in cp:
                 best_match = cp["_data"]
                 best_path = cp["_path"]
@@ -102,15 +139,15 @@
         if "_data" in cp:
             best_match = cp["_data"]
             best_path = cp["_path"]
         return best_path, best_match
 
     def delete(self, path):
         """删除索引。
-        
+
         数据已删除，但没有清理遗留结构。
         """
         if path in self.paths:
             del self.paths[path]
         cp = self.data
         for c in path:
             if c in cp:
@@ -123,8 +160,7 @@
             del cp["_data"]
             return True
 
     def get_all_paths(self):
         paths = list(self.paths.keys())
         paths.sort()
         return paths
-
```

### Comparing `zenutils-0.3.9/zenutils/typingutils.py` & `zenutils-0.4.8/zenutils/typingutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
-from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
+"""类型转化工具。"""
+from __future__ import (
+    absolute_import,
+    division,
+    generators,
+    nested_scopes,
+    print_function,
+    unicode_literals,
+    with_statement,
+)
 from zenutils.sixutils import *
 
 __all__ = [
     "STRING_ENCODINGS",
     "register_global_caster",
     "smart_cast",
     "Number",
@@ -20,86 +29,104 @@
 
 def cast_int(value):
     """Change the value to int value.
 
     @Returns:
         (None or int): Try to change the value to int.
                        If value is None or empty string, returns None value.
-    
+
     @Parameters:
         value(Any): Any value that will be changed to int value.
-    
+
     @Raises:
         ValueError: invalid literal for int() with base 10: 'xxx'
         TypeError: int() argument must be a string, a bytes-like object or a number, not 'XxxType'
     """
     if value is None:
         return None
     if isinstance(value, (STR_TYPE, BYTES_TYPE)):
         if not value.strip():
             return None
     if isinstance(value, int):
         return value
     return int(value)
 
+
 def cast_float(value):
     """Change the value to float value.
 
     @Returns:
         (None or float): Try to change the value to float.
                          If value is None or empty string, returns None value.
-    
+
     @Parameters:
         value(Any): Any value that will be changed to float value.
-    
+
     @Raises:
         ValueError: could not convert string to float: 'xxx'
         TypeError: float() argument must be a string or a number, not 'XxxType'
     """
     if value is None:
         return None
     if isinstance(value, (STR_TYPE, BYTES_TYPE)):
         if not value.strip():
             return None
     if isinstance(value, float):
         return value
     return float(value)
 
+
 def cast_bool(value):
     """Change the value to bool value.
 
     @Returns:
         (None or bool): Try to change the value to bool.
                         If value is None or empty string, returns None value.
-    
+
     @Parameters:
         value(Any): Any value that will be changed to float value.
     """
     if value is None:
         return None
     if isinstance(value, (STR_TYPE, BYTES_TYPE)):
         if not value.strip():
             return None
     if isinstance(value, bool):
         return value
     if isinstance(value, (STR_TYPE, BYTES_TYPE)):
         if value.lower() in [
-                "true", "yes", "y", "t", "1", "on", "active", "ok",
-                b"true", b"yes", b"y", b"t", b"1", b"on", b"active", b"ok",
-            ]:
+            "true",
+            "yes",
+            "y",
+            "t",
+            "1",
+            "on",
+            "active",
+            "ok",
+            b"true",
+            b"yes",
+            b"y",
+            b"t",
+            b"1",
+            b"on",
+            b"active",
+            b"ok",
+        ]:
             return True
         else:
             return False
     if value:
         return True
     else:
         return False
 
+
 def cast_list(value):
     from zenutils.strutils import force_type_to
+
     if value is None:
         return None
     if isinstance(value, (STR_TYPE, BYTES_TYPE)):
         if not value.strip():
             return None
     if isinstance(value, (list, tuple, set)):
         return list(value)
@@ -112,17 +139,19 @@
             except:
                 pass
     if not isinstance(value, list):
         return [value]
     else:
         return value
 
+
 def cast_bytes(value):
     from zenutils import strutils
     from zenutils import base64utils
+
     if value is None:
         return None
     if isinstance(value, (STR_TYPE, BYTES_TYPE)):
         if not value.strip():
             return None
     if isinstance(value, BYTES_TYPE):
         return value
@@ -134,21 +163,23 @@
             value = force_bytes(value)
             return base64utils.decodebytes(value)
         elif strutils.is_urlsafeb64_decodable(value):
             value = force_bytes(value)
             return base64utils.urlsafe_b64decode(value)
     return force_bytes(value)
 
+
 def cast_str(value):
     if value is None:
         return None
     if isinstance(value, STR_TYPE):
         return value
     return force_text(value)
 
+
 def cast_dict(value):
     if value is None:
         return None
     if isinstance(value, (STR_TYPE, BYTES_TYPE)):
         if not value.strip():
             return None
     if isinstance(value, dict):
@@ -156,37 +187,39 @@
     if isinstance(value, (STR_TYPE, BYTES_TYPE)):
         try:
             return json.loads(value)
         except:
             pass
     return dict(value)
 
+
 def cast_numeric(value):
     if value is None:
         return None
     if isinstance(value, (STR_TYPE, BYTES_TYPE)):
         if not value.strip():
             return None
     if isinstance(value, Number):
         return value
     value = force_text(value)
     if "." in value:
         return float(value)
     else:
         return int(value)
 
+
 def cast_uuid(value):
     """Change the value to UUID type.
 
     @Returns:
         (UUID): The UUID typed value.
-    
+
     @Parameters:
         value(Any): Any value that can be changed to UUID type.
-    
+
     @Examples:
         assert str(cast_uuid(85188153587611980436344659581497329339)) == "4016a43f-406e-47b4-b332-e0f9016546bb"
         assert str(cast_uuid("4016a43f-406e-47b4-b332-e0f9016546bb")) == "4016a43f-406e-47b4-b332-e0f9016546bb"
         assert str(cast_uuid((1075225663, 16494, 18356, 179, 50, 247360074892987))) == "4016a43f-406e-47b4-b332-e0f9016546bb"
         assert str(cast_uuid(b'@\x16\xa4?@nG\xb4\xb32\xe0\xf9\x01eF\xbb')) == "4016a43f-406e-47b4-b332-e0f9016546bb"
     """
     if value is None:
@@ -203,65 +236,72 @@
         pass
     try:
         return uuid.UUID(int=value)
     except:
         pass
     return uuid.UUID(value)
 
+
 TYPE_CASTERS = {}
 
+
 def register_global_caster(type, caster):
     TYPE_CASTERS[type] = caster
 
+
 register_global_caster(int, cast_int)
 register_global_caster(float, cast_float)
 register_global_caster(bool, cast_bool)
 register_global_caster(BYTES_TYPE, cast_bytes)
 register_global_caster(STR_TYPE, cast_str)
 register_global_caster(list, cast_list)
 register_global_caster(dict, cast_dict)
 register_global_caster(Number, cast_numeric)
 register_global_caster(uuid.UUID, cast_uuid)
 
 try:
     import typing
+
     register_global_caster(typing.List, cast_list)
     register_global_caster(typing.Mapping, cast_dict)
 except Exception:
     pass
 
+
 def smart_cast(type, value, field_name=None):
     """Cast the value to the given type smartly.
 
     @Returns:
         (Any): The given typed value.
-    
+
     @Parameters:
         type(Class): The type you want the value changed to.
         value(Any): The value will be changed.
-        field_name(str, optional):  It is used in the message of the exception 
+        field_name(str, optional):  It is used in the message of the exception
                                     which will be raised if the value failed to change into the given type.
 
     @Examples:
         assert smart_cast(int, "1234") == 1234
         assert smart_cast(bool, "yes") is True
         assert smart_cast(str, b"hello") == "hello"
     """
     if type in TYPE_CASTERS:
         type_func = TYPE_CASTERS[type]
     elif callable(type):
         type_func = type
     else:
         if field_name:
-            raise TypeError("not supported type, field={field_name}, type={type}, value={value}".format(
-                field_name=field_name,
-                type=force_text(type(value)),
-                value=force_text(value),
-            ))
+            raise TypeError(
+                "not supported type, field={field_name}, type={type}, value={value}".format(
+                    field_name=field_name,
+                    type=force_text(type(value)),
+                    value=force_text(value),
+                )
+            )
         else:
-            raise TypeError("not supported type, type={type}, value={value}".format(
-                type=force_text(type(value)),
-                value=force_text(value),
-            ))
+            raise TypeError(
+                "not supported type, type={type}, value={value}".format(
+                    type=force_text(type(value)),
+                    value=force_text(value),
+                )
+            )
     return type_func(value)
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zenutils-0.3.9/zenutils.egg-info/SOURCES.txt` & `zenutils-0.4.8/zenutils.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,53 +5,66 @@
 requirements.txt
 setup.py
 zenutils/__init__.py
 zenutils/base64utils.py
 zenutils/baseutils.py
 zenutils/cacheutils.py
 zenutils/cipherutils.py
+zenutils/dateutils.py
 zenutils/dictutils.py
+zenutils/errorutils.py
 zenutils/fsutils.py
 zenutils/funcutils.py
 zenutils/hashutils.py
 zenutils/httputils.py
+zenutils/importutils.py
 zenutils/jsonutils.py
 zenutils/listutils.py
 zenutils/logutils.py
 zenutils/nameutils.py
 zenutils/numericutils.py
+zenutils/packutils.py
+zenutils/perfutils.py
 zenutils/randomutils.py
+zenutils/serviceutils.py
 zenutils/sixutils.py
+zenutils/socketserverutils.py
 zenutils/strutils.py
 zenutils/sysutils.py
 zenutils/threadutils.py
 zenutils/treeutils.py
 zenutils/typingutils.py
+zenutils/xmlrpcutils.py
 zenutils.egg-info/PKG-INFO
 zenutils.egg-info/SOURCES.txt
 zenutils.egg-info/dependency_links.txt
 zenutils.egg-info/not-zip-safe
 zenutils.egg-info/top_level.txt
 zenutils/tests/__init__.py
 zenutils/tests/t08_01.py
 zenutils/tests/test_baseutils.py
 zenutils/tests/test_cacheutils.py
 zenutils/tests/test_cipherutils.py
+zenutils/tests/test_dateutils.py
 zenutils/tests/test_dictutils.py
+zenutils/tests/test_errorutils.py
 zenutils/tests/test_fsutils.py
 zenutils/tests/test_funcutils.py
 zenutils/tests/test_hashutils.py
 zenutils/tests/test_httputils.py
 zenutils/tests/test_import_all.py
+zenutils/tests/test_importutils.py
 zenutils/tests/test_jsonutils.py
 zenutils/tests/test_listutils.py
 zenutils/tests/test_logutils.py
 zenutils/tests/test_nameutils.py
 zenutils/tests/test_numericutils.py
+zenutils/tests/test_packutils.py
 zenutils/tests/test_randomutils.py
+zenutils/tests/test_serviceutils.py
 zenutils/tests/test_sixutils.py
 zenutils/tests/test_strutils.py
 zenutils/tests/test_sysutils.py
 zenutils/tests/test_threadutils.py
 zenutils/tests/test_treeutils.py
 zenutils/tests/test_typingutils.py
 zenutils/tests/assets/a.txt
```


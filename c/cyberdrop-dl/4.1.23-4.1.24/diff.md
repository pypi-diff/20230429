# Comparing `tmp/cyberdrop-dl-4.1.23.tar.gz` & `tmp/cyberdrop-dl-4.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.1.23.tar", last modified: Fri Apr 28 17:40:27 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.1.24.tar", last modified: Sat Apr 29 00:51:13 2023, max compression
```

## Comparing `cyberdrop-dl-4.1.23.tar` & `cyberdrop-dl-4.1.24.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.997600 cyberdrop-dl-4.1.23/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 17:40:26.997600 cyberdrop-dl-4.1.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.985599 cyberdrop-dl-4.1.23/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.989600 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.989600 cyberdrop-dl-4.1.23/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/client/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.997600 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.997600 cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17579 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.997600 cyberdrop-dl-4.1.23/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20272 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.989600 cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 17:40:26.000000 cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-28 17:40:26.000000 cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:40:26.000000 cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 17:40:26.000000 cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 17:40:26.000000 cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 17:40:26.000000 cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-28 17:40:26.997600 cyberdrop-dl-4.1.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.751474 cyberdrop-dl-4.1.24/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-29 00:51:13.751474 cyberdrop-dl-4.1.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.743473 cyberdrop-dl-4.1.24/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.747473 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.747473 cyberdrop-dl-4.1.24/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/client/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.747473 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.751474 cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17579 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.751474 cyberdrop-dl-4.1.24/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20272 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.743473 cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-29 00:51:13.000000 cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-29 00:51:13.000000 cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:51:13.000000 cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-29 00:51:13.000000 cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-29 00:51:13.000000 cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 00:51:13.000000 cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-29 00:51:13.751474 cyberdrop-dl-4.1.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/setup.py
```

### Comparing `cyberdrop-dl-4.1.23/LICENSE` & `cyberdrop-dl-4.1.24/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/PKG-INFO` & `cyberdrop-dl-4.1.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.23
+Version: 4.1.24
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.23 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.24 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.23/README.md` & `cyberdrop-dl-4.1.24/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,15 +241,22 @@
     async def fix_bunkr_entries(self, url: URL, original_filename: str) -> None:
         complete_row = None
         url_path = await get_db_path(url)
         self.curs.execute("""SELECT * FROM media WHERE url_path = ?""", (url_path,))
         sql_res = self.curs.fetchall()
         for row in sql_res:
             if row[7] == 1:
-                complete_row = row
+                if complete_row:
+                    if row[6] == original_filename:
+                        await self._remove_entry(url_path, complete_row[6])
+                        complete_row = row
+                    else:
+                        await self._remove_entry(url_path, row[6])
+                else:
+                    complete_row = row
             else:
                 if len(sql_res) < 2:
                     await self._update_row_original_filename(url_path, original_filename)
                     break
                 await self._remove_entry(url_path, row[6])
         if complete_row and complete_row[6] != original_filename:
             await self._update_row_original_filename(url_path, original_filename)
```

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/client/rate_limiting.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/client/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import re
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Dict, Tuple, List
+from typing import TYPE_CHECKING, Dict, List, Tuple
 
 import aiofiles
 import bs4
 from bs4 import BeautifulSoup
 from yarl import URL
 
 from ..base_functions.base_functions import (
@@ -24,15 +24,17 @@
     from ..client.client import ScrapeSession
 
 
 @dataclass
 class ParseSpec:
     """Class for specific selectors of supported domains"""
     domain: str
-    
+
+    login_path: str = field(init=False)
+
     title_block_tag: str = "h1[class=p-title-value]"
     title_clutter_tag: str = field(init=False)
 
     posts_block_tag: str = "div[class*=message-main]"
     posts_number_tag: str = field(init=False)
     posts_number_attribute: str = "href"
 
@@ -57,50 +59,51 @@
     attachment_tag: str = "a"
     attachment_attribute: str = "href"
 
     next_page_tag: str = 'a[class="pageNav-jump pageNav-jump--next"]'
     next_page_attribute: str = "href"
 
     def __post_init__(self):
-        if self.domain in ("simpcity", "xbunker", "socialmediagirls"):
+        if self.domain in ("simpcity", "socialmediagirls", "xbunker"):
+            self.login_path = "login"
             self.title_clutter_tag = "a" if self.domain in ("simpcity", "xbunker") else "span"
             self.posts_number_tag = "li[class=u-concealed] a"
             self.images_tag = "div[class*=bbImage]"
             self.images_attribute = "data-src"
 
         elif self.domain == "nudostar":
+            self.login_path = "forum/login"
             self.title_clutter_tag = "span"
             self.posts_number_tag = "a[class=u-concealed]"
             self.images_tag = "img[class*=bbImage]"
             self.images_attribute = "src"
 
 
 class ForumLogin:
     def __init__(self, name: str, username: str, password: str):
         self.name = name
         self.logged_in = False
         self.username = username
         self.password = password
 
-    async def login(self, session: ScrapeSession, url: URL, quiet: bool) -> None:
+    async def login(self, session: ScrapeSession, url: URL, spec: ParseSpec, quiet: bool) -> None:
         """Handles forum logging in"""
         if not self.username or not self.password:
             log(f"Login wasn't provided for {self.name}", quiet=quiet, style="red")
             raise FailedLoginFailure()
         attempt = 0
         while True:
             try:
                 if self.logged_in:
                     return
                 if attempt == 5:
                     raise FailedLoginFailure()
 
                 assert url.host is not None
-                domain = URL("https://" + url.host) / "forum/login" if "nudostar" in url.host else \
-                    URL("https://" + url.host) / "login"
+                domain = URL("https://" + url.host) / spec.login_path
 
                 text = await session.get_text(domain)
                 await asyncio.sleep(5)
                 soup = BeautifulSoup(text, 'html.parser')
 
                 inputs = soup.select('form input')
                 data = {
@@ -124,63 +127,51 @@
                 self.logged_in = True
             except asyncio.exceptions.TimeoutError:
                 attempt += 1
                 continue
 
 
 class XenforoCrawler:
-    domains = ("nudostar", "simpcity", "socialmediagirls", "xbunker")
+    domains = {
+        "nudostar": "NudoStar",
+        "simpcity": "SimpCity",
+        "socialmediagirls": "SocialMediaGirls",
+        "xbunker": "XBunker",
+    }
 
     def __init__(self, *, scraping_mapper, args: Dict, SQL_Helper: SQLHelper, quiet: bool):
         self.include_id = args["Runtime"]["include_id"]
         self.quiet = quiet
         self.separate_posts = args["Forum_Options"]["separate_posts"]
         self.output_last = args["Forum_Options"]["output_last_forum_post"]
         self.output_last_file = args["Files"]["output_last_forum_post_file"]
 
-        self.nudostar = ForumLogin("NudoStar",
-                                   args["Authentication"]["nudostar_username"],
-                                   args["Authentication"]["nudostar_password"])
-
-        self.simpcity = ForumLogin("SimpCity",
-                                   args["Authentication"]["simpcity_username"],
-                                   args["Authentication"]["simpcity_password"])
-
-        self.socialmediagirls = ForumLogin("SocialMediaGirls",
-                                           args["Authentication"]["socialmediagirls_username"],
-                                           args["Authentication"]["socialmediagirls_password"])
-
-        self.xbunker = ForumLogin("XBunker",
-                                  args["Authentication"]["xbunker_username"],
-                                  args["Authentication"]["xbunker_password"])
+        auth_args = args["Authentication"]
+        self.forums = {domain: ForumLogin(name,
+                                          auth_args[f"{domain}_username"],
+                                          auth_args[f"{domain}_password"])
+                       for domain, name in self.domains.items()}
 
         self.scraping_mapper = scraping_mapper
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> Tuple[CascadeItem, str]:
         """Xenforo forum director"""
         log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
         cascade = CascadeItem({})
 
         scrape_url, post_num = await self.get_thread_url_and_post_num(url)
         title = ""
         try:
             assert url.host is not None
-            if "simpcity" in url.host:
-                await self.simpcity.login(session, url, self.quiet)
-            elif "socialmediagirls" in url.host:
-                await self.socialmediagirls.login(session, url, self.quiet)
-            elif "xbunker" in url.host:
-                await self.xbunker.login(session, url, self.quiet)
-            elif "nudostar" in url.host:
-                await self.nudostar.login(session, url, self.quiet)
-
             domain = next((domain for domain in self.domains if domain in url.host), None)
             if domain:
-                title = await self.parse_forum(session, scrape_url, ParseSpec(domain), cascade, "", post_num)
+                parse_spec = ParseSpec(domain)
+                await self.forums[domain].login(session, url, parse_spec, self.quiet)
+                title = await self.parse_forum(session, scrape_url, parse_spec, cascade, "", post_num)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return cascade, ""
 
         await self.SQL_Helper.insert_cascade(cascade)
```

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/main.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.1.24/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.23
+Version: 4.1.24
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.23 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.24 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.23/setup.cfg` & `cyberdrop-dl-4.1.24/setup.cfg`

 * *Files identical despite different names*


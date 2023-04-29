# Comparing `tmp/ofscraper-1.82.tar.gz` & `tmp/ofscraper-1.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-1.82.tar", max compression
+gzip compressed data, was "ofscraper-1.83.tar", max compression
```

## Comparing `ofscraper-1.82.tar` & `ofscraper-1.83.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1067 2023-04-13 21:26:07.930007 ofscraper-1.82/LICENSE
--rw-r--r--   0        0        0     5679 2023-04-28 17:03:56.331089 ofscraper-1.82/README.md
--rw-r--r--   0        0        0     1235 2023-04-28 17:03:56.331089 ofscraper-1.82/pyproject.toml
--rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.82/src/__init__.py
--rw-r--r--   0        0        0      733 2023-04-28 17:03:56.331089 ofscraper-1.82/src/__version__.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.82/src/api/__init__.py
--rw-r--r--   0        0        0     2169 2023-04-28 05:28:10.687970 ofscraper-1.82/src/api/highlights.py
--rw-r--r--   0        0        0      838 2023-04-28 05:28:10.687970 ofscraper-1.82/src/api/init.py
--rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.82/src/api/me.py
--rw-r--r--   0        0        0     3580 2023-04-28 05:28:10.687970 ofscraper-1.82/src/api/messages.py
--rw-r--r--   0        0        0     1788 2023-04-28 05:28:10.687970 ofscraper-1.82/src/api/paid.py
--rw-r--r--   0        0        0     7626 2023-04-28 11:23:57.457623 ofscraper-1.82/src/api/posts.py
--rw-r--r--   0        0        0     3247 2023-04-28 05:28:10.687970 ofscraper-1.82/src/api/profile.py
--rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.82/src/api/subscriptions.py
--rw-r--r--   0        0        0     5441 2023-04-28 05:28:10.687970 ofscraper-1.82/src/api/timeline.py
--rw-r--r--   0        0        0     4781 2023-04-28 11:23:57.457623 ofscraper-1.82/src/constants.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.82/src/db/__init__.py
--rw-r--r--   0        0        0    11266 2023-04-28 05:28:10.688970 ofscraper-1.82/src/db/operations.py
--rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.82/src/db/queries.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.82/src/interaction/__init__.py
--rw-r--r--   0        0        0     3169 2023-04-28 05:28:10.688970 ofscraper-1.82/src/interaction/like.py
--rw-r--r--   0        0        0     5080 2023-04-28 05:28:10.688970 ofscraper-1.82/src/prompts/prompt_functions.py
--rw-r--r--   0        0        0      359 2023-04-14 18:21:19.249081 ofscraper-1.82/src/prompts/prompt_strings.py
--rw-r--r--   0        0        0    17909 2023-04-28 11:23:57.457623 ofscraper-1.82/src/prompts/prompts.py
--rwxr-xr-x   0        0        0    19166 2023-04-28 14:14:09.709648 ofscraper-1.82/src/scraper.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.82/src/utils/__init__.py
--rw-r--r--   0        0        0     2726 2023-04-28 11:23:57.458623 ofscraper-1.82/src/utils/args.py
--rw-r--r--   0        0        0     8856 2023-04-28 05:28:10.689970 ofscraper-1.82/src/utils/auth.py
--rw-r--r--   0        0        0     8874 2023-04-28 11:59:24.168331 ofscraper-1.82/src/utils/config.py
--rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.82/src/utils/dates.py
--rw-r--r--   0        0        0    10235 2023-04-28 16:55:56.692036 ofscraper-1.82/src/utils/download.py
--rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.82/src/utils/encoding.py
--rw-r--r--   0        0        0     2938 2023-04-28 16:51:38.491314 ofscraper-1.82/src/utils/exit.py
--rw-r--r--   0        0        0     2795 2023-04-28 14:37:12.121950 ofscraper-1.82/src/utils/paths.py
--rw-r--r--   0        0        0     2998 2023-04-28 05:28:10.690970 ofscraper-1.82/src/utils/profiles.py
--rw-r--r--   0        0        0      779 2023-04-28 05:28:10.690970 ofscraper-1.82/src/utils/separate.py
--rw-r--r--   0        0        0     6888 1970-01-01 00:00:00.000000 ofscraper-1.82/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-13 21:26:07.930007 ofscraper-1.83/LICENSE
+-rw-r--r--   0        0        0     5800 2023-04-29 01:35:38.362445 ofscraper-1.83/README.md
+-rw-r--r--   0        0        0     1235 2023-04-29 01:32:56.731751 ofscraper-1.83/pyproject.toml
+-rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.83/src/__init__.py
+-rw-r--r--   0        0        0      733 2023-04-29 01:32:56.731751 ofscraper-1.83/src/__version__.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.83/src/api/__init__.py
+-rw-r--r--   0        0        0     2169 2023-04-28 05:28:10.687970 ofscraper-1.83/src/api/highlights.py
+-rw-r--r--   0        0        0      838 2023-04-28 05:28:10.687970 ofscraper-1.83/src/api/init.py
+-rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.83/src/api/me.py
+-rw-r--r--   0        0        0     3580 2023-04-28 05:28:10.687970 ofscraper-1.83/src/api/messages.py
+-rw-r--r--   0        0        0     1788 2023-04-28 05:28:10.687970 ofscraper-1.83/src/api/paid.py
+-rw-r--r--   0        0        0     7626 2023-04-28 11:23:57.457623 ofscraper-1.83/src/api/posts.py
+-rw-r--r--   0        0        0     3247 2023-04-28 05:28:10.687970 ofscraper-1.83/src/api/profile.py
+-rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.83/src/api/subscriptions.py
+-rw-r--r--   0        0        0     5441 2023-04-28 05:28:10.687970 ofscraper-1.83/src/api/timeline.py
+-rw-r--r--   0        0        0     4781 2023-04-28 11:23:57.457623 ofscraper-1.83/src/constants.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.83/src/db/__init__.py
+-rw-r--r--   0        0        0    11266 2023-04-28 05:28:10.688970 ofscraper-1.83/src/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.83/src/db/queries.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.83/src/interaction/__init__.py
+-rw-r--r--   0        0        0     3169 2023-04-28 05:28:10.688970 ofscraper-1.83/src/interaction/like.py
+-rw-r--r--   0        0        0     5080 2023-04-28 05:28:10.688970 ofscraper-1.83/src/prompts/prompt_functions.py
+-rw-r--r--   0        0        0      359 2023-04-14 18:21:19.249081 ofscraper-1.83/src/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    17909 2023-04-28 11:23:57.457623 ofscraper-1.83/src/prompts/prompts.py
+-rwxr-xr-x   0        0        0    19166 2023-04-28 14:14:09.709648 ofscraper-1.83/src/scraper.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.83/src/utils/__init__.py
+-rw-r--r--   0        0        0     2726 2023-04-28 11:23:57.458623 ofscraper-1.83/src/utils/args.py
+-rw-r--r--   0        0        0     8856 2023-04-28 05:28:10.689970 ofscraper-1.83/src/utils/auth.py
+-rw-r--r--   0        0        0     8874 2023-04-28 11:59:24.168331 ofscraper-1.83/src/utils/config.py
+-rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.83/src/utils/dates.py
+-rw-r--r--   0        0        0    10201 2023-04-29 01:21:35.196542 ofscraper-1.83/src/utils/download.py
+-rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.83/src/utils/encoding.py
+-rw-r--r--   0        0        0     2938 2023-04-28 16:51:38.491314 ofscraper-1.83/src/utils/exit.py
+-rw-r--r--   0        0        0     2795 2023-04-28 14:37:12.121950 ofscraper-1.83/src/utils/paths.py
+-rw-r--r--   0        0        0     2998 2023-04-28 05:28:10.690970 ofscraper-1.83/src/utils/profiles.py
+-rw-r--r--   0        0        0      779 2023-04-28 05:28:10.690970 ofscraper-1.83/src/utils/separate.py
+-rw-r--r--   0        0        0     7009 1970-01-01 00:00:00.000000 ofscraper-1.83/PKG-INFO
```

### Comparing `ofscraper-1.82/LICENSE` & `ofscraper-1.83/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/README.md` & `ofscraper-1.83/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-A fork of onlyfans-scraper. It has been optimized to make it more feature complete with dc's onlyfans script.
+A fork of onlyfans-scraper. It has been optimized to make it more feature complete with digitalcriminal's onlyfans script.
 A matter of fact with the right settings transitioning between the two scripts should be a easy enough process
 
 In addition there are numerous filtering features to control exactly which type of content you want to scrape.
 https://github.com/datawhores/ofscraper/blob/main/CHANGES.md
 
 <h3>DISCLAIMERS:</h3>
 <ol>
     <li>
         This tool is not affiliated, associated, or partnered with OnlyFans in any way. We are not authorized, endorsed, or sponsored by OnlyFans. All OnlyFans trademarks remain the property of Fenix International Limited.
     </li>
     <li>
         This is a theoritical program only and is for educational purposes. If you choose to use it then it may or may not work. You solely accept full responsability and indemnify the creator, hostors, contributors and all other involved persons from any any all responsability.
     </li>
 
- ## 1.82 Changes:
+ ## 1.8x Changes:
  - sync keys names across config(old keys will still work)
   * change username to model_username in metadata
   * change site_name to sitename in metadata
  - remove --purchased args
  - add purchase and pinned as post types
  - add letter-count argument
    * This is for counting letters and not words for
@@ -27,14 +27,17 @@
     * run with poetry run pytest
  - print path for each file
  - responsetype mapping in config
     * This is for example keeping all messages or paid post in same folder, but also allow long time users to keep their current structure
  - added a Post class to serve as a 'single source of truth' for all responsetypes
  - removed unused functions like download_paid that are no longer needed
  - prompts and config functions have been revamped
+ - shutdown handler
+ - removed .tempmedia
+ - added extension to responsetype profile downloads
  - fixed bugs caused by duplicate uploads on pages
  - additional bugs and fixes
 
   ## Description:
   command-line program to download media, and to process other batch operations such as liking and unliking posts.
     
 
@@ -141,15 +144,15 @@
     
 
 # Migrating from DC script
 
 You will need to change the settings so that the metadata option is compatible with your current folders
 Additionally you might want to set the save_path, dir_path, and filename so they output similar outputs
 
-The metadata path from dc's script is used for duplicate check so as long as your set the right path.
+The metadata path from digitalcriminal's script is used for duplicate check so as long as your set the right path.
 Files won't download a second time
 
 https://github.com/datawhores/ofscraper/wiki/Migrating-from-DC-script
 https://github.com/datawhores/ofscraper/wiki/Config-Options
 https://github.com/datawhores/ofscraper/wiki/Customizing-save-path
 
 Ask in the discord or open an issue if you need help with what to change to accomplish this
```

### Comparing `ofscraper-1.82/pyproject.toml` & `ofscraper-1.83/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "1.82"
+version = "1.83"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
```

### Comparing `ofscraper-1.82/src/__init__.py` & `ofscraper-1.83/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/__version__.py` & `ofscraper-1.83/src/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/       
 """
 
 __title__ = 'ofscraper'
-__version__ = '1.82'
+__version__ = '1.83'
 __author__ = 'datawhores'
 __author_email__ = 'datawhores@riseup.net'
 __description__ = 'A command-line program to quickly download,like or unlike posts, and more'
 __url__ = 'https://github.com/datawhores/ofscraper'
 __license__ = 'GNU General Public License v3 or later (GPLv3+)'
 __copyright__ = 'Copyright 2023'
```

### Comparing `ofscraper-1.82/src/api/highlights.py` & `ofscraper-1.83/src/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/api/init.py` & `ofscraper-1.83/src/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/api/me.py` & `ofscraper-1.83/src/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/api/messages.py` & `ofscraper-1.83/src/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/api/paid.py` & `ofscraper-1.83/src/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/api/posts.py` & `ofscraper-1.83/src/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/api/profile.py` & `ofscraper-1.83/src/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/api/subscriptions.py` & `ofscraper-1.83/src/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/api/timeline.py` & `ofscraper-1.83/src/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/constants.py` & `ofscraper-1.83/src/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/db/operations.py` & `ofscraper-1.83/src/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/db/queries.py` & `ofscraper-1.83/src/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/interaction/like.py` & `ofscraper-1.83/src/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/prompts/prompt_functions.py` & `ofscraper-1.83/src/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/prompts/prompts.py` & `ofscraper-1.83/src/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/scraper.py` & `ofscraper-1.83/src/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/utils/args.py` & `ofscraper-1.83/src/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/utils/auth.py` & `ofscraper-1.83/src/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/utils/config.py` & `ofscraper-1.83/src/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/utils/dates.py` & `ofscraper-1.83/src/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/utils/download.py` & `ofscraper-1.83/src/utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,18 +135,18 @@
                         pathlib.Path(temp).unlink(missing_ok=True)
                         with open(temp, 'wb') as f:
                             pathstr=str(path_to_file)
                             bar=tqdm(desc=(pathstr[:50] + '....') if len(pathstr) > 50 else pathstr ,total=total, unit_scale=True, unit_divisor=1024, unit='B', leave=False)
                             num_bytes_downloaded = r.num_bytes_downloaded
                             async for chunk in r.aiter_bytes(chunk_size=1024):
                                 f.write(chunk)
-                                bar.update(
-                                    r.num_bytes_downloaded - num_bytes_downloaded)
-                                num_bytes_downloaded = r.num_bytes_downloaded                           
-                            if pathlib.Path(temp).exists() and  abs(total-pathlib.Path(temp).stat().st_size)<=1000:
+                                bar.update(r.num_bytes_downloaded - num_bytes_downloaded)
+                                num_bytes_downloaded = r.num_bytes_downloaded 
+                                                    
+                            if pathlib.Path(temp).exists() and num_bytes_downloaded==total:
                                 shutil.move(temp,path_to_file)
                                 if ele.postdate:
                                     set_time(path_to_file, convert_local_time(ele.postdate))
                                 if id_:
                                     operations.write_media_table(ele,path_to_file,model_id,username)
                                 return media_type,total
                             else:
```

### Comparing `ofscraper-1.82/src/utils/encoding.py` & `ofscraper-1.83/src/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/utils/exit.py` & `ofscraper-1.83/src/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/utils/paths.py` & `ofscraper-1.83/src/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/utils/profiles.py` & `ofscraper-1.83/src/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/src/utils/separate.py` & `ofscraper-1.83/src/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.82/PKG-INFO` & `ofscraper-1.83/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 1.82
+Version: 1.83
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -25,30 +25,30 @@
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: win32-setctime (>=1.1.0,<2.0.0)
 Requires-Dist: xxhash (>=3.2.0,<4.0.0)
 Project-URL: Homepage, https://github.com/datawhores/ofscraper
 Description-Content-Type: text/markdown
 
-A fork of onlyfans-scraper. It has been optimized to make it more feature complete with dc's onlyfans script.
+A fork of onlyfans-scraper. It has been optimized to make it more feature complete with digitalcriminal's onlyfans script.
 A matter of fact with the right settings transitioning between the two scripts should be a easy enough process
 
 In addition there are numerous filtering features to control exactly which type of content you want to scrape.
 https://github.com/datawhores/ofscraper/blob/main/CHANGES.md
 
 <h3>DISCLAIMERS:</h3>
 <ol>
     <li>
         This tool is not affiliated, associated, or partnered with OnlyFans in any way. We are not authorized, endorsed, or sponsored by OnlyFans. All OnlyFans trademarks remain the property of Fenix International Limited.
     </li>
     <li>
         This is a theoritical program only and is for educational purposes. If you choose to use it then it may or may not work. You solely accept full responsability and indemnify the creator, hostors, contributors and all other involved persons from any any all responsability.
     </li>
 
- ## 1.82 Changes:
+ ## 1.8x Changes:
  - sync keys names across config(old keys will still work)
   * change username to model_username in metadata
   * change site_name to sitename in metadata
  - remove --purchased args
  - add purchase and pinned as post types
  - add letter-count argument
    * This is for counting letters and not words for
@@ -58,14 +58,17 @@
     * run with poetry run pytest
  - print path for each file
  - responsetype mapping in config
     * This is for example keeping all messages or paid post in same folder, but also allow long time users to keep their current structure
  - added a Post class to serve as a 'single source of truth' for all responsetypes
  - removed unused functions like download_paid that are no longer needed
  - prompts and config functions have been revamped
+ - shutdown handler
+ - removed .tempmedia
+ - added extension to responsetype profile downloads
  - fixed bugs caused by duplicate uploads on pages
  - additional bugs and fixes
 
   ## Description:
   command-line program to download media, and to process other batch operations such as liking and unliking posts.
     
 
@@ -172,15 +175,15 @@
     
 
 # Migrating from DC script
 
 You will need to change the settings so that the metadata option is compatible with your current folders
 Additionally you might want to set the save_path, dir_path, and filename so they output similar outputs
 
-The metadata path from dc's script is used for duplicate check so as long as your set the right path.
+The metadata path from digitalcriminal's script is used for duplicate check so as long as your set the right path.
 Files won't download a second time
 
 https://github.com/datawhores/ofscraper/wiki/Migrating-from-DC-script
 https://github.com/datawhores/ofscraper/wiki/Config-Options
 https://github.com/datawhores/ofscraper/wiki/Customizing-save-path
 
 Ask in the discord or open an issue if you need help with what to change to accomplish this
```


# Comparing `tmp/ofscraper-1.84.tar.gz` & `tmp/ofscraper-1.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-1.84.tar", max compression
+gzip compressed data, was "ofscraper-1.85.tar", max compression
```

## Comparing `ofscraper-1.84.tar` & `ofscraper-1.85.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1067 2023-04-13 21:26:07.930007 ofscraper-1.84/LICENSE
--rw-r--r--   0        0        0     5800 2023-04-29 01:50:36.060807 ofscraper-1.84/README.md
--rw-r--r--   0        0        0     1235 2023-04-29 01:54:19.338130 ofscraper-1.84/pyproject.toml
--rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.84/src/__init__.py
--rw-r--r--   0        0        0      733 2023-04-29 01:54:19.338130 ofscraper-1.84/src/__version__.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.84/src/api/__init__.py
--rw-r--r--   0        0        0     2169 2023-04-28 05:28:10.687970 ofscraper-1.84/src/api/highlights.py
--rw-r--r--   0        0        0      838 2023-04-28 05:28:10.687970 ofscraper-1.84/src/api/init.py
--rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.84/src/api/me.py
--rw-r--r--   0        0        0     3580 2023-04-28 05:28:10.687970 ofscraper-1.84/src/api/messages.py
--rw-r--r--   0        0        0     1788 2023-04-28 05:28:10.687970 ofscraper-1.84/src/api/paid.py
--rw-r--r--   0        0        0     7626 2023-04-28 11:23:57.457623 ofscraper-1.84/src/api/posts.py
--rw-r--r--   0        0        0     3247 2023-04-28 05:28:10.687970 ofscraper-1.84/src/api/profile.py
--rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.84/src/api/subscriptions.py
--rw-r--r--   0        0        0     5441 2023-04-28 05:28:10.687970 ofscraper-1.84/src/api/timeline.py
--rw-r--r--   0        0        0     4781 2023-04-28 11:23:57.457623 ofscraper-1.84/src/constants.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.84/src/db/__init__.py
--rw-r--r--   0        0        0    11266 2023-04-28 05:28:10.688970 ofscraper-1.84/src/db/operations.py
--rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.84/src/db/queries.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.84/src/interaction/__init__.py
--rw-r--r--   0        0        0     3169 2023-04-28 05:28:10.688970 ofscraper-1.84/src/interaction/like.py
--rw-r--r--   0        0        0     5080 2023-04-28 05:28:10.688970 ofscraper-1.84/src/prompts/prompt_functions.py
--rw-r--r--   0        0        0      359 2023-04-14 18:21:19.249081 ofscraper-1.84/src/prompts/prompt_strings.py
--rw-r--r--   0        0        0    17909 2023-04-28 11:23:57.457623 ofscraper-1.84/src/prompts/prompts.py
--rwxr-xr-x   0        0        0    19166 2023-04-29 01:50:36.060807 ofscraper-1.84/src/scraper.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.84/src/utils/__init__.py
--rw-r--r--   0        0        0     2726 2023-04-28 11:23:57.458623 ofscraper-1.84/src/utils/args.py
--rw-r--r--   0        0        0     8856 2023-04-28 05:28:10.689970 ofscraper-1.84/src/utils/auth.py
--rw-r--r--   0        0        0     8874 2023-04-28 11:59:24.168331 ofscraper-1.84/src/utils/config.py
--rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.84/src/utils/dates.py
--rw-r--r--   0        0        0    10215 2023-04-29 01:56:03.543214 ofscraper-1.84/src/utils/download.py
--rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.84/src/utils/encoding.py
--rw-r--r--   0        0        0     2938 2023-04-29 01:50:36.061807 ofscraper-1.84/src/utils/exit.py
--rw-r--r--   0        0        0     2795 2023-04-29 01:50:36.061807 ofscraper-1.84/src/utils/paths.py
--rw-r--r--   0        0        0     2998 2023-04-28 05:28:10.690970 ofscraper-1.84/src/utils/profiles.py
--rw-r--r--   0        0        0      779 2023-04-28 05:28:10.690970 ofscraper-1.84/src/utils/separate.py
--rw-r--r--   0        0        0     7009 1970-01-01 00:00:00.000000 ofscraper-1.84/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-13 21:26:07.930007 ofscraper-1.85/LICENSE
+-rw-r--r--   0        0        0     5800 2023-04-29 01:50:36.060807 ofscraper-1.85/README.md
+-rw-r--r--   0        0        0     1235 2023-04-29 17:53:24.975654 ofscraper-1.85/pyproject.toml
+-rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.85/src/__init__.py
+-rw-r--r--   0        0        0      733 2023-04-29 17:53:24.975654 ofscraper-1.85/src/__version__.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.85/src/api/__init__.py
+-rw-r--r--   0        0        0     2169 2023-04-28 05:28:10.687970 ofscraper-1.85/src/api/highlights.py
+-rw-r--r--   0        0        0      838 2023-04-28 05:28:10.687970 ofscraper-1.85/src/api/init.py
+-rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.85/src/api/me.py
+-rw-r--r--   0        0        0     3580 2023-04-28 05:28:10.687970 ofscraper-1.85/src/api/messages.py
+-rw-r--r--   0        0        0     1788 2023-04-28 05:28:10.687970 ofscraper-1.85/src/api/paid.py
+-rw-r--r--   0        0        0     7626 2023-04-28 11:23:57.457623 ofscraper-1.85/src/api/posts.py
+-rw-r--r--   0        0        0     3247 2023-04-28 05:28:10.687970 ofscraper-1.85/src/api/profile.py
+-rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.85/src/api/subscriptions.py
+-rw-r--r--   0        0        0     5441 2023-04-28 05:28:10.687970 ofscraper-1.85/src/api/timeline.py
+-rw-r--r--   0        0        0     4781 2023-04-28 11:23:57.457623 ofscraper-1.85/src/constants.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.85/src/db/__init__.py
+-rw-r--r--   0        0        0    11266 2023-04-28 05:28:10.688970 ofscraper-1.85/src/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.85/src/db/queries.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.85/src/interaction/__init__.py
+-rw-r--r--   0        0        0     3169 2023-04-28 05:28:10.688970 ofscraper-1.85/src/interaction/like.py
+-rw-r--r--   0        0        0     5080 2023-04-28 05:28:10.688970 ofscraper-1.85/src/prompts/prompt_functions.py
+-rw-r--r--   0        0        0      359 2023-04-14 18:21:19.249081 ofscraper-1.85/src/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    17909 2023-04-28 11:23:57.457623 ofscraper-1.85/src/prompts/prompts.py
+-rwxr-xr-x   0        0        0    19166 2023-04-29 01:50:36.060807 ofscraper-1.85/src/scraper.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.85/src/utils/__init__.py
+-rw-r--r--   0        0        0     2726 2023-04-28 11:23:57.458623 ofscraper-1.85/src/utils/args.py
+-rw-r--r--   0        0        0     8856 2023-04-28 05:28:10.689970 ofscraper-1.85/src/utils/auth.py
+-rw-r--r--   0        0        0     8874 2023-04-28 11:59:24.168331 ofscraper-1.85/src/utils/config.py
+-rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.85/src/utils/dates.py
+-rw-r--r--   0        0        0    10256 2023-04-29 17:53:07.287469 ofscraper-1.85/src/utils/download.py
+-rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.85/src/utils/encoding.py
+-rw-r--r--   0        0        0     2938 2023-04-29 01:50:36.061807 ofscraper-1.85/src/utils/exit.py
+-rw-r--r--   0        0        0     2795 2023-04-29 01:50:36.061807 ofscraper-1.85/src/utils/paths.py
+-rw-r--r--   0        0        0     2998 2023-04-28 05:28:10.690970 ofscraper-1.85/src/utils/profiles.py
+-rw-r--r--   0        0        0      779 2023-04-28 05:28:10.690970 ofscraper-1.85/src/utils/separate.py
+-rw-r--r--   0        0        0     7009 1970-01-01 00:00:00.000000 ofscraper-1.85/PKG-INFO
```

### Comparing `ofscraper-1.84/LICENSE` & `ofscraper-1.85/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/README.md` & `ofscraper-1.85/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/pyproject.toml` & `ofscraper-1.85/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "1.84"
+version = "1.85"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
```

### Comparing `ofscraper-1.84/src/__init__.py` & `ofscraper-1.85/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/api/highlights.py` & `ofscraper-1.85/src/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/api/init.py` & `ofscraper-1.85/src/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/api/me.py` & `ofscraper-1.85/src/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/api/messages.py` & `ofscraper-1.85/src/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/api/paid.py` & `ofscraper-1.85/src/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/api/posts.py` & `ofscraper-1.85/src/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/api/profile.py` & `ofscraper-1.85/src/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/api/subscriptions.py` & `ofscraper-1.85/src/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/api/timeline.py` & `ofscraper-1.85/src/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/constants.py` & `ofscraper-1.85/src/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/db/operations.py` & `ofscraper-1.85/src/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/db/queries.py` & `ofscraper-1.85/src/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/interaction/like.py` & `ofscraper-1.85/src/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/prompts/prompt_functions.py` & `ofscraper-1.85/src/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/prompts/prompts.py` & `ofscraper-1.85/src/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/scraper.py` & `ofscraper-1.85/src/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/utils/args.py` & `ofscraper-1.85/src/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/utils/auth.py` & `ofscraper-1.85/src/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/utils/config.py` & `ofscraper-1.85/src/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/utils/dates.py` & `ofscraper-1.85/src/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/utils/download.py` & `ofscraper-1.85/src/utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,16 +139,16 @@
                             pathstr=str(path_to_file)
                             bar=tqdm(desc=(pathstr[:50] + '....') if len(pathstr) > 50 else pathstr ,total=total, unit_scale=True, unit_divisor=1024, unit='B', leave=False)
                             num_bytes_downloaded = r.num_bytes_downloaded
                             async for chunk in r.aiter_bytes(chunk_size=1024):
                                 f.write(chunk)
                                 bar.update(r.num_bytes_downloaded - num_bytes_downloaded)
                                 num_bytes_downloaded = r.num_bytes_downloaded 
-                                                    
-                        if pathlib.Path(temp).exists() and num_bytes_downloaded==total:
+                        int("ddsd")                          
+                        if pathlib.Path(temp).exists() and abs(total-pathlib.Path(temp).absolute.stat().st_size)<=-500:
                             shutil.move(temp,path_to_file)
                             if ele.postdate:
                                 set_time(path_to_file, convert_local_time(ele.postdate))
                             if id_:
                                 operations.write_media_table(ele,path_to_file,model_id,username)
                             return media_type,total
                         else:
```

### Comparing `ofscraper-1.84/src/utils/encoding.py` & `ofscraper-1.85/src/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/utils/exit.py` & `ofscraper-1.85/src/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/utils/paths.py` & `ofscraper-1.85/src/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/utils/profiles.py` & `ofscraper-1.85/src/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/src/utils/separate.py` & `ofscraper-1.85/src/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.84/PKG-INFO` & `ofscraper-1.85/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 1.84
+Version: 1.85
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```


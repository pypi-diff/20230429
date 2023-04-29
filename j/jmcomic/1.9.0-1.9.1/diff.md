# Comparing `tmp/jmcomic-1.9.0.tar.gz` & `tmp/jmcomic-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-74i2wywx/jmcomic-1.9.0.tar", last modified: Thu Apr 27 12:09:06 2023, max compression
+gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-dzo_jz90/jmcomic-1.9.1.tar", last modified: Sat Apr 29 05:41:16 2023, max compression
```

## Comparing `jmcomic-1.9.0.tar` & `jmcomic-1.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:09:06.000000 jmcomic-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-27 12:08:57.000000 jmcomic-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-27 12:09:06.000000 jmcomic-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-27 12:08:57.000000 jmcomic-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 12:09:06.000000 jmcomic-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-27 12:08:57.000000 jmcomic-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:09:06.000000 jmcomic-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:09:06.000000 jmcomic-1.9.0/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 12:08:57.000000 jmcomic-1.9.0/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-27 12:08:57.000000 jmcomic-1.9.0/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-04-27 12:08:57.000000 jmcomic-1.9.0/src/jmcomic/jm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-27 12:08:57.000000 jmcomic-1.9.0/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-27 12:08:57.000000 jmcomic-1.9.0/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-04-27 12:08:57.000000 jmcomic-1.9.0/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-04-27 12:08:57.000000 jmcomic-1.9.0/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:09:06.000000 jmcomic-1.9.0/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-27 12:09:06.000000 jmcomic-1.9.0/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-27 12:09:06.000000 jmcomic-1.9.0/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:09:06.000000 jmcomic-1.9.0/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 12:09:06.000000 jmcomic-1.9.0/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 12:09:06.000000 jmcomic-1.9.0/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:41:16.000000 jmcomic-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-29 05:41:07.000000 jmcomic-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-29 05:41:16.000000 jmcomic-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-29 05:41:07.000000 jmcomic-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 05:41:16.000000 jmcomic-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-29 05:41:07.000000 jmcomic-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-29 05:41:07.000000 jmcomic-1.9.1/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-29 05:41:07.000000 jmcomic-1.9.1/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-04-29 05:41:07.000000 jmcomic-1.9.1/src/jmcomic/jm_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-29 05:41:07.000000 jmcomic-1.9.1/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-29 05:41:07.000000 jmcomic-1.9.1/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-04-29 05:41:07.000000 jmcomic-1.9.1/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-04-29 05:41:07.000000 jmcomic-1.9.1/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-1.9.0/LICENSE` & `jmcomic-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-1.9.0/PKG-INFO` & `jmcomic-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-1.9.0/README.md` & `jmcomic-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-1.9.0/setup.py` & `jmcomic-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.9.0/src/jmcomic/api.py` & `jmcomic-1.9.1/src/jmcomic/api.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.9.0/src/jmcomic/jm_client.py` & `jmcomic-1.9.1/src/jmcomic/jm_client.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.9.0/src/jmcomic/jm_config.py` & `jmcomic-1.9.1/src/jmcomic/jm_config.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.9.0/src/jmcomic/jm_entity.py` & `jmcomic-1.9.1/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.9.0/src/jmcomic/jm_option.py` & `jmcomic-1.9.1/src/jmcomic/jm_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,17 @@
     Bd_Title_Id_Image = 3
 
     # 根目录 / Photo标题 / 图片文件
     Bd_Title_Image = 4
     # 根目录 / Photo号 / 图片文件
     Bd_Id_Image = 5
 
+    # 根目录 / AlbumId / Photo序号 / 图片文件
+    Bd_Id_Index_image = 6  # 禁漫网站的默认下载方式
+
     AdditionalHandler = Callable[
         ['DownloadDirTree', Optional[JmAlbumDetail], JmPhotoDetail],
         str
     ]
     additional_tree_flag_handler_mapping: Dict[int, AdditionalHandler] = {}
 
     dsl_support = {
@@ -159,14 +162,18 @@
 
         elif flag in (4, 5):
             # 根目录 / Photo标题 / 图片文件
             # 根目录 / Photo号 / 图片文件
 
             return dirpath(None, photo_dir(4))
 
+        elif flag == 6:
+            # 根目录 / AlbumId / Photo序号 / 图片文件
+            return dirpath(photo.album_id, str(photo.album_index))
+
         else:
             if flag in self.additional_tree_flag_handler_mapping:
                 return self.additional_tree_flag_handler_mapping[flag](self, album, photo)
             else:
                 raise NotImplementedError
 
     @staticmethod
```

### Comparing `jmcomic-1.9.0/src/jmcomic/jm_toolkit.py` & `jmcomic-1.9.1/src/jmcomic/jm_toolkit.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.9.0/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-1.9.1/src/jmcomic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```


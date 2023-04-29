# Comparing `tmp/TsProject-1.0.3.tar.gz` & `tmp/TsProject-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TsProject-1.0.3.tar", last modified: Sat Apr 29 11:29:42 2023, max compression
+gzip compressed data, was "TsProject-1.0.4.tar", last modified: Sat Apr 29 11:59:22 2023, max compression
```

## Comparing `TsProject-1.0.3.tar` & `TsProject-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 11:29:42.792353 TsProject-1.0.3/
--rw-rw-rw-   0        0        0     1113 2023-04-29 11:29:42.792353 TsProject-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-04-29 08:09:39.000000 TsProject-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 11:29:42.789840 TsProject-1.0.3/TsProject.egg-info/
--rw-rw-rw-   0        0        0     1113 2023-04-29 11:29:42.000000 TsProject-1.0.3/TsProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-04-29 11:29:42.000000 TsProject-1.0.3/TsProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 11:29:42.000000 TsProject-1.0.3/TsProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-29 11:29:42.000000 TsProject-1.0.3/TsProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 11:29:42.000000 TsProject-1.0.3/TsProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      130 2023-04-29 11:28:28.000000 TsProject-1.0.3/__init__.py
--rw-rw-rw-   0        0        0     1000 2023-04-29 11:05:48.000000 TsProject-1.0.3/_core.py
--rw-rw-rw-   0        0        0       42 2023-04-29 11:29:42.793356 TsProject-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2488 2023-04-29 11:29:18.000000 TsProject-1.0.3/setup.py
--rw-rw-rw-   0        0        0       17 2023-04-29 11:28:32.000000 TsProject-1.0.3/test.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:59:22.575888 TsProject-1.0.4/
+-rw-rw-rw-   0        0        0       17 2023-04-29 11:59:06.000000 TsProject-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      508 2023-04-29 11:59:22.574893 TsProject-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-04-29 08:09:39.000000 TsProject-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 11:59:22.572894 TsProject-1.0.4/TsProject.egg-info/
+-rw-rw-rw-   0        0        0      508 2023-04-29 11:59:22.000000 TsProject-1.0.4/TsProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-04-29 11:59:22.000000 TsProject-1.0.4/TsProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:59:22.000000 TsProject-1.0.4/TsProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-29 11:59:22.000000 TsProject-1.0.4/TsProject.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-29 11:59:22.000000 TsProject-1.0.4/TsProject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:59:22.000000 TsProject-1.0.4/TsProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-29 11:59:22.000000 TsProject-1.0.4/TsProject.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      130 2023-04-29 11:28:28.000000 TsProject-1.0.4/__init__.py
+-rw-rw-rw-   0        0        0     1001 2023-04-29 11:47:33.000000 TsProject-1.0.4/_core.py
+-rw-rw-rw-   0        0        0       42 2023-04-29 11:59:22.575888 TsProject-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     4004 2023-04-29 11:58:35.000000 TsProject-1.0.4/setup.py
+-rw-rw-rw-   0        0        0       17 2023-04-29 11:51:24.000000 TsProject-1.0.4/test.py
```

### Comparing `TsProject-1.0.3/_core.py` & `TsProject-1.0.4/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # @Time : 2023/04/29 16:12
 # @Author : Kqy
-# @Version : 1.0.1
+# @Version : 1.0.3
 # @Website : https://www.tsginkgo.cn/
 
 
 import os, requests;
 
 # Edit The Lambda
 def TSFileUploadPost(FilePath=None, UploaderKey=None, Description=None):    # Def Post Lambda
@@ -14,15 +14,15 @@
     """
     if (os.path.getsize(FilePath)>52428800):
         return {"code": -1, "error": f'文件{FilePath}超过最大大小限制50MB！'};
 
     UploadUrl = "https://www.tsginkgo.cn/file-uploader/api/upload/public/";
 
     try:
-        data = {'UploaderKey': UploaderKey, 'Description':Description}; # Post Data
+        data = {'UploaderKey': UploaderKey, 'Description': Description}; # Post Data
         files = {'file': open(FilePath, 'rb')};  # Post File
         res = requests.post(UploadUrl, data=data, files=files).text;    # Get Post  
         return {"code": 0, "res": res};  # Return Result
     except Exception as e:
         return {"code": -1, "error": str(e)};
 
 # if "__name__" == "__main__":
```


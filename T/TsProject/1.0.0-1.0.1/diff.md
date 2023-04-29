# Comparing `tmp/TsProject-1.0.0.tar.gz` & `tmp/TsProject-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TsProject-1.0.0.tar", last modified: Sat Apr 29 08:26:33 2023, max compression
+gzip compressed data, was "TsProject-1.0.1.tar", last modified: Sat Apr 29 08:33:27 2023, max compression
```

## Comparing `TsProject-1.0.0.tar` & `TsProject-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 08:26:33.322268 TsProject-1.0.0/
--rw-rw-rw-   0        0        0     1113 2023-04-29 08:26:33.322268 TsProject-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-04-29 08:09:39.000000 TsProject-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 08:26:33.320268 TsProject-1.0.0/TsProject.egg-info/
--rw-rw-rw-   0        0        0     1113 2023-04-29 08:26:33.000000 TsProject-1.0.0/TsProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-29 08:26:33.000000 TsProject-1.0.0/TsProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 08:26:33.000000 TsProject-1.0.0/TsProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-29 08:26:33.000000 TsProject-1.0.0/TsProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 08:26:33.000000 TsProject-1.0.0/TsProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 08:26:33.323269 TsProject-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2381 2023-04-29 08:26:25.000000 TsProject-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 08:33:27.233223 TsProject-1.0.1/
+-rw-rw-rw-   0        0        0     1113 2023-04-29 08:33:27.232224 TsProject-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-04-29 08:09:39.000000 TsProject-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 08:33:27.230223 TsProject-1.0.1/TsProject.egg-info/
+-rw-rw-rw-   0        0        0     1113 2023-04-29 08:33:27.000000 TsProject-1.0.1/TsProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-29 08:33:27.000000 TsProject-1.0.1/TsProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 08:33:27.000000 TsProject-1.0.1/TsProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-29 08:33:27.000000 TsProject-1.0.1/TsProject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 08:33:27.000000 TsProject-1.0.1/TsProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 08:33:27.233223 TsProject-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2381 2023-04-29 08:33:20.000000 TsProject-1.0.1/setup.py
```

### Comparing `TsProject-1.0.0/PKG-INFO` & `TsProject-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TsProject
-Version: 1.0.0
+Version: 1.0.1
 Summary: TsProject Init: File POST to Cloud
 Home-page: https://www.tsginkgo.cn/about
 Author: Kqy
 Author-email: 2765301200@qq.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://www.tsginkgo.cn
 Project-URL: Funding, https://www.tsginkgo.cn
```

### Comparing `TsProject-1.0.0/TsProject.egg-info/PKG-INFO` & `TsProject-1.0.1/TsProject.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TsProject
-Version: 1.0.0
+Version: 1.0.1
 Summary: TsProject Init: File POST to Cloud
 Home-page: https://www.tsginkgo.cn/about
 Author: Kqy
 Author-email: 2765301200@qq.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://www.tsginkgo.cn
 Project-URL: Funding, https://www.tsginkgo.cn
```

### Comparing `TsProject-1.0.0/setup.py` & `TsProject-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
  
     name="TsProject",  # Required 项目名称
-    version="1.0.0",  # Required 发布版本号
+    version="1.0.1",  # Required 发布版本号
     description="TsProject Init: File POST to Cloud",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://www.tsginkgo.cn/about",  # Optional github项目地址
     author="Kqy",  # Optional 作者
     author_email="2765301200@qq.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
```


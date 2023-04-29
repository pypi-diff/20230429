# Comparing `tmp/TsProject-1.0.5.tar.gz` & `tmp/TsProject-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TsProject-1.0.5.tar", last modified: Sat Apr 29 12:19:09 2023, max compression
+gzip compressed data, was "TsProject-1.0.6.tar", last modified: Sat Apr 29 13:23:20 2023, max compression
```

## Comparing `TsProject-1.0.5.tar` & `TsProject-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 12:19:09.559096 TsProject-1.0.5/
--rw-rw-rw-   0        0        0       17 2023-04-29 11:59:06.000000 TsProject-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      566 2023-04-29 12:19:09.558105 TsProject-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       92 2023-04-29 12:15:24.000000 TsProject-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 12:19:09.541603 TsProject-1.0.5/TsProject/
--rw-rw-rw-   0        0        0        0 2023-04-29 12:16:15.000000 TsProject-1.0.5/TsProject/__init__.py
--rw-rw-rw-   0        0        0     1005 2023-04-29 12:17:50.000000 TsProject-1.0.5/TsProject/post.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:19:09.556106 TsProject-1.0.5/TsProject.egg-info/
--rw-rw-rw-   0        0        0      566 2023-04-29 12:19:09.000000 TsProject-1.0.5/TsProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-29 12:19:09.000000 TsProject-1.0.5/TsProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 12:19:09.000000 TsProject-1.0.5/TsProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-29 12:19:09.000000 TsProject-1.0.5/TsProject.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-29 12:19:09.000000 TsProject-1.0.5/TsProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-29 12:19:09.000000 TsProject-1.0.5/TsProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-29 12:19:09.000000 TsProject-1.0.5/TsProject.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-29 12:19:09.559096 TsProject-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     4170 2023-04-29 12:18:41.000000 TsProject-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:23:20.121132 TsProject-1.0.6/
+-rw-rw-rw-   0        0        0       17 2023-04-29 11:59:06.000000 TsProject-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      566 2023-04-29 13:23:20.120142 TsProject-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2023-04-29 12:15:24.000000 TsProject-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 13:23:20.101282 TsProject-1.0.6/TsProject/
+-rw-rw-rw-   0        0        0      400 2023-04-29 13:21:40.000000 TsProject-1.0.6/TsProject/TsExtra.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 12:28:22.000000 TsProject-1.0.6/TsProject/TsINIT.txt
+-rw-rw-rw-   0        0        0     3238 2023-04-29 13:22:59.000000 TsProject-1.0.6/TsProject/TsPost.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 12:16:15.000000 TsProject-1.0.6/TsProject/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:23:20.118135 TsProject-1.0.6/TsProject.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-04-29 13:23:19.000000 TsProject-1.0.6/TsProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-29 13:23:20.000000 TsProject-1.0.6/TsProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 13:23:19.000000 TsProject-1.0.6/TsProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-29 13:23:20.000000 TsProject-1.0.6/TsProject.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-29 13:23:20.000000 TsProject-1.0.6/TsProject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-29 13:23:20.000000 TsProject-1.0.6/TsProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-29 13:23:19.000000 TsProject-1.0.6/TsProject.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-29 13:23:20.121132 TsProject-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     4232 2023-04-29 13:23:04.000000 TsProject-1.0.6/setup.py
```

### Comparing `TsProject-1.0.5/PKG-INFO` & `TsProject-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TsProject
-Version: 1.0.5
+Version: 1.0.6
 Summary: TsProject Init: File POST to Cloud
 Home-page: https://www.tsginkgo.cn
 Author: Kqy
 Author-email: 2765301200@qq.com
 License: MIT
 Project-URL: Bug Reports, https://www.tsginkgo.cn
 Project-URL: Funding, https://www.tsginkgo.cn
```

### Comparing `TsProject-1.0.5/TsProject.egg-info/PKG-INFO` & `TsProject-1.0.6/TsProject.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TsProject
-Version: 1.0.5
+Version: 1.0.6
 Summary: TsProject Init: File POST to Cloud
 Home-page: https://www.tsginkgo.cn
 Author: Kqy
 Author-email: 2765301200@qq.com
 License: MIT
 Project-URL: Bug Reports, https://www.tsginkgo.cn
 Project-URL: Funding, https://www.tsginkgo.cn
```

### Comparing `TsProject-1.0.5/setup.py` & `TsProject-1.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="TsProject",
-    version="1.0.5",
+    version="1.0.6",
     keywords=['Tsginkgo', 'Ksuser', 'Kqy'],
     description="TsProject Init: File POST to Cloud",
     long_description=long_description,
     license="MIT",
     url="https://www.tsginkgo.cn",
     author="Kqy",
     author_email="2765301200@qq.com",
@@ -106,7 +106,11 @@
     project_urls={  # Optional 和项目相关的 其他网页连接资源
         "Bug Reports": "https://www.tsginkgo.cn",
         "Funding": "https://www.tsginkgo.cn",
         "Say Thanks!": "https://www.tsginkgo.cn",
         "Source": "https://www.tsginkgo.cn/about",
     },
 )
+
+
+# python setup.py sdist bdist_wheel
+# twine upload dist/*
```


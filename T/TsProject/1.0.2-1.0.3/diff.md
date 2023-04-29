# Comparing `tmp/TsProject-1.0.2.tar.gz` & `tmp/TsProject-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TsProject-1.0.2.tar", last modified: Sat Apr 29 11:08:34 2023, max compression
+gzip compressed data, was "TsProject-1.0.3.tar", last modified: Sat Apr 29 11:29:42 2023, max compression
```

## Comparing `TsProject-1.0.2.tar` & `TsProject-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 11:08:34.590737 TsProject-1.0.2/
--rw-rw-rw-   0        0        0     1113 2023-04-29 11:08:34.589666 TsProject-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-04-29 08:09:39.000000 TsProject-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 11:08:34.586657 TsProject-1.0.2/TsProject.egg-info/
--rw-rw-rw-   0        0        0     1113 2023-04-29 11:08:34.000000 TsProject-1.0.2/TsProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-29 11:08:34.000000 TsProject-1.0.2/TsProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 11:08:34.000000 TsProject-1.0.2/TsProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-29 11:08:34.000000 TsProject-1.0.2/TsProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 11:08:34.000000 TsProject-1.0.2/TsProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 11:08:34.590737 TsProject-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2433 2023-04-29 11:07:30.000000 TsProject-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:29:42.792353 TsProject-1.0.3/
+-rw-rw-rw-   0        0        0     1113 2023-04-29 11:29:42.792353 TsProject-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-04-29 08:09:39.000000 TsProject-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 11:29:42.789840 TsProject-1.0.3/TsProject.egg-info/
+-rw-rw-rw-   0        0        0     1113 2023-04-29 11:29:42.000000 TsProject-1.0.3/TsProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-04-29 11:29:42.000000 TsProject-1.0.3/TsProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:29:42.000000 TsProject-1.0.3/TsProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-29 11:29:42.000000 TsProject-1.0.3/TsProject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:29:42.000000 TsProject-1.0.3/TsProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      130 2023-04-29 11:28:28.000000 TsProject-1.0.3/__init__.py
+-rw-rw-rw-   0        0        0     1000 2023-04-29 11:05:48.000000 TsProject-1.0.3/_core.py
+-rw-rw-rw-   0        0        0       42 2023-04-29 11:29:42.793356 TsProject-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2488 2023-04-29 11:29:18.000000 TsProject-1.0.3/setup.py
+-rw-rw-rw-   0        0        0       17 2023-04-29 11:28:32.000000 TsProject-1.0.3/test.py
```

### Comparing `TsProject-1.0.2/PKG-INFO` & `TsProject-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TsProject
-Version: 1.0.2
+Version: 1.0.3
 Summary: TsProject Init: File POST to Cloud
 Home-page: https://www.tsginkgo.cn/about
 Author: Kqy
 Author-email: 2765301200@qq.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://www.tsginkgo.cn
 Project-URL: Funding, https://www.tsginkgo.cn
```

### Comparing `TsProject-1.0.2/TsProject.egg-info/PKG-INFO` & `TsProject-1.0.3/TsProject.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TsProject
-Version: 1.0.2
+Version: 1.0.3
 Summary: TsProject Init: File POST to Cloud
 Home-page: https://www.tsginkgo.cn/about
 Author: Kqy
 Author-email: 2765301200@qq.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://www.tsginkgo.cn
 Project-URL: Funding, https://www.tsginkgo.cn
```

### Comparing `TsProject-1.0.2/setup.py` & `TsProject-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
  
     name="TsProject",  # Required 项目名称
-    version="1.0.2",  # Required 发布版本号
+    version="1.0.3",  # Required 发布版本号
     description="TsProject Init: File POST to Cloud",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://www.tsginkgo.cn/about",  # Optional github项目地址
     author="Kqy",  # Optional 作者
     author_email="2765301200@qq.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
@@ -41,15 +41,16 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
    
     keywords="Tsginkgo, Ksuser, Kqy",  # Optional 搜索关键字
  
     
-    packages=find_packages(),  # Required
+    # packages=find_packages(""),  # Required
+    packages=[''],
    
     python_requires=">=3.7, <4",  # python 版本要求
  
     install_requires=["requests"],  # Optional 第三方依赖库
    
     project_urls={  # Optional 和项目相关的 其他网页连接资源
         "Bug Reports": "https://www.tsginkgo.cn",
@@ -57,8 +58,9 @@
         "Say Thanks!": "https://www.tsginkgo.cn",
         "Source": "https://www.tsginkgo.cn/about",
     },
 )
 
 
 # python setup.py sdist
+# python setup.py bdist_wheel
 # twine upload dist/*
```


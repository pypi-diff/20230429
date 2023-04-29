# Comparing `tmp/je_load_density_dev-0.0.8.tar.gz` & `tmp/je_load_density_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\je_load_density_dev-0.0.8.tar", last modified: Fri Apr 29 07:45:05 2022, max compression
+gzip compressed data, was "dist\je_load_density_dev-0.0.9.tar", last modified: Wed Jun  1 08:46:45 2022, max compression
```

## Comparing `je_load_density_dev-0.0.8.tar` & `je_load_density_dev-0.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/
--rw-rw-rw-   0        0        0     1085 2022-02-16 16:26:47.000000 je_load_density_dev-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1149 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      654 2022-04-22 18:56:31.000000 je_load_density_dev-0.0.8/README.md
--rw-rw-rw-   0        0        0      797 2022-04-29 07:45:04.000000 je_load_density_dev-0.0.8/dev_setup.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/
--rw-rw-rw-   0        0        0      943 2022-04-29 05:47:13.000000 je_load_density_dev-0.0.8/je_load_density/__init__.py
--rw-rw-rw-   0        0        0     1139 2022-04-22 18:00:17.000000 je_load_density_dev-0.0.8/je_load_density/__main__.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/utils/
--rw-rw-rw-   0        0        0        2 2022-04-14 17:19:55.000000 je_load_density_dev-0.0.8/je_load_density/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/utils/exception/
--rw-rw-rw-   0        0        0       47 2022-04-22 18:00:18.000000 je_load_density_dev-0.0.8/je_load_density/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      389 2022-04-23 16:57:42.000000 je_load_density_dev-0.0.8/je_load_density/utils/exception/exception.py
--rw-rw-rw-   0        0        0      474 2022-04-23 16:59:15.000000 je_load_density_dev-0.0.8/je_load_density/utils/exception/exception_tag.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/utils/executor/
--rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_load_density_dev-0.0.8/je_load_density/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     2130 2022-04-29 05:44:10.000000 je_load_density_dev-0.0.8/je_load_density/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/utils/file_process/
--rw-rw-rw-   0        0        0        0 2022-04-06 14:25:38.000000 je_load_density_dev-0.0.8/je_load_density/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      301 2022-04-29 05:42:25.000000 je_load_density_dev-0.0.8/je_load_density/utils/file_process/create_project_structure.py
--rw-rw-rw-   0        0        0      711 2022-04-13 06:06:05.000000 je_load_density_dev-0.0.8/je_load_density/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/utils/get_data_strcture/
--rw-rw-rw-   0        0        0        2 2022-03-12 10:53:49.000000 je_load_density_dev-0.0.8/je_load_density/utils/get_data_strcture/__init__.py
--rw-rw-rw-   0        0        0     1578 2022-04-28 14:46:01.000000 je_load_density_dev-0.0.8/je_load_density/utils/get_data_strcture/get_api_data.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/utils/html_report/
--rw-rw-rw-   0        0        0        0 2022-04-24 08:19:36.000000 je_load_density_dev-0.0.8/je_load_density/utils/html_report/__init__.py
--rw-rw-rw-   0        0        0     6789 2022-04-29 07:44:55.000000 je_load_density_dev-0.0.8/je_load_density/utils/html_report/html_report_generate.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/utils/json/
--rw-rw-rw-   0        0        0        0 2022-03-13 22:28:06.000000 je_load_density_dev-0.0.8/je_load_density/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/utils/json/json_file/
--rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_load_density_dev-0.0.8/je_load_density/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1326 2022-04-29 05:47:13.000000 je_load_density_dev-0.0.8/je_load_density/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/utils/json/json_format/
--rw-rw-rw-   0        0        0        2 2022-03-12 10:53:49.000000 je_load_density_dev-0.0.8/je_load_density/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1169 2022-04-29 05:57:34.000000 je_load_density_dev-0.0.8/je_load_density/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/utils/test_record/
--rw-rw-rw-   0        0        0        0 2022-03-07 01:22:48.000000 je_load_density_dev-0.0.8/je_load_density/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0      340 2022-03-25 17:42:29.000000 je_load_density_dev-0.0.8/je_load_density/utils/test_record/record_test_result_class.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/wrapper/
--rw-rw-rw-   0        0        0       39 2022-04-22 18:00:17.000000 je_load_density_dev-0.0.8/je_load_density/wrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/wrapper/env_with_user/
--rw-rw-rw-   0        0        0        0 2022-04-15 10:11:14.000000 je_load_density_dev-0.0.8/je_load_density/wrapper/env_with_user/__init__.py
--rw-rw-rw-   0        0        0      935 2022-04-26 14:33:53.000000 je_load_density_dev-0.0.8/je_load_density/wrapper/env_with_user/wrapper_env_and_user.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/wrapper/locust_as_library/
--rw-rw-rw-   0        0        0       57 2022-04-22 18:00:17.000000 je_load_density_dev-0.0.8/je_load_density/wrapper/locust_as_library/__init__.py
--rw-rw-rw-   0        0        0     3332 2022-04-29 06:04:45.000000 je_load_density_dev-0.0.8/je_load_density/wrapper/locust_as_library/locust_as_library.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density/wrapper/locust_template/
--rw-rw-rw-   0        0        0        0 2022-04-14 17:19:55.000000 je_load_density_dev-0.0.8/je_load_density/wrapper/locust_template/__init__.py
--rw-rw-rw-   0        0        0     3925 2022-04-29 06:15:57.000000 je_load_density_dev-0.0.8/je_load_density/wrapper/locust_template/http_user_with_api_testka.py
-drwxrwxrwx   0        0        0        0 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density_dev.egg-info/
--rw-rw-rw-   0        0        0     1149 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1690 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/je_load_density_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-04-29 07:45:05.000000 je_load_density_dev-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      789 2022-04-29 07:27:32.000000 je_load_density_dev-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:45.000000 je_load_density_dev-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1332 2022-06-01 08:46:45.000000 je_load_density_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      837 2022-06-01 08:03:32.000000 je_load_density_dev-0.0.9/README.md
+-rw-rw-rw-   0        0        0      797 2022-06-01 08:37:10.000000 je_load_density_dev-0.0.9/dev_setup.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/
+-rw-rw-rw-   0        0        0      943 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/__init__.py
+-rw-rw-rw-   0        0        0     1139 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/__main__.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/utils/
+-rw-rw-rw-   0        0        0        2 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/utils/exception/
+-rw-rw-rw-   0        0        0       47 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      389 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/exception/exception.py
+-rw-rw-rw-   0        0        0      474 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/exception/exception_tag.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/utils/executor/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     2269 2022-06-01 08:01:40.000000 je_load_density_dev-0.0.9/je_load_density/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      303 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/file_process/create_project_structure.py
+-rw-rw-rw-   0        0        0      711 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/utils/get_data_strcture/
+-rw-rw-rw-   0        0        0        2 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/get_data_strcture/__init__.py
+-rw-rw-rw-   0        0        0     1578 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/get_data_strcture/get_api_data.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/utils/html_report/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/html_report/__init__.py
+-rw-rw-rw-   0        0        0     6846 2022-05-31 08:20:19.000000 je_load_density_dev-0.0.9/je_load_density/utils/html_report/html_report_generate.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/utils/json/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1310 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1169 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0      359 2022-05-31 08:20:19.000000 je_load_density_dev-0.0.9/je_load_density/utils/test_record/test_record_class.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/wrapper/
+-rw-rw-rw-   0        0        0       39 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/wrapper/env_with_user/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/wrapper/env_with_user/__init__.py
+-rw-rw-rw-   0        0        0      935 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/wrapper/env_with_user/wrapper_env_and_user.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/wrapper/locust_as_library/
+-rw-rw-rw-   0        0        0       57 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/wrapper/locust_as_library/__init__.py
+-rw-rw-rw-   0        0        0     3357 2022-05-31 08:20:19.000000 je_load_density_dev-0.0.9/je_load_density/wrapper/locust_as_library/locust_as_library.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density/wrapper/locust_template/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/wrapper/locust_template/__init__.py
+-rw-rw-rw-   0        0        0     3925 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/je_load_density/wrapper/locust_template/http_user_with_api_testka.py
+drwxrwxrwx   0        0        0        0 2022-06-01 08:46:45.000000 je_load_density_dev-0.0.9/je_load_density_dev.egg-info/
+-rw-rw-rw-   0        0        0     1332 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1683 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2022-06-01 08:46:44.000000 je_load_density_dev-0.0.9/je_load_density_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-06-01 08:46:45.000000 je_load_density_dev-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      789 2022-05-06 19:46:08.000000 je_load_density_dev-0.0.9/setup.py
```

### Comparing `je_load_density_dev-0.0.8/LICENSE` & `je_load_density_dev-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `je_load_density_dev-0.0.8/PKG-INFO` & `je_load_density_dev-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_load_density_dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/JE-Chen/LoadTesting
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
@@ -35,8 +35,21 @@
 
 ## install 
 
 ```
 pip install je_locust_wrapper
 ```
 
+## require
+
+```
+python 3.7 or later  
+```
+
+* Test on
+    * windows 10 ~ 11
+    * osx 10.5 ~ 11 big sur
+    * ubuntu 20.0.4
+    * raspberry pi 3B+
+
+| All test in test dir
```

### Comparing `je_load_density_dev-0.0.8/dev_setup.py` & `je_load_density_dev-0.0.9/dev_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as README:
     long_description = README.read()
 
 setuptools.setup(
     name="je_load_density_dev",
-    version="0.0.08",
+    version="0.0.09",
     author="JE-Chen",
     author_email="zenmailman@gmail.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JE-Chen/LoadTesting",
     packages=setuptools.find_packages(),
```

### Comparing `je_load_density_dev-0.0.8/je_load_density/__init__.py` & `je_load_density_dev-0.0.9/je_load_density/__init__.py`

 * *Files identical despite different names*

### Comparing `je_load_density_dev-0.0.8/je_load_density/__main__.py` & `je_load_density_dev-0.0.9/je_load_density/__main__.py`

 * *Files identical despite different names*

### Comparing `je_load_density_dev-0.0.8/je_load_density/utils/executor/action_executor.py` & `je_load_density_dev-0.0.9/je_load_density/utils/executor/action_executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,18 +35,21 @@
     :return: recode string, response as list
     """
     execute_record_string = ""
     event_response_list = []
     try:
         if len(action_list) > 0 or type(action_list) is not list:
             for action in action_list:
-                event_response = _execute_event(action)
-                print("execute: ", str(action))
-                execute_record_string = "".join(execute_record_string)
-                event_response_list.append(event_response)
+                try:
+                    event_response = _execute_event(action)
+                    print("execute: ", str(action))
+                    execute_record_string = "".join(execute_record_string)
+                    event_response_list.append(event_response)
+                except Exception as error:
+                    print(repr(error), file=sys.stderr)
         else:
             raise JELoadingTestExecuteException(executor_list_error)
         return execute_record_string, event_response_list
     except Exception as error:
         print(repr(error), file=sys.stderr)
```

### Comparing `je_load_density_dev-0.0.8/je_load_density/utils/file_process/get_dir_file_list.py` & `je_load_density_dev-0.0.9/je_load_density/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `je_load_density_dev-0.0.8/je_load_density/utils/get_data_strcture/get_api_data.py` & `je_load_density_dev-0.0.9/je_load_density/utils/get_data_strcture/get_api_data.py`

 * *Files identical despite different names*

### Comparing `je_load_density_dev-0.0.8/je_load_density/utils/html_report/html_report_generate.py` & `je_load_density_dev-0.0.9/je_load_density/utils/html_report/html_report_generate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 
-from je_load_density.utils.test_record.record_test_result_class import test_record
+from je_load_density.utils.test_record.test_record_class import test_record_instance
 from je_load_density.utils.exception.exception import HTMLException
 from je_load_density.utils.exception.exception_tag import html_generate_no_data_tag
 from threading import Lock
 
 _lock = Lock()
 
 _html_string_head = \
@@ -163,35 +163,35 @@
 
 def generate_html(html_name: str = "default_name"):
     """
     format html_string and output html file
     :param html_name: save html file name
     :return: html_string
     """
-    if len(test_record.record_list) == 0 and len(test_record.error_record_list) == 0:
+    if len(test_record_instance.test_record_list) == 0 and len(test_record_instance.error_record_list) == 0:
         raise HTMLException(html_generate_no_data_tag)
     else:
         success_list = list()
-        for record_data in test_record.record_list:
+        for record_data in test_record_instance.test_record_list:
             success_list.append(
                 _success_table.format(
                     Method=record_data.get("http_method"),
                     test_url=record_data.get("test_url"),
                     name=record_data.get("name"),
                     status_code=record_data.get("status_code"),
                     text=record_data.get("text"),
                     content=record_data.get("content"),
                     headers=record_data.get("headers"),
                 )
             )
         failure_list = list()
-        if len(test_record.error_record_list) == 0:
+        if len(test_record_instance.error_record_list) == 0:
             pass
         else:
-            for record_data in test_record.error_record_list:
+            for record_data in test_record_instance.error_record_list:
                 failure_list.append(
                     _failure_table.format(
                         http_method=record_data[0].get("http_method"),
                         test_url=record_data[0].get("test_url"),
                         name=record_data[0].get("name"),
                         status_code=record_data[0].get("status_code"),
                         error=record_data[0].get("error"),
```

### Comparing `je_load_density_dev-0.0.8/je_load_density/utils/json/json_file/json_file.py` & `je_load_density_dev-0.0.9/je_load_density/utils/json/json_file/json_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import os.path
 from pathlib import Path
 from threading import Lock
 
 from je_load_density.utils.exception.exception import JELoadingTestJsonException
 from je_load_density.utils.exception.exception_tag import cant_find_json_error
 from je_load_density.utils.exception.exception_tag import cant_save_json_error
```

### Comparing `je_load_density_dev-0.0.8/je_load_density/utils/json/json_format/json_process.py` & `je_load_density_dev-0.0.9/je_load_density/utils/json/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_load_density_dev-0.0.8/je_load_density/wrapper/env_with_user/wrapper_env_and_user.py` & `je_load_density_dev-0.0.9/je_load_density/wrapper/env_with_user/wrapper_env_and_user.py`

 * *Files identical despite different names*

### Comparing `je_load_density_dev-0.0.8/je_load_density/wrapper/locust_as_library/locust_as_library.py` & `je_load_density_dev-0.0.9/je_load_density/wrapper/locust_as_library/locust_as_library.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import gevent
 from locust.env import Environment
 from locust.stats import stats_printer, stats_history
 from locust.log import setup_logging
 from locust import User
 from locust import events
 
-from je_load_density.utils.test_record.record_test_result_class import test_record
+from je_load_density.utils.test_record.test_record_class import test_record_instance
 
 setup_logging("INFO", None)
 
 
 @events.request.add_listener
 def handle_request(request_type, name, response_time, response_length, response,
                    context, exception, start_time, url, **kwargs):
@@ -24,25 +24,25 @@
     :param exception: default request event value
     :param start_time: default request event value
     :param url: default request event value
     :param kwargs: catch some unknown param
     :return: None
     """
     if exception:
-        test_record.error_record_list.append(
+        test_record_instance.error_record_list.append(
                 {
                     "http_method": request_type,
                     "test_url": url,
                     "name": name,
                     "status_code": response.status_code,
                     "error": exception
                  }
         )
     else:
-        test_record.record_list.append(
+        test_record_instance.test_record_list.append(
                 {
                     "http_method": request_type,
                     "test_url": url,
                     "name": name,
                     "status_code": response.status_code,
                     "text": response.text,
                     "content": response.content,
```

### Comparing `je_load_density_dev-0.0.8/je_load_density/wrapper/locust_template/http_user_with_api_testka.py` & `je_load_density_dev-0.0.9/je_load_density/wrapper/locust_template/http_user_with_api_testka.py`

 * *Files identical despite different names*

### Comparing `je_load_density_dev-0.0.8/je_load_density_dev.egg-info/PKG-INFO` & `je_load_density_dev-0.0.9/je_load_density_dev.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-load-density-dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/JE-Chen/LoadTesting
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
@@ -35,8 +35,21 @@
 
 ## install 
 
 ```
 pip install je_locust_wrapper
 ```
 
+## require
+
+```
+python 3.7 or later  
+```
+
+* Test on
+    * windows 10 ~ 11
+    * osx 10.5 ~ 11 big sur
+    * ubuntu 20.0.4
+    * raspberry pi 3B+
+
+| All test in test dir
```

### Comparing `je_load_density_dev-0.0.8/je_load_density_dev.egg-info/SOURCES.txt` & `je_load_density_dev-0.0.9/je_load_density_dev.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 je_load_density/utils/html_report/html_report_generate.py
 je_load_density/utils/json/__init__.py
 je_load_density/utils/json/json_file/__init__.py
 je_load_density/utils/json/json_file/json_file.py
 je_load_density/utils/json/json_format/__init__.py
 je_load_density/utils/json/json_format/json_process.py
 je_load_density/utils/test_record/__init__.py
-je_load_density/utils/test_record/record_test_result_class.py
+je_load_density/utils/test_record/test_record_class.py
 je_load_density/wrapper/__init__.py
 je_load_density/wrapper/env_with_user/__init__.py
 je_load_density/wrapper/env_with_user/wrapper_env_and_user.py
 je_load_density/wrapper/locust_as_library/__init__.py
 je_load_density/wrapper/locust_as_library/locust_as_library.py
 je_load_density/wrapper/locust_template/__init__.py
 je_load_density/wrapper/locust_template/http_user_with_api_testka.py
```

### Comparing `je_load_density_dev-0.0.8/setup.py` & `je_load_density_dev-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as README:
     long_description = README.read()
 
 setuptools.setup(
     name="je_load_density",
-    version="0.0.06",
+    version="0.0.07",
     author="JE-Chen",
     author_email="zenmailman@gmail.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JE-Chen/LoadTesting",
     packages=setuptools.find_packages(),
```


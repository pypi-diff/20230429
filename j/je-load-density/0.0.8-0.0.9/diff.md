# Comparing `tmp/je_load_density-0.0.8.tar.gz` & `tmp/je_load_density-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\je_load_density-0.0.8.tar", last modified: Wed Jun  1 09:00:59 2022, max compression
+gzip compressed data, was "dist\je_load_density-0.0.9.tar", last modified: Sun Jun 26 22:49:43 2022, max compression
```

## Comparing `je_load_density-0.0.8.tar` & `je_load_density-0.0.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:59.000000 je_load_density-0.0.8/
--rw-rw-rw-   0        0        0     1085 2022-05-06 19:46:08.000000 je_load_density-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1328 2022-06-01 09:00:59.000000 je_load_density-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      837 2022-06-01 08:03:32.000000 je_load_density-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:58.000000 je_load_density-0.0.8/je_load_density/
--rw-rw-rw-   0        0        0      943 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/__init__.py
--rw-rw-rw-   0        0        0     1139 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/__main__.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:58.000000 je_load_density-0.0.8/je_load_density/utils/
--rw-rw-rw-   0        0        0        2 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:59.000000 je_load_density-0.0.8/je_load_density/utils/exception/
--rw-rw-rw-   0        0        0       47 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      389 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/exception/exception.py
--rw-rw-rw-   0        0        0      474 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/exception/exception_tag.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:59.000000 je_load_density-0.0.8/je_load_density/utils/executor/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     2269 2022-06-01 08:01:40.000000 je_load_density-0.0.8/je_load_density/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:59.000000 je_load_density-0.0.8/je_load_density/utils/file_process/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      303 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/file_process/create_project_structure.py
--rw-rw-rw-   0        0        0      711 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:59.000000 je_load_density-0.0.8/je_load_density/utils/get_data_strcture/
--rw-rw-rw-   0        0        0        2 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/get_data_strcture/__init__.py
--rw-rw-rw-   0        0        0     1578 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/get_data_strcture/get_api_data.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:59.000000 je_load_density-0.0.8/je_load_density/utils/html_report/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/html_report/__init__.py
--rw-rw-rw-   0        0        0     6846 2022-05-31 08:20:19.000000 je_load_density-0.0.8/je_load_density/utils/html_report/html_report_generate.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:59.000000 je_load_density-0.0.8/je_load_density/utils/json/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:59.000000 je_load_density-0.0.8/je_load_density/utils/json/json_file/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1310 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:59.000000 je_load_density-0.0.8/je_load_density/utils/json/json_format/
--rw-rw-rw-   0        0        0        2 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1169 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:59.000000 je_load_density-0.0.8/je_load_density/utils/test_record/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0      359 2022-05-31 08:20:19.000000 je_load_density-0.0.8/je_load_density/utils/test_record/test_record_class.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:59.000000 je_load_density-0.0.8/je_load_density/wrapper/
--rw-rw-rw-   0        0        0       39 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/wrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:59.000000 je_load_density-0.0.8/je_load_density/wrapper/env_with_user/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/wrapper/env_with_user/__init__.py
--rw-rw-rw-   0        0        0      935 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/wrapper/env_with_user/wrapper_env_and_user.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:59.000000 je_load_density-0.0.8/je_load_density/wrapper/locust_as_library/
--rw-rw-rw-   0        0        0       57 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/wrapper/locust_as_library/__init__.py
--rw-rw-rw-   0        0        0     3357 2022-05-31 08:20:19.000000 je_load_density-0.0.8/je_load_density/wrapper/locust_as_library/locust_as_library.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:59.000000 je_load_density-0.0.8/je_load_density/wrapper/locust_template/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/wrapper/locust_template/__init__.py
--rw-rw-rw-   0        0        0     3925 2022-05-06 19:46:08.000000 je_load_density-0.0.8/je_load_density/wrapper/locust_template/http_user_with_api_testka.py
-drwxrwxrwx   0        0        0        0 2022-06-01 09:00:58.000000 je_load_density-0.0.8/je_load_density.egg-info/
--rw-rw-rw-   0        0        0     1328 2022-06-01 09:00:58.000000 je_load_density-0.0.8/je_load_density.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1650 2022-06-01 09:00:58.000000 je_load_density-0.0.8/je_load_density.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-01 09:00:58.000000 je_load_density-0.0.8/je_load_density.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-06-01 09:00:58.000000 je_load_density-0.0.8/je_load_density.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-06-01 09:00:58.000000 je_load_density-0.0.8/je_load_density.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-01 09:00:59.000000 je_load_density-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      789 2022-06-01 09:00:57.000000 je_load_density-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2022-05-06 19:46:08.000000 je_load_density-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1850 2022-06-26 22:49:43.000000 je_load_density-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1359 2022-06-21 01:57:31.000000 je_load_density-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/
+-rw-rw-rw-   0        0        0      914 2022-06-26 16:30:42.000000 je_load_density-0.0.9/je_load_density/__init__.py
+-rw-rw-rw-   0        0        0     1139 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/__main__.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/utils/
+-rw-rw-rw-   0        0        0        2 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/utils/exception/
+-rw-rw-rw-   0        0        0       47 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      389 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/exception/exception.py
+-rw-rw-rw-   0        0        0      474 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/exception/exception_tag.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/utils/executor/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     2808 2022-06-26 16:25:35.000000 je_load_density-0.0.9/je_load_density/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      303 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/file_process/create_project_structure.py
+-rw-rw-rw-   0        0        0      711 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/utils/get_data_strcture/
+-rw-rw-rw-   0        0        0        2 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/get_data_strcture/__init__.py
+-rw-rw-rw-   0        0        0     1578 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/get_data_strcture/get_api_data.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/utils/html_report/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/html_report/__init__.py
+-rw-rw-rw-   0        0        0     6846 2022-05-31 08:20:19.000000 je_load_density-0.0.9/je_load_density/utils/html_report/html_report_generate.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/utils/json/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1310 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1169 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0      359 2022-05-31 08:20:19.000000 je_load_density-0.0.9/je_load_density/utils/test_record/test_record_class.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/wrapper/
+-rw-rw-rw-   0        0        0       39 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/wrapper/env_with_user/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/wrapper/env_with_user/__init__.py
+-rw-rw-rw-   0        0        0      935 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/wrapper/env_with_user/wrapper_env_and_user.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/wrapper/locust_as_library/
+-rw-rw-rw-   0        0        0       57 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/wrapper/locust_as_library/__init__.py
+-rw-rw-rw-   0        0        0     3357 2022-05-31 08:20:19.000000 je_load_density-0.0.9/je_load_density/wrapper/locust_as_library/locust_as_library.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density/wrapper/locust_template/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/wrapper/locust_template/__init__.py
+-rw-rw-rw-   0        0        0     3925 2022-05-06 19:46:08.000000 je_load_density-0.0.9/je_load_density/wrapper/locust_template/http_user_with_api_testka.py
+drwxrwxrwx   0        0        0        0 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density.egg-info/
+-rw-rw-rw-   0        0        0     1850 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1650 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2022-06-26 22:49:43.000000 je_load_density-0.0.9/je_load_density.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-06-26 22:49:43.000000 je_load_density-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      789 2022-06-26 22:49:42.000000 je_load_density-0.0.9/setup.py
```

### Comparing `je_load_density-0.0.8/LICENSE` & `je_load_density-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `je_load_density-0.0.8/PKG-INFO` & `je_load_density-0.0.9/je_load_density.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: je_load_density
-Version: 0.0.8
+Name: je-load-density
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/JE-Chen/LoadTesting
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
@@ -22,15 +22,21 @@
 
 #### Features
 * HTTP HTTPS stress testing and load testing
 * Action FIle
 * response compare
 * CLI with action file
 ---
-[![CircleCI](https://circleci.com/gh/JE-Chen/JE_LocustWrapper/tree/main.svg?style=svg)](https://circleci.com/gh/JE-Chen/JE_LocustWrapper/tree/main)
+
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/JE-Chen/LoadDensity/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/JE-Chen/LoadDensity/tree/main)
+
+[![LoadDensity GitHub Actions Dev](https://github.com/JE-Chen/LoadDensity/actions/workflows/load-density-github-actions_dev.yml/badge.svg)](https://github.com/JE-Chen/LoadDensity/actions/workflows/load-density-github-actions_dev.yml)
+
+[![LoadDensity GitHub Actions Stable](https://github.com/JE-Chen/LoadDensity/actions/workflows/load-density-github-actions_stable.yml/badge.svg)](https://github.com/JE-Chen/LoadDensity/actions/workflows/load-density-github-actions_stable.yml)
+
 ### Documentation
 [![Documentation Status](https://readthedocs.org/projects/loaddensity/badge/?version=latest)](https://loaddensity.readthedocs.io/en/latest/?badge=latest)
 
 https://loaddensity.readthedocs.io/en/latest/
 ---
 
 ## install
```

### Comparing `je_load_density-0.0.8/je_load_density/__init__.py` & `je_load_density-0.0.9/je_load_density/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # start
 from je_load_density.wrapper.locust_as_library.locust_as_library import start_test
 from je_load_density.wrapper.env_with_user.wrapper_env_and_user import loading_test_with_user
 
 # executor
 from je_load_density.utils.executor.action_executor import execute_action
 from je_load_density.utils.executor.action_executor import execute_files
+from je_load_density.utils.executor.action_executor import executor
 # file
 from je_load_density.utils.file_process.get_dir_file_list import get_dir_files_as_list
 # report
 from je_load_density.utils.html_report.html_report_generate import generate_html
 
-# the dict use can update
-from je_load_density.utils.executor.action_executor import event_dict
```

### Comparing `je_load_density-0.0.8/je_load_density/__main__.py` & `je_load_density-0.0.9/je_load_density/__main__.py`

 * *Files identical despite different names*

### Comparing `je_load_density-0.0.8/je_load_density/utils/executor/action_executor.py` & `je_load_density-0.0.9/je_load_density/utils/executor/action_executor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,77 @@
 import sys
+from typing import Tuple
 
 from je_load_density.utils.exception.exception import JELoadingTestExecuteException
-from je_load_density.wrapper.env_with_user.wrapper_env_and_user import loading_test_with_user
 from je_load_density.utils.exception.exception_tag import executor_data_error
 from je_load_density.utils.exception.exception_tag import executor_list_error
 from je_load_density.utils.json.json_file.json_file import read_action_json
+from je_load_density.wrapper.env_with_user.wrapper_env_and_user import loading_test_with_user
+
 
+class Executor(object):
 
-event_dict = {
-    "loading_test_with_user": loading_test_with_user,
-}
-
-
-def _execute_event(action: list):
-    """
-    :param action: execute action
-    :return: what event return
-    """
-    event = event_dict.get(action[0])
-    if len(action) == 2:
-        return event(**action[1])
-    else:
-        raise JELoadingTestExecuteException(executor_data_error)
-
-
-def execute_action(action_list: list):
-    """
-    :param action_list: like this structure
-    [
-        ["method on event_dict", {"param": params}],
-        ["method on event_dict", {"param": params}]
-    ]
-    for loop and use execute_event function to execute
-    :return: recode string, response as list
-    """
-    execute_record_string = ""
-    event_response_list = []
-    try:
-        if len(action_list) > 0 or type(action_list) is not list:
-            for action in action_list:
-                try:
-                    event_response = _execute_event(action)
-                    print("execute: ", str(action))
-                    execute_record_string = "".join(execute_record_string)
-                    event_response_list.append(event_response)
-                except Exception as error:
-                    print(repr(error), file=sys.stderr)
+    def __init__(self):
+        self.event_dict = {
+            "loading_test_with_user": loading_test_with_user,
+        }
+
+    def _execute_event(self, action: list):
+        """
+        :param action: execute action
+        :return: what event return
+        """
+        event = self.event_dict.get(action[0])
+        if len(action) == 2:
+            return event(**action[1])
         else:
-            raise JELoadingTestExecuteException(executor_list_error)
+            raise JELoadingTestExecuteException(executor_data_error)
+
+    def execute_action(self, action_list: list) -> Tuple[str, list]:
+        """
+        :param action_list: like this structure
+        [
+            ["method on event_dict", {"param": params}],
+            ["method on event_dict", {"param": params}]
+        ]
+        for loop and use execute_event function to execute
+        :return: recode string, response as list
+        """
+        execute_record_string = ""
+        event_response_list = []
+        try:
+            if len(action_list) > 0 or type(action_list) is list:
+                pass
+            else:
+                raise JELoadingTestExecuteException(executor_list_error)
+        except Exception as error:
+            print(repr(error), file=sys.stderr)
+        for action in action_list:
+            try:
+                event_response = self._execute_event(action)
+                print("execute: ", str(action))
+                execute_record_string = "".join(execute_record_string)
+                event_response_list.append(event_response)
+            except Exception as error:
+                print(repr(error), file=sys.stderr)
         return execute_record_string, event_response_list
-    except Exception as error:
-        print(repr(error), file=sys.stderr)
+
+    def execute_files(self, execute_files_list: list):
+        """
+        :param execute_files_list: list include execute files path
+        :return: every execute detail as list
+        """
+        execute_detail_list = list()
+        for file in execute_files_list:
+            execute_detail_list.append(self.execute_action(read_action_json(file)))
+        return execute_detail_list
+
+
+executor = Executor()
+
+
+def execute_action(action_list: list) -> Tuple[str, list]:
+    return executor.execute_action(action_list)
 
 
-def execute_files(execute_files_list: list):
-    """
-    :param execute_files_list: list include execute files path
-    :return: every execute detail as list
-    """
-    execute_detail_list = list()
-    for file in execute_files_list:
-        execute_detail_list.append(execute_action(read_action_json(file)))
-    return execute_detail_list
+def execute_files(execute_files_list: list) -> list:
+    return executor.execute_files(execute_files_list)
```

### Comparing `je_load_density-0.0.8/je_load_density/utils/file_process/get_dir_file_list.py` & `je_load_density-0.0.9/je_load_density/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `je_load_density-0.0.8/je_load_density/utils/get_data_strcture/get_api_data.py` & `je_load_density-0.0.9/je_load_density/utils/get_data_strcture/get_api_data.py`

 * *Files identical despite different names*

### Comparing `je_load_density-0.0.8/je_load_density/utils/html_report/html_report_generate.py` & `je_load_density-0.0.9/je_load_density/utils/html_report/html_report_generate.py`

 * *Files identical despite different names*

### Comparing `je_load_density-0.0.8/je_load_density/utils/json/json_file/json_file.py` & `je_load_density-0.0.9/je_load_density/utils/json/json_file/json_file.py`

 * *Files identical despite different names*

### Comparing `je_load_density-0.0.8/je_load_density/utils/json/json_format/json_process.py` & `je_load_density-0.0.9/je_load_density/utils/json/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_load_density-0.0.8/je_load_density/wrapper/env_with_user/wrapper_env_and_user.py` & `je_load_density-0.0.9/je_load_density/wrapper/env_with_user/wrapper_env_and_user.py`

 * *Files identical despite different names*

### Comparing `je_load_density-0.0.8/je_load_density/wrapper/locust_as_library/locust_as_library.py` & `je_load_density-0.0.9/je_load_density/wrapper/locust_as_library/locust_as_library.py`

 * *Files identical despite different names*

### Comparing `je_load_density-0.0.8/je_load_density/wrapper/locust_template/http_user_with_api_testka.py` & `je_load_density-0.0.9/je_load_density/wrapper/locust_template/http_user_with_api_testka.py`

 * *Files identical despite different names*

### Comparing `je_load_density-0.0.8/je_load_density.egg-info/PKG-INFO` & `je_load_density-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: je-load-density
-Version: 0.0.8
+Name: je_load_density
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/JE-Chen/LoadTesting
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
@@ -22,15 +22,21 @@
 
 #### Features
 * HTTP HTTPS stress testing and load testing
 * Action FIle
 * response compare
 * CLI with action file
 ---
-[![CircleCI](https://circleci.com/gh/JE-Chen/JE_LocustWrapper/tree/main.svg?style=svg)](https://circleci.com/gh/JE-Chen/JE_LocustWrapper/tree/main)
+
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/JE-Chen/LoadDensity/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/JE-Chen/LoadDensity/tree/main)
+
+[![LoadDensity GitHub Actions Dev](https://github.com/JE-Chen/LoadDensity/actions/workflows/load-density-github-actions_dev.yml/badge.svg)](https://github.com/JE-Chen/LoadDensity/actions/workflows/load-density-github-actions_dev.yml)
+
+[![LoadDensity GitHub Actions Stable](https://github.com/JE-Chen/LoadDensity/actions/workflows/load-density-github-actions_stable.yml/badge.svg)](https://github.com/JE-Chen/LoadDensity/actions/workflows/load-density-github-actions_stable.yml)
+
 ### Documentation
 [![Documentation Status](https://readthedocs.org/projects/loaddensity/badge/?version=latest)](https://loaddensity.readthedocs.io/en/latest/?badge=latest)
 
 https://loaddensity.readthedocs.io/en/latest/
 ---
 
 ## install
```

### Comparing `je_load_density-0.0.8/je_load_density.egg-info/SOURCES.txt` & `je_load_density-0.0.9/je_load_density.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_load_density-0.0.8/setup.py` & `je_load_density-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as README:
     long_description = README.read()
 
 setuptools.setup(
     name="je_load_density",
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


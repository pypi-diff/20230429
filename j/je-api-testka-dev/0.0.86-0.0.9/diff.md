# Comparing `tmp/je_api_testka_dev-0.0.86.tar.gz` & `tmp/je_api_testka_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_api_testka_dev-0.0.86.tar", last modified: Sat Apr 29 10:41:08 2023, max compression
+gzip compressed data, was "dist\je_api_testka_dev-0.0.9.tar", last modified: Sat Mar 12 10:59:14 2022, max compression
```

## Comparing `je_api_testka_dev-0.0.86.tar` & `je_api_testka_dev-0.0.9.tar`

### file list

```diff
@@ -1,79 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.703219 je_api_testka_dev-0.0.86/
--rw-rw-rw-   0        0        0     2798 2023-04-29 10:41:08.703219 je_api_testka_dev-0.0.86/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2023-04-29 10:38:01.000000 je_api_testka_dev-0.0.86/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.612462 je_api_testka_dev-0.0.86/je_api_testka/
--rw-rw-rw-   0        0        0     2845 2023-04-21 12:29:52.000000 je_api_testka_dev-0.0.86/je_api_testka/__init__.py
--rw-rw-rw-   0        0        0     2349 2023-04-26 11:14:38.000000 je_api_testka_dev-0.0.86/je_api_testka/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.616451 je_api_testka_dev-0.0.86/je_api_testka/requests_wrapper/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/requests_wrapper/__init__.py
--rw-rw-rw-   0        0        0     5026 2023-04-18 12:51:28.000000 je_api_testka_dev-0.0.86/je_api_testka/requests_wrapper/request_method.py
--rw-rw-rw-   0        0        0     2615 2023-04-18 12:51:28.000000 je_api_testka_dev-0.0.86/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.617448 je_api_testka_dev-0.0.86/je_api_testka/utils/
--rw-rw-rw-   0        0        0        2 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.620441 je_api_testka_dev-0.0.86/je_api_testka/utils/assert_result/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/assert_result/__init__.py
--rw-rw-rw-   0        0        0      981 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/assert_result/result_check.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.623432 je_api_testka_dev-0.0.86/je_api_testka/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     3483 2023-04-22 14:19:05.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.627422 je_api_testka_dev-0.0.86/je_api_testka/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-04-21 12:29:52.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0     2392 2023-04-21 12:29:52.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.629416 je_api_testka_dev-0.0.86/je_api_testka/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     5366 2023-04-21 12:29:52.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.632408 je_api_testka_dev-0.0.86/je_api_testka/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      709 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.639389 je_api_testka_dev-0.0.86/je_api_testka/utils/generate_report/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/generate_report/__init__.py
--rw-rw-rw-   0        0        0     8977 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/generate_report/html_report_generate.py
--rw-rw-rw-   0        0        0     3966 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/generate_report/json_report.py
--rw-rw-rw-   0        0        0     1637 2023-04-18 12:51:28.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/generate_report/xml_report.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.642382 je_api_testka_dev-0.0.86/je_api_testka/utils/get_data_strcture/
--rw-rw-rw-   0        0        0        2 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/get_data_strcture/__init__.py
--rw-rw-rw-   0        0        0     1588 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/get_data_strcture/get_api_data.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.643379 je_api_testka_dev-0.0.86/je_api_testka/utils/json/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.646372 je_api_testka_dev-0.0.86/je_api_testka/utils/json/json_file/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1337 2023-04-14 12:58:39.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.649363 je_api_testka_dev-0.0.86/je_api_testka/utils/json/json_format/
--rw-rw-rw-   0        0        0        2 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1286 2023-04-18 12:51:28.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.652355 je_api_testka_dev-0.0.86/je_api_testka/utils/mock_server/
--rw-rw-rw-   0        0        0        0 2023-04-20 12:43:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/mock_server/__init__.py
--rw-rw-rw-   0        0        0     1445 2023-04-21 12:29:52.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/mock_server/flask_mock_server.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.655347 je_api_testka_dev-0.0.86/je_api_testka/utils/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-05 13:27:19.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3280 2023-04-18 12:51:28.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.657341 je_api_testka_dev-0.0.86/je_api_testka/utils/project/
--rw-rw-rw-   0        0        0        0 2023-04-18 12:51:28.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/project/__init__.py
--rw-rw-rw-   0        0        0     2982 2023-04-18 12:51:28.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/project/create_project_structure.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.662328 je_api_testka_dev-0.0.86/je_api_testka/utils/project/template/
--rw-rw-rw-   0        0        0        0 2023-04-18 12:51:28.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/project/template/__init__.py
--rw-rw-rw-   0        0        0      633 2023-04-18 12:51:28.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/project/template/template_executor.py
--rw-rw-rw-   0        0        0      633 2023-04-18 12:51:28.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/project/template/template_keyword.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.665321 je_api_testka_dev-0.0.86/je_api_testka/utils/socket_server/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/socket_server/__init__.py
--rw-rw-rw-   0        0        0     2465 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/socket_server/api_testka_socket_server.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.668312 je_api_testka_dev-0.0.86/je_api_testka/utils/test_record/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0      381 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/test_record/test_record_class.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.670308 je_api_testka_dev-0.0.86/je_api_testka/utils/xml/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.672302 je_api_testka_dev-0.0.86/je_api_testka/utils/xml/change_xml_structure/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/xml/change_xml_structure/__init__.py
--rw-rw-rw-   0        0        0     2498 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.677289 je_api_testka_dev-0.0.86/je_api_testka/utils/xml/xml_file/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2424 2023-04-02 11:29:16.000000 je_api_testka_dev-0.0.86/je_api_testka/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:41:08.701225 je_api_testka_dev-0.0.86/je_api_testka_dev.egg-info/
--rw-rw-rw-   0        0        0     2798 2023-04-29 10:41:08.000000 je_api_testka_dev-0.0.86/je_api_testka_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2455 2023-04-29 10:41:08.000000 je_api_testka_dev-0.0.86/je_api_testka_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:41:08.000000 je_api_testka_dev-0.0.86/je_api_testka_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-29 10:41:08.000000 je_api_testka_dev-0.0.86/je_api_testka_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-29 10:41:08.000000 je_api_testka_dev-0.0.86/je_api_testka_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      937 2023-04-29 10:40:49.000000 je_api_testka_dev-0.0.86/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 10:41:08.704216 je_api_testka_dev-0.0.86/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      930 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/README.md
+-rw-rw-rw-   0        0        0      966 2022-03-12 10:59:10.000000 je_api_testka_dev-0.0.9/dev_setup.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/
+-rw-rw-rw-   0        0        0     2866 2022-03-07 01:22:48.000000 je_api_testka_dev-0.0.9/je_api_testka/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/record/
+-rw-rw-rw-   0        0        0        0 2022-03-07 01:22:48.000000 je_api_testka_dev-0.0.9/je_api_testka/record/__init__.py
+-rw-rw-rw-   0        0        0      258 2022-03-07 01:22:48.000000 je_api_testka_dev-0.0.9/je_api_testka/record/record.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/requests_wrapper/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/requests_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     3134 2022-03-11 09:34:19.000000 je_api_testka_dev-0.0.9/je_api_testka/requests_wrapper/request_method.py
+-rw-rw-rw-   0        0        0     1294 2022-03-02 15:06:29.000000 je_api_testka_dev-0.0.9/je_api_testka/requests_wrapper/requests_data_structure.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/
+-rw-rw-rw-   0        0        0       35 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/assert_result/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:52:53.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/assert_result/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/exception/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     2754 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/exception/api_test_eceptions_tag.py
+-rw-rw-rw-   0        0        0     1906 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/exception/api_test_exceptions.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/execute_action/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/execute_action/__init__.py
+-rw-rw-rw-   0        0        0     1159 2022-03-12 09:24:21.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/execute_action/action_executor.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/get_data_strcture/
+-rw-rw-rw-   0        0        0        2 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/get_data_strcture/__init__.py
+-rw-rw-rw-   0        0        0     1063 2022-03-11 13:13:40.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/get_data_strcture/get_api_data.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/
+-rw-rw-rw-   0        0        0       40 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1324 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1046 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_search/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_search/__init__.py
+-rw-rw-rw-   0        0        0     1084 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_search/json_search.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/xml_file/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/xml_file/__init__.py
+-rw-rw-rw-   0        0        0     2480 2022-03-02 15:06:29.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/xml_file/xml_file.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/
+-rw-rw-rw-   0        0        0      930 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1378 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      958 2022-03-11 16:12:43.000000 je_api_testka_dev-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `je_api_testka_dev-0.0.86/je_api_testka/utils/json/json_file/json_file.py` & `je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_file/json_file.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 import json
 from pathlib import Path
 from threading import Lock
 
-from je_api_testka.utils.exception.exception_tags import cant_find_json_error
-from je_api_testka.utils.exception.exception_tags import cant_save_json_error
-from je_api_testka.utils.exception.exceptions import APITesterJsonException
+from je_api_testka.utils.exception.api_test_exceptions import APITesterJsonException
+from je_api_testka.utils.exception.api_test_eceptions_tag import api_test_cant_find_json_error
+from je_api_testka.utils.exception.api_test_eceptions_tag import api_test_cant_save_json_error
 
 lock = Lock()
 
 
 def read_action_json(json_file_path: str):
     """
-    read the action json
     :param json_file_path json file's path to read
     """
     try:
         lock.acquire()
         file_path = Path(json_file_path)
         if file_path.exists() and file_path.is_file():
             with open(json_file_path) as read_file:
-                return json.load(read_file)
+                return read_file.read()
     except APITesterJsonException:
-        raise APITesterJsonException(cant_find_json_error)
+        raise APITesterJsonException(api_test_cant_find_json_error)
     finally:
         lock.release()
 
 
-def write_action_json(json_save_path: str, action_json: list):
+def write_action_json(json_save_path: str, action_json: str):
     """
-    write action json
     :param json_save_path  json save path
     :param action_json the json str include action to write
     """
     try:
         lock.acquire()
         with open(json_save_path, "w+") as file_to_write:
-            file_to_write.write(json.dumps(action_json, indent=4))
+            file_to_write.write(action_json)
     except APITesterJsonException:
-        raise APITesterJsonException(cant_save_json_error)
+        raise APITesterJsonException(api_test_cant_save_json_error)
     finally:
         lock.release()
+
```

### Comparing `je_api_testka_dev-0.0.86/je_api_testka/utils/xml/xml_file/xml_file.py` & `je_api_testka_dev-0.0.9/je_api_testka/utils/xml/xml_file/xml_file.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,63 @@
 import xml.dom.minidom
 from xml.etree import ElementTree
-
-from je_api_testka.utils.exception.exception_tags import cant_read_xml_error
-from je_api_testka.utils.exception.exception_tags import xml_type_error
-from je_api_testka.utils.exception.exceptions import APITesterXMLException
-from je_api_testka.utils.exception.exceptions import APITesterXMLTypeException
+from xml.dom.minidom import parse
+from xml.dom.minidom import parseString
+from xml.dom import minidom
+
+from je_api_testka.utils.exception.api_test_eceptions_tag import api_test_cant_read_xml_error
+from je_api_testka.utils.exception.api_test_eceptions_tag import api_test_xml_type_error
+from je_api_testka.utils.exception.api_test_exceptions import APITesterXMLException
+from je_api_testka.utils.exception.api_test_exceptions import APITesterXMLTypeException
 
 
 def reformat_xml_file(xml_string: str):
     dom = xml.dom.minidom.parseString(xml_string)
     return dom.toprettyxml()
 
 
 class XMLParser(object):
 
-    def __init__(self, xml_string: str, xml_type: str = "string"):
-        """
-        :param xml_string: full xml string
-        :param xml_type: file or string
-        """
+    def __init__(self, xml_string: str, xml_type: str):
         self.element_tree = ElementTree
         self.tree = None
         self.xml_root = None
         self.xml_from_type = "string"
         self.xml_string = xml_string.strip()
         xml_type = xml_type.lower()
         if xml_type not in ["file", "string"]:
-            raise APITesterXMLTypeException(xml_type_error)
+            raise APITesterXMLTypeException(api_test_xml_type_error)
         if xml_type == "string":
             self.xml_parser_from_string()
         else:
             self.xml_parser_from_file()
 
     def xml_parser_from_string(self, **kwargs):
-        """
-        :param kwargs: any another param
-        :return: xml root element tree
-        """
         try:
             self.xml_root = ElementTree.fromstring(self.xml_string, **kwargs)
         except APITesterXMLException:
-            raise APITesterXMLException(cant_read_xml_error)
+            raise APITesterXMLException(api_test_cant_read_xml_error)
         return self.xml_root
 
     def xml_parser_from_file(self, **kwargs):
-        """
-        :param kwargs: any another param
-        :return: xml root element tree
-        """
         try:
             self.tree = ElementTree.parse(self.xml_string, **kwargs)
         except APITesterXMLException:
-            raise APITesterXMLException(cant_read_xml_error)
+            raise APITesterXMLException(api_test_cant_read_xml_error)
         self.xml_root = self.tree.getroot()
         self.xml_from_type = "file"
         return self.xml_root
 
+    def find_tag(self, tag_name: [str, None] = None):
+        if self.xml_from_type == "string":
+            return self.xml_root.iter(tag_name)
+        else:
+            return self.tree.iter(tag_name)
+
+    def xml_iterparse(self, xml_string: str, **kwargs):
+        return self.element_tree.iterparse(xml_string, **kwargs)
+
     def write_xml(self, write_xml_filename: str, write_content: str):
-        """
-        :param write_xml_filename:  xml file name
-        :param write_content: content to write
-        """
         write_content = write_content.strip()
         content = self.element_tree.fromstring(write_content)
         tree = self.element_tree.ElementTree(content)
         tree.write(write_xml_filename, encoding="utf-8")
```


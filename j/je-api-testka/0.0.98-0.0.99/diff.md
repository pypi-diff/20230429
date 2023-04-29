# Comparing `tmp/je_api_testka-0.0.98.tar.gz` & `tmp/je_api_testka-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_api_testka-0.0.98.tar", last modified: Thu Apr 13 01:59:43 2023, max compression
+gzip compressed data, was "je_api_testka-0.0.99.tar", last modified: Fri Apr 14 13:07:11 2023, max compression
```

## Comparing `je_api_testka-0.0.98.tar` & `je_api_testka-0.0.99.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.843577 je_api_testka-0.0.98/
--rw-rw-rw-   0        0        0     2647 2023-04-13 01:59:43.842575 je_api_testka-0.0.98/PKG-INFO
--rw-rw-rw-   0        0        0     2025 2023-03-31 01:27:07.000000 je_api_testka-0.0.98/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.707850 je_api_testka-0.0.98/je_api_testka/
--rw-rw-rw-   0        0        0     2630 2023-03-31 09:09:21.000000 je_api_testka-0.0.98/je_api_testka/__init__.py
--rw-rw-rw-   0        0        0     2002 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.740230 je_api_testka-0.0.98/je_api_testka/requests_wrapper/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/requests_wrapper/__init__.py
--rw-rw-rw-   0        0        0     5040 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/requests_wrapper/request_method.py
--rw-rw-rw-   0        0        0     2527 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.743221 je_api_testka-0.0.98/je_api_testka/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.748289 je_api_testka-0.0.98/je_api_testka/utils/assert_result/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/assert_result/__init__.py
--rw-rw-rw-   0        0        0      981 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/assert_result/result_check.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.754356 je_api_testka-0.0.98/je_api_testka/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 09:04:52.000000 je_api_testka-0.0.98/je_api_testka/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     2918 2023-04-13 01:01:18.000000 je_api_testka-0.0.98/je_api_testka/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.759307 je_api_testka-0.0.98/je_api_testka/utils/create_graph/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/create_graph/__init__.py
--rw-rw-rw-   0        0        0      972 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/create_graph/create_graph.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.768280 je_api_testka-0.0.98/je_api_testka/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     3318 2023-03-31 09:07:20.000000 je_api_testka-0.0.98/je_api_testka/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0     2330 2023-03-31 09:07:06.000000 je_api_testka-0.0.98/je_api_testka/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.772649 je_api_testka-0.0.98/je_api_testka/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     5086 2023-04-13 01:01:25.000000 je_api_testka-0.0.98/je_api_testka/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.779191 je_api_testka-0.0.98/je_api_testka/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      709 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.788168 je_api_testka-0.0.98/je_api_testka/utils/generate_report/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/generate_report/__init__.py
--rw-rw-rw-   0        0        0     8977 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/generate_report/html_report_generate.py
--rw-rw-rw-   0        0        0     3966 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/generate_report/json_report.py
--rw-rw-rw-   0        0        0     1565 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/generate_report/xml_report.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.793152 je_api_testka-0.0.98/je_api_testka/utils/get_data_strcture/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/get_data_strcture/__init__.py
--rw-rw-rw-   0        0        0     1588 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/get_data_strcture/get_api_data.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.795146 je_api_testka-0.0.98/je_api_testka/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.801125 je_api_testka-0.0.98/je_api_testka/utils/json/json_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1337 2023-04-13 01:01:25.000000 je_api_testka-0.0.98/je_api_testka/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.805623 je_api_testka-0.0.98/je_api_testka/utils/json/json_format/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1152 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.810605 je_api_testka-0.0.98/je_api_testka/utils/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-06 01:01:22.000000 je_api_testka-0.0.98/je_api_testka/utils/package_manager/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-04-06 01:43:15.000000 je_api_testka-0.0.98/je_api_testka/utils/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.816586 je_api_testka-0.0.98/je_api_testka/utils/socket_server/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/socket_server/__init__.py
--rw-rw-rw-   0        0        0     2465 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/socket_server/api_testka_socket_server.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.823562 je_api_testka-0.0.98/je_api_testka/utils/test_record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0      381 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/test_record/test_record_class.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.826554 je_api_testka-0.0.98/je_api_testka/utils/xml/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.832532 je_api_testka-0.0.98/je_api_testka/utils/xml/change_xml_structure/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/xml/change_xml_structure/__init__.py
--rw-rw-rw-   0        0        0     2498 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.839511 je_api_testka-0.0.98/je_api_testka/utils/xml/xml_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2424 2023-03-28 03:04:09.000000 je_api_testka-0.0.98/je_api_testka/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:59:43.732259 je_api_testka-0.0.98/je_api_testka.egg-info/
--rw-rw-rw-   0        0        0     2647 2023-04-13 01:59:43.000000 je_api_testka-0.0.98/je_api_testka.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2023-04-13 01:59:43.000000 je_api_testka-0.0.98/je_api_testka.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 01:59:43.000000 je_api_testka-0.0.98/je_api_testka.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 01:59:43.000000 je_api_testka-0.0.98/je_api_testka.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-13 01:59:43.000000 je_api_testka-0.0.98/je_api_testka.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      925 2023-04-13 01:59:21.000000 je_api_testka-0.0.98/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 01:59:43.844575 je_api_testka-0.0.98/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.487694 je_api_testka-0.0.99/
+-rw-rw-rw-   0        0        0     2647 2023-04-14 13:07:11.483706 je_api_testka-0.0.99/PKG-INFO
+-rw-rw-rw-   0        0        0     2025 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.235370 je_api_testka-0.0.99/je_api_testka/
+-rw-rw-rw-   0        0        0     2630 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/__init__.py
+-rw-rw-rw-   0        0        0     2002 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.287231 je_api_testka-0.0.99/je_api_testka/requests_wrapper/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/requests_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     5040 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/requests_wrapper/request_method.py
+-rw-rw-rw-   0        0        0     2527 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.288229 je_api_testka-0.0.99/je_api_testka/utils/
+-rw-rw-rw-   0        0        0        2 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.305184 je_api_testka-0.0.99/je_api_testka/utils/assert_result/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/assert_result/__init__.py
+-rw-rw-rw-   0        0        0      981 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/assert_result/result_check.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.316154 je_api_testka-0.0.99/je_api_testka/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     2918 2023-04-08 05:13:49.000000 je_api_testka-0.0.99/je_api_testka/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.326126 je_api_testka-0.0.99/je_api_testka/utils/create_graph/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/create_graph/__init__.py
+-rw-rw-rw-   0        0        0      972 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/create_graph/create_graph.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.349065 je_api_testka-0.0.99/je_api_testka/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     3318 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0     2330 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.352058 je_api_testka-0.0.99/je_api_testka/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     5086 2023-04-14 12:58:39.000000 je_api_testka-0.0.99/je_api_testka/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.361033 je_api_testka-0.0.99/je_api_testka/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      709 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.396937 je_api_testka-0.0.99/je_api_testka/utils/generate_report/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/generate_report/__init__.py
+-rw-rw-rw-   0        0        0     8977 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/generate_report/html_report_generate.py
+-rw-rw-rw-   0        0        0     3966 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/generate_report/json_report.py
+-rw-rw-rw-   0        0        0     1565 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/generate_report/xml_report.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.406911 je_api_testka-0.0.99/je_api_testka/utils/get_data_strcture/
+-rw-rw-rw-   0        0        0        2 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/get_data_strcture/__init__.py
+-rw-rw-rw-   0        0        0     1588 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/get_data_strcture/get_api_data.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.408906 je_api_testka-0.0.99/je_api_testka/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.410900 je_api_testka-0.0.99/je_api_testka/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1337 2023-04-14 12:58:39.000000 je_api_testka-0.0.99/je_api_testka/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.420874 je_api_testka-0.0.99/je_api_testka/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1152 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.434836 je_api_testka-0.0.99/je_api_testka/utils/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-05 13:27:19.000000 je_api_testka-0.0.99/je_api_testka/utils/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-04-06 11:50:16.000000 je_api_testka-0.0.99/je_api_testka/utils/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.448800 je_api_testka-0.0.99/je_api_testka/utils/socket_server/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/socket_server/__init__.py
+-rw-rw-rw-   0        0        0     2465 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/socket_server/api_testka_socket_server.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.458773 je_api_testka-0.0.99/je_api_testka/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0      381 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/test_record/test_record_class.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.459770 je_api_testka-0.0.99/je_api_testka/utils/xml/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/xml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.469743 je_api_testka-0.0.99/je_api_testka/utils/xml/change_xml_structure/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/xml/change_xml_structure/__init__.py
+-rw-rw-rw-   0        0        0     2498 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.479719 je_api_testka-0.0.99/je_api_testka/utils/xml/xml_file/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/xml/xml_file/__init__.py
+-rw-rw-rw-   0        0        0     2424 2023-04-02 11:29:16.000000 je_api_testka-0.0.99/je_api_testka/utils/xml/xml_file/xml_file.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:11.267285 je_api_testka-0.0.99/je_api_testka.egg-info/
+-rw-rw-rw-   0        0        0     2647 2023-04-14 13:07:11.000000 je_api_testka-0.0.99/je_api_testka.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2023-04-14 13:07:11.000000 je_api_testka-0.0.99/je_api_testka.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:07:11.000000 je_api_testka-0.0.99/je_api_testka.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 13:07:11.000000 je_api_testka-0.0.99/je_api_testka.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-14 13:07:11.000000 je_api_testka-0.0.99/je_api_testka.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      925 2023-04-14 13:06:48.000000 je_api_testka-0.0.99/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:07:11.487694 je_api_testka-0.0.99/setup.cfg
```

### Comparing `je_api_testka-0.0.98/PKG-INFO` & `je_api_testka-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_api_testka
-Version: 0.0.98
+Version: 0.0.99
 Summary: APT Testing Automation Framework
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/APITestka
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
```

### Comparing `je_api_testka-0.0.98/README.md` & `je_api_testka-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/__init__.py` & `je_api_testka-0.0.99/je_api_testka/__init__.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/__main__.py` & `je_api_testka-0.0.99/je_api_testka/__main__.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/requests_wrapper/request_method.py` & `je_api_testka-0.0.99/je_api_testka/requests_wrapper/request_method.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/requests_wrapper/requests_http_method_wrapper.py` & `je_api_testka-0.0.99/je_api_testka/requests_wrapper/requests_http_method_wrapper.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/assert_result/result_check.py` & `je_api_testka-0.0.99/je_api_testka/utils/assert_result/result_check.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/callback/callback_function_executor.py` & `je_api_testka-0.0.99/je_api_testka/utils/callback/callback_function_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/create_graph/create_graph.py` & `je_api_testka-0.0.99/je_api_testka/utils/create_graph/create_graph.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/exception/exception_tags.py` & `je_api_testka-0.0.99/je_api_testka/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/exception/exceptions.py` & `je_api_testka-0.0.99/je_api_testka/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/executor/action_executor.py` & `je_api_testka-0.0.99/je_api_testka/utils/executor/action_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/file_process/get_dir_file_list.py` & `je_api_testka-0.0.99/je_api_testka/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/generate_report/html_report_generate.py` & `je_api_testka-0.0.99/je_api_testka/utils/generate_report/html_report_generate.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/generate_report/json_report.py` & `je_api_testka-0.0.99/je_api_testka/utils/generate_report/json_report.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/generate_report/xml_report.py` & `je_api_testka-0.0.99/je_api_testka/utils/generate_report/xml_report.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/get_data_strcture/get_api_data.py` & `je_api_testka-0.0.99/je_api_testka/utils/get_data_strcture/get_api_data.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/json/json_file/json_file.py` & `je_api_testka-0.0.99/je_api_testka/utils/json/json_file/json_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/json/json_format/json_process.py` & `je_api_testka-0.0.99/je_api_testka/utils/json/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/package_manager/package_manager_class.py` & `je_api_testka-0.0.99/je_api_testka/utils/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/socket_server/api_testka_socket_server.py` & `je_api_testka-0.0.99/je_api_testka/utils/socket_server/api_testka_socket_server.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py` & `je_api_testka-0.0.99/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka/utils/xml/xml_file/xml_file.py` & `je_api_testka-0.0.99/je_api_testka/utils/xml/xml_file/xml_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/je_api_testka.egg-info/PKG-INFO` & `je_api_testka-0.0.99/je_api_testka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-api-testka
-Version: 0.0.98
+Version: 0.0.99
 Summary: APT Testing Automation Framework
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/APITestka
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
```

### Comparing `je_api_testka-0.0.98/je_api_testka.egg-info/SOURCES.txt` & `je_api_testka-0.0.99/je_api_testka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_api_testka-0.0.98/pyproject.toml` & `je_api_testka-0.0.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is stable version
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_api_testka"
-version = "0.0.98"
+version = "0.0.99"
 authors = [
     { name = "JE-Chen", email = "zenmailman@gmail.com" },
 ]
 description = "APT Testing Automation Framework"
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.7"
 license = { text = "MIT" }
```


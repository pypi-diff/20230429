# Comparing `tmp/QATLibrary-23.4.1.tar.gz` & `tmp/QATLibrary-23.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QATLibrary-23.4.1.tar", last modified: Sat Apr 22 00:18:10 2023, max compression
+gzip compressed data, was "QATLibrary-23.5.2.tar", last modified: Sat Apr 29 07:23:24 2023, max compression
```

## Comparing `QATLibrary-23.4.1.tar` & `QATLibrary-23.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:18:10.111556 QATLibrary-23.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-22 00:18:10.111556 QATLibrary-23.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-22 00:18:10.111556 QATLibrary-23.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:18:10.107556 QATLibrary-23.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:18:10.111556 QATLibrary-23.4.1/src/QATLibrary/
--rw-r--r--   0 runner    (1001) docker     (123)    17056 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/src/QATLibrary/QATLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/src/QATLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/src/QATLibrary/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/src/QATLibrary/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12033 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/src/QATLibrary/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/src/QATLibrary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:18:10.111556 QATLibrary-23.4.1/src/QATLibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-22 00:18:10.000000 QATLibrary-23.4.1/src/QATLibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-22 00:18:10.000000 QATLibrary-23.4.1/src/QATLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:18:10.000000 QATLibrary-23.4.1/src/QATLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-22 00:18:10.000000 QATLibrary-23.4.1/src/QATLibrary.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:18:10.000000 QATLibrary-23.4.1/src/QATLibrary.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-22 00:18:10.000000 QATLibrary-23.4.1/src/QATLibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 00:18:10.000000 QATLibrary-23.4.1/src/QATLibrary.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 07:23:24.094325 QATLibrary-23.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-29 07:23:24.094325 QATLibrary-23.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-29 07:23:24.098325 QATLibrary-23.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 07:23:24.094325 QATLibrary-23.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 07:23:24.094325 QATLibrary-23.5.2/src/QATLibrary/
+-rw-r--r--   0 runner    (1001) docker     (123)    16601 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/src/QATLibrary/QATLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/src/QATLibrary/TLSAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/src/QATLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/src/QATLibrary/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/src/QATLibrary/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-29 07:23:02.000000 QATLibrary-23.5.2/src/QATLibrary/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 07:23:24.094325 QATLibrary-23.5.2/src/QATLibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-29 07:23:24.000000 QATLibrary-23.5.2/src/QATLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-29 07:23:24.000000 QATLibrary-23.5.2/src/QATLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 07:23:24.000000 QATLibrary-23.5.2/src/QATLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-29 07:23:24.000000 QATLibrary-23.5.2/src/QATLibrary.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 07:23:24.000000 QATLibrary-23.5.2/src/QATLibrary.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-29 07:23:24.000000 QATLibrary-23.5.2/src/QATLibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 07:23:24.000000 QATLibrary-23.5.2/src/QATLibrary.egg-info/top_level.txt
```

### Comparing `QATLibrary-23.4.1/LICENSE.md` & `QATLibrary-23.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `QATLibrary-23.4.1/PKG-INFO` & `QATLibrary-23.5.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: QATLibrary
-Version: 23.4.1
+Version: 23.5.2
 Summary: Data/Configuration Driven REST API Test Automation Library. Can be used as a Robot Framework Library or as standalone CLI tool.
-Home-page: https://github.com/sharif314/QATLibrary
+Home-page: https://github.com/toil-free/QATLibrary.git
 Author: Sharif Rahman
 Author-email: shrif.sbu@gmail.com
 License: MIT
-Project-URL: Docs, https://github.com/sharif314/QATLibrary/README.md
-Project-URL: Issue Tracker, https://github.com/sharif314/QATLibrary/issues
+Project-URL: Docs, https://github.com/toil-free/QATLibrary/README.md
+Project-URL: Issue Tracker, https://github.com/toil-free/QATLibrary/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # QATLibrary 
 ![gh ci](https://github.com/sharif314/QATLibrary/workflows/QATLibrary%20CI/badge.svg)
@@ -118,46 +120,69 @@
 This command should generate two sample files like below - 
 1. [Sample CSV Test Data](https://github.com/sharif314/QATLibrary/blob/main/sample/TestCases.csv): Test Cases or Data file. 
 Test cases gets generated based on this file's content using Robot Framework. 
 
 2. [Sample Config YAML](https://github.com/sharif314/QATLibrary/blob/main/sample/config.yaml): This file contains various runtime configurations 
 for tests. Can be utilize to accommodate various CI or Test environments. Please follow the inline comments for more details -  
     ```yaml
-    host: httpbin.org           # Required
+    ---
+    # optional args; uncomment as-needed
+    base_url: httpbin.org           # base url/server name. Default localhost
+    timeout: 10                     # In seconds. Default 5 seconds
+    allow_redirects: True           # Allow Redirects. Default True.
+    stream: False                   # True/False. Default False.
     
-    #optional args
-    timeout: 5                  # Default 5 seconds
-    allow_redirects:            # Allow Redirects. Default True. 
-    stream:                     # True/False. 
-    http_proxy:                 # HTTP Proxy. Default None. 
-    https_proxy:                # HTTPS Proxy. Default None.
-    
-    verify_server_cert: True    # True/False or path to CA Bundle. Default False. 
-    certificate:                # .pem format certificate. Default None
-    private_key:                # .pem format private key (unencrypted). Default None
-    
-    # Required if using Basic/Digest Auth (Default None)
-    authUser:             
-    authPass:
-    
-    # Required if using OAuth1 auth (Default None)
-    oauth1_app_key:
-    oauth1_app_secret:
-    oauth1_user_token:
-    oauth1_user_token_secret:
-    ```
+    ## global headers - these are added to every request from your data csv. All headers should be strings.
+    headers:
+      user-agent: QATLibrary                                  # this is a static header
+      Authorization: Basic c29tZXVzZXI6bm90dmVyeXNlY3JldHBhc3M=
+      # dynamic headers can be added with ${} syntax like below -
+      X-correlation-id: ${str(__import__('uuid').uuid4())}         # dynamic headers use python's eval func.
+      random-digit: ${str(__import__('random').randint(0,99))}     # dynamic headers use python's eval func.
+    
+    
+    ## To enable proxies for http/https, enable the following config.
+    #proxies:
+    #  http_proxy:                   # HTTP proxy. Default None.
+    #  https_proxy:                  # HTTPS proxy. Default None.
+    #  no_proxy:                     # Bypass proxy
+    
+    ## SSL/TLS configuration for REST API calls. Enable to configure.
+    #tls:
+    #  verify_server_cert: True      # True/False or path to CA Bundle. Default False.
+    #  certificate:                  # .pem format certificate. Default None
+    #  private_key:                  # .pem format private key (unencrypted). Default None.
+    
+    ## Note that the specific details of how to obtain an access token may vary depending on the authentication scheme and API provider.
+    ## Be sure to check the API documentation for instructions on how to obtain an access token for your use case.
+    ## bearer auth / access token config. Enable below configs if required.
+    
+    #bearer_auth:
+    #  token_url:                                # token_url for bearer auth
+    #  payload:                                  # generic payload. supports all direct key/value. below are the common ones.
+    #    client_id:
+    #    client_secret:
+    #    scope:
+    #    grant_type:
+    
+    ## Enable following block for bearer auth TLS config.
+    #  tls:
+    #    verify_server_cert: True       # True/False or path to CA Bundle. Default False.
+    #    certificate:                  # .pem format certificate. Default None
+    #    private_key:                  # .pem format private key (unencrypted). Default None
+   ```
 
 Once the files are generated, you can rename them according to your test suites or requirements.  
 
 ## Contributing
 This is [Sharif](https://www.linkedin.com/in/sharif-rahman/). I started this project basically to make my life 
 a bit easier around simple REST API tests. This project is ideal for you if want to get some automated tests done 
 quickly for your projects without coding and powerful assertion methods out of the box. 
 
-QATLibrary is on [GitHub](https://github.com/sharif314/QATLibrary). 
+QATLibrary is on [GitHub](https://github.com/toil-free/QATLibrary.git). 
 Get in touch, via GitHub or otherwise, if you've got something to contribute, it'd be most welcome! 
-Please follow the [CONTRIBUTING.md](https://github.com/sharif314/QATLibrary/blob/main/CONTRIBUTING.md) for detailed guidelines.
+Please follow the [CONTRIBUTING.md]( https://github.com/toil-free/QATLibrary/blob/main/CONTRIBUTING.md) for detailed guidelines.
 
 ## License 
-QATLibrary is open source software provided under the MIT License. Please follow [LICENSE.md](https://github.com/sharif314/QATLibrary/blob/main/LICENSE.md) for more details. 
+QATLibrary is open source software provided under the MIT License. Please follow [LICENSE.md]( https://github.com/toil-free/QATLibrary/blob/main/LICENSE.md) for more details.
```

### Comparing `QATLibrary-23.4.1/README.md` & `QATLibrary-23.5.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -93,44 +93,67 @@
 This command should generate two sample files like below - 
 1. [Sample CSV Test Data](https://github.com/sharif314/QATLibrary/blob/main/sample/TestCases.csv): Test Cases or Data file. 
 Test cases gets generated based on this file's content using Robot Framework. 
 
 2. [Sample Config YAML](https://github.com/sharif314/QATLibrary/blob/main/sample/config.yaml): This file contains various runtime configurations 
 for tests. Can be utilize to accommodate various CI or Test environments. Please follow the inline comments for more details -  
     ```yaml
-    host: httpbin.org           # Required
+    ---
+    # optional args; uncomment as-needed
+    base_url: httpbin.org           # base url/server name. Default localhost
+    timeout: 10                     # In seconds. Default 5 seconds
+    allow_redirects: True           # Allow Redirects. Default True.
+    stream: False                   # True/False. Default False.
     
-    #optional args
-    timeout: 5                  # Default 5 seconds
-    allow_redirects:            # Allow Redirects. Default True. 
-    stream:                     # True/False. 
-    http_proxy:                 # HTTP Proxy. Default None. 
-    https_proxy:                # HTTPS Proxy. Default None.
-    
-    verify_server_cert: True    # True/False or path to CA Bundle. Default False. 
-    certificate:                # .pem format certificate. Default None
-    private_key:                # .pem format private key (unencrypted). Default None
-    
-    # Required if using Basic/Digest Auth (Default None)
-    authUser:             
-    authPass:
-    
-    # Required if using OAuth1 auth (Default None)
-    oauth1_app_key:
-    oauth1_app_secret:
-    oauth1_user_token:
-    oauth1_user_token_secret:
-    ```
+    ## global headers - these are added to every request from your data csv. All headers should be strings.
+    headers:
+      user-agent: QATLibrary                                  # this is a static header
+      Authorization: Basic c29tZXVzZXI6bm90dmVyeXNlY3JldHBhc3M=
+      # dynamic headers can be added with ${} syntax like below -
+      X-correlation-id: ${str(__import__('uuid').uuid4())}         # dynamic headers use python's eval func.
+      random-digit: ${str(__import__('random').randint(0,99))}     # dynamic headers use python's eval func.
+    
+    
+    ## To enable proxies for http/https, enable the following config.
+    #proxies:
+    #  http_proxy:                   # HTTP proxy. Default None.
+    #  https_proxy:                  # HTTPS proxy. Default None.
+    #  no_proxy:                     # Bypass proxy
+    
+    ## SSL/TLS configuration for REST API calls. Enable to configure.
+    #tls:
+    #  verify_server_cert: True      # True/False or path to CA Bundle. Default False.
+    #  certificate:                  # .pem format certificate. Default None
+    #  private_key:                  # .pem format private key (unencrypted). Default None.
+    
+    ## Note that the specific details of how to obtain an access token may vary depending on the authentication scheme and API provider.
+    ## Be sure to check the API documentation for instructions on how to obtain an access token for your use case.
+    ## bearer auth / access token config. Enable below configs if required.
+    
+    #bearer_auth:
+    #  token_url:                                # token_url for bearer auth
+    #  payload:                                  # generic payload. supports all direct key/value. below are the common ones.
+    #    client_id:
+    #    client_secret:
+    #    scope:
+    #    grant_type:
+    
+    ## Enable following block for bearer auth TLS config.
+    #  tls:
+    #    verify_server_cert: True       # True/False or path to CA Bundle. Default False.
+    #    certificate:                  # .pem format certificate. Default None
+    #    private_key:                  # .pem format private key (unencrypted). Default None
+   ```
 
 Once the files are generated, you can rename them according to your test suites or requirements.  
 
 ## Contributing
 This is [Sharif](https://www.linkedin.com/in/sharif-rahman/). I started this project basically to make my life 
 a bit easier around simple REST API tests. This project is ideal for you if want to get some automated tests done 
 quickly for your projects without coding and powerful assertion methods out of the box. 
 
-QATLibrary is on [GitHub](https://github.com/sharif314/QATLibrary). 
+QATLibrary is on [GitHub](https://github.com/toil-free/QATLibrary.git). 
 Get in touch, via GitHub or otherwise, if you've got something to contribute, it'd be most welcome! 
-Please follow the [CONTRIBUTING.md](https://github.com/sharif314/QATLibrary/blob/main/CONTRIBUTING.md) for detailed guidelines.
+Please follow the [CONTRIBUTING.md]( https://github.com/toil-free/QATLibrary/blob/main/CONTRIBUTING.md) for detailed guidelines.
 
 ## License 
-QATLibrary is open source software provided under the MIT License. Please follow [LICENSE.md](https://github.com/sharif314/QATLibrary/blob/main/LICENSE.md) for more details. 
+QATLibrary is open source software provided under the MIT License. Please follow [LICENSE.md]( https://github.com/toil-free/QATLibrary/blob/main/LICENSE.md) for more details.
```

### Comparing `QATLibrary-23.4.1/src/QATLibrary/QATLibrary.py` & `QATLibrary-23.5.2/src/QATLibrary/QATLibrary.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,162 +1,181 @@
 from __future__ import print_function
+
 import csv
 import json
+import re
+import requests
+import pprint
+
 from robot.libraries.BuiltIn import BuiltIn
 from robot.api import logger
 from robot.api.deco import keyword
-import requests
 from requests import Request, Session
-from requests.auth import HTTPDigestAuth
 from jsonschema import validate, exceptions
-import pprint
 
-import ssl
-from requests.adapters import HTTPAdapter
-from urllib3.poolmanager import PoolManager
+from .TLSAdapter import TLSAdapter
+
 
 class QATLibrary(object):
     ROBOT_LISTENER_API_VERSION = 3
     ROBOT_LIBRARY_SCOPE = 'TEST SUITE'
+    HEADER_VAR_EXP = re.compile(r"\${[^}]*}")
+
+    # init session
+    session = Session()
+    session.mount('https://', TLSAdapter())
 
     def __init__(self):
         self.ROBOT_LIBRARY_LISTENER = self
         self.current_suite = None
 
         self.builtin = BuiltIn()
+        self.base_url = BuiltIn().get_variable_value(name='${base_url}', default='localhost')
         self.timeout = BuiltIn().get_variable_value(name='${timeout}', default=10)
         self.allow_redirects = BuiltIn().get_variable_value(name='${allow_redirects}', default=True)
         self.stream = BuiltIn().get_variable_value(name='${stream}', default=False)
-        self.proxy = BuiltIn().get_variable_value(name='${proxy}', default=None)
-        self.authUser = BuiltIn().get_variable_value(name='${authUser}', default=None)
-        self.authPass = BuiltIn().get_variable_value(name='${authPass}', default=None)
-        self.oauth1_app_key = BuiltIn().get_variable_value(name='${oauth1_app_key}', default=None)
-        self.oauth1_app_secret = BuiltIn().get_variable_value(name='${oauth1_app_secret}', default=None)
-        self.oauth1_user_token = BuiltIn().get_variable_value(name='${oauth1_user_token}', default=None)
-        self.oauth1_user_token_secret = BuiltIn().get_variable_value(name='${oauth1_user_token_secret}', default=None)
-        self.verify = BuiltIn().get_variable_value('${verify_server_cert}', default=True)
-        self.certificate = BuiltIn().get_variable_value('${certificate}', default=None)
-        self.private_key = BuiltIn().get_variable_value('${private_key}', default=None)
-        self.http_proxy = BuiltIn().get_variable_value('${http_proxy}', default=None)
-        self.https_proxy = BuiltIn().get_variable_value('${https_proxy}', default=None)
+
+        self.verify = BuiltIn().get_variable_value('${tls.verify_server_cert}', default=True)
+        self.certificate = BuiltIn().get_variable_value('${tls.certificate}', default=None)
+        self.private_key = BuiltIn().get_variable_value('${tls.private_key}', default=None)
+        self.proxies = BuiltIn().get_variable_value('${proxies}', default={})
 
     def _start_suite(self, suite, result):
         self.current_suite = suite
 
     @keyword('QAT Dynamic Tests Setup')
-    def qat_dynamic_tests_setup(self, csvFile, encoding='utf-8', kwname=None, *args):
-        data = self.__generate_dict_data_from_csv(csvFile=csvFile, encoding=encoding)
+    def qat_dynamic_tests_setup(self, csv_file, encoding='utf-8', kwname=None, *args):
+        data = self.__generate_dict_data_from_csv(csv_file=csv_file, encoding=encoding)
 
         try:
-            for testCase in data:
-                if testCase['execute'] not in ['N', 'False', 'false']:
-                    tc = self.current_suite.tests.create(name=testCase['testName'] or 'Untitled Test',
-                                                         tags=self.__setup_test_tags(testCase),
-                                                         doc=self.__setup_test_documentation(testCase))
+            tc = self.current_suite.tests.create(name='Setup Global Test Variables',
+                                                 tags='SYSTEM',
+                                                 doc='Sets up injectable variables if required')
+            tc.body.create_keyword(name='Setup Global Vars', args=[data])
+
+            for i, test_case in enumerate(data, 0):
+                if test_case['execute'] not in ['N', 'False', 'false']:
+                    tc = self.current_suite.tests.create(name=test_case['testName'] or 'Untitled Test',
+                                                         tags=self.__setup_test_tags(test_case),
+                                                         doc=self.__setup_test_documentation(test_case))
                     tc.body.create_keyword(name='Data Driven HTTP Request',
-                                       args=[testCase])
+                                           args=["${data}" + f'[{i}]'])
 
                     if kwname is not None:
                         tc.body.create_keyword(name=kwname, args=args)
             logger.info('Dynamic Tests Creation Successful!')
         except Exception as e:
             logger.error(e)
             raise Exception('Dynamic Tests creation failed!')
 
+    @keyword
+    def setup_global_vars(self, data):
+        # setup data source
+        self.builtin.set_global_variable('${data}', data)
+
+        # set bearer token if configured
+        if self.builtin.get_variable_value('${bearer_auth}'):
+            bearer_token = requests.post(
+                url=self.builtin.get_variable_value('${bearer_auth.token_url}'),
+                data=self.builtin.get_variable_value('${bearer_auth.payload}'),
+                proxies=self.proxies,
+                allow_redirects=self.allow_redirects,
+                stream=self.stream,
+                timeout=self.timeout,
+                cert=(self.builtin.get_variable_value('${bearer_auth.tls.private_key}'),
+                      self.builtin.get_variable_value('${bearer_auth.tls.key}')),
+                verify=self.builtin.get_variable_value('${bearer_auth.tls.verify_server_cert}', True)
+            ).json()['access_token']
+            self.builtin.set_global_variable('${BEARER_AUTH}', {'Authorization': f'Bearer {bearer_token}'})
+
     @keyword('Data Driven HTTP Request')
     def qat_data_driven_http_request(self, data):
         logger.debug('Raw Test Data: ' + json.dumps(data, indent=2))
-        session = Session()
-        session.mount('https://', TLSAdapter())
-
         logger.debug('Preparing HTTP Request..')
-        prepped = session.prepare_request(Request(method=data['reqType'].upper(),
-                                                  url=self.__set_url(data),
-                                                  headers=self.__set_headers(data),
-                                                  params=self.__set_params(data),
-                                                  data=self.__set_payload(data),
-                                                  cookies=self.__set_cookies(data),
-                                                  auth=self.__set_auth(data)))
-        self.__log_prepped_request(prepped, data, encoding='utf-8')
-        response = session.send(prepped,
-                                allow_redirects=self.allow_redirects,
-                                stream=self.stream,
-                                timeout=self.timeout,
-                                cert=self.__set_ssl_cert(),
-                                proxies=self.__set_proxy(),
-                                verify=self.__verify_server_cert())
+        prepped = self.session.prepare_request(Request(method=data['reqType'].upper(),
+                                                       url=self.__set_url(data),
+                                                       headers=self.__set_headers(data),
+                                                       params=self.__set_params(data),
+                                                       data=self.__set_payload(data),
+                                                       cookies=self.__set_cookies(data)))
+        self.__log_prepped_request(prepped, data)
+        response = self.session.send(prepped,
+                                     allow_redirects=self.allow_redirects,
+                                     stream=self.stream,
+                                     timeout=self.timeout,
+                                     cert=self.__set_ssl_cert(),
+                                     proxies=self.__set_proxy(),
+                                     verify=self.__verify_server_cert())
 
         self.__log_response(response)
         self.__assert_response(response, data)
 
     """ Setup Configurations """
+
     @staticmethod
-    def __generate_dict_data_from_csv(csvFile, encoding='utf-8'):
+    def __generate_dict_data_from_csv(csv_file, encoding='utf-8'):
         """ Takes CSV file. Default encoding for CSV is utf-8,
         override the correct encoding while invoking this method."""
         data = []
 
-        with open(csvFile, encoding=encoding) as csvFile:
-            csv_reader = csv.DictReader(csvFile)
+        with open(csv_file, encoding=encoding) as csv_file:
+            csv_reader = csv.DictReader(csv_file)
             for row in csv_reader:
                 data.append(row)
         return data
 
     @staticmethod
-    def __setup_test_documentation(testCase):
-        if testCase['documentation'] and testCase['testId']:
-            return '[' + testCase['testId'] + '] ' + testCase['documentation']
+    def __setup_test_documentation(test_case):
+        if test_case['documentation'] and test_case['testId']:
+            return '[' + test_case['testId'] + '] ' + test_case['documentation']
         else:
-            return testCase['documentation'] or ''
+            return test_case['documentation'] or ''
 
     @staticmethod
-    def __setup_test_tags(testCase):
-        if testCase['tags']:
-            return testCase['tags'].split(',')
+    def __setup_test_tags(test_case):
+        if test_case['tags']:
+            return test_case['tags'].split(',')
         else:
             return ['REST API', 'QAT']
 
-    def __set_auth(self, data):
-        if data['authType'].lower() == 'basic':
-            return (self.builtin.get_variable_value('${authUser}'),
-                    self.builtin.get_variable_value('${authPass}'))
-        elif data['authType'].lower() == 'digest':
-            return HTTPDigestAuth(self.builtin.get_variable_value('${authUser}'),
-                                  self.builtin.get_variable_value('${authPass}'))
-        elif data['authType'].lower() == 'oauth1':
-            from requests_oauthlib import OAuth1
-            return OAuth1(self.builtin.get_variable_value('${oauth1_app_key}'),
-                          self.builtin.get_variable_value('${oauth1_app_secret}'),
-                          self.builtin.get_variable_value('${oauth1_user_token}'),
-                          self.builtin.get_variable_value('${oauth1_user_token_secret}'))
-        else:
-            return None
-
     """ Setup Request Payload """
 
     @staticmethod
     def __set_payload(data):
         if data['reqPayload']:
             return data['reqPayload']
         return None
 
     """ Setup Request URL """
 
     def __set_url(self, data):
         url = (data['protocol'] or 'http').lower() + '://' + \
-              self.builtin.get_variable_value('${host}', default='localhost')
+              self.builtin.get_variable_value('${base_url}', default='localhost')
         if data['port']:
             url += ':' + data['port']
         url += data['endPoint']
         return url
 
     """ Setup Headers """
 
     def __set_headers(self, data):
-        return self.__get_dict(data['reqHeaders'])
+        # add bearer auth if available
+        global_headers = self.builtin.get_variable_value('${BEARER_AUTH}', {})
+
+        # process global headers
+        config_headers = self.builtin.get_variable_value('${headers}', {})
+        if config_headers:
+            for k, v in config_headers.items():
+                global_headers[k] = eval(re.sub(r'\${(.*?)}', r'\1', v)) if self.HEADER_VAR_EXP.search(v) else v
+
+        # check for user defined headers
+        usr_def_headers = self.__get_dict(data['reqHeaders'])
+        if usr_def_headers:
+            return dict(global_headers.items() | usr_def_headers.items())
+        return global_headers
 
     """ Setup Request Parameters """
 
     def __set_params(self, data):
         return self.__get_dict(data['reqParams'])
 
     """ Setup Headers """
@@ -183,21 +202,15 @@
             return self.verify
         else:
             return False
 
     """ Configure Proxies """
 
     def __set_proxy(self):
-        if self.http_proxy or self.https_proxy:
-            return {
-                'http': self.http_proxy,
-                'https': self.https_proxy
-            }
-        else:
-            return None
+        return self.proxies
 
     """ Configure Verify SSL Certs """
 
     def __verify_ssl_cert(self):
         if self.builtin.get_variable_value('${verify_ssl_cert}') in ['True', 'true', 'yes']:
             return True
         if self.builtin.get_variable_value('${verify_ssl_cert}') is not None:
@@ -215,21 +228,23 @@
         self.__assert_headers(response, data, err['errors'])
         self.__assert_sla(response, data, err['errors'])
 
         if err['errors']:
             raise AssertionError(pprint.pformat(err, indent=2))
 
     """ Get JSON String to Dict """
+
     @staticmethod
-    def __get_dict(jsonData, default=None):
-        if bool(jsonData):
-            return json.loads(jsonData)
+    def __get_dict(json_str, default=None):
+        if bool(json_str):
+            return json.loads(json_str)
         return default
 
     """ Get list items from String or JSON. Only takes values from { "values": [] } or comma separated strings """
+
     @staticmethod
     def __get_values_from_json_or_string(data, key, delimeter=None):
         try:
             return json.loads(data[key])['values'] or []
         except (KeyError, json.decoder.JSONDecodeError) as e:
             logger.trace(e)
             return data[key].split(delimeter) or []
@@ -269,74 +284,72 @@
     """ Validate Response """
 
     def __assert_response_body(self, response, data, err):
         if data['rspShouldContain'] or data['rspShouldNotContain']:
             logger.info('Running Response Body Assertions..')
 
             if data['rspShouldContain']:
-                validContents = self.__get_values_from_json_or_string(data=data,
-                                                                      key='rspShouldContain',
-                                                                      delimeter=',')
-                for content in validContents:
+                valid_contents = self.__get_values_from_json_or_string(data=data,
+                                                                       key='rspShouldContain',
+                                                                       delimeter=',')
+                for content in valid_contents:
                     if not content.strip() in response.text:
                         err.append('Response body does not contain expected: ' + content.strip())
 
             if data['rspShouldNotContain']:
-                invalidContents = self.__get_values_from_json_or_string(data=data,
-                                                                        key='rspShouldNotContain',
-                                                                        delimeter=',')
-                for content in invalidContents:
+                invalid_contents = self.__get_values_from_json_or_string(data=data,
+                                                                         key='rspShouldNotContain',
+                                                                         delimeter=',')
+                for content in invalid_contents:
                     if content.strip() in response.text:
                         err.append('Response body contains unexpected: ' + content.strip())
 
         else:
             logger.info('Skipping Response Body Assertions')
 
     """ Validate Response Headers """
 
     def __assert_headers(self, response, data, err):
-        expectedHeaders = self.__get_dict(data['rspHeadersShouldContain'], default={})
-        unexpectedHeaders = self.__get_dict(data['rspHeadersShouldNotContain'], default={})
+        expected_headers = self.__get_dict(data['rspHeadersShouldContain'], default={})
+        unexpected_headers = self.__get_dict(data['rspHeadersShouldNotContain'], default={})
 
-        if expectedHeaders or unexpectedHeaders:
+        if expected_headers or unexpected_headers:
             logger.info('Running Response Headers assertions..')
-            if not all(header in response.headers.items() for header in expectedHeaders.items()):
+            if not all(header in response.headers.items() for header in expected_headers.items()):
                 logger.error(pprint.pformat(response.headers)
                              + ' Does not contain one or more expected headers: '
-                             + pprint.pformat(expectedHeaders))
+                             + pprint.pformat(expected_headers))
                 err.append('Response Headers missing expected value(s)')
 
-            if any(header in response.headers.items() for header in unexpectedHeaders.items()):
+            if any(header in response.headers.items() for header in unexpected_headers.items()):
                 logger.error(pprint.pformat(response.headers)
                              + ' contains one or more unexpected headers: '
-                             + pprint.pformat(unexpectedHeaders))
+                             + pprint.pformat(unexpected_headers))
                 err.append('Response Headers contains unexpected value(s)')
         else:
             logger.info('Skipping Response Headers Assertion')
 
     """ Validate Response SLA """
 
     @staticmethod
     def __assert_sla(response, data, err):
         if data['rspSLA']:
-            rspSLA = float(data['rspSLA'])
-            actualRspTime = response.elapsed.total_seconds() * 1000
-            if rspSLA < actualRspTime:
+            rsp_sla = float(data['rspSLA'])
+            rsp_time = response.elapsed.total_seconds() * 1000
+            if rsp_sla < rsp_time:
                 err.append(
-                    'Expected Response SLA: ' + str(rspSLA) + '(ms) but actual was: ' + str(actualRspTime) + '(ms)')
+                    'Expected Response SLA: ' + str(rsp_sla) + '(ms) but actual was: ' + str(rsp_time) + '(ms)')
             else:
                 logger.info('Response SLA Validation Successful')
         else:
             logger.info("Response SLA not configured. Skipping validation.")
 
     """ Log Request """
 
-    def __log_prepped_request(self, prepped, data, encoding=None):
-        encoding = encoding or requests.utils.get_encoding_from_headers(prepped.headers)
-        # logger.trace(encoding)
+    def __log_prepped_request(self, prepped, data):
         body = None
         if prepped.body:
             try:
                 body = prepped.body
             except AttributeError:
                 body = self.__set_payload(data)
         headers = '\n'.join(['{}: {}'.format(*hv) for hv in prepped.headers.items()])
@@ -348,16 +361,15 @@
 URL: {prepped.url}
 Timeout: {self.timeout}
 Allow Redirects: {self.allow_redirects}
 Stream: {self.stream}
 Verify Server Cert: {self.verify}
 SSL Certificate: {self.certificate}
 SSL Private Key: {self.private_key}
-HTTP Proxy: {self.http_proxy}
-HTTPS Proxy: {self.https_proxy}
+Proxies: {self.proxies}
 ----------------------------------------------------------------------------------
 [Request Headers]
 ----------------------------------------------------------------------------------
 {headers}
 ----------------------------------------------------------------------------------
 [Request Body]
 ----------------------------------------------------------------------------------
@@ -388,19 +400,8 @@
 [Response Body]
 ----------------------------------------------------------------------------------
 {response.text}
 ==================================================================================
 """)
 
 
-class TLSAdapter(HTTPAdapter):
-    """Transport adapter that forces use of TLSv1.2.
-            All Tomcat Servers Require TLSv1.2 in DEV, QA, CTE or PROD environment."""
-
-    def init_poolmanager(self, connections, maxsize, block=False, **kwargs):
-        """Create and initialize the urllib3 PoolManager to use TLSv.12."""
-        self.poolmanager = PoolManager(
-            num_pools=connections, maxsize=maxsize,
-            block=block, ssl_version=ssl.PROTOCOL_TLSv1_2)
-
-
 globals()[__name__] = QATLibrary
```

### Comparing `QATLibrary-23.4.1/src/QATLibrary/cli.py` & `QATLibrary-23.5.2/src/QATLibrary/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+import argparse
+import sys
+import os
+import platform
+
 from robot.api import TestSuite
 from robot.conf import RobotSettings
 from robot.output import LOGGER, pyloggingconf
 from robot.api import ResultWriter
 from pathlib import Path
-import argparse
-import sys
-import os
-import platform
 from termcolor import *
 from .version import VERSION
 
-
 ACTIONS = ['init', 'clean', 'run']
 CONFIG_FILE_NAME = 'config.yaml'
 CSV_DATA_FILE_NAME = 'TestCases.csv'
 INTRO = '=' * 78
 
 
 def print_qat_cli_intro(args):
@@ -36,62 +36,60 @@
 def colored_msg(msg, color=None):
     if os.name == 'nt':
         print(msg)
     else:
         cprint(msg, color)
 
 
-def isFile(arg_value):
+def is_file(arg_value):
     if not Path(arg_value).is_file():
         raise argparse.ArgumentTypeError('File does not exist: ' + arg_value)
     return arg_value
 
 
-def isDir(arg_value):
+def is_dir(arg_value):
     if not Path(arg_value).is_dir():
         raise argparse.ArgumentTypeError('Directory does not exist: ' + arg_value)
     return arg_value
 
 
 def input_csv(arg_value):
-    isFile(arg_value)
+    is_file(arg_value)
     if '.csv' not in arg_value:
         raise argparse.ArgumentTypeError('-f or --file value must be a .csv file')
     return arg_value
 
 
 def _clean(target_dir):
-    report_exts=('.html', '.xml')
+    report_exts = ('.html', '.xml')
     target_files = os.listdir(target_dir)
 
     for file_name in target_files:
         if file_name.endswith(report_exts):
             print('Removing file: ', os.path.join(target_dir, file_name))
             os.remove(os.path.join(target_dir, file_name))
     colored_msg('Cleanup complete!', 'green')
 
 
 def _init():
-    from .templates import CONFIG_FILE_CONTENT, CSV_DATA_FILE_CONTENT
+    _create_template_files()
 
-    print('Initializing QAT Sample files..')
-    _create_template_file(CONFIG_FILE_NAME, CONFIG_FILE_CONTENT)
-    _create_template_file(CSV_DATA_FILE_NAME, CSV_DATA_FILE_CONTENT)
-    print(f"""
-You may run: 
-    qat run -f { CSV_DATA_FILE_NAME } -c { CONFIG_FILE_NAME } """)
 
-
-def _create_template_file(file_name, file_content):
-    if not Path(file_name).is_file():
-        with open(file_name, "w") as file:
-            file.write(file_content)
-        colored_msg('==> QAT sample file created: ' + file_name, 'green')
-    else:
-        colored_msg('==> Skipping... File exists: ' + file_name, 'yellow')
+def _create_template_files():
+    import shutil
+    import pkg_resources
+    for f in os.listdir(pkg_resources.resource_filename('QATLibrary', 'templates')):
+        if not Path(f).is_file():
+            shutil.copy(pkg_resources.resource_filename('QATLibrary', f'templates/{f}'), f)
+            colored_msg('==> QAT sample file created: ' + f, 'green')
+        else:
+            colored_msg('==> Skipping... File exists: ' + f, 'yellow')
+    print(f"""
+    You may run: 
+        qat run -c {CONFIG_FILE_NAME} -f {CSV_DATA_FILE_NAME} """)
 
 
 def _create_test_suite(args):
     print_qat_cli_intro(args)
     suite = TestSuite(name=args.file.split('/')[-1] + ' | ' + 'QAT ',
                       doc='Runs (Quick) API Tests from Input CSV Data')
     suite.resource.imports.library('QATLibrary')
@@ -124,15 +122,15 @@
 
     parser.add_argument('action', metavar='action', type=str,
                         choices=ACTIONS,
                         help='Action for QAT CLI. Valid choices: ' + str(ACTIONS))
 
     parser.add_argument('-c', '--config',
                         help='Config yaml file with required settings or variables. ',
-                        required='run' in sys.argv, type=isFile)
+                        required='run' in sys.argv, type=is_file)
 
     parser.add_argument('-f', '--file',
                         help='CSV File Input. Relative/absolute path accepted.',
                         required='run' in sys.argv, type=input_csv)
 
     parser.add_argument('-e', '--encoding',
                         help='Encoding for CSV Input File',
@@ -158,15 +156,15 @@
                         default='output.xml',
                         help='Output xml file name',
                         required=False, type=str)
 
     parser.add_argument('-d', '--directory',
                         help='Target Directory for "init" or "clean". Default current directory.',
                         default=os.getcwd(),
-                        required=False, type=isDir)
+                        required=False, type=is_dir)
 
     parser.add_argument('-rc', '--return_rc',
                         action='store_true',
                         help='Return error status code on test failures. Default False',
                         required=False)
 
     args = parser.parse_args()
```

### Comparing `QATLibrary-23.4.1/src/QATLibrary.egg-info/PKG-INFO` & `QATLibrary-23.5.2/src/QATLibrary.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: QATLibrary
-Version: 23.4.1
+Version: 23.5.2
 Summary: Data/Configuration Driven REST API Test Automation Library. Can be used as a Robot Framework Library or as standalone CLI tool.
-Home-page: https://github.com/sharif314/QATLibrary
+Home-page: https://github.com/toil-free/QATLibrary.git
 Author: Sharif Rahman
 Author-email: shrif.sbu@gmail.com
 License: MIT
-Project-URL: Docs, https://github.com/sharif314/QATLibrary/README.md
-Project-URL: Issue Tracker, https://github.com/sharif314/QATLibrary/issues
+Project-URL: Docs, https://github.com/toil-free/QATLibrary/README.md
+Project-URL: Issue Tracker, https://github.com/toil-free/QATLibrary/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # QATLibrary 
 ![gh ci](https://github.com/sharif314/QATLibrary/workflows/QATLibrary%20CI/badge.svg)
@@ -118,46 +120,69 @@
 This command should generate two sample files like below - 
 1. [Sample CSV Test Data](https://github.com/sharif314/QATLibrary/blob/main/sample/TestCases.csv): Test Cases or Data file. 
 Test cases gets generated based on this file's content using Robot Framework. 
 
 2. [Sample Config YAML](https://github.com/sharif314/QATLibrary/blob/main/sample/config.yaml): This file contains various runtime configurations 
 for tests. Can be utilize to accommodate various CI or Test environments. Please follow the inline comments for more details -  
     ```yaml
-    host: httpbin.org           # Required
+    ---
+    # optional args; uncomment as-needed
+    base_url: httpbin.org           # base url/server name. Default localhost
+    timeout: 10                     # In seconds. Default 5 seconds
+    allow_redirects: True           # Allow Redirects. Default True.
+    stream: False                   # True/False. Default False.
     
-    #optional args
-    timeout: 5                  # Default 5 seconds
-    allow_redirects:            # Allow Redirects. Default True. 
-    stream:                     # True/False. 
-    http_proxy:                 # HTTP Proxy. Default None. 
-    https_proxy:                # HTTPS Proxy. Default None.
-    
-    verify_server_cert: True    # True/False or path to CA Bundle. Default False. 
-    certificate:                # .pem format certificate. Default None
-    private_key:                # .pem format private key (unencrypted). Default None
-    
-    # Required if using Basic/Digest Auth (Default None)
-    authUser:             
-    authPass:
-    
-    # Required if using OAuth1 auth (Default None)
-    oauth1_app_key:
-    oauth1_app_secret:
-    oauth1_user_token:
-    oauth1_user_token_secret:
-    ```
+    ## global headers - these are added to every request from your data csv. All headers should be strings.
+    headers:
+      user-agent: QATLibrary                                  # this is a static header
+      Authorization: Basic c29tZXVzZXI6bm90dmVyeXNlY3JldHBhc3M=
+      # dynamic headers can be added with ${} syntax like below -
+      X-correlation-id: ${str(__import__('uuid').uuid4())}         # dynamic headers use python's eval func.
+      random-digit: ${str(__import__('random').randint(0,99))}     # dynamic headers use python's eval func.
+    
+    
+    ## To enable proxies for http/https, enable the following config.
+    #proxies:
+    #  http_proxy:                   # HTTP proxy. Default None.
+    #  https_proxy:                  # HTTPS proxy. Default None.
+    #  no_proxy:                     # Bypass proxy
+    
+    ## SSL/TLS configuration for REST API calls. Enable to configure.
+    #tls:
+    #  verify_server_cert: True      # True/False or path to CA Bundle. Default False.
+    #  certificate:                  # .pem format certificate. Default None
+    #  private_key:                  # .pem format private key (unencrypted). Default None.
+    
+    ## Note that the specific details of how to obtain an access token may vary depending on the authentication scheme and API provider.
+    ## Be sure to check the API documentation for instructions on how to obtain an access token for your use case.
+    ## bearer auth / access token config. Enable below configs if required.
+    
+    #bearer_auth:
+    #  token_url:                                # token_url for bearer auth
+    #  payload:                                  # generic payload. supports all direct key/value. below are the common ones.
+    #    client_id:
+    #    client_secret:
+    #    scope:
+    #    grant_type:
+    
+    ## Enable following block for bearer auth TLS config.
+    #  tls:
+    #    verify_server_cert: True       # True/False or path to CA Bundle. Default False.
+    #    certificate:                  # .pem format certificate. Default None
+    #    private_key:                  # .pem format private key (unencrypted). Default None
+   ```
 
 Once the files are generated, you can rename them according to your test suites or requirements.  
 
 ## Contributing
 This is [Sharif](https://www.linkedin.com/in/sharif-rahman/). I started this project basically to make my life 
 a bit easier around simple REST API tests. This project is ideal for you if want to get some automated tests done 
 quickly for your projects without coding and powerful assertion methods out of the box. 
 
-QATLibrary is on [GitHub](https://github.com/sharif314/QATLibrary). 
+QATLibrary is on [GitHub](https://github.com/toil-free/QATLibrary.git). 
 Get in touch, via GitHub or otherwise, if you've got something to contribute, it'd be most welcome! 
-Please follow the [CONTRIBUTING.md](https://github.com/sharif314/QATLibrary/blob/main/CONTRIBUTING.md) for detailed guidelines.
+Please follow the [CONTRIBUTING.md]( https://github.com/toil-free/QATLibrary/blob/main/CONTRIBUTING.md) for detailed guidelines.
 
 ## License 
-QATLibrary is open source software provided under the MIT License. Please follow [LICENSE.md](https://github.com/sharif314/QATLibrary/blob/main/LICENSE.md) for more details. 
+QATLibrary is open source software provided under the MIT License. Please follow [LICENSE.md]( https://github.com/toil-free/QATLibrary/blob/main/LICENSE.md) for more details.
```


# Comparing `tmp/brease-sdk-1.1.0.tar.gz` & `tmp/brease-sdk-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brease-sdk-1.1.0.tar", last modified: Fri Apr 21 00:41:45 2023, max compression
+gzip compressed data, was "brease-sdk-1.1.1.tar", last modified: Sat Apr 29 00:41:56 2023, max compression
```

## Comparing `brease-sdk-1.1.0.tar` & `brease-sdk-1.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.299965 brease-sdk-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-21 00:41:45.299965 brease-sdk-1.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2432 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 00:41:45.299965 brease-sdk-1.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.295965 brease-sdk-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.295965 brease-sdk-1.1.0/src/brease_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-21 00:41:45.000000 brease-sdk-1.1.0/src/brease_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-21 00:41:45.000000 brease-sdk-1.1.0/src/brease_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:41:45.000000 brease-sdk-1.1.0/src/brease_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-21 00:41:45.000000 brease-sdk-1.1.0/src/brease_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-21 00:41:45.000000 brease-sdk-1.1.0/src/brease_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.295965 brease-sdk-1.1.0/src/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6362 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/contextid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.295965 brease-sdk-1.1.0/src/sdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.299965 brease-sdk-1.1.0/src/sdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)      537 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1244 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/operations/addrule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1322 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/operations/evaluaterules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1045 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/operations/getallrules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/operations/removerule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1416 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/operations/replacerule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.299965 brease-sdk-1.1.0/src/sdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/addruleinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/apiaddruleresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/apiallrulesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      670 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/apievaluaterulesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      608 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/apireplaceruleresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1344 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/condition.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/conditionbasekey.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      678 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/conditionbaseref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/conditiontype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/evaluaterulesinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1491 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/expressionarray.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/modelsevaluationresult.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2142 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/modelsrule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      757 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/modelstarget.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/replaceruleinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.299965 brease-sdk-1.1.0/src/sdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.530219 brease-sdk-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-29 00:41:56.530219 brease-sdk-1.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2649 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 00:41:56.530219 brease-sdk-1.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.522219 brease-sdk-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.522219 brease-sdk-1.1.1/src/brease_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-29 00:41:56.000000 brease-sdk-1.1.1/src/brease_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-29 00:41:56.000000 brease-sdk-1.1.1/src/brease_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:41:56.000000 brease-sdk-1.1.1/src/brease_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 00:41:56.000000 brease-sdk-1.1.1/src/brease_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-29 00:41:56.000000 brease-sdk-1.1.1/src/brease_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.522219 brease-sdk-1.1.1/src/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6362 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/contextid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.522219 brease-sdk-1.1.1/src/sdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.522219 brease-sdk-1.1.1/src/sdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      537 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/operations/addrule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1308 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/operations/evaluaterules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/operations/getallrules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/operations/removerule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/operations/replacerule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.526219 brease-sdk-1.1.1/src/sdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      582 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/addruleinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      602 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/apiaddruleresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/apiallrulesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/apievaluaterulesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      606 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/apireplaceruleresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/condition.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      506 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/conditionbasekey.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      674 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/conditionbaseref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/conditiontype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      934 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/evaluaterulesinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1483 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/expressionarray.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/modelsevaluationresult.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2126 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/modelsrule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/modelstarget.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/replaceruleinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.530219 brease-sdk-1.1.1/src/sdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/utils/utils.py
```

### Comparing `brease-sdk-1.1.0/LICENSE.md` & `brease-sdk-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.0/PKG-INFO` & `brease-sdk-1.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brease-sdk
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: dotindustries
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -52,35 +52,35 @@
                 target_value="maiores",
                 type="molestiae",
             ),
         ),
     ),
     context_id="quod",
 )
-    
+
 res = s.context_id.add_rule(req, operations.AddRuleSecurity(
     api_token="Bearer YOUR_BEARER_TOKEN_HERE",
 ))
 
 if res.api_add_rule_response is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
 ## Available Resources and Operations
 
 
-### context_id
+### [context_id](docs/contextid/README.md)
 
-* `add_rule` - Adds a new rule to the context
-* `evaluate_rules` - Evaluate rules within a context on the provided object
-* `get_all_rules` - Returns all rules with the context
-* `remove_rule` - Removes a rule from the context
-* `replace_rule` - Replaces an existing rule within the context
+* [add_rule](docs/contextid/README.md#add_rule) - Adds a new rule to the context
+* [evaluate_rules](docs/contextid/README.md#evaluate_rules) - Evaluate rules within a context on the provided object
+* [get_all_rules](docs/contextid/README.md#get_all_rules) - Returns all rules with the context
+* [remove_rule](docs/contextid/README.md#remove_rule) - Removes a rule from the context
+* [replace_rule](docs/contextid/README.md#replace_rule) - Replaces an existing rule within the context
 <!-- End SDK Available Operations -->
 
 ### Maturity
 
 This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
 to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
 looking for the latest version.
```

### Comparing `brease-sdk-1.1.0/README.md` & `brease-sdk-1.1.1/src/brease_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: brease-sdk
+Version: 1.1.1
+Summary: Python Client SDK Generated by Speakeasy
+Home-page: UNKNOWN
+Author: dotindustries
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # brease-sdk
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
 ```bash
 pip install brease-sdk
@@ -40,42 +52,44 @@
                 target_value="maiores",
                 type="molestiae",
             ),
         ),
     ),
     context_id="quod",
 )
-    
+
 res = s.context_id.add_rule(req, operations.AddRuleSecurity(
     api_token="Bearer YOUR_BEARER_TOKEN_HERE",
 ))
 
 if res.api_add_rule_response is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
 ## Available Resources and Operations
 
 
-### context_id
+### [context_id](docs/contextid/README.md)
 
-* `add_rule` - Adds a new rule to the context
-* `evaluate_rules` - Evaluate rules within a context on the provided object
-* `get_all_rules` - Returns all rules with the context
-* `remove_rule` - Removes a rule from the context
-* `replace_rule` - Replaces an existing rule within the context
+* [add_rule](docs/contextid/README.md#add_rule) - Adds a new rule to the context
+* [evaluate_rules](docs/contextid/README.md#evaluate_rules) - Evaluate rules within a context on the provided object
+* [get_all_rules](docs/contextid/README.md#get_all_rules) - Returns all rules with the context
+* [remove_rule](docs/contextid/README.md#remove_rule) - Removes a rule from the context
+* [replace_rule](docs/contextid/README.md#replace_rule) - Replaces an existing rule within the context
 <!-- End SDK Available Operations -->
 
 ### Maturity
 
 This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
 to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
 looking for the latest version.
 
 ### Contributions
 
 While we value open-source contributions to this SDK, this library is generated programmatically.
 Feel free to open a PR or a Github issue as a proof of concept and we'll do our best to include it in a future release !
 
 ### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
+
+
```

### Comparing `brease-sdk-1.1.0/setup.py` & `brease-sdk-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="brease-sdk",
-    version="1.1.0",
+    version="1.1.1",
     author="dotindustries",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
-        "certifi==2022.12.07",
+        "certifi==2022.12.7",
         "charset-normalizer==2.1.1",
         "dataclasses-json-speakeasy==0.5.8",
         "idna==3.3",
         "marshmallow==3.17.1",
         "marshmallow-enum==1.5.1",
         "mypy-extensions==0.4.3",
         "packaging==21.3",
```

### Comparing `brease-sdk-1.1.0/src/brease_sdk.egg-info/SOURCES.txt` & `brease-sdk-1.1.1/src/brease_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.0/src/sdk/contextid.py` & `brease-sdk-1.1.1/src/sdk/contextid.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.0/src/sdk/models/operations/__init__.py` & `brease-sdk-1.1.1/src/sdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.0/src/sdk/models/operations/addrule.py` & `brease-sdk-1.1.1/src/sdk/models/operations/addrule.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from ..shared import apiaddruleresponse as shared_apiaddruleresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
 class AddRuleSecurity:
     
-    api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'http', 'sub_type': 'bearer', 'field_name': 'Authorization' }})  
+    api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'http', 'sub_type': 'bearer', 'field_name': 'Authorization' }})
     
 
 @dataclasses.dataclass
 class AddRuleRequest:
     
-    context_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'contextID', 'style': 'simple', 'explode': False }})  
-    add_rule_input: Optional[shared_addruleinput.AddRuleInput] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    context_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'contextID', 'style': 'simple', 'explode': False }})
+    add_rule_input: Optional[shared_addruleinput.AddRuleInput] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclasses.dataclass
 class AddRuleResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     api_add_rule_response: Optional[shared_apiaddruleresponse.APIAddRuleResponse] = dataclasses.field(default=None)
-    r"""OK"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    r"""OK"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/operations/evaluaterules.py` & `brease-sdk-1.1.1/src/sdk/models/operations/evaluaterules.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from ..shared import evaluaterulesinput as shared_evaluaterulesinput
 from typing import Optional
 
 
 @dataclasses.dataclass
 class EvaluateRulesSecurity:
     
-    api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'http', 'sub_type': 'bearer', 'field_name': 'Authorization' }})  
+    api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'http', 'sub_type': 'bearer', 'field_name': 'Authorization' }})
     
 
 @dataclasses.dataclass
 class EvaluateRulesRequest:
     
-    context_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'contextID', 'style': 'simple', 'explode': False }})  
-    evaluate_rules_input: Optional[shared_evaluaterulesinput.EvaluateRulesInput] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    context_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'contextID', 'style': 'simple', 'explode': False }})
+    evaluate_rules_input: Optional[shared_evaluaterulesinput.EvaluateRulesInput] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclasses.dataclass
 class EvaluateRulesResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     api_evaluate_rules_response: Optional[shared_apievaluaterulesresponse.APIEvaluateRulesResponse] = dataclasses.field(default=None)
-    r"""OK"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    r"""OK"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/operations/getallrules.py` & `brease-sdk-1.1.1/src/sdk/models/operations/getallrules.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from ..shared import apiallrulesresponse as shared_apiallrulesresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetAllRulesSecurity:
     
-    api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'http', 'sub_type': 'bearer', 'field_name': 'Authorization' }})  
+    api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'http', 'sub_type': 'bearer', 'field_name': 'Authorization' }})
     
 
 @dataclasses.dataclass
 class GetAllRulesRequest:
     
-    context_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'contextID', 'style': 'simple', 'explode': False }})  
+    context_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'contextID', 'style': 'simple', 'explode': False }})
     
 
 @dataclasses.dataclass
 class GetAllRulesResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     api_all_rules_response: Optional[shared_apiallrulesresponse.APIAllRulesResponse] = dataclasses.field(default=None)
-    r"""OK"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    r"""OK"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/operations/removerule.py` & `brease-sdk-1.1.1/src/sdk/models/operations/removerule.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 import requests as requests_http
 from typing import Optional
 
 
 @dataclasses.dataclass
 class RemoveRuleSecurity:
     
-    api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'http', 'sub_type': 'bearer', 'field_name': 'Authorization' }})  
+    api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'http', 'sub_type': 'bearer', 'field_name': 'Authorization' }})
     
 
 @dataclasses.dataclass
 class RemoveRuleRequest:
     
-    context_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'contextID', 'style': 'simple', 'explode': False }})  
-    id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})  
+    context_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'contextID', 'style': 'simple', 'explode': False }})
+    id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     
 
 @dataclasses.dataclass
 class RemoveRuleResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/operations/replacerule.py` & `brease-sdk-1.1.1/src/sdk/models/operations/replacerule.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 from ..shared import replaceruleinput as shared_replaceruleinput
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ReplaceRuleSecurity:
     
-    api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'http', 'sub_type': 'bearer', 'field_name': 'Authorization' }})  
+    api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'http', 'sub_type': 'bearer', 'field_name': 'Authorization' }})
     
 
 @dataclasses.dataclass
 class ReplaceRuleRequest:
     
-    context_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'contextID', 'style': 'simple', 'explode': False }})  
-    id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})  
-    replace_rule_input: Optional[shared_replaceruleinput.ReplaceRuleInput] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    context_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'contextID', 'style': 'simple', 'explode': False }})
+    id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
+    replace_rule_input: Optional[shared_replaceruleinput.ReplaceRuleInput] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclasses.dataclass
 class ReplaceRuleResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     api_replace_rule_response: Optional[shared_apireplaceruleresponse.APIReplaceRuleResponse] = dataclasses.field(default=None)
-    r"""OK"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    r"""OK"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/shared/__init__.py` & `brease-sdk-1.1.1/src/sdk/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.0/src/sdk/models/shared/addruleinput.py` & `brease-sdk-1.1.1/src/sdk/models/shared/addruleinput.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class AddRuleInput:
     
-    rule: Optional[shared_modelsrule.ModelsRule] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rule'), 'exclude': lambda f: f is None }})  
+    rule: Optional[shared_modelsrule.ModelsRule] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rule'), 'exclude': lambda f: f is None }})
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/shared/apiaddruleresponse.py` & `brease-sdk-1.1.1/src/sdk/models/shared/apiaddruleresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class APIAddRuleResponse:
     r"""OK"""
     
-    rule: Optional[shared_modelsrule.ModelsRule] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rule'), 'exclude': lambda f: f is None }})  
+    rule: Optional[shared_modelsrule.ModelsRule] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rule'), 'exclude': lambda f: f is None }})
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/shared/apiallrulesresponse.py` & `brease-sdk-1.1.1/src/sdk/models/shared/apiallrulesresponse.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class APIAllRulesResponse:
     r"""OK"""
     
-    code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('code'), 'exclude': lambda f: f is None }})  
-    rules: Optional[list[shared_modelsrule.ModelsRule]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rules'), 'exclude': lambda f: f is None }})  
+    code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('code'), 'exclude': lambda f: f is None }})
+    rules: Optional[list[shared_modelsrule.ModelsRule]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rules'), 'exclude': lambda f: f is None }})
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/shared/apievaluaterulesresponse.py` & `brease-sdk-1.1.1/src/sdk/models/shared/apievaluaterulesresponse.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class APIEvaluateRulesResponse:
     r"""OK"""
     
-    results: Optional[list[shared_modelsevaluationresult.ModelsEvaluationResult]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})  
+    results: Optional[list[shared_modelsevaluationresult.ModelsEvaluationResult]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/shared/apireplaceruleresponse.py` & `brease-sdk-1.1.1/src/sdk/models/shared/apireplaceruleresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class APIReplaceRuleResponse:
     r"""OK"""
     
-    rule: Optional[shared_modelsrule.ModelsRule] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rule'), 'exclude': lambda f: f is None }})  
+    rule: Optional[shared_modelsrule.ModelsRule] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rule'), 'exclude': lambda f: f is None }})
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/shared/condition.py` & `brease-sdk-1.1.1/src/sdk/models/shared/condition.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ConditionBase2:
     
-    ref: Optional[shared_conditionbaseref.ConditionBaseRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ref'), 'exclude': lambda f: f is None }})  
+    ref: Optional[shared_conditionbaseref.ConditionBaseRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ref'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Condition:
     
-    base: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('base'), 'exclude': lambda f: f is None }})  
-    parameter: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameter'), 'exclude': lambda f: f is None }})  
-    type: Optional[shared_conditiontype_enum.ConditionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})  
+    base: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('base'), 'exclude': lambda f: f is None }})
+    parameter: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameter'), 'exclude': lambda f: f is None }})
+    type: Optional[shared_conditiontype_enum.ConditionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/shared/conditionbaseref.py` & `brease-sdk-1.1.1/src/sdk/models/shared/conditionbaseref.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ConditionBaseRef:
     
-    dst: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dst'), 'exclude': lambda f: f is None }})  
-    src: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('src'), 'exclude': lambda f: f is None }})  
+    dst: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dst'), 'exclude': lambda f: f is None }})
+    src: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('src'), 'exclude': lambda f: f is None }})
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/shared/evaluaterulesinput.py` & `brease-sdk-1.1.1/src/sdk/models/shared/evaluaterulesinput.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class EvaluateRulesInput:
     
-    object: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object') }})  
-    override_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('overrideCode'), 'exclude': lambda f: f is None }})  
-    override_rules: Optional[list[shared_modelsrule.ModelsRule]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('overrideRules'), 'exclude': lambda f: f is None }})  
+    object: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object') }})
+    override_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('overrideCode'), 'exclude': lambda f: f is None }})
+    override_rules: Optional[list[shared_modelsrule.ModelsRule]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('overrideRules'), 'exclude': lambda f: f is None }})
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/shared/expressionarray.py` & `brease-sdk-1.1.1/src/sdk/models/shared/expressionarray.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ExpressionArrayExpression3:
     
-    condition: Optional[shared_condition.Condition] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('condition'), 'exclude': lambda f: f is None }})  
+    condition: Optional[shared_condition.Condition] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('condition'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ExpressionArrayExpression2:
     
-    or_: Optional[ExpressionArray] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('or'), 'exclude': lambda f: f is None }})  
+    or_: Optional[ExpressionArray] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('or'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ExpressionArrayExpression1:
     
-    and_: Optional[ExpressionArray] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('and'), 'exclude': lambda f: f is None }})  
+    and_: Optional[ExpressionArray] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('and'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ExpressionArray:
     
-    expression: Optional[list[Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expression'), 'exclude': lambda f: f is None }})  
+    expression: Optional[list[Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expression'), 'exclude': lambda f: f is None }})
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/shared/modelsevaluationresult.py` & `brease-sdk-1.1.1/src/sdk/models/shared/modelsevaluationresult.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ModelsEvaluationResult:
     
-    action: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('action'), 'exclude': lambda f: f is None }})  
-    action_target_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('actionTargetType'), 'exclude': lambda f: f is None }})  
-    target_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('targetID'), 'exclude': lambda f: f is None }})  
-    value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Value'), 'exclude': lambda f: f is None }})  
+    action: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('action'), 'exclude': lambda f: f is None }})
+    action_target_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('actionTargetType'), 'exclude': lambda f: f is None }})
+    target_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('targetID'), 'exclude': lambda f: f is None }})
+    value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Value'), 'exclude': lambda f: f is None }})
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/shared/modelsrule.py` & `brease-sdk-1.1.1/src/sdk/models/shared/modelsrule.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ModelsRuleExpression3:
     
-    condition: Optional[shared_condition.Condition] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('condition'), 'exclude': lambda f: f is None }})  
+    condition: Optional[shared_condition.Condition] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('condition'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ModelsRuleExpression2:
     
-    or_: Optional[shared_expressionarray.ExpressionArray] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('or'), 'exclude': lambda f: f is None }})  
+    or_: Optional[shared_expressionarray.ExpressionArray] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('or'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ModelsRuleExpression1:
     
-    and_: Optional[shared_expressionarray.ExpressionArray] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('and'), 'exclude': lambda f: f is None }})  
+    and_: Optional[shared_expressionarray.ExpressionArray] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('and'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ModelsRule:
     
-    action: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('action') }})  
-    expression: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expression') }})  
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    target: shared_modelstarget.ModelsTarget = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('target') }})  
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
+    action: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('action') }})
+    expression: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expression') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    target: shared_modelstarget.ModelsTarget = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('target') }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
```

### Comparing `brease-sdk-1.1.0/src/sdk/models/shared/modelstarget.py` & `brease-sdk-1.1.1/src/sdk/models/shared/modelstarget.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ModelsTarget:
     
-    target: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('target') }})  
-    type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
-    target_value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('targetValue'), 'exclude': lambda f: f is None }})  
+    target: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('target') }})
+    type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    target_value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('targetValue'), 'exclude': lambda f: f is None }})
```

### Comparing `brease-sdk-1.1.0/src/sdk/sdk.py` & `brease-sdk-1.1.1/src/sdk/sdk.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     context_id: ContextID
     r"""Rule domain context"""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "1.1.0"
-    _gen_version: str = "2.19.1"
+    _sdk_version: str = "1.1.1"
+    _gen_version: str = "2.23.4"
 
     def __init__(self,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
```

### Comparing `brease-sdk-1.1.0/src/sdk/utils/retries.py` & `brease-sdk-1.1.1/src/sdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.0/src/sdk/utils/utils.py` & `brease-sdk-1.1.1/src/sdk/utils/utils.py`

 * *Files identical despite different names*


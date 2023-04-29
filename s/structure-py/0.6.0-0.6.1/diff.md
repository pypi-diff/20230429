# Comparing `tmp/structure_py-0.6.0.tar.gz` & `tmp/structure_py-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structure_py-0.6.0.tar", last modified: Fri Apr 28 01:00:45 2023, max compression
+gzip compressed data, was "structure_py-0.6.1.tar", last modified: Sat Apr 29 00:58:07 2023, max compression
```

## Comparing `structure_py-0.6.0.tar` & `structure_py-0.6.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:00:45.209058 structure_py-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-28 01:00:30.000000 structure_py-0.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-28 01:00:45.205058 structure_py-0.6.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3703 2023-04-28 01:00:30.000000 structure_py-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:00:45.209058 structure_py-0.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-28 01:00:30.000000 structure_py-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:00:45.205058 structure_py-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:00:45.205058 structure_py-0.6.0/src/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4614 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/companies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:00:45.205058 structure_py-0.6.0/src/sdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:00:45.205058 structure_py-0.6.0/src/sdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      700 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/operations/enrich_company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      706 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/operations/enrich_person.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1089 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/operations/list_employees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/operations/list_jobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      486 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/operations/list_users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      975 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/operations/login.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/operations/me.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/operations/search_companies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1522 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/operations/search_people.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:00:45.205058 structure_py-0.6.0/src/sdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/shared/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2625 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/shared/company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7483 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/shared/person.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      334 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2695 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/people.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3225 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2603 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:00:45.205058 structure_py-0.6.0/src/sdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-28 01:00:30.000000 structure_py-0.6.0/src/sdk/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:00:45.205058 structure_py-0.6.0/src/structure_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-28 01:00:45.000000 structure_py-0.6.0/src/structure_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-28 01:00:45.000000 structure_py-0.6.0/src/structure_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:00:45.000000 structure_py-0.6.0/src/structure_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 01:00:45.000000 structure_py-0.6.0/src/structure_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 01:00:45.000000 structure_py-0.6.0/src/structure_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:58:07.275996 structure_py-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 00:57:50.000000 structure_py-0.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-29 00:58:07.275996 structure_py-0.6.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3703 2023-04-29 00:57:50.000000 structure_py-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 00:58:07.275996 structure_py-0.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-29 00:57:50.000000 structure_py-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:58:07.267996 structure_py-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:58:07.271996 structure_py-0.6.1/src/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4614 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/companies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:58:07.271996 structure_py-0.6.1/src/sdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:58:07.271996 structure_py-0.6.1/src/sdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      695 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/operations/enrich_company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      701 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/operations/enrich_person.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/operations/list_employees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1072 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/operations/list_jobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      482 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/operations/list_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      969 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/operations/login.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/operations/me.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1531 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/operations/search_companies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1514 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/operations/search_people.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:58:07.271996 structure_py-0.6.1/src/sdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/shared/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2597 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/shared/company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7409 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/shared/person.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2695 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/people.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3225 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2603 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:58:07.271996 structure_py-0.6.1/src/sdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-29 00:57:50.000000 structure_py-0.6.1/src/sdk/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:58:07.275996 structure_py-0.6.1/src/structure_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-29 00:58:07.000000 structure_py-0.6.1/src/structure_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-29 00:58:07.000000 structure_py-0.6.1/src/structure_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:58:07.000000 structure_py-0.6.1/src/structure_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 00:58:07.000000 structure_py-0.6.1/src/structure_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-29 00:58:07.000000 structure_py-0.6.1/src/structure_py.egg-info/top_level.txt
```

### Comparing `structure_py-0.6.0/LICENSE.md` & `structure_py-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `structure_py-0.6.0/PKG-INFO` & `structure_py-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structure_py
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Structure
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structure_py Version: 0.6.0 Summary: Python Client
+Metadata-Version: 2.1 Name: structure_py Version: 0.6.1 Summary: Python Client
 SDK Generated by Speakeasy Home-page: UNKNOWN Author: Structure License:
 UNKNOWN Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE.md
    [https://user-images.githubusercontent.com/6267663/229523981-b357a689-adc6-
                          4905-ac0e-e432aee5800b.png]
                            ****** Python SDK ******
                Discover rich information on people and companies
```

### Comparing `structure_py-0.6.0/README.md` & `structure_py-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `structure_py-0.6.0/setup.py` & `structure_py-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="structure_py",
-    version="0.6.0",
+    version="0.6.1",
     author="Structure",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `structure_py-0.6.0/src/sdk/accounts.py` & `structure_py-0.6.1/src/sdk/accounts.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.6.0/src/sdk/companies.py` & `structure_py-0.6.1/src/sdk/companies.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.6.0/src/sdk/models/operations/__init__.py` & `structure_py-0.6.1/src/sdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.6.0/src/sdk/models/operations/enrich_company.py` & `structure_py-0.6.1/src/sdk/models/operations/list_employees.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from typing import Optional
 
 
 @dataclasses.dataclass
-class EnrichCompanyRequest:
+class ListEmployeesRequest:
     
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
-
     r"""ID of the company"""
+    offset: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
+    r"""The offset number to start at"""
+    per_page: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'per_page', 'style': 'form', 'explode': True }})
+    r"""Number of results per page (0-100)"""
     
 
 @dataclasses.dataclass
-class EnrichCompanyResponse:
+class ListEmployeesResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     body: Optional[bytes] = dataclasses.field(default=None)
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `structure_py-0.6.0/src/sdk/models/operations/enrich_person.py` & `structure_py-0.6.1/src/sdk/models/operations/list_jobs.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from typing import Optional
 
 
 @dataclasses.dataclass
-class EnrichPersonRequest:
+class ListJobsRequest:
     
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
-
-    r"""LinkedIn ID of the person"""
+    r"""ID of the company"""
+    offset: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
+    r"""The offset number to start at"""
+    per_page: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'per_page', 'style': 'form', 'explode': True }})
+    r"""Number of results per page (0-100)"""
     
 
 @dataclasses.dataclass
-class EnrichPersonResponse:
+class ListJobsResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     body: Optional[bytes] = dataclasses.field(default=None)
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `structure_py-0.6.0/src/sdk/models/operations/list_employees.py` & `structure_py-0.6.1/src/sdk/models/operations/enrich_person.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,32 +3,21 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListEmployeesRequest:
+class EnrichPersonRequest:
     
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
-
-    r"""ID of the company"""
-    offset: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
-
-    r"""The offset number to start at"""
-    per_page: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'per_page', 'style': 'form', 'explode': True }})
-
-    r"""Number of results per page (0-100)"""
+    r"""LinkedIn ID of the person"""
     
 
 @dataclasses.dataclass
-class ListEmployeesResponse:
+class EnrichPersonResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     body: Optional[bytes] = dataclasses.field(default=None)
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `structure_py-0.6.0/src/sdk/models/operations/login.py` & `structure_py-0.6.1/src/sdk/models/operations/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,20 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class LoginApplicationJSON:
     
     email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
-
     r"""The email of the user"""
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""The password of the user"""
     
 
 @dataclasses.dataclass
 class LoginResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     body: Optional[bytes] = dataclasses.field(default=None)
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `structure_py-0.6.0/src/sdk/models/operations/search_companies.py` & `structure_py-0.6.1/src/sdk/models/operations/search_companies.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,32 +9,24 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCompaniesApplicationJSON:
     
     filter: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filter'), 'exclude': lambda f: f is None }})
-
     r"""Filter for searching"""
     limit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('limit'), 'exclude': lambda f: f is None }})
-
     r"""Number of results per page (0-100) default 10"""
     page: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('page'), 'exclude': lambda f: f is None }})
-
     r"""The offset number to start at"""
     query: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query'), 'exclude': lambda f: f is None }})
-
     r"""Query for searching"""
     
 
 @dataclasses.dataclass
 class SearchCompaniesResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     body: Optional[bytes] = dataclasses.field(default=None)
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `structure_py-0.6.0/src/sdk/models/operations/search_people.py` & `structure_py-0.6.1/src/sdk/models/operations/search_people.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,32 +9,24 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchPeopleApplicationJSON:
     
     filter: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filter'), 'exclude': lambda f: f is None }})
-
     r"""Filter for searching"""
     limit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('limit'), 'exclude': lambda f: f is None }})
-
     r"""Number of results per page (0-100)"""
     page: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('page'), 'exclude': lambda f: f is None }})
-
     r"""The offset number to start at"""
     query: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query'), 'exclude': lambda f: f is None }})
-
     r"""Query for searching"""
     
 
 @dataclasses.dataclass
 class SearchPeopleResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     body: Optional[bytes] = dataclasses.field(default=None)
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `structure_py-0.6.0/src/sdk/models/shared/account.py` & `structure_py-0.6.1/src/sdk/models/shared/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,21 @@
 import dataclasses
 
 
 @dataclasses.dataclass
 class Account:
     
     account_users: list[str] = dataclasses.field()
-
     r"""List of the users in the account"""
     created_at: str = dataclasses.field()
-
     r"""Timestamp of the account creation date"""
     id: float = dataclasses.field()
-
     r"""The id of the account"""
     name: str = dataclasses.field()
-
     r"""The name of the account"""
     owner_id: float = dataclasses.field()
-
     r"""The id of the account owner"""
     personal: bool = dataclasses.field()
-
     r"""If the account is personal or belonging to another account"""
     updated_at: str = dataclasses.field()
-
     r"""Timestamp of the last account update date"""
```

### Comparing `structure_py-0.6.0/src/sdk/models/shared/company.py` & `structure_py-0.6.1/src/sdk/models/shared/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,91 +5,63 @@
 
 
 @dataclasses.dataclass
 class Company:
     r"""returns the company"""
     
     about: str = dataclasses.field()
-
     r"""The company's description"""
     affiliated: list[str] = dataclasses.field()
-
     r"""Affiliated companies to the company"""
     company_size: str = dataclasses.field()
-
     r"""The size of the company"""
     country_code: str = dataclasses.field()
-
     r"""The country's country code"""
     employees: list[str] = dataclasses.field()
-
     r"""A sample of the company's employees. See the employees endpoint for the full list."""
     employees_in_linkedin: float = dataclasses.field()
-
     r"""The number of company employees on LinkedIn"""
     followers: float = dataclasses.field()
-
     r"""The number of company followers on LinkedIn"""
     founded: float = dataclasses.field()
-
     r"""The year the company was founded"""
     funding: str = dataclasses.field()
-
     r"""The funding status of the company"""
     headquarters: str = dataclasses.field()
-
     r"""The country's headquarters"""
     id: float = dataclasses.field()
-
     r"""The key for looking up the company"""
     industries: str = dataclasses.field()
-
     r"""The company's industries"""
     investors: str = dataclasses.field()
-
     r"""The company's investors"""
     jobs: list[str] = dataclasses.field()
-
     r"""Sample of company's Jobs. See the jobs endpoint for the full list."""
     lid: str = dataclasses.field()
-
     r"""The company's LinkedIn ID"""
     locations: list[str] = dataclasses.field()
-
     r"""The company's locations"""
     logo: str = dataclasses.field()
-
     r"""URL to the company's logo"""
     name: str = dataclasses.field()
-
     r"""The company's name"""
     organization_type: str = dataclasses.field()
-
     r"""The type of organization"""
     profiles: list[str] = dataclasses.field()
-
     r"""The company's profiles"""
     region: str = dataclasses.field()
-
     r"""The comapny's headquarters region"""
     similar: list[str] = dataclasses.field()
-
     r"""Similar companies to this company"""
     slogan: str = dataclasses.field()
-
     r"""The company's slogan"""
     specialities: str = dataclasses.field()
-
     r"""The company's specialities"""
     sphere: str = dataclasses.field()
-
     r"""The company's sphere of products"""
     type: str = dataclasses.field()
-
     r"""The type of company (public, private, etc.)"""
     url: str = dataclasses.field()
-
     r"""The company's linkedIn URL"""
     website: str = dataclasses.field()
-
     r"""The company's website"""
```

### Comparing `structure_py-0.6.0/src/sdk/models/shared/person.py` & `structure_py-0.6.1/src/sdk/models/shared/person.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,229 +5,155 @@
 
 
 @dataclasses.dataclass
 class Person:
     r"""returns the person"""
     
     birth_date: str = dataclasses.field()
-
     r"""The birth date of the person"""
     birth_year: float = dataclasses.field()
-
     r"""The birth year of the person"""
     certifications: list[str] = dataclasses.field()
-
     r"""The certifications of the person"""
     education: list[str] = dataclasses.field()
-
     r"""The educational history of the person"""
     emails: list[str] = dataclasses.field()
-
     r"""The personal and work emails of the person"""
     experience: list[str] = dataclasses.field()
-
     r"""The works experience of the person"""
     facebook_id: str = dataclasses.field()
-
     r"""The Facebook ID of the person"""
     facebook_url: str = dataclasses.field()
-
     r"""The Facebook URL of the person"""
     facebook_username: str = dataclasses.field()
-
     r"""The Facebook username of the person"""
     first_name: str = dataclasses.field()
-
     r"""The first name of the person"""
     full_name: str = dataclasses.field()
-
     r"""The full name of the person"""
     gender: str = dataclasses.field()
-
     r"""The gender of the person"""
     github_url: str = dataclasses.field()
-
     r"""The Github URL of the person"""
     github_username: str = dataclasses.field()
-
     r"""The Github username of the person"""
     id: float = dataclasses.field()
-
     r"""The key for looking up the company"""
     industry: str = dataclasses.field()
-
     r"""The industry of the person"""
     inferred_salary: str = dataclasses.field()
-
     r"""The inferred salary band for the person"""
     inferred_years_experience: float = dataclasses.field()
-
     r"""The inferred years of experience for the person"""
     interests: list[str] = dataclasses.field()
-
     r"""The interests of the person"""
     job_company_facebook_url: str = dataclasses.field()
-
     r"""The current job company Facebook URL"""
     job_company_founded: str = dataclasses.field()
-
     r"""The current job company founded year"""
     job_company_id: str = dataclasses.field()
-
     r"""The current job company ID"""
     job_company_industry: str = dataclasses.field()
-
     r"""The current job company industry"""
     job_company_linkedin_id: str = dataclasses.field()
-
     r"""The current job company id on LinkedIn"""
     job_company_linkedin_url: str = dataclasses.field()
-
     r"""The current job company LinkedIn URL"""
     job_company_location_address_line_2: str = dataclasses.field()
-
     r"""The current job company location street adress second line"""
     job_company_location_continent: str = dataclasses.field()
-
     r"""The current job company location continent"""
     job_company_location_country: str = dataclasses.field()
-
     r"""The current job company location country"""
     job_company_location_geo: str = dataclasses.field()
-
     r"""The current job company location geo coordinates"""
     job_company_location_locality: str = dataclasses.field()
-
     r"""The current job company location city"""
     job_company_location_metro: str = dataclasses.field()
-
     r"""The current job company location metro"""
     job_company_location_name: str = dataclasses.field()
-
     r"""The current job company location name"""
     job_company_location_postal_code: str = dataclasses.field()
-
     r"""The current job company location postal code"""
     job_company_location_region: str = dataclasses.field()
-
     r"""The current job company location region"""
     job_company_location_street_address: str = dataclasses.field()
-
     r"""The current job company location street address"""
     job_company_name: str = dataclasses.field()
-
     r"""The current job company name"""
     job_company_size: str = dataclasses.field()
-
     r"""The current job company size"""
     job_company_twitter_url: str = dataclasses.field()
-
     r"""The current job company Twitter URL"""
     job_company_website: str = dataclasses.field()
-
     r"""The current job company website"""
     job_last_updated: str = dataclasses.field()
-
     r"""The last update date for the job"""
     job_start_date: str = dataclasses.field()
-
     r"""The start date for the current job"""
     job_summary: str = dataclasses.field()
-
     r"""The summary for the current job"""
     job_title: str = dataclasses.field()
-
     r"""The current job title of the person"""
     job_title_levels: list[str] = dataclasses.field()
-
     r"""The current job title levels"""
     job_title_role: str = dataclasses.field()
-
     r"""The current job title role of the person"""
     job_title_sub_role: str = dataclasses.field()
-
     r"""The current job title sub-role of the person"""
     languages: list[str] = dataclasses.field()
-
     r"""The languages of the person"""
     last_name: str = dataclasses.field()
-
     r"""The last name of the person"""
     linkedin_connections: float = dataclasses.field()
-
     r"""The number of LinkedIn connections for the person"""
     linkedin_id: float = dataclasses.field()
-
     r"""The linkedIn ID of the person"""
     linkedin_url: str = dataclasses.field()
-
     r"""The linkedIn URL of the person"""
     linkedin_username: str = dataclasses.field()
-
     r"""The linkedIn user name of the person"""
     location_address_line_two: str = dataclasses.field()
-
     r"""The current location street address second line for the person"""
     location_continent: str = dataclasses.field()
-
     r"""The current location continent for the person"""
     location_country: str = dataclasses.field()
-
     r"""The current location country for the person"""
     location_geo: list[str] = dataclasses.field()
-
     r"""The current location geo coordinates for the person"""
     location_last_updated: str = dataclasses.field()
-
     r"""The current location last updated date for the person"""
     location_locality: str = dataclasses.field()
-
     r"""The current location city for the person"""
     location_metro: str = dataclasses.field()
-
     r"""The current location metro for the person"""
     location_name: str = dataclasses.field()
-
     r"""The current location name for the person"""
     location_postal_code: str = dataclasses.field()
-
     r"""The current location postal code for the person"""
     location_region: str = dataclasses.field()
-
     r"""The current location region for the person"""
     location_street_address: str = dataclasses.field()
-
     r"""The current location street address for the person"""
     middle_initial: str = dataclasses.field()
-
     r"""The middle initial of the person"""
     middle_name: str = dataclasses.field()
-
     r"""The middle name of the person"""
     mobile_phone: str = dataclasses.field()
-
     r"""The mobile phone of the person"""
     phone_numbers: list[str] = dataclasses.field()
-
     r"""The phone numbers of the person"""
     profiles: list[str] = dataclasses.field()
-
     r"""The social profiles of the person"""
     skills: list[str] = dataclasses.field()
-
     r"""The skills of the person"""
     street_addresses: list[str] = dataclasses.field()
-
     r"""The street addresses of the person"""
     summary: str = dataclasses.field()
-
     r"""The self-summary of the person's work experience"""
     twitter_url: str = dataclasses.field()
-
     r"""The Twitter URL of the person"""
     twitter_username: str = dataclasses.field()
-
     r"""The Twitter username of the person"""
     work_email: str = dataclasses.field()
-
     r"""The work email of the person"""
```

### Comparing `structure_py-0.6.0/src/sdk/people.py` & `structure_py-0.6.1/src/sdk/people.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.6.0/src/sdk/sdk.py` & `structure_py-0.6.1/src/sdk/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     user: User
     r"""User"""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.6.0"
-    _gen_version: str = "2.23.2"
+    _sdk_version: str = "0.6.1"
+    _gen_version: str = "2.23.4"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `structure_py-0.6.0/src/sdk/user.py` & `structure_py-0.6.1/src/sdk/user.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.6.0/src/sdk/utils/retries.py` & `structure_py-0.6.1/src/sdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.6.0/src/sdk/utils/utils.py` & `structure_py-0.6.1/src/sdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.6.0/src/structure_py.egg-info/PKG-INFO` & `structure_py-0.6.1/src/structure_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structure-py
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Structure
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structure-py Version: 0.6.0 Summary: Python Client
+Metadata-Version: 2.1 Name: structure-py Version: 0.6.1 Summary: Python Client
 SDK Generated by Speakeasy Home-page: UNKNOWN Author: Structure License:
 UNKNOWN Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE.md
    [https://user-images.githubusercontent.com/6267663/229523981-b357a689-adc6-
                          4905-ac0e-e432aee5800b.png]
                            ****** Python SDK ******
                Discover rich information on people and companies
```

### Comparing `structure_py-0.6.0/src/structure_py.egg-info/SOURCES.txt` & `structure_py-0.6.1/src/structure_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*


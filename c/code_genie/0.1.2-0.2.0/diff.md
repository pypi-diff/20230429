# Comparing `tmp/code_genie-0.1.2.tar.gz` & `tmp/code_genie-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_genie-0.1.2.tar", last modified: Thu Apr 27 10:15:44 2023, max compression
+gzip compressed data, was "code_genie-0.2.0.tar", last modified: Sat Apr 29 16:20:51 2023, max compression
```

## Comparing `code_genie-0.1.2.tar` & `code_genie-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,40 @@
--rw-r--r--   0        0        0      399 2023-04-27 10:15:39.146621 code_genie-0.1.2/.bumpversion.cfg
--rw-r--r--   0        0        0     1831 2023-04-25 05:29:52.444630 code_genie-0.1.2/.gitignore
--rw-r--r--   0        0        0      635 2023-04-27 10:15:39.147415 code_genie-0.1.2/.readthedocs.yaml
--rw-r--r--   0        0        0       91 2023-04-25 05:29:52.445152 code_genie-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-04-20 10:01:19.112941 code_genie-0.1.2/LICENSE
--rw-r--r--   0        0        0     1556 2023-04-27 10:15:39.147818 code_genie-0.1.2/README.md
--rw-r--r--   0        0        0      456 2023-04-25 05:29:52.446244 code_genie-0.1.2/TODO.md
--rw-r--r--   0        0        0       72 2023-04-27 10:15:39.148170 code_genie-0.1.2/code_genie/__init__.py
--rw-r--r--   0        0        0     1752 2023-04-25 05:29:52.447321 code_genie-0.1.2/code_genie/client.py
--rw-r--r--   0        0        0     5153 2023-04-27 10:15:39.149106 code_genie-0.1.2/code_genie/genie.py
--rw-r--r--   0        0        0      679 2023-04-27 10:15:39.149821 code_genie-0.1.2/docs/Makefile
--rw-r--r--   0        0        0       92 2023-04-27 10:15:39.151209 code_genie-0.1.2/docs/api.rst
--rw-r--r--   0        0        0     1492 2023-04-27 10:15:39.151752 code_genie-0.1.2/docs/conf.py
--rw-r--r--   0        0        0       81 2023-04-27 10:15:39.152197 code_genie-0.1.2/docs/examples.rst
--rw-r--r--   0        0        0      284 2023-04-27 10:15:39.153008 code_genie-0.1.2/docs/generated/code_genie.client.rst
--rw-r--r--   0        0        0      226 2023-04-27 10:15:39.153533 code_genie-0.1.2/docs/generated/code_genie.genie.rst
--rw-r--r--   0        0        0      123 2023-04-27 10:15:39.154001 code_genie-0.1.2/docs/genie.rst
--rw-r--r--   0        0        0     1110 2023-04-27 10:15:39.154405 code_genie-0.1.2/docs/index.rst
--rw-r--r--   0        0        0      800 2023-04-27 10:15:39.155023 code_genie-0.1.2/docs/make.bat
--rw-r--r--   0        0        0    73251 2023-04-27 10:15:39.156165 code_genie-0.1.2/docs/notebooks/Starter.ipynb
--rw-r--r--   0        0        0       54 2023-04-27 10:15:39.156660 code_genie-0.1.2/docs/requirements.in
--rw-r--r--   0        0        0     3100 2023-04-27 10:15:39.156993 code_genie-0.1.2/docs/requirements.txt
--rw-r--r--   0        0        0     1212 2023-04-27 10:15:39.157311 code_genie-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 05:29:52.448133 code_genie-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      861 2023-04-27 07:56:53.649350 code_genie-0.1.2/tests/test_genie.py
--rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 code_genie-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      399 2023-04-29 16:20:39.492222 code_genie-0.2.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1871 2023-04-29 16:20:39.492906 code_genie-0.2.0/.gitignore
+-rw-r--r--   0        0        0      635 2023-04-27 10:15:39.147415 code_genie-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0       91 2023-04-25 05:29:52.445152 code_genie-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-04-20 10:01:19.112941 code_genie-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1549 2023-04-29 16:20:39.493569 code_genie-0.2.0/README.md
+-rw-r--r--   0        0        0      484 2023-04-29 16:20:39.494222 code_genie-0.2.0/TODO.md
+-rw-r--r--   0        0        0      240 2023-04-29 16:20:39.494897 code_genie-0.2.0/code_genie/__init__.py
+-rw-r--r--   0        0        0     3041 2023-04-29 16:20:39.495446 code_genie-0.2.0/code_genie/_cache.py
+-rw-r--r--   0        0        0     1678 2023-04-29 16:20:39.496137 code_genie-0.2.0/code_genie/client.py
+-rw-r--r--   0        0        0       89 2023-04-29 16:20:39.496555 code_genie-0.2.0/code_genie/genie/__init__.py
+-rw-r--r--   0        0        0     4705 2023-04-29 16:20:39.497081 code_genie-0.2.0/code_genie/genie/base.py
+-rw-r--r--   0        0        0      501 2023-04-29 16:20:39.497458 code_genie-0.2.0/code_genie/genie/genie.py
+-rw-r--r--   0        0        0     3407 2023-04-29 16:20:39.497737 code_genie-0.2.0/code_genie/genie/pandas.py
+-rw-r--r--   0        0        0      679 2023-04-27 10:15:39.149821 code_genie-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0       92 2023-04-27 10:15:39.151209 code_genie-0.2.0/docs/api.rst
+-rw-r--r--   0        0        0     1492 2023-04-27 10:15:39.151752 code_genie-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0       81 2023-04-27 10:15:39.152197 code_genie-0.2.0/docs/examples.rst
+-rw-r--r--   0        0        0      284 2023-04-27 10:15:39.153008 code_genie-0.2.0/docs/generated/code_genie.client.rst
+-rw-r--r--   0        0        0      226 2023-04-27 10:15:39.153533 code_genie-0.2.0/docs/generated/code_genie.genie.rst
+-rw-r--r--   0        0        0      123 2023-04-27 10:15:39.154001 code_genie-0.2.0/docs/genie.rst
+-rw-r--r--   0        0        0     1110 2023-04-27 10:15:39.154405 code_genie-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-04-27 10:15:39.155023 code_genie-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0    64853 2023-04-29 16:20:39.498904 code_genie-0.2.0/docs/notebooks/Starter.ipynb
+-rw-r--r--   0        0        0     1619 2023-04-29 16:20:39.499378 code_genie-0.2.0/docs/notebooks/_cache_starter/_meta.json
+-rw-r--r--   0        0        0      173 2023-04-29 16:20:39.499698 code_genie-0.2.0/docs/notebooks/_cache_starter/count_high_earners_86151.py
+-rw-r--r--   0        0        0       90 2023-04-29 16:20:39.499976 code_genie-0.2.0/docs/notebooks/_cache_starter/count_missing_35951.py
+-rw-r--r--   0        0        0      466 2023-04-29 16:20:39.500316 code_genie-0.2.0/docs/notebooks/_cache_starter/generate_employee_df_41317.py
+-rw-r--r--   0        0        0      247 2023-04-29 16:20:39.500621 code_genie-0.2.0/docs/notebooks/_cache_starter/make_boxplots_25996.py
+-rw-r--r--   0        0        0      485 2023-04-29 16:20:39.500926 code_genie-0.2.0/docs/notebooks/_cache_starter/make_salaries_missing_76197.py
+-rw-r--r--   0        0        0      419 2023-04-29 16:20:39.501241 code_genie-0.2.0/docs/notebooks/_cache_starter/plot_salary_distribution_54098.py
+-rw-r--r--   0        0        0       54 2023-04-27 10:15:39.156660 code_genie-0.2.0/docs/requirements.in
+-rw-r--r--   0        0        0     3100 2023-04-27 10:15:39.156993 code_genie-0.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1212 2023-04-27 10:15:39.157311 code_genie-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 05:29:52.448133 code_genie-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      475 2023-04-29 16:20:39.501753 code_genie-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1559 2023-04-29 16:20:39.502197 code_genie-0.2.0/tests/test_cache.py
+-rw-r--r--   0        0        0      776 2023-04-29 16:20:39.502598 code_genie-0.2.0/tests/test_genie.py
+-rw-r--r--   0        0        0      839 2023-04-29 16:20:39.503091 code_genie-0.2.0/tox.ini
+-rw-r--r--   0        0        0     3021 1970-01-01 00:00:00.000000 code_genie-0.2.0/PKG-INFO
```

### Comparing `code_genie-0.1.2/.gitignore` & `code_genie-0.2.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -129,7 +129,11 @@
 .pyre/
 
 # intellij
 .idea/
 
 # keys
 key/
+
+# test cache
+tests/_cache
+test_reports
```

### Comparing `code_genie-0.1.2/.readthedocs.yaml` & `code_genie-0.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.2/LICENSE` & `code_genie-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.2/README.md` & `code_genie-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # code-genie
 This library is your copilot for jupyter notebooks
 
-Latest version: 0.1.2
+Latest version: 0.2.0
 
 ## Documentation
 
-- [Started Notebook](https://code-genie.readthedocs.io/en/latest/notebooks/Starter.html)
-- [All Exampples](https://code-genie.readthedocs.io/en/latest/examples.html)
-- [API Documentation](https://code-genie.readthedocs.io/en/latest/api.html)
+- [Starter Notebook](https://code-genie.readthedocs.io/en/main/notebooks/Starter.html)
+- [All Examples](https://code-genie.readthedocs.io/en/main/examples.html)
+- [API Documentation](https://code-genie.readthedocs.io/en/main/api.html)
 
 ## Installation
 
 ```bash
 pip install code-genie
 ```
```

### Comparing `code_genie-0.1.2/code_genie/client.py` & `code_genie-0.2.0/code_genie/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 import os
-from typing import Union, List, Dict, Tuple, Optional
+from typing import Dict, List, Optional, Tuple, Union
 from uuid import UUID
 
 import requests
 from pydantic import BaseModel
 
 
 class GetExecutableRequest(BaseModel):
     instructions: Union[str, List[str]]
     inputs: Dict[str, str]
     allowed_imports: Optional[List[str]] = None
 
 
-class GetPandasExecutableRequest(BaseModel):
-    instructions: Union[str, List[str]]
+class GetPandasExecutableRequest(GetExecutableRequest):
     inputs: Optional[Dict[str, str]] = None
-    allowed_imports: Optional[List[str]] = None
     columns: Optional[List[str]] = None
 
 
 class GetExecutableResponse(BaseModel):
     id: UUID
     code: str
     fn_name: str
 
 
 class Client:
-
     TOKEN_ENV_VAR = "CODE_GENIE_TOKEN"
     URL = "https://code-scribe-pzj44qvhfa-el.a.run.app"
     ENDPOINT_GENERIC = "get-executable/generic"
     ENDPOINT_PANDAS = "get-executable/pandas"
 
-    def __init__(self):
-        self._token = os.environ[self.TOKEN_ENV_VAR]
+    def __init__(self, token: Optional[str] = None):
+        self._token = token or os.environ[self.TOKEN_ENV_VAR]
 
     def _get_response(self, endpoint, data):
-        headers = {
-            "token": self._token,
-            "Content-Type": "application/json"
-        }
+        headers = {"token": self._token, "Content-Type": "application/json"}
         response = requests.post(url=f"{self.URL}/{endpoint}", data=data.json(), headers=headers)
         # if error found, raise the error
         response.raise_for_status()
         return GetExecutableResponse.parse_obj(response.json())
 
     def get_generic(self, request: GetExecutableRequest) -> Tuple[str, str]:
         # send a request with given data
```

### Comparing `code_genie-0.1.2/code_genie/genie.py` & `code_genie-0.2.0/code_genie/genie/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,67 @@
+import random
 from abc import ABC, abstractmethod
-from typing import Union, List, Dict, Callable, Tuple, Optional
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-from code_genie.client import Client, GetExecutableRequest, GetPandasExecutableRequest
+from code_genie._cache import _CacheManager, _CacheValue
+from code_genie.client import Client
 
 
 class GenieBase(ABC):
-
-    def __init__(self,
-                 instructions: Union[str, List[str]],
-                 inputs: Dict[str, str],
-                 allowed_imports: Optional[List[str]] = None,
-                 client: Optional[Client] = None):
+    def __init__(
+        self,
+        instructions: Union[str, List[str]],
+        inputs: Optional[Dict[str, str]] = None,
+        allowed_imports: Optional[List[str]] = None,
+        override: bool = False,
+        client: Optional[Client] = None,
+        cache_dir: Optional[str] = None,
+    ):
         """Initialize a genie instance
 
         Args:
             instructions: text instructions on the task required to be performed. use the keywords in inputs argument
                 to refer to the inputs.
             inputs: a dictionary of inputs to the function. the keys are the names of the inputs and the values are
                 small description of the inputs.
             allowed_imports: a list of imports which are allowed to be used in the code. note that this is not
-                strictly enforced yet. but it should work most of the times.
+                strictly enforced yet, but simplpy passed to the GPT API in the prompt.
+            override: if a genie has been generated before with the same args, then it will be loaded from cache be
+                default. set override to True to make a new API call and recreate the genie.
             client: an instance of the client to use for making requests to the api. if not provided, a new instance
                 will be created.
+            cache_dir: if provided, the code generated by the genie will be cached in this directory. if not
+                provided, the global default is used. it is recommended to use set_cache_dir() method to set this.
 
         Returns:
             A callable which can be used to execute the code generated by the genie.
         """
         self._inputs = inputs
         if isinstance(instructions, str):
             instructions = [instructions]
         self._instructions = instructions
         self._allowed_imports = allowed_imports
+
+        # check cache
+        cache = _CacheManager(cache_dir)
+        cache_key = self._get_hash_str()
+        cache_value = cache.get(cache_key)
+        self._filename = cache_value.filename if cache_value else self._generate_export_filename()
+        if not override:
+            if cache_value is not None:
+                print(f"Loading executor from cache file {cache_value.filename}, set override = True to rerun")
+                self._code = cache_value.code
+                self._fn_name = cache_value.fn_name
+                self._executor = self._extract_executable(self._code, self._fn_name)
+                return
+        # override or cache not found
         self._code, self._fn_name = self._get_code(client=client or Client())
         self._executor = self._extract_executable(self._code, self._fn_name)
+        cache.update(cache_key, _CacheValue(code=self._code, fn_name=self._fn_name, filename=self._filename))
+        print(f"Executor saved to cache file {self._filename}")
 
     @abstractmethod
     def _get_code(self, client: Client) -> Tuple[str, str]:
         raise NotImplementedError
 
     @classmethod
     def _extract_executable(cls, code: str, fn_name: str) -> Callable:
@@ -49,68 +74,38 @@
         return self._executor(*args, **kwargs)
 
     @property
     def code(self):
         """The code generated by the genie"""
         return self._code
 
+    def _generate_export_filename(self) -> str:
+        # use fn name with random 5 digit suffix
+        return f"{self._fn_name}_{random.randint(10000, 99999)}.py"
+
+    def _hash_attributes(self) -> List[Any]:
+        return [self._instructions, self._inputs, self._allowed_imports]
+
+    def _get_hash_str(self) -> str:
+        sep = "::"
+        hash_str = []
+        for attr in self._hash_attributes():
+            # if string, add as is
+            if isinstance(attr, str):
+                hash_str.append(attr)
+            # if list of str, then join using sep
+            elif isinstance(attr, list):
+                hash_str.append(sep.join(attr))
+            # if dict, then convert to tuple of items
+            elif isinstance(attr, dict):
+                hash_str.append(sep.join([f"{k}={v}" for k, v in attr.items()]))
+            # if None, return empty str
+            elif attr is None:
+                hash_str.append("")
+            else:
+                raise ValueError(f"Cannot hash attribute of type {type(attr)}")
+        return sep.join(hash_str)
 
-class Genie(GenieBase):
-    """A generic genie creator with no presets or additional functionality
-    """
-
-    def _get_code(self, client: Client) -> Tuple[str, str]:
-        return client.get_generic(
-            GetExecutableRequest(instructions=self._instructions,
-                                 inputs=self._inputs,
-                                 allowed_imports=self._allowed_imports))
-
-
-class PandasGenie(GenieBase):
-    """Pandas specific genie creator. This is specially configured to work with pandas dataframes.
-    """
-
-    def __init__(self,
-                 instructions: Union[str, List[str]],
-                 columns: Optional[List[str]] = None,
-                 inputs: Optional[Dict[str, str]] = None,
-                 allowed_imports: Optional[List[str]] = None,
-                 client: Optional[Client] = None):
-        """Initialize the Pandas Genie
-
-        Args:
-            instructions: text instructions on the task required to be performed. use the keywords in inputs argument
-                to refer to the inputs.
-            columns: a list of column names in the dataframe to be used as inputs. this helps the genie infer the
-                correct column name even if a slightly misspelled name is provided in the instructions.
-            inputs: a dictionary of inputs to the function. the keys are the names of the inputs and the values are
-                small description of the inputs. a default input of "df" referring to a pandas dataframe will be used
-                if not provided.
-            allowed_imports: a list of imports which are allowed to be used in the code. note that this is not
-                strictly enforced yet. default imports: ["pandas", "numpy", "math", "datetime", "matplotlib", "seaborn"]
-            client: an instance of the client to use for making requests to the api. if not provided, a new instance
-                will be created.
-
-        Returns:
-            A callable which can be used to execute the code generated by the genie.
-        """
-        self._columns = self._process_columns(columns)
-        super().__init__(instructions, inputs, allowed_imports, client)
-
-    @staticmethod
-    def _process_columns(columns: Optional[List[str]] = None) -> List[str]:
-        if columns is None:
-            return columns
-        # check input should be a list of strings
-        if isinstance(input, str):
-            raise TypeError("input should be an iterable, not a string")
-        elif all(isinstance(item, str) for item in columns):
-            return list(columns)
-        else:
-            raise TypeError("input should be an iterable of strings")
-
-    def _get_code(self, client: Client) -> Tuple[str, str]:
-        return client.get_pandas(
-            GetPandasExecutableRequest(instructions=self._instructions,
-                                       inputs=self._inputs,
-                                       columns=self._columns,
-                                       allowed_imports=self._allowed_imports))
+    @property
+    def filename(self):
+        """The filename of the cache file"""
+        return self._filename
```

### Comparing `code_genie-0.1.2/docs/Makefile` & `code_genie-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.2/docs/conf.py` & `code_genie-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.2/docs/index.rst` & `code_genie-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.2/docs/make.bat` & `code_genie-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.2/docs/notebooks/Starter.ipynb` & `code_genie-0.2.0/docs/notebooks/Starter.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.967504493388067%*

 * *Differences: {"'cells'": '{4: {\'source\': [\'load_dotenv("../../.env")  # replace with path to your env '*

 * *            "file']}, 5: {'id': 'd450035c-7bb4-47e9-b876-8e3564c0a003', 'source': {insert: [(0, "*

 * *            "'## setup cache\\n'), (2, 'By default the package will cache genie invocations in a "*

 * *            'temp file. This would mean that any genies created will be lost once you restart the '*

 * *            'kernel or rerun the notebook at another time. to keep the cached genies, you can set '*

 * *            'a custom […]*

```diff
@@ -1,10 +1,21 @@
 {
     "cells": [
         {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "7d9eda1b-110d-4a01-a3b9-57fcb5cd724f",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "%load_ext autoreload\n",
+                "%autoreload 2"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "id": "260d5faf-d4ea-4924-8623-af9ab1544598",
             "metadata": {},
             "source": [
                 "# Starter Notebook\n",
                 "\n",
                 "Use this notebook as a starting point for using the library."
@@ -50,97 +61,81 @@
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "load_dotenv(\"../.env\")  # replace with path to your env file"
+                "load_dotenv(\"../../.env\")  # replace with path to your env file"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b3dc2f0a-ca73-41e8-9a50-0672d1a58bc7",
+            "id": "d450035c-7bb4-47e9-b876-8e3564c0a003",
             "metadata": {},
             "source": [
-                "## Create data\n",
+                "## setup cache\n",
                 "\n",
-                "while you should import your own dataset, we can use code-genie to generate the data for this analysis"
+                "By default the package will cache genie invocations in a temp file. This would mean that any genies created will be lost once you restart the kernel or rerun the notebook at another time. to keep the cached genies, you can set a custom path where genies would be stored so that you will not lose them when you rerun the notebook.\n",
+                "\n",
+                "You can modify the cached code if you'd like and those modifications would be loaded the next time you run the code."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
-            "id": "d5bfbd38-e760-468b-8d14-11d18f183da8",
+            "id": "8a18da38-ec68-4ecc-95bc-58c8ecdfda51",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from code_genie import Genie, PandasGenie"
+                "from code_genie import set_cache_dir\n",
+                "set_cache_dir(\"./_cache_starter\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "b3dc2f0a-ca73-41e8-9a50-0672d1a58bc7",
+            "metadata": {},
+            "source": [
+                "## Create data\n",
+                "\n",
+                "while you should import your own dataset, we can use code-genie to generate the data for this analysis"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
-            "id": "91de25d6-84dd-4019-bfd9-60fe3582d169",
+            "id": "d5bfbd38-e760-468b-8d14-11d18f183da8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "data_gen = Genie(inputs=[],\n",
-                "                 instructions=[\"generate a pandas dataframe containing 100 rows with employee information with following columns:\",\n",
-                "                               \"id: random employee id\",\n",
-                "                               \"name: employee name\",\n",
-                "                               \"salary: salary per annum in USD\",\n",
-                "                               \"department: should be either engineering or product\"])"
+                "from code_genie.genie import Genie, PandasGenie"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
-            "id": "77a48d24-1edf-44f0-baa8-2f222cada1fe",
+            "id": "91de25d6-84dd-4019-bfd9-60fe3582d169",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "import pandas as pd\n",
-                        "import numpy as np\n",
-                        "\n",
-                        "def generate_employee_df():\n",
-                        "    \n",
-                        "    # Generate random employee IDs\n",
-                        "    ids = np.random.randint(1000, 9999, 100)\n",
-                        "    \n",
-                        "    # Generate random employee names\n",
-                        "    first_names = ['John', 'Jane', 'Sam', 'Samantha', 'William', 'Liam', 'Emma', 'Olivia']\n",
-                        "    last_names = ['Smith', 'Johnson', 'Brown', 'Garcia', 'Miller', 'Davis', 'Wilson', 'Lopez']\n",
-                        "    names = []\n",
-                        "    for i in range(100):\n",
-                        "        name = np.random.choice(first_names) + ' ' + np.random.choice(last_names)\n",
-                        "        names.append(name)\n",
-                        "    \n",
-                        "    # Generate random employee salaries\n",
-                        "    salaries = np.random.randint(50000, 250000, 100)\n",
-                        "    \n",
-                        "    # Generate random department assignments\n",
-                        "    departments = np.random.choice(['engineering', 'product'], 100)\n",
-                        "    \n",
-                        "    # Create the DataFrame\n",
-                        "    employee_df = pd.DataFrame({'ID': ids,\n",
-                        "                                'Name': names,\n",
-                        "                                'Salary': salaries,\n",
-                        "                                'Department': departments})\n",
-                        "    \n",
-                        "    return employee_df\n",
-                        "\n"
+                        "Loading executor from cache file generate_employee_df_41317.py, set override = True to rerun\n"
                     ]
                 }
             ],
             "source": [
-                "print(data_gen.code)"
+                "data_gen = Genie(instructions=[\"generate a pandas dataframe containing 100 rows with employee information with following columns:\",\n",
+                "                               \"id: random employee id\",\n",
+                "                               \"name: employee name\",\n",
+                "                               \"salary: salary per annum in USD\",\n",
+                "                               \"department: should be either engineering or product\"],\n",
+                "                override=False)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "id": "e7f67149-b53f-4c7f-9b4b-fc7e1972391f",
             "metadata": {},
@@ -184,67 +179,67 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>ID</th>\n",
-                            "      <th>Name</th>\n",
-                            "      <th>Salary</th>\n",
-                            "      <th>Department</th>\n",
+                            "      <th>id</th>\n",
+                            "      <th>name</th>\n",
+                            "      <th>salary</th>\n",
+                            "      <th>department</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>4554</td>\n",
-                            "      <td>Olivia Garcia</td>\n",
-                            "      <td>111675</td>\n",
+                            "      <td>9853</td>\n",
+                            "      <td>Employee_1</td>\n",
+                            "      <td>43446</td>\n",
                             "      <td>engineering</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>5812</td>\n",
-                            "      <td>Emma Lopez</td>\n",
-                            "      <td>97897</td>\n",
+                            "      <td>2444</td>\n",
+                            "      <td>Employee_2</td>\n",
+                            "      <td>142980</td>\n",
                             "      <td>engineering</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>9191</td>\n",
-                            "      <td>William Wilson</td>\n",
-                            "      <td>88243</td>\n",
-                            "      <td>product</td>\n",
+                            "      <td>1450</td>\n",
+                            "      <td>Employee_3</td>\n",
+                            "      <td>93806</td>\n",
+                            "      <td>engineering</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>9156</td>\n",
-                            "      <td>William Miller</td>\n",
-                            "      <td>113960</td>\n",
-                            "      <td>product</td>\n",
+                            "      <td>3799</td>\n",
+                            "      <td>Employee_4</td>\n",
+                            "      <td>125635</td>\n",
+                            "      <td>engineering</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>5926</td>\n",
-                            "      <td>Sam Davis</td>\n",
-                            "      <td>166372</td>\n",
-                            "      <td>product</td>\n",
+                            "      <td>3559</td>\n",
+                            "      <td>Employee_5</td>\n",
+                            "      <td>105519</td>\n",
+                            "      <td>engineering</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "     ID            Name  Salary   Department\n",
-                            "0  4554   Olivia Garcia  111675  engineering\n",
-                            "1  5812      Emma Lopez   97897  engineering\n",
-                            "2  9191  William Wilson   88243      product\n",
-                            "3  9156  William Miller  113960      product\n",
-                            "4  5926       Sam Davis  166372      product"
+                            "     id        name  salary   department\n",
+                            "0  9853  Employee_1   43446  engineering\n",
+                            "1  2444  Employee_2  142980  engineering\n",
+                            "2  1450  Employee_3   93806  engineering\n",
+                            "3  3799  Employee_4  125635  engineering\n",
+                            "4  3559  Employee_5  105519  engineering"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -261,79 +256,57 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "id": "9b04199c-2abe-4de4-a74f-eda4b14f572a",
             "metadata": {},
-            "outputs": [],
-            "source": [
-                "data_gen_add_missing = PandasGenie(\"make salaries for around 10% of the employees missing\",\n",
-                "                                   columns=list(df.columns))"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 10,
-            "id": "89dfcf18-1456-48e4-8564-ac5efc005ec8",
-            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "import numpy as np\n",
-                        "import pandas as pd\n",
-                        "\n",
-                        "def add_missing_salaries(df):\n",
-                        "    # get 10% of rows as integer\n",
-                        "    num_missing = int(len(df)*0.1)\n",
-                        "    # get list of random indices to set to NaN\n",
-                        "    random_indices = np.random.choice(df.index, num_missing, replace=False)\n",
-                        "    # set the chosen indices' salaries to NaN\n",
-                        "    df.loc[random_indices, 'Salary'] = np.nan\n",
-                        "    # return the updated dataframe\n",
-                        "    return df\n",
-                        "\n"
+                        "Executor saved to cache file make_salaries_missing_76197.py\n"
                     ]
                 }
             ],
             "source": [
-                "print(data_gen_add_missing.code)"
+                "data_gen_add_missing = PandasGenie(\"make salaries for around 10% of the employees missing\",\n",
+                "                                   columns=list(df.columns))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 10,
             "id": "1a408205-c16d-4799-b6a2-1ff0071972cc",
             "metadata": {},
             "outputs": [],
             "source": [
                 "df_missing = data_gen_add_missing(df)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 12,
             "id": "d47d0c97-f170-4ff5-a011-d975ffebfb2a",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "10"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "df_missing[\"Salary\"].isnull().sum()"
+                "df_missing[\"salary\"].isnull().sum()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "228545bc-062d-4129-9003-15cac860e7bf",
             "metadata": {},
             "source": [
@@ -346,53 +319,47 @@
             "metadata": {},
             "source": [
                 "### find number of missing values in each column"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 13,
             "id": "934df451-afaf-458c-a36c-a0c0277969b2",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "import pandas as pd\n",
-                        "\n",
-                        "def find_missing_values(df):\n",
-                        "    num_missing = df.isna().sum()\n",
-                        "    return num_missing\n",
-                        "\n"
+                        "Executor saved to cache file count_missing_35951.py\n"
                     ]
                 }
             ],
             "source": [
-                "num_missing = PandasGenie(\"find number of missing values in each column\")\n",
-                "print(num_missing.code)"
+                "num_missing = PandasGenie(\"find number of missing values in each column\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 14,
             "id": "5ad11b01-bffc-45ae-ae68-ce9d971d5c51",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "ID             0\n",
-                            "Name           0\n",
-                            "Salary        10\n",
-                            "Department     0\n",
+                            "id             0\n",
+                            "name           0\n",
+                            "salary        10\n",
+                            "department     0\n",
                             "dtype: int64"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "num_missing(df_missing)"
             ]
@@ -403,112 +370,203 @@
             "metadata": {},
             "source": [
                 "### plot distribution of salary"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 15,
             "id": "2b9d7bf3-1638-41e9-a44f-a138f1b4294e",
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Executor saved to cache file plot_salary_distribution_54098.py\n"
+                    ]
+                }
+            ],
             "source": [
                 "dist_salary = PandasGenie(\"plot distribution of salary, create bins of 10K each\", columns=df_missing.columns)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 16,
             "id": "465c1afb-4fa8-4644-8fcf-48c25f44a31b",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAA0EAAAIjCAYAAADFthA8AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/NK7nSAAAACXBIWXMAAA9hAAAPYQGoP6dpAABUgklEQVR4nO39d3hU1f7/f7+mZCYhPaQCCaEIoYUOBhAEgYCIFI8CiqLYOCKi2A42xAZ6FPWHiMdC8YOKchTEhkIE9CAqIChR7GJQKQJCQDCFrPsP79lfhiQQ0iZkPx/XletiZlb2e63Ze6+ZF3tmxWGMMQIAAAAAm3AGugMAAAAAUJ0IQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQBgE2eeeabOPPPMQHejQrZu3SqHw6F58+ZVea158+bJ4XBo69at1n2pqak655xzqry2JK1atUoOh0OrVq2qlnoAYCeEIACooTZv3qx//OMfatiwoYKDg1W/fn3169dPM2fODHTXKo3D4bB+3G63YmJi1LFjR02cOFFfffVVpdV58sknqyU4lUdN7hsA1FYOY4wJdCcAAP4++ugj9e7dWykpKRozZowSExO1bds2ffzxx/rhhx/0/fffn/Q2fVeBatKVBYfDoX79+umSSy6RMUb79+/X559/rkWLFunPP//Ugw8+qEmTJlntjTHKy8tTUFCQXC5Xmeu0bt1asbGxJzX2I0eOqKCgQF6vVw6HQ9LfV4Jat26tN998s8zbKW/fioqKlJ+fL4/HI6eT/7MEgMrkDnQHAADF3X///YqMjNS6desUFRXl99iuXbsC06mjFBYWqqioSB6Pp8LbatasmUaPHu133/Tp0zV48GDdeOONSktL09lnny3p79AUHBxc4ZrH8+effyo0NFQul+ukglZlczqdVT5WALAr/msJAGqgH374Qa1atSoWgCQpPj7e7/bcuXPVp08fxcfHy+v1qmXLlpo9e/YJa+Tn5+uuu+5Sx44dFRkZqdDQUJ1xxhlauXKlXzvf93AefvhhPfbYY2rSpIm8Xq8+/fRThYaGauLEicW2/csvv8jlcmnatGknN/D/v7p162rhwoVyu926//77i/Xl6I+P7dixQ5dddpkaNGggr9erpKQkDRkyxPouT2pqqr788kutXr3a+uid76qY73s/q1ev1jXXXKP4+Hg1aNDA77GjvxPk895776ldu3YKDg5Wy5Yt9dprr/k9fvfdd1tXj4527DaP17fSvhO0aNEidezYUSEhIYqNjdXo0aP166+/+rW59NJLFRYWpl9//VVDhw5VWFiY4uLidNNNN+nIkSMnePYBoPbjShAA1EANGzbU2rVrlZ2drdatWx+37ezZs9WqVSude+65crvdeuONN3TNNdeoqKhI48ePL/X3cnNz9eyzz2rUqFG68sordeDAAT333HPKzMzUp59+qnbt2vm1nzt3rv766y9dddVV8nq9SklJ0bBhw/Tyyy9rxowZfldNXnrpJRljdNFFF5X7OUhJSVGvXr20cuVK5ebmKiIiosR25513nr788ktNmDBBqamp2rVrl5YvX66cnBylpqbqscce04QJExQWFqbbb79dkpSQkOC3jWuuuUZxcXG666679Oeffx63X999951GjBihcePGacyYMZo7d67OP/98LVu2TP369TupMZalb0ebN2+eLrvsMnXu3FnTpk3Tzp079fjjj2vNmjXauHGjX2g+cuSIMjMz1bVrVz388MNasWKFHnnkETVp0kT//Oc/T6qfAFDrGABAjfPee+8Zl8tlXC6XycjIMLfccot59913TX5+frG2hw4dKnZfZmamady4sd99vXr1Mr169bJuFxYWmry8PL82f/zxh0lISDBjx4617vvpp5+MJBMREWF27drl1/7dd981ksw777zjd396erpfrdJIMuPHjy/18YkTJxpJ5vPPP/fry9y5c63+SjL//ve/j1unVatWJfZn7ty5RpLp0aOHKSwsLPGxn376ybqvYcOGRpJ59dVXrfv2799vkpKSTPv27a37pkyZYkp6iS1pm6X1beXKlUaSWblypTHGmPz8fBMfH29at25tDh8+bLV78803jSRz1113WfeNGTPGSDL33HOP3zbbt29vOnbsWKwWANgNH4cDgBqoX79+Wrt2rc4991x9/vnneuihh5SZman69etr6dKlfm1DQkKsf+/fv1+7d+9Wr1699OOPP2r//v2l1nC5XNZ3eoqKirR3714VFhaqU6dO+uyzz4q1P++88xQXF+d3X9++fVWvXj298MIL1n3Z2dn64osvin3PpzzCwsIkSQcOHCjx8ZCQEHk8Hq1atUp//PFHuetceeWVZf7+T7169TRs2DDrdkREhC655BJt3LhRO3bsKHcfTmT9+vXatWuXrrnmGr/vCg0aNEhpaWl66623iv3OuHHj/G6fccYZ+vHHH6usjwBwqiAEAUAN1blzZ7322mv6448/9Omnn2ry5Mk6cOCA/vGPf/gtH71mzRr17dtXoaGhioqKUlxcnG677TZJOm4IkqT58+crPT1dwcHBqlu3ruLi4vTWW2+V+HuNGjUqdp/T6dRFF12kJUuW6NChQ5KkF154QcHBwTr//PMrMnxJ0sGDByVJ4eHhJT7u9Xr14IMP6p133lFCQoJ69uyphx566KTDSEljK03Tpk2Lfd+nWbNmklTi94cqy88//yxJat68ebHH0tLSrMd9goODi4XW6OjoCoVFAKgtCEEAUMN5PB517txZDzzwgGbPnq2CggItWrRI0t8LKJx11lnavXu3ZsyYobfeekvLly/XDTfcIOnvKzylWbBggS699FI1adJEzz33nJYtW6bly5erT58+Jf7e0VecjnbJJZfo4MGDWrJkiYwxevHFF3XOOecoMjKywmPPzs6Wy+U6bki5/vrr9e2332ratGkKDg7WnXfeqRYtWmjjxo1lrlPa2MqrpEURJFXrogSBXNkOAGo6FkYAgFNIp06dJEnbt2+XJL3xxhvKy8vT0qVLlZKSYrU7doW3kvz3v/9V48aN9dprr/m9aZ8yZcpJ9al169Zq3769XnjhBTVo0EA5OTmV8gddc3JytHr1amVkZJR6JcinSZMmuvHGG3XjjTfqu+++U7t27fTII49owYIFkkoPJeXx/fffyxjjt81vv/1W0t+rvUl/X3GRpH379vktVnDs1ZqT6VvDhg0lSd9884369Onj99g333xjPQ4AODGuBAFADbRy5UqZEv6W9dtvvy3p/30kyve//Ue33b9/v+bOnXvCGiX97ieffKK1a9eedH8vvvhivffee3rsscdUt25dDRw48KS3cbS9e/dq1KhROnLkiLVqWkkOHTqkv/76y+++Jk2aKDw8XHl5edZ9oaGh2rdvX4X65PPbb79p8eLF1u3c3Fw9//zzateunRITE60+SNIHH3xgtfvzzz81f/78Ytsra986deqk+Ph4PfXUU35je+edd7RlyxYNGjSovEMCANvhShAA1EATJkzQoUOHNGzYMKWlpSk/P18fffSRXn75ZaWmpuqyyy6T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LQAAAAC1WEBD0IMPPqjk5GTNnTvXuq9Ro0YB7BEAAACA2i6gIWjp0qXKzMzU+eefr9WrV6t+/fq65pprdOWVV5bYPi8vT3l5edbt3Nzc6uoqgHLKycnR7t27q61ebGysUlJSqq0egMDbsmVLtdZjngFOfQENQT/++KNmz56tSZMm6bbbbtO6det03XXXyePxaMyYMcXaT5s2TVOnTg1ATwGUR05OjtLSWujw4UPVVjMkpI6+/noLb1AAGzi8f48kh0aPHl2tdZlngFNfQENQUVGROnXqpAceeECS1L59e2VnZ+upp54qMQRNnjxZkyZNsm7n5uYqOTm52voL4OTs3r1bhw8fUtexUxSRlFrl9XK3b9Unc6Zq9+7dvDkBbKDg0AFJRu0uvFVxjdKqpSbzDFA7BDQEJSUlqWXLln73tWjRQq+++mqJ7b1er7xeb3V0DUAlikhKVUxK80B3A0AtFRafwhwD4KQEdIns7t2765tvvvG779tvv1XDhg0D1CMAAAAAtV1AQ9ANN9ygjz/+WA888IC+//57vfjii3r66ac1fvz4QHYLAAAAQC0W0BDUuXNnLV68WC+99JJat26te++9V4899pguuuiiQHYLAAAAQC0W0O8ESdI555yjc845J9DdAAAAAGATAb0SBAAAAADVjRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYIQQAAAABshRAEAAAAwFYCGoLuvvtuORwOv5+0tLRAdgkA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V66s7H4AAAAAQLUo13eCAAAAAOBUVa4rQb179z7ux97ef//9cncIAAAAAKpSuUKQ7/tAPgUFBdq0aZOys7M1ZsyYyugXAAAAAFSJcoWgRx99tMT77777bh08eLBCHQIAAACAqlSp3wkaPXq05syZU5mbBAAAAIBKVakhaO3atQoODq7MTQIAAABApSrXx+GGDx/ud9sYo+3bt2v9+vW68847K6VjAAAAAFAVyhWCIiMj/W47nU41b95c99xzj/r3718pHQMAAACAqlCuEDR37tzK7gcAAAAAVItyhSCfDRs2aMuWLZKkVq1aqX379pXSKQAAAACoKuUKQbt27dLIkSO1atUqRUVFSZL27dun3r17a+HChYqLi6vMPgIAAABApSnX6nATJkzQgQMH9OWXX2rv3r3au3evsrOzlZubq+uuu66y+wgAAAAAlaZcV4KWLVumFStWqEWLFtZ9LVu21KxZs1gYAQAAAECNVq4rQUVFRQoKCip2f1BQkIqKiircKQAAAACoKuUKQX369NHEiRP122+/Wff9+uuvuuGGG3TWWWdVWucAAAAAoLKVKwQ98cQTys3NVWpqqpo0aaImTZqoUaNGys3N1cyZMyu7jwAAAABQacr1naDk5GR99tlnWrFihb7++mtJUosWLdS3b99K7RwAAAAAVLaTuhL0/vvvq2XLlsrNzZXD4VC/fv00YcIETZgwQZ07d1arVq304YcfVlVfAQAAAKDCTioEPfbYY7ryyisVERFR7LHIyEhdffXVmjFjRqV1DgAAAAAq20mFoM8//1wDBgwo9fH+/ftrw4YNFe4UAAAAAFSVkwpBO3fuLHFpbB+3263ff/+9wp0CAAAAgKpyUiGofv36ys7OLvXxL774QklJSRXuFAAAAABUlZMKQWeffbbuvPNO/fXXX8UeO3z4sKZMmaJzzjmn0joHAAAAAJXtpJbIvuOOO/Taa6+pWbNmuvbaa9W8eXNJ0tdff61Zs2bpyJEjuv3226ukowAAAABQGU4qBCUkJOijjz7SP//5T02ePFnGGEmSw+FQZmamZs2apYSEhCrpKAAAAABUhpP+Y6kNGzbU22+/rT/++EPff/+9jDE67bTTFB0dXRX9AwAAAIBKddIhyCc6OlqdO3euzL4AAAAAQJU7qYURAAAAAOBURwgCAAAAYCuEIAAAAAC2QggCAAAAYCuEIAAAAAC2QggCAAAAYCuEIAAAAAC2QggCAAAAYCuEIAAAAAC2QggCAAAAYCuEIAAAAAC2QggCAAAAYCuEIAAAAAC2QggCAAAAYCuEIAAAAAC2EtAQNHv2bKWnpysiIkIRERHKyMjQO++8E8guAQAAAKjlAhqCGjRooOnTp2vDhg1av369+vTpoyFDhujLL78MZLcAAAAA1GLuQBYfPHiw3+37779fs2fP1scff6xWrVoFqFcAAAAAarOAhqCjHTlyRIsWLdKff/6pjIyMEtvk5eUpLy/Pup2bm1td3QNwCtmyZUutqgMA1a0657e8vDx5vd5qqcW8DZ+Ah6DNmzcrIyNDf/31l8LCwrR48WK1bNmyxLbTpk3T1KlTq7mHAE4Vh/fvkeTQ6NGjq7VuQV5+tdYDgKoSkHnU4ZCMqb56Yt5GDQhBzZs316ZNm7R//37997//1ZgxY7R69eoSg9DkyZM1adIk63Zubq6Sk5Ors7sAarCCQwckGbW78FbFNUqr8nrbN69V9tKnVVhYWOW1AKA6BGoeZd5GdQt4CPJ4PGratKkkqWPHjlq3bp0ef/xx/ec//ynW1uv1VtvlUgCnrrD4FMWkNK/yOrnbt1Z5DQAIhOqeR5m3Ud1q3N8JKioq8vveDwAAAABUpoBeCZo8ebIGDhyolJQUHThwQC+++KJWrVqld999N5DdAgAAAFCLBTQE7dq1S5dccom2b9+uyMhIpaen691331W/fv0C2S0AAAAAtVhAQ9Bzzz0XyPIAAAAAbKjGfScIAAAAAKoSIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCCAAAAANgKIQgAAACArRCC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TBEREXI4HNq0aZMk//kmODhYDRo0UHR09AnPE98frQ4LCys2j61YsUIJCQnWPBAdHa1LLrlEv/32m9Vm1qxZSk5OlsvlksvlUnh4+HHH6PF4FBISYvX/6HqLFi1SbGysVS8sLEx9+/bVJ5984jfGhIQEuVwuud1uRUREVKheWlqatb/OPvtsORwOPfbYY1VWLzIystj5OGDAgCodn8fjUUREhEJDQxUaGqrOnTsrJyfHqpeYmGidI6GhoSecV6OiotSkSZNix6hvHihpznE4HPr3v//tNw/ExsYqNDT0hOfFicbYrFkzuVwu6xxv2bKlnnrqKb/n9GTGeLxzYtWqVWrTpo21f7xerwYMGOA3p8yaNUsNGza02tSpU+e49YKCghQUFCSPx1Pstf3oudX3unfsOX30cxoVFWXNI6XN1fXq1bPOsYiICL96vu3VrVtXTqdTLpdLDodD+/btsx7/66+/NH78eEVHR1vPaWRkZKn7MDU11e+cPrbe3LlzFR0dbbWJj4/Xddddp/379/vtw/j4eGueqVu3boXG53tt981rQ4YM0ddff+03vqioKLndbrndbsXGxlao3tGv7926dfM7rk62XocOHeR2uxUcHKyQkJBix4yvntPpLHYOjhs3zqpXt25d1alTR4mJieV6j3a0E71nPrpmaa9JlcKgwhYuXGg8Ho+ZM2eO+fLLL82VV15poqKizM6dO/3avf322+b22283r732mpFkFi9e7Pf49OnTTWRkpFmyZIn5/PPPzbnnnmsaNWpkDh8+bLUZMGCAadu2rfn444/Nhx9+aJo2bWpGjRplPb5//36TkJBgLrroItO9e3czbtw44/V6zR133GHOPvtsk5KSYlasWGFcLpd56KGHzIgRI0xERIRxuVxm4cKF5vTTTzfdunWztldYWGhat25t+vbtazZu3GjefvttExsbayZPnmy1+fHHH02dOnXMkCFDzOzZs82dd95pnE6nGTlypAkKCjLZ2dlm4cKFxul0mpiYGPPcc8+ZoUOHGpfLZTp37lyuWpMmTTJfffWVmTlzpnG5XObxxx83qampJj093QwcONDaHyNGjDChoaEmNDTUvPfeexUa3+mnn26aNm1q7r//fuN0Os2LL75ofv/9d+sYqIrxPfjgg0aS6devn/nkk0/Mjz/+aCZPnmyCgoKs461z585Gkpk3b16Fj5vzzjvPrFq1ysyePdsEBweb66+/3kgyK1euNGvWrDEOh8NERUWZOXPmmMsvv9w4HA7Trl27co9x4sSJJjQ01DidTjNv3jyzaNEiExYWZsaMGWPtwxtuuMF4PB4TGhpq3n///QqfF5mZmaZ+/frG4/GYe++910yZMsVERESYJUuWGJfLZQYOHGjCw8PN+eefb9xutznzzDPLXM93ji9YsMBIMj179jTZ2dnmpZdeMiEhIWbYsGHWOT5//nwjycTExJiNGzeaO+64wwQFBZnu3buXeSzZ2dnm1ltvNW6324wbN86aV9asWWOd49OnTzc9e/Y0LpfLSDIbN240xvjPN+eff74JCQkxiYmJZs2aNcc9T2bOnGlGjBhhwsPD/eaxH3/80YSEhJiUlBTzyCOPmDvuuMM4nU7TvHlz07FjR+s88Xg8pnXr1qZ58+ZmyJAhJiwszDRq1KjUMc6ePdsMHTrUeDwev3q+MY4aNco8++yzZvz48cbtdpvhw4ebiIgIs2vXLmuMHTp0MM2bNzdnnHGGSUpKMk2aNCl3vYceesh89dVX5h//+IeRZOLj482jjz7q95xWZr2OHTuaHj16mOuvv9643W6zcuVKs3fv3iqrd+utt5rIyEiTkZFh3G63efvtt83rr79udu7cadUbMGCASUxMNBkZGaZevXqmS5cux51Xp06dakJCQszw4cOtmkfPA6tXr/abV+fMmWMcDod5/PHHrXmgR48eJiYmxoSFhZmlS5ce97w40Ri7dOlikpOTzejRo43b7TZ33XWXcblc5vXXXy/XGE90TiQlJZmOHTuam266yTidTjNw4ECTkpJiDh48aJ0TZ555pklMTDRnn322CQsLMx07diy1Xrdu3cwNN9xgoqKizNixY63X9uzsbOs5HTFihImOjjZOp9PMnDnTOqd99Z599llz2mmnmfr165uwsDDz4osvljpXN2zY0Nx///3mtttuM06n03Tu3LlY/0eOHGmuv/566/Xo22+/tbYzbtw4k5ycbDp37myaNWtmWrVqZVq3bl3qPkxKSjL33Xefeeihh4zX6zWtW7e26q1Zs8Y4nU7TunVrM2vWLHPNNdcYl8tlGjZsaM477zzrvIiIiDApKSnm9NNPN7169TIJCQkVGt8ll1xi5s+fb0aOHGnCwsJM//79TXJysiksLDTjxo0zDRo0MI0aNTJdunQxbdq0MS1atKhQPd/r++mnn27cbrffcXWy9SZNmmR69OhhLrroIuN0Os2TTz5pHTPz5s2z6nXu3NmkpaWZiIgIs3nzZrN9+3azf/9+a/+99957pkmTJiYyMtK0bdv2pN6jLVu2zGpTlvfMvppZWVlm/fr1xV6TKgshqBJ06dLFjB8/3rp95MgRU69ePTNt2rRSf+fYEFRUVGQSExPNv//9b+u+ffv2Ga/Xa1566SVjjDFfffWVkWTWrVtntXnnnXeMw+Ewv/76qzHGmCeffNJER0ebvLw8q82tt95qmjdvbnbt2mUkmd69e5tBgwaZffv2maCgILNo0SLTtWtXc/XVV5stW7YYSWbt2rXGmL+Dm9PpNDt27LC2N3v2bBMREWHVuOWWW0yrVq38xjdixAiTmZlpoqOjzbPPPms6dOhgnE6nWbRokfUcxcXFVUqt4cOHmzp16pjly5dbk9348eOt8b388svW/qjI+KZMmWLatm3rNz6fqhrfrbfeamJjY/1qHX28+Y6biIgI63irzOMmOjraNGnSxBQVFZmhQ4cah8NhjdEYY9LT0ys0xkGDBpmxY8f6PZ/Dhw83devWNePHj7fG99BDD1n7sCLj27dvn3G5XObNN9+0zgvf/mvRooU5++yz/c7Drl27mksvvbRc9SSZV155xWpzyy23GJfLZW37ggsuMP379/fbtu/5LO857ptXLrjgAjNo0CBztHbt2lkh6Oj5xneezJ8/3+pLWc+To8dY2jxw+umnG0nm559/Nl26dDGjRo2yxuibKy+99NIyjfHoebOkMXbt2tVcdtllRpJZvny5SUxMNDfddJNVz3fs3HrrrRWq98svv5j69eubNm3amLCwMPPoo49az2ll1xszZowZMmSINb6rr77aGGOqrN6IESPM6NGjS613zz33WK8bvnoPP/xwmecBX83jvW4MGTLE9OnTx5rrfOfcJ598Ys0DZT0vShpjq1atzD333OM3xg4dOpjbbrutwmM89pxo2rSpkWSys7OtMfbv39/ExcWZZ555xnTp0sVcccUVVj3fOXHDDTeU+Tn95ZdfjCQzatQo06pVK7/Xdt9z6junW7ZsacaPH29t77fffrOe07K+tvfu3dtIMqtXry72/icrK8tIMnfddZcxxlh9efTRR63j1NeXGTNmlGkfNmnSxKpX2nnft29f4/F4TH5+vklMTDSXX3659Xz59uHYsWMrPD7f/rnuuuus+TQoKMgKNDt27LDGd/PNN1eo3saNG039+vVNQkKCdRz7ns+K1MvMzLTeD6alpVn1evXqZa677jq/969HH0u+Y+bDDz+0js2TeT/oc6L3zEfX9Dn2Namy8HG4CsrPz9eGDRvUt29f6z6n06m+fftq7dq1Zd7OTz/9pB07dvhtJzIyUl27drW2s3btWkVFRalTp05Wm759+8rpdFof/1i7dq169uwpj8djtcnMzNQ333yjnJwcSdJXX32lvn37asOGDSooKFDfvn2VmZmptWvXKi0tTSkpKX4127Rp4/fHazMzM5Wbm6svv/zSanN0vyWpX79++uCDD/Tnn3+qU6dO2rRpk4qKiqx2TqdTAwcOVEhISIVr7dixQ4WFherbt6+MMdq1a5ff+Pr372/tj4qO77vvvlO9evWUlZWlrKws5eTkKD8/v8rGt3TpUrVv315ZWVmKj49Xu3bttG7dOquN77jp2bOnVaeyjps+ffrojz/+0KhRo+RwOLRmzRoZY/z6N3ToUAUFBZV7jN26dVNWVpbatm2rtWvX6vPPP9f//vc/7d27V3379rXG169fP2sfVmR8TqdTR44cUXBwsHVe/PHHHwoJCdGPP/6o9u3b+52HmZmZ+uyzz8pVT5KCgoKsNunp6Tpy5Ii6dOlitRk4cKDftn0fiSnvOe5T0nnSs2dP699Hzze+8+Tcc8+1+lLW80SStm3bVmrNzMxMffHFF3I4HKpTp442bNigmJgY6/nzzZW7d+8u0xglWR+fKale3759tWzZMkVGRioqKko7duywPj7VqVMn69j5888/y12vqKhIF198sW6++WYNGzZMeXl5fs9pZdeT/v54SXx8vL7//nstWrRIe/bsqZJ6ffr00VtvvaVmzZopMzNTmzdv1vPPP68lS5ZY9RISEqzXDV+9nJycMs+rPqUdL2vWrNFbb72lMWPGWK+tvnOuS5cu1u2ynhclPafdunXT0qVL9euvv6p///5avny5vv32W7Vp06bCY5T8z4muXbtKkoKDg602H3/8sbxerz744ANt2LBBycnJVj3fOfHDDz+U+Tldv369JOmbb7454Wv7li1brOewTZs2SkpKsm6X5fU2MzPT+vhweHh4ie9/JFltfH1xu93Wcerry5EjR8q0D3/44QdJUkxMTKl92rJliyIiIrRt2zbt2LFDTqfTer58+/DIkSOVMr5evXrpzTffVKNGjbRz504VFBSooKDAqucbn8fjKXe9Q4cO6cILL9SsWbOs4+ro57Mi9dauXWt9dPDbb7/1a/Piiy9qz549euCBBzR58mStWbPGOpZ8x0yPHj2sY7Osx4zvOC7Le+ajj1+fY1+TKgshqIJ2796tI0eO+E1MkpSQkKAdO3aUeTu+tsfbzo4dOxQfH+/3uNvtVkxMjF+bkrYhSTfeeKO6d++uvXv3Wtv1eDyKioryq3NszdK2V1KbzZs3KywsTFdddZUOHz6shQsXKi4uTkVFRQoKClJUVJTfdpxOZ7lrSdLChQv166+/Kj8/X4cPH1ZBQYGMMVUyvq5du2revHlatmyZrrvuOhUWFqpHjx7aunVrlY3vxx9/1KpVq1RYWKjXX39dF154oYwx2rBhg9/vJScn+x1vlXHcZGdnS5I1Ee3du9d6ITu6jjGm3GP817/+pZEjR+r2229Xbm6u2rdvr7Fjx/rtQ982jrcPyzq+8PBwZWRk6N5775XD4ZAkPf3001q7dq3y8vKs0OLrn69OeeqdiG+7J5orTuYcP3bbR4uNjfV7/OjxVeQ8+eOPP0ptEx0drUOHDumCCy5Qfn6+jhw5osLCQr/nLyEhQbt27SrzGEuq9+abbyosLEwPPPCAdu7cqeXLlys/P1+SlJeXV6n1HnzwQbndbl133XVKSEjQkSNH/J7Tyq43YMAAPf/888rKytJ5552n/fv3a+DAgfr1118rvV5ISIgOHjyo6dOna8CAAbruuuvkdDo1fPhw6/udBQUF1vHi205J50h5jtGEhAQdPHhQ4eHh6tGjh/XaevQ557t9MufFsc/pzJkz1bJlSzVo0ED333+/fvzxR82aNUspKSmVMsaj6/nevE2ePFl//PGHYmJilJubq19++UU5OTk6cuSIjDEVqnf//fere/fuOnDgQInndG5urg4fPqyYmBi/ubWkec5Xq7SacXFxOnjwoDIyMqzj/9g2kqzvb/j6kpubW+w4/f3330+4D+Pi4iRJHTp0UOvWrUtsExoaqu3bt+uqq66ytnXo0CG/dgkJCTpw4ECFxvfkk08qLCxML730kn777TctX75ce/bskcfj0b59+4rVO3ToULnr3XDDDerWrZuGDBni9zu+57O89XzHw4QJE9S5c2cVFRVZbS688EItWLBAo0aNUlxcnP7v//5PU6ZMsY6l8h4zRx+DZXnPfPTxW1qbykIIspHvvvtOCxcurNIazZs316ZNmzRjxgxJ0lVXXaVvv/22Smpt27ZNEydO1M0331wl2z/WwIEDdf755ys9PV0dO3aUJO3fv19vvPFGldUsKipSkyZNJEnt2rXT6NGjJUmLFy+uspo+r776qiQVe8NfmV555RW98MIL1j585plnrC8oV5X/+7//kzFGvXv3lvT3Yg+jRo2q0pp2VFBQoGnTpkmSHn/88Sqt1bt3b23atEk33nijPB6PLrjgAuuNaGX68ccf9fjjj2vevHlWiK5qI0eO1Lnnnqs2bdqobdu2ioqK0rp167Rx48ZKr2WMkSQNGTJEN9xwg5KTkxUaGqpzzjmn2EI+VWnEiBHWlZOqMHPmTH388cdaunSp/vWvfyksLEzjx4+3/ke+MrlcLr322mv69ttvFRMTo+HDh0uS+vfvb101qaiff/65yl/bfWbPni1Jmj9/frXUu++++yRJDz/8cImP5+bm6sknn5Tb7dbdd99d4XrHG99FF12kjRs3auTIkQoODrb+c6ey63344Yd6//33rQVXqsJXX32lJ5980u++q666SpmZmYqLi1NsbKyef/55rV+/3poXaiNCUAXFxsbK5XIVW7Vi586dSkxMLPN2fG2Pt53ExETt2rXL7/HCwkLt3bvXr82x27jtttskSW+99ZYaNGhgtUlMTFR+fr727dvnV+fYmiX16eg+H93G4/GoadOmioiIUEREhNq2basFCxbI6XSqoKDAb8WYnTt3qqioqNy1NmzYoF27dum6666T9PelZN+l0h49eighIaHSx3d0m4iICDVr1kw7d+6skvFJUlJSkuLi4hQREaGQkBDFxsbK4XBo+/btfr+3bds2v+OtosfNzz//rI8//tivRkxMjAoLC4uN0eFwlHuMN998s/71r38pLS3NWtXq+uuvLzaGnTt3Hncfnsz4mjRpotWrV+utt96SJK1evVoFBQUKDg5WQUGBX599dcpT70R82z3RXFGWc/zY2yW12b17t9/jR4+vIudJdHR0sTYFBQW64IIL9NtvvyksLEwJCQnWXOl2u/2ev507dyo+Pr7MYyypXmhoqJo2bao6deqoWbNmcrvdWrVqlSTJ6/VWWr3169dr165dSklJkdvt1rXXXquioiLdeOONuuCCCyq9XkltfCsl+j5aVpn1Dh06JLfbrZYtW1ptEhMT1aJFC+3du1fS3x/x9B0vR7cp6/HiU1KbDz/8UJI0btw4v9fWo8853+2TOS+OHuO2bdt02223acaMGRo8eLDcbrcaN26sESNGWP/xU9ExHrsPO3bsqE2bNmnfvn2aMWOGIiIitG/fPmuVOofDUa5648aNkyQ999xzx31t971+7N27Vw6Hw2/7x9bz1Sqp5rXXXqu1a9cqLCxMp512Wqnvf6T/d5XK15eIiIhix2lcXNxx9+G1116r999/X9Lf/wl4bJsDBw5owIABcjqdatasmYKCgqxt1alTx29bO3fuVHh4eIXGFxkZqdNOO00ej0c9evTQ119/re+//175+fmKiooqVq9OnTrlqvfhhx/qhx9+sFZ/8wXA8847Tw899FC560nSI488IofDoVWrVik9Pf247199H+X0vbcpzzHja3v0e5gTvWc++vgtrU1lIQRVkMfjUceOHZWVlWXdV1RUpKysLGVkZJR5O40aNVJiYqLfdnJzc/XJJ59Y28nIyNC+ffusj0JJ0vvvv6+ioiLrYM3IyNAHH3xgfSzs2muvVVZWlho1amRNIhkZGcrKylLHjh0VFBSkrKwsLV++XBkZGdZ3h46uuXnzZr/Ja/ny5YqIiLBeKH3bO5pve0VFRSosLFS7du3kdDqtdkVFRVq2bJkOHz5c7lpnnXWWNm/erMzMTHXr1k2bNm1Sp06dVLduXY0YMUKdOnVSUFCQli9fbu2Pyhxf586d9cMPP6hBgwZVMj5J6t69u77++mtrG74lUX2fmfYdNx988IHVpqLHjfT3EqQhISFq1qyZ9YLevXt3ORwOv/4tXbpUBQUF5R7joUOH5HQ6rePFN0av12sdt4mJiVqxYoW1DytjfJL0v//9T82bN5ckvfvuu2rVqpU2bdrkdx4uX75cHTt2LFc9SX5Lh2ZnZ8vlcln/25yRkaFly5b5bdv38ZiTHcvy5cutsRz7HPv43mBK/vONbx544403rL6U9TyR/v4o5tE1fQHou+++U+fOndW9e3drv3bs2FF//PGH9fz55krfR2ZPNEZJCgsLK3WMR887vqVcDx06ZNXzHTvh4eHlqnfo0CF98cUX2rRpkzZt2qT09HTVqVNHN998s1asWFHp9UoaX5s2bbRnzx61adOm0uutXr1anTt3tr5f5ns+v/32WzVv3twKI77XDV+9hg0blnle9SlpfC+//LL1n2dHv7b6zrl169ZZt8t6Xhw7xvfff18FBQXWVRjfGF0ul4KDgys8Rqn4OeETGRmpTz75ROnp6Vq/fr2GDx+ujh076pdffrHq+c6Jpk2bllrP99r+xhtvKDQ0VP369fOrd7zX9hYtWljP4ebNm7Vjxw7rdmlzta/e4sWL1b1792Ln9LHvfySpc+fOkmT15ciRI9Zx6utLUFBQifswPz/fqjd8+HA1b97ceh3y9Sk3N1f9+/eXx+NRXFyc1Sff3FZUVGQ9X759GBQUVCnjy8rKUteuXWWMUb169awly331fOMrLCwsV724uDhrnvnss8+sjwQ++uijmj9//knXk2TVXLt2rbp3765GjRqd8P2r788puN1uv2Pmo48+so7Nk3k/eKLn1Nfm6OPX59jXpEpTqcss2NTChQuN1+s18+bNM1999ZW56qqrTFRUlN8qLsYYc+DAAbNx40azceNGa2WUjRs3mp9//tkY8/eyjlFRUeb11183X3zxhRkyZEiJS/O2b9/efPLJJ+Z///ufOe200/yWmNy3b59JSEgwF198sRkxYoSpU6eO8Xq95qGHHjLbt28327dvN++//75xu93m4YcfNiNGjDCRkZHWEtkZGRkmIyPD2p5vWc7+/fubTZs2mWXLlpm4uLgSl0Ts2rWref75580999xjnE6nueCCC4zD4TDvvfeetYR03bp1zdy5c82wYcOMy+UynTp1Kletm2++2WzZssXMmjXLb/nFXr16mYEDB1r7Y8SIESYsLMyEhoaad999t0Lj69Spk5k/f741vvbt25vY2Fiza9euKhvfLbfcYiSZSy+91Hz33XfmhRdeMF6v17jdbut469Kli3E4HGb+/PmVctx88cUXJjY21rjdbvOf//zHanP0Etnz5s0zV155pXE4HNaKeeUZ49ChQ01UVJS1RPZrr71mYmNjzeDBg619OGnSJGuJ7JUrV1Z4fP/5z3/Mv/71LxMcHGwmTpxo2rZta7p27WpWr15t3G63Ofvss01ERIQZOXKkcbvdpnfv3mWu5zvHP/jgAyPJdOzY0fz3v/81TzzxhKlTp44ZNmyYdY4///zzxuFwmJiYGLNp0yYzZcoUa4nsso4lOzvbzJs3zwQHB5s77rjDmlfmzp1rXC6Xefjhh83atWvN1VdfbS2RvXDhQrNx40Zz++23W305dons450nH330kZk1a5aJjo72m8c+/PBDExISYpo2bWoSExPN5MmTrSWPt2/fbvLy8qy50rek69ChQ01YWJhp3LhxqWP89NNPzfTp001wcLBfvVdffdW4XC7Tp08f89JLL5mJEycat9tthg4darxer8nOzrbm1A4dOpi0tDTTs2dPk5SUVGxp3rLW882bW7ZssfZXvXr1/JbIrsx6LpfL9OrVyxqfy+UyLVq0MKeddpr566+/qmR8Y8aMMUFBQeacc84xbrfbTJ482bhcLvPhhx9a9QYMGGCSkpJMt27dTL169UzXrl2PO68uXrzYREdHm7Fjx1o133zzTRMcHGzNdb7V1yZMmGBt5+jX1h49epi6detaS2Qf77w40RgbN25smjZtasaMGWPcbre59957TXBwsHnyySfLNcbjnRN16tQx5557rpk/f76ZOnWqcTqdJj4+3gwfPtxvjL179zZJSUnmnHPOMWFhYaZTp06l1jv//PNNaGioiYyMNBMmTLBe27/66itrbj12iWzfOe2rN2fOHHPaaaeZBg0amPDwcPPSSy+VOle3a9fOhIeHm+uvv97vnD506JC1vccee8y8+uqrpmfPnkaSWbJkidm4caPZs2ePGTdunElJSTFdunQxzZs3N61btzatWrUqdR82a9bMhIeHm7vuusuEhIRY718OHTpkLXOekpJimjVrZiZMmGAtHb99+3ZTWFhoLXPesGFD061bN3PmmWeahISEco/P4/GYf/zjH2bRokXmwgsvtJbIjomJMTt37rSWc27UqJE5/fTTTXp6umnRokWFns9j30/qmCWyT6bezTffbEaOHGlCQkL86m3fvt08//zz1nvECRMmmGHDhpnw8HAzf/5807hxY9OzZ09r/y1fvtxaIjs9Pb1c79GOPa9Le8/sq/n++++b9evXF3tNqiyEoEoyc+ZMk5KSYjwej+nSpYv5+OOPi7VZuXKlkVTsZ8yYMcaYv5cgvfPOO01CQoLxer3mrLPOMt98843fNvbs2WNGjRplwsLCTEREhLnsssvMgQMH/Np8/vnnpkePHiXWkmTmzp1rXnnlFdOsWTMTFBRkoqOjTVhYmPUmbfv27X7b27p1qxk4cKAJCQkxsbGx5sYbbzQFBQXFxhYTE2PVCA8PN2eddZZ57733rDYzZswwYWFhRpJxOp2mV69e5a7Vrl074/F4TOPGjc3cuXOtx3r16mUmTpxo7Y+goCATHx9vIiIiKjw+30QkyURHR5sRI0aY77//vsrHN3HiRNO6dWvj9XpNWlqaefrpp/2Ot86dO5uxY8dW2nETFBRkJJkbb7zRHGvBggUmMjLSSDIOh8NkZGRUaIxBQUEmIiLC1K1b1wQHB5vGjRub22+/3eTl5fntw3r16pmYmJhKGZ/b7TYul8u4XC6TmJhoLadujDGvvPKKOe2004zT6TRut9sEBQWdVL3SzvE6deqY6dOnFzvH27RpY1JTU43H4zGtWrUyb7311kmNxev1mtjY2BJr9urVyzRr1swKP8f+3HXXXVZfPB6PqV+/vomMjDzheeL72yslzWMvvfRSqfPOypUrjTF/z5X169c3TqfTOJ1OExoaWqbjsaR6CxYssM45X6A899xzzaeffmqM+X9zalxcnHE6ncblcpmwsLBy1/PNm0fvr4YNG1ohqLLrLViwwNSpU8caX3x8vLnyyiutNwtVNT6Xy2U8Ho/xeDymbdu2ZsmSJX714uPjrXPE9/evjjcP+JbGPvYnMzPTmutiY2ONx+OxzkWfo+eBmJgYU6dOnTLPYaWNsXHjxlb/PR6Pad68uXnkkUdMUVFRucZ4vHNi5cqVpn79+tZ9devWNXfccYffMtAzZ840ycnJ1j4MDg4+br3jvbYfO7eGhoYWO6ePfk4jIyOteaS0ufp49XzbK20fz5071xw+fNhcc8011n+4ut1uEx4eXuo+PFG9KVOmlNrmp59+svZhbGysNc9ER0eXe3z33XefFah95+GFF15ovv76a2OMscYXERFh7cOYmJgKPZ/Hvp88OgSdbD3fn0corebMmTNNvXr1jMPhsM79pk2bmptvvtns37/fqhcdHW2Cg4NNQkKCCQ4OLtd7tKOP+eO9Zz66ZmmvSZXBYUwt/sYTAAAAAByD7wQBAAAAsBVCEAAAAABbIQQBAAAAsBVCEAAAAABbIQQBAAAAsBVCEAAAAABbIQQBAAAAsBVCEAAAAABbIQQBAE5J8+bNU1RUVKC7AQA4BRGCAAAB8fvvv+uf//ynUlJS5PV6lZiYqMzMTK1ZsybQXQMA1HLuQHcAAGBP5513nvLz8zV//nw1btxYO3fuVFZWlvbs2VNtfcjPz5fH46m2egCAmoErQQCAardv3z59+OGHevDBB9W7d281bNhQXbp00eTJk3XuuedKkmbMmKE2bdooNDRUycnJuuaaa3Tw4MFSt/nDDz9oyJAhSkhIUFhYmDp37qwVK1b4tUlNTdW9996rSy65RBEREbrqqqvUp08fXXvttX7tfv/9d3k8HmVlZVX+4AEAAUcIAgBUu7CwMIWFhWnJkiXKy8srsY3T6dT/9//9f/ryyy81f/58vf/++7rllltK3ebBgwd19tlnKysrSxs3btSAAQM0ePBg5eTk+LV7+OGH1bZtW23cuFF33nmnrrjiCr344ot+/ViwYIHq16+vPn36VM6AAQA1isMYYwLdCQCA/bz66qu68sordfjwYXXo0EG9evXSyJEjlZ6eXmL7//73vxo3bpx2794t6e+FEa6//nrt27ev1BqtW7fWuHHjrCs9qampat++vRYvXmy1+euvv1SvXj099dRTuuCCCyRJbdu21fDhwzVlypRKGi0AoCbhShAAICDOO+88/fbbb1q6dKkGDBigVatWqUOHDpo3b54kacWKFTrrrLNUv359hYeH6+KLL9aePXt06NChErd38OBB3XTTTWrRooWioqIUFhamLVu2FLsS1KlTJ7/bwcHBuvjiizVnzhxJ0meffabs7GxdeumllT5mAEDNQAgCAARMcHCw+vXrpzvvvFMfffSRLr30Uk2ZMkVbt27VOeeco/T0dL366qvasGGDZs2aJenvxQxKctNNN2nx4sV64IEH9OGHH2rTpk1q06ZNsfahoaHFfveKK67Q8uXL9csvv2ju3Lnq06ePGjZsWPkDBgDUCKwOBwCoMVq2bKklS5Zow4YNKioq0iOPPCKn8+//r3vllVeO+7tr1qzRpZdeqmHDhkn6+8rQ1q1by1S3TZs26tSpk5555hm9+OKLeuKJJyo0DgBAzUYIAgBUuz179uj888/X2LFjlZ6ervDwcK1fv14PPfSQhgwZoqZNm6qgoEAzZ87U4MGDtWbNGj311FPH3eZpp52m1157TYMHD5bD4dCdd96poqKiMvfpiiuu0LXXXqvQ0FArSAEAaic+DgcAqHZhYWHq2rWrHn30UfXs2VOtW7fWnXfeqSuvvFJPPPGE2rZtqxkzZujBBx9U69at9cILL2jatGnH3eaMGTMUHR2tbt26afDgwcrMzFSHDh3K3KdRo0bJ7XZr1KhRCg4OrugQAQA1GKvDAQAgaevWrWrSpInWrVt3UuEJAHDqIQQBAGytoKBAe/bs0U033aSffvpJa9asCXSXAABVjI/DAQBsbc2aNUpKStK6detO+L0jAEDtwJUgAAAAALbClSAAAAAAtkIIAgAAAGArhCAAAAAAtkIIAgAAAGArhCAAAAAAtkIIAgAAAGArhCAAAAAAtkIIAgAAAGAr/z8mgRwAp9kDDgAAAABJRU5ErkJggg==\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAjYAAAHHCAYAAACskBIUAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/NK7nSAAAACXBIWXMAAA9hAAAPYQGoP6dpAABAuUlEQVR4nO3deZxN9ePH8fc1yzVmzIwls4ghRHZSIoVMyd6XsvxkjVJ8bSVUiJLlG5FE+coeSVKpaGwpX9mJyL5MZIlmxljGmPn8/ugx9+GaGeaOO3Ov4/V8PO7j4Zz7Oee873HHvJ17zrk2Y4wRAACABeTxdAAAAAB3odgAAADLoNgAAADLoNgAAADLoNgAAADLoNgAAADLoNgAAADLoNgAAADLoNgAAADLoNgAXurNN9+UzWbLlW3Vq1dP9erVc0yvWbNGNptNixYtypXtd+7cWSVKlMiVbWVXYmKiunXrpvDwcNlsNvXt2zfXtp3297FmzZpc2yZwu6LYALlg5syZstlsjkfevHkVGRmphg0b6v3339f58+fdsp0TJ07ozTff1Pbt292yPnfy5mxZ8c4772jmzJl68cUXNWfOHHXo0CHTsVeuXNHEiRNVrVo1BQcHKzQ0VBUqVNDzzz+v33//PRdTA3ceX08HAO4kI0aMUMmSJZWcnKyTJ09qzZo16tu3r8aPH6+vv/5alStXdox94403NGjQIJfWf+LECQ0fPlwlSpRQ1apVs7zcDz/84NJ2suNG2aZNm6bU1NQcz3ArVq1apYceekjDhg276dhWrVrp+++/V7t27dS9e3clJyfr999/19KlS1W7dm2VK1cuFxIDdyaKDZCLGjVqpBo1ajimBw8erFWrVqlp06Zq3ry59uzZo4CAAEmSr6+vfH1z9kf04sWLypcvn/z9/XN0Ozfj5+fn0e1nxenTp1W+fPmbjtu0aZOWLl2qkSNH6rXXXnN67oMPPlBcXFwOJcy6CxcuKDAw0NMxgBzBR1GAhz322GMaMmSIjh49qrlz5zrmZ3SOTUxMjOrUqaPQ0FAFBQWpbNmyjl+ea9as0QMPPCBJ6tKli+Njr5kzZ0r65zyaihUrasuWLXr00UeVL18+x7LXn2OTJiUlRa+99prCw8MVGBio5s2bKzY21mlMiRIl1Llz53TLXrvOm2XL6BybCxcu6OWXX1axYsVkt9tVtmxZvfvuuzLGOI2z2Wzq1auXlixZoooVK8put6tChQpatmxZxjv8OqdPn9Zzzz2nsLAw5c2bV1WqVNGsWbMcz6ed33L48GF9++23juxHjhzJcH0HDx6UJD388MPpnvPx8VGhQoUc00ePHtVLL72ksmXLKiAgQIUKFdIzzzyT6bqv9dNPP+mZZ55R8eLFZbfbVaxYMfXr10+XLl1yGte5c2cFBQXp4MGDaty4sfLnz6/27dtr2LBh8vPz05kzZ9Kt+/nnn1doaKguX7580xyAt6HYAF4g7XyNG30k9Ntvv6lp06ZKSkrSiBEjNG7cODVv3lzr1q2TJN13330aMWKEpH9+Mc2ZM0dz5szRo48+6ljH2bNn1ahRI1WtWlUTJkxQ/fr1b5hr5MiR+vbbbzVw4ED17t1bMTExio6OTvfL82ayku1axhg1b95c7733np588kmNHz9eZcuW1YABA9S/f/9043/++We99NJLatu2rcaOHavLly+rVatWOnv27A1zXbp0SfXq1dOcOXPUvn17/ec//1FISIg6d+6siRMnOrLPmTNHhQsXVtWqVR3Z77rrrgzXGRUVJUmaN2+erl69esPtb9q0Sf/73//Utm1bvf/+++rRo4dWrlypevXq6eLFizdc9vPPP9fFixf14osvatKkSWrYsKEmTZqkjh07pht79epVNWzYUEWKFNG7776rVq1aqUOHDrp69ao+++wzp7FXrlzRokWL1KpVK+XNm/eGGQCvZADkuBkzZhhJZtOmTZmOCQkJMdWqVXNMDxs2zFz7I/ree+8ZSebMmTOZrmPTpk1GkpkxY0a65+rWrWskmalTp2b4XN26dR3Tq1evNpJM0aJFTUJCgmP+woULjSQzceJEx7yoqCjTqVOnm67zRtk6depkoqKiHNNLliwxkszbb7/tNO7pp582NpvNHDhwwDFPkvH393eat2PHDiPJTJo0Kd22rjVhwgQjycydO9cx78qVK6ZWrVomKCjI6bVHRUWZJk2a3HB9xhiTmprq2NdhYWGmXbt2ZvLkyebo0aPpxl68eDHdvPXr1xtJZvbs2Y55aX8fq1evvuGyo0aNMjabzWlbnTp1MpLMoEGD0o2vVauWqVmzptO8xYsXp9sWcDvhiA3gJYKCgm54dVRoaKgk6auvvsr2ibZ2u11dunTJ8viOHTsqf/78jumnn35aERER+u6777K1/az67rvv5OPjo969ezvNf/nll2WM0ffff+80Pzo6WqVKlXJMV65cWcHBwTp06NBNtxMeHq527do55vn5+al3795KTEzUjz/+6HJ2m82m5cuX6+2331aBAgU0f/589ezZU1FRUWrTpo3TOTZp51NJUnJyss6ePavSpUsrNDRUW7duveF2rl32woUL+uuvv1S7dm0ZY7Rt27Z041988cV08zp27KgNGzY4Pj6T/jnSVKxYMdWtW9eVlw14DYoN4CUSExOdSsT12rRpo4cffljdunVTWFiY2rZtq4ULF7pUcooWLerSicJlypRxmrbZbCpdunSWzgG5FUePHlVkZGS6/XHfffc5nr9W8eLF062jQIEC+vvvv2+6nTJlyihPHud/CjPbTlbZ7Xa9/vrr2rNnj06cOKH58+froYce0sKFC9WrVy/HuEuXLmno0KGO84gKFy6su+66S3FxcYqPj7/hNo4dO6bOnTurYMGCCgoK0l133eUoI9cv6+vrq7vvvjvdOtq0aSO73a558+Y5llu6dKnat2+fa/dQAtyNYgN4gT/++EPx8fEqXbp0pmMCAgK0du1arVixQh06dNCvv/6qNm3a6PHHH1dKSkqWtnPt//LdJbNfgFnN5A4+Pj4ZzjfXnWjsCREREWrbtq3Wrl2rMmXKaOHChY5zb/79739r5MiRat26tRYuXKgffvhBMTExKlSo0A0La0pKih5//HHH+U9LlixRTEyM42Ts65e12+3pypv0T/lr2rSpo9gsWrRISUlJevbZZ9306oHcR7EBvMCcOXMkSQ0bNrzhuDx58qhBgwYaP368du/erZEjR2rVqlVavXq1pMxLRnbt37/fadoYowMHDjhdwVSgQIEML2G+/miHK9mioqJ04sSJdB/Npd3cLu0E3VsVFRWl/fv3pysC7t6O9M9HXJUrV1ZycrL++usvSf8UiU6dOmncuHF6+umn9fjjj6tOnTo3vSR8586d2rdvn8aNG6eBAweqRYsWio6OVmRkpMu5OnbsqH379mnTpk2aN2+eqlWrpgoVKmTnJQJegWIDeNiqVav01ltvqWTJkmrfvn2m486dO5duXtqN7pKSkiTJcW8Sd90rZfbs2U7lYtGiRfrzzz/VqFEjx7xSpUrpl19+0ZUrVxzzli5dmu6ycFeyNW7cWCkpKfrggw+c5r/33nuy2WxO278VjRs3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oqOj1bt3bx08eNDd2RQREaHy5cs7zbvvvvt07NixTJcZPHiw4uPjHY/Y2Fi35wIAAN7J5WKzfPlylS9fXhs3blTlypVVuXJlbdiwQRUqVFBMTIxbwz388MPau3ev07x9+/YpKioq02XsdruCg4OdHgAA4M7g8kdRgwYNUr9+/TR69Oh08wcOHKjHH3/cbeH69eun2rVr65133lHr1q21ceNGffzxx/r444/dtg0AAGAdLh+x2bNnj5577rl087t27ardu3e7JVSaBx54QF9++aXmz5+vihUr6q233tKECRPUvn17t24HAABYg8tHbO666y5t375dZcqUcZq/ffv2HLlSqmnTpmratKnb1wsAAKzH5WLTvXt3Pf/88zp06JBq164tSVq3bp3GjBmj/v37uz0gAABAVrlcbIYMGaL8+fNr3LhxGjx4sCQpMjJSb775pnr37u32gAAAAFnlcrGx2Wzq16+f+vXrp/Pnz0uS8ufP7/ZgAAAArnK52FyLQgMAALxJtm7QBwAA4I0oNgAAwDIoNgAAwDJcKjbJyclq0KCB9u/fn1N5AAAAss2lYuPn56dff/01p7IAAADcEpc/inr22Wc1ffr0nMgCAABwS1y+3Pvq1av65JNPtGLFCt1///0KDAx0en78+PFuCwcAAOAKl4vNrl27VL16dUnSvn37nJ6z2WzuSQUAAJANLheb1atX50QOAACAW5bty70PHDig5cuX69KlS5IkY4zbQgEAAGSHy8Xm7NmzatCgge699141btxYf/75pyTpueee08svv+z2gAAAAFnlcrHp16+f/Pz8dOzYMeXLl88xv02bNlq2bJlbwwEAALjC5XNsfvjhBy1fvlx333230/wyZcro6NGjbgsGAADgKpeP2Fy4cMHpSE2ac+fOyW63uyUUAABAdrhcbB555BHNnj3bMW2z2ZSamqqxY8eqfv36bg0HAADgCpc/iho7dqwaNGigzZs368qVK3r11Vf122+/6dy5c1q3bl1OZAQAAMgSl4/YVKxYUfv27VOdOnXUokULXbhwQS1bttS2bdtUqlSpnMgIAACQJS4fsZGkkJAQvf766+7OAgAAcEuyVWz+/vtvTZ8+XXv27JEklS9fXl26dFHBggXdGg4AAMAVNuPiLYPXrl2rZs2aKSQkRDVq1JAkbdmyRXFxcfrmm2/06KOP5kjQ7EpI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+Ph41atXTxEREY7HZ5995uloAADAC3n1ERtjjKcjAACA24hXH7EBAABwBcUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYBsUGAABYxm1RbCZPnqwSJUoob968qlmzpjZu3OjpSAAAwAt5fbH57LPP1L9/fw0bNkxbt25VlSpV1LBhQ50+fdrT0QAAgJfx+mIzfvx4de/eXV26dFH58uU1depU5cuXT5988omnowEAAC/j1cXmypUr2rJli6Kjox3z8uTJo+joaK1fv96DyQAAgDfy9XSAG/nrr7+UkpKisLAwp/lhYWH6/fffM1wmKSlJSUlJjun4+HhJUkJCgtvzpSZddPs6AQC4neTE79dr12uMcWk5ry422TFq1CgNHz483fxixYp5IA0AANYWMiFn13/+/HmFhIRkebxXF5vChQvLx8dHp06dcpp/6tQphYeHZ7jM4MGD1b9/f8d0amqqzp07p0KFCslms7ktW0JCgooVK6bY2FgFBwe7bb057XbMTebcQebcQebcQebckZOZjTE6f/68IiMjXVrOq4uNv7+/7r//fq1cuVJPPfWUpH+KysqVK9WrV68Ml7Hb7bLb7U7zQkNDcyxjcHDwbfMGvNbtmJvMuYPMuYPMuYPMuSOnMrtypCaNVxcbSerfv786deqkGjVq6MEHH9SECRN04cIFdenSxdPRAACAl/H6YtOmTRudOXNGQ4cO1cmTJ1W1alUtW7Ys3QnFAAAAXl9sJKlXr16ZfvTkKXa7XcOGDUv3sZe3ux1zkzl3kDl3kDl3kDl3eGNmm3H1OioAAAAv5dU36AMAAHAFxQYAAFgGxQYAAFgGxQYAAFjGHVtsRo8eLZvNpr59+zrmXb58WT179lShQoUUFBSkVq1apbvr8bFjx9SkSRPly5dPRYoU0YABA3T16lWnMWvWrFH16tVlt9tVunRpzZw5M932J0+erBIlSihv3ryqWbOmNm7cmGHON998UzabzelRrlw5r84sScePH9ezzz6rQoUKKSAgQJUqVdLmzZsdzxtjNHToUEVERCggIEDR0dHav3+/0zrOnTun9u3bKzg4WKGhoXruueeUmJjoNObXX3/VI488orx586pYsWIaO3Zsuiyff/65ypUrp7x586pSpUr67rvv0o0pUaJEuv1ss9nUs2dPr93PKSkpGjJkiEqWLKmAgACVKlVKb731ltP3qnjbfpb+uT163759FRUVpYCAANWuXVubNm3ymsxr165Vs2bNFBkZKZvNpiVLljgt4+l8GWUpVKiQfHx8ZLfbM8y8ePFiPfHEE447sG/fvj3dtnL7PR4eHi4fHx/5+/uny5ycnKyBAweqUqVKCgwMVGRkpDp27KgTJ054dD9HRETIbrfrrrvuUlhYWIb7+s0331S5cuUUGBioAgUKKDo6Whs2bPBo7pu9P67Vo0cP2Ww2TZgwwaOZb/TzdVPmDrRx40ZTokQJU7lyZdOnTx/H/B49ephixYqZlStXms2bN5uHHnrI1K5d2/H81atXTcWKFU10dLTZtm2b+e6770zhwoXN4MGDHWMOHTpk8uXLZ/r37292795tJk2aZHx8fMyyZcscYxYsWGD8/f3NJ598Yn777TfTvXt3Exoaak6dOpUu67Bhw0yFChXMn3/+6XicOXPGqzOfO3fOREVFmc6dO5sNGzaYQ4cOmeXLl5sDBw44xowePdqEhISYJUuWmB07dpjmzZubkiVLmkuXLjnGPPnkk6ZKlSrml19+MT/99JMpXbq0adeuneP5+Ph4ExYWZtq3b2927dpl5s+fbwICAsxHH33kGLNu3Trj4+Njxo4da3bv3m3eeOMN4+fnZ3bu3OmU+fTp0077OCYmxkgyq1ev9tr9PHLkSFOoUCGzdOlSc/jwYfP555+boKAgM3HiRK/dz8YY07p1a1O+fHnz448/mv3795thw4aZ4OBg88cff3hF5g8//NC8/vrrZvHixUaS+fLLL53yezrftfs0LcuQIUNM9+7dzQMPPGAkmc8++8wp8+zZs83w4cPNtGnTjCSzbdu2dH8vuf0e79u3r3n++edNdHS0kWRmzJjhGBMXF2eio6PNZ599Zn7//Xezfv168+CDD5r777/fKXNu7+clS5aYyZMnmzJlypgiRYpk+P6YN2+eiYmJMQcPHjS7du0yzz33nAkODjanT5/22vdHmsWLF5sqVaqYyMhI895773l8X2f283Uzd1yxOX/+vClTpoyJiYkxdevWdRSbuLg44+fnZz7//HPH2D179hhJZv369cYYY7777juTJ08ec/LkSceYKVOmmODgYJOUlGSMMebVV181FSpUcNpmmzZtTMOGDR3TDz74oOnZs6djOiUlxURGRppRo0alyzts2DBTpUqVDF+Lt2YeOHCgqVOnToaZjTEmNTXVhIeHm//85z9Or8Vut5v58+cbY4zZvXu3kWQ2bdrkGPP9998bm81mjh8/bowx5sMPPzQFChRwvI60bZctW9Yx3bp1a9OkSROn7desWdO88MILmeYzxpg+ffqYUqVKmdTUVK/dz02aNDFdu3Z1mteyZUvTvn17Y4x37ueLFy8aHx8fs3TpUqf51atXN6+//rrXZb7+F5c35cssiyTTv39/k5HDhw9nWGw8/R6XZJ599tkMM6fZuHGjkWSOHj1qjPH8frbb7RkWm+vFx8cbSWbFihVekTuz98cff/xhihYtanbt2mWioqKcio2nM1/785UVd9xHUT179lSTJk0UHR3tNH/Lli1KTk52ml+uXDkVL15c69evlyStX79elSpVcrrrccOGDZWQkKDffvvNMeb6dTds2NCxjitXrmjLli1OY/LkyaPo6GjHmOvt379fkZGRuueee9S+fXsdO3bMqzN//fXXqlGjhp555hkVKVJE1apV07Rp0xzPHz58WCdPnnRaX0hIiGrWrOmUOzQ0VDVq1HCMiY6OVp48eRyHddevX69HH31U/v7+Trn37t2rv//+O0uvLSNXrlzR3Llz1bVrV9lsNq/dz7Vr19bKlSu1b98+SdKOHTv0888/q1GjRl67n69evaqUlBTlzZvXaX5AQIB+/vlnr8x8LW/Kl1kWSdq7d2+mryEjnn6PZyVzfHy8bDab47v/PL2fa9asecO8aa/3448/VkhIiKpUqeIVuaX0+zo1NVUdOnTQgAEDVKFChXSvw9OZr/35yoo7qtgsWLBAW7du1ahRo9I9d/LkSfn7+6f7wsywsDCdPHnSMeb6r3JIm77ZmISEBF26dEl//fWXUlJSMhyTto5r1axZUzNnztSyZcs0ZcoUHT58WI888ojOnz/vtZkPHTqkKVOmqEyZMlq+fLlefPFF9e7dW7NmzXLa7o3Wd/LkSRUpUsTpeV9fXxUsWNAtry2j3GmWLFmiuLg4de7c2bEOb9zPgwYNUtu2bVWuXDn5+fmpWrVq6tu3r9q3b++0XW/az/nz51etWrX01ltv6cSJE0pJSdHcuXO1fv16/fnnn16Z+VrelC+zLJIUFxeX6WvI7HV58j1+s8yXL1/WwIED1a5dO8cXLXp6P9/oa32WLl2qoKAg5c2bV++9955iYmJUuHBhr8gtpd/XY8aMka+vr3r37p3h6/F05pv9XF7vtvhKBXeIjY1Vnz59FBMTk+5/i94s7X/fklS5cmXVrFlTUVFRWrhwoQICAjyYLHOpqamqUaOG3nnnHUlStWrVtGvXLk2dOlWdOnXycLqbmz59uho1aqTIyEhPR7mhhQsXat68efr0009VoUIFbd++XX379lVkZKRX7+c5c+aoa9euKlq0qHx8fFS9enW1a9dOW7Zs8XQ0eKHk5GS1bt1axhhNmTLF03GypH79+tq+fbv++usvTZs2Ta1bt9aGDRvSlQNvsGXLFk2cOFFbt26VzWbzdBy3uGOO2GzZskWnT59W9erV5evrK19fX/344496//335evrq7CwMF25ciVdkz116pTCw8MlSeHh4emuEkibvtmY4OBgBQQEqHDhwvLx8clwTNo6biQ0NFT33nuvDhw4oPDwcK/MHBERofLlyzvNu++++xwfoaUtc6P1hYeH6/Tp007PX716VefOnXPLa8tsXx89elQrVqxQt27dHPO8dT8PGDDAcdSmUqVK6tChg/r16+c4Iumt+7lUqVL68ccflZiYqNjYWG3cuFHJycm65557vDZzGm/Kl1kWSemOvNyMp9/jmWVOKzVHjx5VTEyM42hN2rY8uZ8zeg1pAgMDVbp0aT300EOaPn26fH19NX36dK/ILTnv659++kmnT59W8eLFHb8bjx49qpdfflklSpTwisxZ/f2Y5o4pNg0aNNDOnTu1fft2x6NGjRpq3769489+fn5auXKlY5m9e/fq2LFjqlWrliSpVq1a2rlzp9NfcNoPW9ov8lq1ajmtI21M2jr8/f11//33O41JTU3VypUrHWNuJDExUQcPHlRERITuv/9+r8z88MMPp/sMd9++fYqKipIklSxZUuHh4U7rS0hI0IYNG5xyx8XFOf0vftWqVUpNTXV8tl2rVi2tXbtWycnJTrnLli2rAgUKZOm1XW/GjBkqUqSImjRp4pjnrfv54sWLjvMT0vj4+Cg1NVWSd+9n6Z9//CMiIvT3339r+fLlatGihddn9qZ8mWWRpLJly2b6GjLi6fd4RpnTSs3+/fu1YsUKFSpUyOl5T+/n6y/hvpHU1FQlJSV5RW7JeV936NBBv/76q9PvxsjISA0YMEDLly/3iszX/nxlSZZPM7aga6+KMuafyx2LFy9uVq1aZTZv3mxq1aplatWq5Xg+7XLHJ554wmzfvt0sW7bM3HXXXRle7jhgwACzZ88eM3ny5Awvd7Tb7WbmzJlm9+7d5vnnnzehoaFOVxukefnll82aNWvM4cOHzbp160x0dLQpXLiw49JBb8y8ceNG4+vra0aOHGn2799v5s2bZ/Lly2fmzp3rGDN69GgTGhpqvvrqK/Prr7+aFi1aZHjJbLVq1cyGDRvMzz//bMqUKeN0eWFcXJwJCwszHTp0MLt27TILFiww+fLlS3d5oa+vr3n33XfNnj17zLBhwzK9DDklJcUUL17cDBw4MN1z3rifO3XqZIoWLeq43Hvx4sWmcOHC5tVXX/Xq/bxs2TLz/fffm0OHDpkffvjBVKlSxdSsWdNcuXLFKzJv2LDBbNu2zWzbts1IMuPHjzfbtm1zXI3j6XzXXxobGhpqFixYYBYuXGjq1atnJJkxY8Y4ZT579qzZtm2b+fbbb40ks2DBArNt2zbz559/OtaV2+/xqVOnmi+++MK0bNnSSDLDhw93ZL5y5Ypp3ry5ufvuu8327dudbsVw7VU3ub2fv/rqK/PLL7+YevXqmcjIyHTvj8TERDN48GCzfv16c+TIEbN582bTpUsXY7fbza5du7z2/XG966+K8tS+zuzn62YoNtcUm0uXLpmXXnrJFChQwOTLl8/861//cvrBN8aYI0eOmEaNGpmAgABTuHBh8/LLL5vk5GSnMatXrzZVq1Y1/v7+5p577nG6P0OaSZMmmeLFixt/f3/z4IMPml9++SXDjG3atDERERHG39/fFC1a1LRp08bpfjDemNkYY7755htTsWJFY7fbTbly5czHH3/s9HxqaqoZMmSICQsLM3a73TRo0MDs3bvXaczZs2dNu3btTFBQkAkODjZdunQx58+fdxqzY8cOU6dOHWO3203RokXN6NGj02VZuHChuffee42/v7+pUKGC+fbbbzPMvHz5ciMpXQ5jvHM/JyQkmD59+pjixYubvHnzmnvuuce8/vrrTv/we+N+/uyzz8w999xj/P39TXh4uOnZs6eJi4vzmsyrV682ktI9OnXq5BX5rpWWpUCBAjfMPGPGjAyfHzZsmGNduf0eT7sPTEaZ0y5Lz+iRdm8pT+znsLAw4+fnl2nuS5cumX/9618mMjLS+Pv7m4iICNO8eXOzceNGp/V52/vjehkVG0/s68x+vm7GZsw1tykFAAC4jd0x59gAAADro9gAAADLoNgAAADLoNgAAADLoNgAAADLoNgAAADLoNgAAADLoNgAuK3MnDnT5e9CAnDnoNgAyFVnzpzRiy++qOLFi8tutys8PFwNGzbUunXrPB0NgAX4ejoAgDtLq1atdOXKFc2aNUv33HOPTp06pZUrV+rs2bO5luHKlSvy9/fPte0ByD0csQGQa+Li4vTTTz9pzJgxql+/vqKiovTggw9q8ODBat68uSRp/PjxqlSpkgIDA1WsWDG99NJLSkxMzHSdBw8eVIsWLRQWFqagoCA98MADWrFihdOYEiVK6K233lLHjh0VHBys559/Xo899ph69erlNO7MmTPy9/dP9w3EAG4fFBsAuSYoKEhBQUFasmSJkpKSMhyTJ08evf/++/rtt980a9YsrVq1Sq+++mqm60xMTFTjxo21cuVKbdu2TU8++aSaNWumY8eOOY179913VaVKFW3btk1DhgxRt27d9OmnnzrlmDt3rooWLarHHnvMPS8YQK7jSzAB5KovvvhC3bt316VLl1S9enXVrVtXbdu2VeXKlTMcv2jRIvXo0UN//fWXpH9OHu7bt6/i4uIy3UbFihXVo0cPxxGZEiVKqFq1avryyy8dYy5fvqzIyEhNnTpVrVu3liRVqVJFLVu21LBhw9z0agHkNo7YAMhVrVq10okTJ/T111/rySef1Jo1a1S9enXNnDlTkrRixQo1aNBARYsWVf78+dWhQwedPXtWFy9ezHB9iYmJeuWVV3TfffcpNDRUQUFB2rNnT7ojNjVq1HCazps3rzp06KBPPvlEkrR161bt2rVLnTt3dvtrBpB7KDYAcl3evHn1+OOPa8iQIfrf//6nzp07a9iwYTpy5IiaNm2qypUr64svvtCWLVs0efJkSf+c8JuRV155RV9++aXeeecd/fTTT9q+fbsqVaqUbnxgYGC6Zbt166aYmBj98ccfmjFjhh577DFFRUW5/wUDyDVcFQXA48qXL68lS5Zoy5YtSk1N1bhx45Qnzz//71q4cOENl123bp06d+6sf/3rX5L+OYJz5MiRLG23UqVKqlGjhqZNm6ZPP/1UH3zwwS29DgCeR7EBkGvOnj2rZ555Rl27dlXlypWVP39+bd68WWPHjlWLFi1UunRpJScna9KkSWrWrJnWrVunqVOn3nCdZcqU0eLFi9WsWTPZbDYNGTJEqampWc7UrVs39erVS4GBgY5yBOD2xUdRAHJNUFCQatasqffee0+PPvqoKlasqCFDhqh79+764IMPVKVKFY0fP15jxoxRxYoVNW/ePI0aNeqG6xw/frwKFCig2rVrq1mzZmrYsKGqV6+e5Uzt2rWTr6+v2rVrp7x5897qSwTgYVwVBeCOduTIEZUqVUqbNm1yqRAB8E4UGwB3pOTkZJ09e1avvPKKDh8+zFc6ABbBR1EA7kjr1q1TRESENm3adNPzeADcPjhiAwAALIMjNgAAwDIoNgAAwDIoNgAAwDIoNgAAwDIoNgAAwDIoNgAAwDIoNgAAwDIoNgAAwDIoNgAAwDL+H+EoGf6VNONaAAAAAElFTkSuQmCC\n",
                         "text/plain": [
-                            "<Figure size 1000x600 with 1 Axes>"
+                            "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "dist_salary(df_missing)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 17,
             "id": "45559024-5905-43df-a021-19a2d0b77dff",
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Executor saved to cache file make_boxplots_25996.py\n"
+                    ]
+                }
+            ],
             "source": [
                 "dept_salary = PandasGenie(\"make boxplots of salary grouped by department\", columns=df_missing.columns)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 18,
             "id": "637d39d9-c0bf-4a20-89bc-37af671c77cd",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAtEAAAHWCAYAAACxJNUiAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/NK7nSAAAACXBIWXMAAA9hAAAPYQGoP6dpAABQp0lEQVR4nO3deVhUdf//8dcAsogCriCpSGaKS+4L5lJJoeaCZq65FGmLlEsuWYloi3eau6WV31vNG0vtVjPNLbUoNVRcUkvTblNT0UoBUUGB8/uji/NjApWDyIA+H9c118Wcz/uc8z4zzvji8JkzNsMwDAEAAADINSdHNwAAAAAUNYRoAAAAwCJCNAAAAGARIRoAAACwiBANAAAAWESIBgAAACwiRAMAAAAWEaIBAAAAiwjRAAAAgEWEaAC33UMPPaSHHnrI0W3c1G+//SabzaYFCxaYy6KiomSz2Qpk//98nL755hvZbDZ9/vnnBbL/AQMGqEqVKgWyr6wK+jgBID8QogFks3//fnXr1k0BAQFyd3fXPffco0cffVSzZs1ydGtFwunTpxUVFaW9e/c6upVsCnNvt1vmL0SZt+LFi6ty5crq2LGj5s+fr9TUVEe3mGvvvPOOVq5c6eg2cmXbtm2KiopSQkKCo1sB8hUhGoCdbdu2qVGjRtq3b58GDhyo2bNn69lnn5WTk5NmzJjh6PYK3BtvvKErV65YWuf06dMaP3685aC6YcMGbdiwwdI6Vt2ot48//liHDx++rfsvDObMmaNFixZp1qxZevbZZ3X+/Hk988wzatKkiU6ePOno9nKlqIXo8ePHE6Jxx3FxdAMACpe3335b3t7e2rlzp3x8fOzGzp0755imskhLS1NGRoZcXV0LZH8uLi5ycbm9b5WXL19W8eLFC+yYrqdYsWIO3X9B6datm8qWLWvej4yMVHR0tPr166cnn3xSP/zwgwO7uz7DMJSSkiIPDw9HtwJAnIkG8A+//vqratWqlS1AS1L58uXt7s+fP1+PPPKIypcvLzc3N9WsWVNz5sy56T6uXr2qyMhINWzYUN7e3vL09FTLli21ZcsWu7rMOcrvvfeepk+frqpVq8rNzU07duyQp6enhgwZkm3bv//+u5ydnTVx4sQb9pCQkKABAwbI29tbPj4+6t+/f45nynKaE71x40a1aNFCPj4+KlGihKpXr67XXntN0t/zexs3bixJevrpp82pA5nzrB966CHVrl1bcXFxatWqlYoXL26ue7254+np6Xrttdfk5+cnT09PderUKdsZ0ypVqmjAgAHZ1s26zZv1ltOc6EuXLumVV15RpUqV5ObmpurVq+u9996TYRh2dTabTREREVq5cqVq164tNzc31apVS+vWrcvW0/Xc7DjHjRunYsWK6Y8//si27qBBg+Tj46OUlJRc7y+rPn366Nlnn1VsbKw2btxoNxYbG6u2bdvK29tbxYsXV+vWrbV161a7msx/J4cOHVL37t3l5eWlMmXKaMiQIdl6yu3rpkqVKurQoYPWr1+vRo0aycPDQx9++KFsNpsuXbqkhQsXms9h5nOf2ccvv/yip556St7e3ipXrpzGjh0rwzB08uRJde7cWV5eXvLz89OUKVOy7Tc1NVXjxo3TfffdJzc3N1WqVEmjRo3KNt0lN895VFSURo4cKUkKDAw0+/3tt99y/dwAhRVnogHYCQgI0Pbt23XgwAHVrl37hrVz5sxRrVq11KlTJ7m4uOjLL7/Uiy++qIyMDA0ePPi66yUlJWnevHnq1auXBg4cqIsXL+r//u//FBoaqh07dqhevXp29fPnz1dKSooGDRokNzc3Va5cWV26dNGSJUs0depUOTs7m7WffvqpDMNQnz59rrt/wzDUuXNnff/993r++ecVFBSkFStWqH///jd9fA4ePKgOHTrogQce0IQJE+Tm5qajR4+aoSooKEgTJkxQZGSkBg0apJYtW0qSmjdvbm7jr7/+Urt27dSzZ0899dRT8vX1veE+3377bdlsNo0ePVrnzp3T9OnTFRISor1791o6K5mb3rIyDEOdOnXSli1bFB4ernr16mn9+vUaOXKkTp06pWnTptnVf//991q+fLlefPFFlSxZUjNnztQTTzyhEydOqEyZMjft72bH2bdvX02YMEFLlixRRESEud7Vq1f1+eef64knnpC7u3uuH49/6tu3rz766CNt2LBBjz76qCRp8+bNateunRo2bKhx48bJycnJDMHfffedmjRpYreN7t27q0qVKpo4caJ++OEHzZw5UxcuXNAnn3xi1lh53Rw+fFi9evXSc889p4EDB6p69epatGiRnn32WTVp0kSDBg2SJFWtWtVuvR49eigoKEj/+te/tGbNGr311lsqXbq0PvzwQz3yyCN69913FR0d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xx+bQXngwIGqXr26GjVqpHLlymU7Ow5cj81gAiNQaDz66KPy8/PTokWLHN3KbZGRkaGgoCB1795db775pqPbAZBPHnroIdWrV4+v48ZdhekcgINcvnxZc+fOVWhoqJydnfXpp5/q66+/trvmc1F3/PhxbdiwQa1bt1Zqaqpmz56tY8eOqXfv3o5uDQCAW0KIBhwkc+rF22+/rZSUFFWvXl3//e9/FRIS4ujW8o2Tk5MWLFigESNGyDAM1a5dW19//bWCgoIc3RoAALeE6RwAAACARXywEAAAALCIEA0AAABYRIgGAAAALCJEAwAAABYRogEAAACLCNEAUAQ99NBDGjp0qKPbAIC7FiEaAJBnv/32m2w2m/bu3evoVkxVqlThm/MA3HaEaABAnly9etXRLQCAwxCiAaCQu3Tpkvr166cSJUqoQoUKmjJlit14amqqRowYoXvuuUeenp5q2rSpvvnmG3N8wYIF8vHx0cqVK1WtWjW5u7srNDRUJ0+eNGt+/fVXde7cWb6+vipRooQaN26sr7/+2m4/VapU0Ztvvql+/frJy8tLgwYNUmBgoCSpfv36stlseuihhyRJAwYMUFhYmN555x35+vrKx8dHEyZMUFpamkaOHKnSpUurYsWKmj9/vt0+Tp48qe7du8vHx0elS5dW586d9dtvv5njmdt97733VKFCBZUpU0aDBw/WtWvXJP09zeX48eMaNmyYbDabbDbbrT78AJAjQjQAFHIjR47Ut99+qy+++EIbNmzQN998o927d5vjERER2r59uz777DP9+OOPevLJJ9W2bVsdOXLErLl8+bLefvttffLJJ9q6dasSEhLUs2dPczw5OVnt27fXpk2btGfPHrVt21YdO3bUiRMn7Hp57733VLduXe3Zs0djx47Vjh07JElff/21zpw5o+XLl5u1mzdv1unTpxUTE6OpU6dq3Lhx6tChg0qVKqXY2Fg9//zzeu655/T7779Lkq5du6bQ0FCVLFlS3333nbZu3aoSJUqobdu2dme9t2zZol9//VVbtmzRwoULtWDBAi1YsECStHz5clWsWFETJkzQmTNndObMmfx7IgAgKwMAUGhdvHjRcHV1NZYuXWou++uvvwwPDw9jyJAhxvHjxw1nZ2fj1KlTduu1adPGGDNmjGEYhjF//nxDkvHDDz+Y4z///LMhyYiNjb3uvmvVqmXMmjXLvB8QEGCEhYXZ1Rw7dsyQZOzZs8duef/+/Y2AgAAjPT3dXFa9enWjZcuW5v20tDTD09PT+PTTTw3DMIxFixYZ1atXNzIyMsya1NRUw8PDw1i/fr3ddtPS0syaJ5980ujRo4ddn9OmTbvucQFAfnBxcIYHANzAr7/+qqtXr6pp06bmstKlS6t69eqSpP379ys9PV3333+/3XqpqakqU6aMed/FxUWNGzc279eoUUM+Pj76+eef1aRJEyUnJysqKkpr1qzRmTNnlJaWpitXrmQ7E92oUaNc916rVi05Of3/P3j6+vqqdu3a5n1nZ2eVKVNG586dkyTt27dPR48eVcmSJe22k5KSol9//dVuu87Ozub9ChUqaP/+/bnuCwDyAyEaAIqw5ORkOTs7Ky4uzi5YSlKJEiVyvZ0RI0Zo48aNeu+993TffffJw8ND3bp1y/bhQU9Pz1xvs1ixYnb3bTZbjssyMjLMY2nYsKGio6OzbatcuXI33G7mNgCgoBCiAaAQq1q1qooVK6bY2FhVrlxZknThwgX98ssvat26terXr6/09HSdO3dOLVu2vO520tLStGvXLjVp0kSSdPjwYSUkJCgoKEiStHXrVg0YMEBdunSR9HegzfqBvutxdXWVJKWnp9/KYUqSGjRooCVLlqh8+fLy8vLK83ZcXV3zpR8AuBE+WAgAhViJEiUUHh6ukSNHavPmzTpw4IAGDBhgTpO4//771adPH/Xr10/Lly/XsWPHtGPHDk2cOFFr1qwxt1OsWDG99NJLio2NVVxcnAYMGKBmzZqZobpatWpavny59u7dq3379ql37965Ortbvnx5eXh4aN26dTp79qwSExPzfKx9+vRR2bJl1blzZ3333Xc6duyYvvnmG7388svmhw9zo0qVKoqJidGpU6f0559/5rkfALgRQjQAFHKTJ09Wy5Yt1bFjR4WEhKhFixZq2LChOT5//nz169dPr7zyiqpXr66wsDDt3LnTPHMtScWLF9fo0aPVu3dvPfjggypRooSWLFlijk+dOlWlSpVS8+bN1bFjR4WGhqpBgwY37c3FxUUzZ87Uhx9+KH9/f3Xu3DnPx1m8eHHFxMSocuXK6tq1q4KCghQeHq6UlBRLZ6YnTJig3377TVWrVrWbBgIA+clmGIbh6CYAALfPggULNHToUCUkJDi6FQC4Y3AmGgAAALCIEA0AAABYxHQOAAAAwCLORAMAAAAWEaIBAAAAiwjRAAAAgEWEaAAAAMAiQjQAAABgESEaAAAAsIgQDQAAAFhEiAYAAAAs+n/GSxRjxNxtOgAAAABJRU5ErkJggg==\n",
                         "text/plain": [
-                            "<Figure size 640x480 with 1 Axes>"
+                            "<Figure size 800x500 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "dept_salary(df_missing)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 21,
             "id": "538ddd26-4b79-4251-9f40-d8a8fc57673f",
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Loading executor from cache file count_high_earners_86151.py, set override = True to rerun\n"
+                    ]
+                }
+            ],
             "source": [
                 "dept_100k = PandasGenie(\"how many people in each department make more than 100K?\", columns=df_missing.columns)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 22,
             "id": "4e2e88e7-ac81-4710-8b45-cd94d3c44912",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "Department\n",
-                            "engineering    34\n",
-                            "product        33\n",
-                            "Name: ID, dtype: int64"
+                            "department\n",
+                            "engineering    20\n",
+                            "product        18\n",
+                            "Name: id, dtype: int64"
                         ]
                     },
-                    "execution_count": 26,
+                    "execution_count": 22,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dept_100k(df_missing)"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "c28b9343-8f96-4d99-a664-f7035a237ace",
+            "metadata": {},
+            "source": [
+                "# Inspecting Code\n",
+                "\n",
+                "All the genies export the generated code to the cache_dir path under individual py files. The exact name of the file used can be found in the log generated on execution. These could be of 2 types:\n",
+                "\n",
+                "1. `Executor saved to cache file make_boxplots_25996.py`: this will be shown the first time we run this\n",
+                "2. `Loading executor from cache file count_high_earners_86151.py, set override = True to rerun`: this will be shown when we run the genie after its cached without setting `override=True`\n",
+                "\n",
+                "all cached py files for the starter notebook can be found [here](https://github.com/thismlguy/code-genie/tree/main/docs/notebooks/_cache_starter)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 24,
+            "id": "b09e7679-9cc2-4b21-9d00-726a6035f570",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "import pandas as pd\n",
+                        "import random\n",
+                        "\n",
+                        "def generate_employee_df():\n",
+                        "    employee_data = {\"id\": [random.randint(1000,9999) for i in range(100)],\n",
+                        "                     \"name\": [\"Employee_\" + str(i) for i in range(1,101)],\n",
+                        "                     \"salary\": [random.randint(40000,150000) for i in range(100)],\n",
+                        "                     \"department\": [\"engineering\" if i<50 else \"product\" for i in range(100)]}\n",
+                        "    \n",
+                        "    employee_df = pd.DataFrame(employee_data)\n",
+                        "    return employee_df\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# the code can be inspected using `code` property:\n",
+                "print(data_gen.code)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "410d75a1-c890-47e2-b09e-0a9c7654c231",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "'generate_employee_df_41317.py'"
+                        ]
+                    },
+                    "execution_count": 9,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# the filename in which a genie is stored can be found using the `filename` property:\n",
+                "data_gen.filename"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d18a8f60-fb8a-456d-aa7d-08d50c9276c5",
+            "id": "7a6435aa-4299-428a-b7df-842a31841e22",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `code_genie-0.1.2/docs/requirements.txt` & `code_genie-0.2.0/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.2/pyproject.toml` & `code_genie-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `code_genie-0.1.2/PKG-INFO` & `code_genie-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code_genie
-Version: 0.1.2
+Version: 0.2.0
 Summary: Copilot to supercharge your notebooks
 Keywords: copilot,jupyter
 Author-email: Aarshay Jain <aarshay.jain@columbia.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,21 +35,21 @@
 Provides-Extra: build
 Provides-Extra: docs
 Provides-Extra: notebook
 
 # code-genie
 This library is your copilot for jupyter notebooks
 
-Latest version: 0.1.2
+Latest version: 0.2.0
 
 ## Documentation
 
-- [Started Notebook](https://code-genie.readthedocs.io/en/latest/notebooks/Starter.html)
-- [All Exampples](https://code-genie.readthedocs.io/en/latest/examples.html)
-- [API Documentation](https://code-genie.readthedocs.io/en/latest/api.html)
+- [Starter Notebook](https://code-genie.readthedocs.io/en/main/notebooks/Starter.html)
+- [All Examples](https://code-genie.readthedocs.io/en/main/examples.html)
+- [API Documentation](https://code-genie.readthedocs.io/en/main/api.html)
 
 ## Installation
 
 ```bash
 pip install code-genie
 ```
```


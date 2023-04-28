# Comparing `tmp/docstring_auditor-0.1.8.tar.gz` & `tmp/docstring_auditor-0.1.9.tar.gz`

## Comparing `docstring_auditor-0.1.8.tar` & `docstring_auditor-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/.aidev
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/Dockerfile
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/action.yml
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/.github/workflows/image-latest.yml
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/.github/workflows/image-release.yml
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/.github/workflows/release.yml
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/docstring_auditor/__init__.py
--rw-r--r--   0        0        0    11465 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/docstring_auditor/main.py
--rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/tests/test_critique.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/tests/test_exit_codes.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/tests/test_extractor.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/tests/test_reporter.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/LICENSE
--rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/README.md
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/.aidev
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/Dockerfile
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/action.yml
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/.github/workflows/image-latest.yml
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/.github/workflows/image-release.yml
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/docstring_auditor/__init__.py
+-rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/docstring_auditor/main.py
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/tests/test_critique.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/tests/test_exit_codes.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/tests/test_extractor.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/tests/test_reporter.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/LICENSE
+-rw-r--r--   0        0        0     6514 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/README.md
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     7275 2020-02-02 00:00:00.000000 docstring_auditor-0.1.9/PKG-INFO
```

### Comparing `docstring_auditor-0.1.8/Dockerfile` & `docstring_auditor-0.1.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.8/action.yml` & `docstring_auditor-0.1.9/action.yml`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.8/.github/workflows/image-latest.yml` & `docstring_auditor-0.1.9/.github/workflows/image-latest.yml`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.8/.github/workflows/image-release.yml` & `docstring_auditor-0.1.9/.github/workflows/image-release.yml`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.8/.github/workflows/test.yml` & `docstring_auditor-0.1.9/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   run:
     name: Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python-version: ['3.10']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
     env:
       OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
@@ -43,8 +43,9 @@
     - name: Run type checking
       run: hatch run dev:lint-types
 
     - name: Run format checking
       run: hatch run dev:lint-format
 
     - name: Run self test
+      if : ${{ matrix.python-version == '3.11' }}
       run: hatch run docstring-auditor
```

### Comparing `docstring_auditor-0.1.8/docstring_auditor/main.py` & `docstring_auditor-0.1.9/docstring_auditor/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,57 +5,61 @@
 import click
 import ast
 import json
 from typing import List, Optional, Dict, Tuple
 import openai
 
 
-def extract_functions(file_path: str) -> List[Optional[str]]:
+def extract_code_block(file_path: str) -> List[Optional[str]]:
     """
-    Extract functions from a Python file.
+    Extract functions and methods from a Python file.
 
-    This function reads a .py file and extracts each of the functions from the
+    This function reads a .py file and extracts each of the functions and methods from the
     file. It returns a list of strings, where each string contains the entire
-    code for a function, including the definition, docstring, and code.
+    code for a function or method, including the definition, docstring, and code.
 
     Parameters
     ----------
     file_path : str
-        The path to the .py file to extract functions from.
+        The path to the .py file to extract functions and methods from.
 
     Returns
     -------
     List[Optional[str]]
         A list of strings, where each string contains the entire code for a
-        function, including the definition, docstring, and code.
+        function or method, including the definition, docstring, and code.
 
     Examples
     --------
     >>> file_path = 'path/to/your/python_file.py'
-    >>> functions = extract_functions(file_path)
-    >>> for function in functions:
-    ...     print(function)
+    >>> functions_and_methods = extract_code_block(file_path)
+    >>> for function_or_method in functions_and_methods:
+    ...     print(function_or_method)
     ...     print('-' * 80)
 
     Notes
     -----
     This function may not work correctly for all cases, especially if there are
     nested functions or other complex structures.
     """
     with open(file_path, "r") as file:
         content = file.read()
 
     tree = ast.parse(content)
-    functions = [
+    functions_and_methods = [
         ast.get_source_segment(content, func)
         for func in tree.body
-        if isinstance(func, ast.FunctionDef)
+        if isinstance(func, (ast.FunctionDef, ast.ClassDef))
     ]
 
-    return functions
+    for cls in [node for node in tree.body if isinstance(node, ast.ClassDef)]:
+        for method in [node for node in cls.body if isinstance(node, ast.FunctionDef)]:
+            functions_and_methods.append(ast.get_source_segment(content, method))
+
+    return functions_and_methods
 
 
 def ask_for_critique(function: str, model: str) -> Dict[str, str]:
     """
     Query OpenAI for a critique of the docstring for a function.
 
     Parameters
@@ -165,44 +169,44 @@
             click.secho(f"A proposed solution to these concerns is:\n\n{solution}\n\n")
 
     return error_count, warning_count
 
 
 def process_file(file_path: str, model: str) -> Tuple[int, int]:
     """
-    Process a single Python file and analyze its functions' docstrings.
+    Process a single Python file and analyze its functions' and methods' docstrings.
 
-    This function processes the given Python file, extracts the functions within it,
+    This function processes the given Python file, extracts the functions and methods within it,
     and analyzes their docstrings for errors and warnings.
     It then returns the total number of errors and warnings found in the
-    docstrings of the functions in the given file.
+    docstrings of the functions and methods in the given file.
 
     Parameters
     ----------
     file_path : str
-        The path to the .py file to analyze the functions' docstrings.
+        The path to the .py file to analyze the functions' and methods' docstrings.
     model : str
         The name of the OpenAI model to use for the analysis.
 
     Returns
     -------
     Tuple[int, int]
-        A tuple containing the total number of errors and warnings found in the docstrings of the functions in the given file.
+        A tuple containing the total number of errors and warnings found in the docstrings of the functions and methods in the given file.
     """
-    functions = extract_functions(file_path)
+    functions_and_methods = extract_code_block(file_path)
 
     error_count = 0
     warning_count = 0
 
-    for idx, function in enumerate(functions):
+    for idx, function_or_method in enumerate(functions_and_methods):
         print(
-            f"Processing function {idx + 1} of {len(functions)} in file {file_path}..."
+            f"Processing function or method {idx + 1} of {len(functions_and_methods)} in file {file_path}..."
         )
-        assert isinstance(function, str)
-        critique = ask_for_critique(function, model)
+        assert isinstance(function_or_method, str)
+        critique = ask_for_critique(function_or_method, model)
         errors, warnings = report_concerns(critique)
         error_count += errors
         warning_count += warnings
 
     return error_count, warning_count
 
 
@@ -262,15 +266,17 @@
 )
 @click.option(
     "--model",
     type=click.STRING,
     default="gpt-4",
     help="The OpenAI model to use for docstring analysis. Default is 'gpt-4'.",
 )
-def docstring_auditor(path: str, ignore_dirs: List[str], error_on_warnings: bool, model: str):
+def docstring_auditor(
+    path: str, ignore_dirs: List[str], error_on_warnings: bool, model: str
+):
     """
     Analyze Python functions' docstrings in a given file or directory and provide critiques and suggestions for improvement.
 
     This program reads a Python file or directory, extracts the functions and their docstrings,
     and then analyzes the docstrings for errors, warnings,
     and possible improvements. The critiques and suggestions are then displayed to the user.
```

### Comparing `docstring_auditor-0.1.8/tests/test_critique.py` & `docstring_auditor-0.1.9/tests/test_critique.py`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.8/tests/test_exit_codes.py` & `docstring_auditor-0.1.9/tests/test_exit_codes.py`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.8/tests/test_reporter.py` & `docstring_auditor-0.1.9/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.8/.gitignore` & `docstring_auditor-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.8/LICENSE` & `docstring_auditor-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.8/README.md` & `docstring_auditor-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Docstring Auditor
 
 [![PyPI version](https://badge.fury.io/py/docstring-auditor.svg)](https://badge.fury.io/py/docstring-auditor)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/docstring-auditor)
 [![tests](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/test.yml)
 [![release](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml/badge.svg)](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml)
+[![release](https://img.shields.io/badge/docker-success-brightgreen)](https://github.com/agencyenterprise/docstring-auditor/pkgs/container/docstring-auditor)
 
 
 Meet _Docstring Auditor_, your go-to solution for maintaining precise and up-to-date Python code documentation.
 Tired of misleading or outdated docstrings? Docstring Auditor harnesses the power of large language models to analyze and critique your docstrings,
 ensuring they align with your code's true purpose. Accessible to both experts and novices,
 Docstring Auditor is your ultimate companion for clear, concise, and informative docstrings.
 Say hello to better code documentation!
```

### Comparing `docstring_auditor-0.1.8/pyproject.toml` & `docstring_auditor-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "docstring-auditor"
-version = "0.1.8"
+version = "0.1.9"
 authors = [{name = "Rob Luke", email = "rob.luke@ae.studio"}]
 description = "A tool to analyze Python functions' docstrings and provide critiques and suggestions for improvement"
 readme = "README.md"
 keywords = ["docstring", "auditor", "openai", "gpt"]
 url = "https://github.com/agencyenterprise/docstring-auditor"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.hatch.package]
```

### Comparing `docstring_auditor-0.1.8/PKG-INFO` & `docstring_auditor-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: docstring-auditor
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool to analyze Python functions' docstrings and provide critiques and suggestions for improvement
 Author-email: Rob Luke <rob.luke@ae.studio>
 License-File: LICENSE
 Keywords: auditor,docstring,gpt,openai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Docstring Auditor
 
 [![PyPI version](https://badge.fury.io/py/docstring-auditor.svg)](https://badge.fury.io/py/docstring-auditor)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/docstring-auditor)
 [![tests](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/test.yml)
 [![release](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml/badge.svg)](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml)
+[![release](https://img.shields.io/badge/docker-success-brightgreen)](https://github.com/agencyenterprise/docstring-auditor/pkgs/container/docstring-auditor)
 
 
 Meet _Docstring Auditor_, your go-to solution for maintaining precise and up-to-date Python code documentation.
 Tired of misleading or outdated docstrings? Docstring Auditor harnesses the power of large language models to analyze and critique your docstrings,
 ensuring they align with your code's true purpose. Accessible to both experts and novices,
 Docstring Auditor is your ultimate companion for clear, concise, and informative docstrings.
 Say hello to better code documentation!
```


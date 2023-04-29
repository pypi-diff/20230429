# Comparing `tmp/tryceratops-1.2.0.tar.gz` & `tmp/tryceratops-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryceratops-1.2.0.tar", max compression
+gzip compressed data, was "tryceratops-2.0.0.tar", max compression
```

## Comparing `tryceratops-1.2.0.tar` & `tryceratops-2.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1084 2023-04-29 18:22:03.770300 tryceratops-1.2.0/LICENSE
--rw-r--r--   0        0        0     6162 2023-04-29 18:22:36.390037 tryceratops-1.2.0/README.md
--rw-r--r--   0        0        0     2143 2023-04-29 18:22:36.434037 tryceratops-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-04-29 18:22:36.390037 tryceratops-1.2.0/src/tryceratops/__init__.py
--rw-r--r--   0        0        0     2218 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/__main__.py
--rw-r--r--   0        0        0     1044 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/analyzers/__init__.py
--rw-r--r--   0        0        0     1746 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/analyzers/base.py
--rw-r--r--   0        0        0     5616 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/analyzers/call.py
--rw-r--r--   0        0        0     2154 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/analyzers/conditional.py
--rw-r--r--   0        0        0     5309 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/analyzers/exception_block.py
--rw-r--r--   0        0        0      342 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/analyzers/exceptions.py
--rw-r--r--   0        0        0     1192 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/analyzers/try_block.py
--rw-r--r--   0        0        0       50 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/files/__init__.py
--rw-r--r--   0        0        0     3610 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/files/discovery.py
--rw-r--r--   0        0        0     1453 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/files/parser.py
--rw-r--r--   0        0        0     3126 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/filters.py
--rw-r--r--   0        0        0      601 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/fixers/__init__.py
--rw-r--r--   0        0        0     2653 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/fixers/base.py
--rw-r--r--   0        0        0     2747 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/fixers/exception_block.py
--rw-r--r--   0        0        0      353 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/fixers/exceptions.py
--rw-r--r--   0        0        0     2121 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/flake_plugin.py
--rw-r--r--   0        0        0     2715 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/interfaces.py
--rw-r--r--   0        0        0      165 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/processors.py
--rw-r--r--   0        0        0     3030 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/runners.py
--rw-r--r--   0        0        0     1065 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/settings.py
--rw-r--r--   0        0        0      627 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/types.py
--rw-r--r--   0        0        0      108 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/violations/__init__.py
--rw-r--r--   0        0        0     1258 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/violations/codes.py
--rw-r--r--   0        0        0     1773 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/violations/violations.py
--rw-r--r--   0        0        0     7341 1970-01-01 00:00:00.000000 tryceratops-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-29 20:16:42.212309 tryceratops-2.0.0/LICENSE
+-rw-r--r--   0        0        0     6179 2023-04-29 20:17:16.602042 tryceratops-2.0.0/README.md
+-rw-r--r--   0        0        0     2146 2023-04-29 20:17:16.662045 tryceratops-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-04-29 20:17:16.602042 tryceratops-2.0.0/src/tryceratops/__init__.py
+-rw-r--r--   0        0        0     2220 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/__main__.py
+-rw-r--r--   0        0        0     1044 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/analyzers/__init__.py
+-rw-r--r--   0        0        0     1746 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/analyzers/base.py
+-rw-r--r--   0        0        0     5616 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/analyzers/call.py
+-rw-r--r--   0        0        0     2154 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/analyzers/conditional.py
+-rw-r--r--   0        0        0     5309 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/analyzers/exception_block.py
+-rw-r--r--   0        0        0      342 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/analyzers/exceptions.py
+-rw-r--r--   0        0        0     1192 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/analyzers/try_block.py
+-rw-r--r--   0        0        0       50 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/files/__init__.py
+-rw-r--r--   0        0        0     3610 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/files/discovery.py
+-rw-r--r--   0        0        0     1454 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/files/parser.py
+-rw-r--r--   0        0        0     3126 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/filters.py
+-rw-r--r--   0        0        0      601 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/fixers/__init__.py
+-rw-r--r--   0        0        0     2653 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/fixers/base.py
+-rw-r--r--   0        0        0     2747 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/fixers/exception_block.py
+-rw-r--r--   0        0        0      353 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/fixers/exceptions.py
+-rw-r--r--   0        0        0     2121 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/flake_plugin.py
+-rw-r--r--   0        0        0     2715 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/interfaces.py
+-rw-r--r--   0        0        0      165 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/processors.py
+-rw-r--r--   0        0        0     3030 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/runners.py
+-rw-r--r--   0        0        0     1065 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/settings.py
+-rw-r--r--   0        0        0      629 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/types.py
+-rw-r--r--   0        0        0      108 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/violations/__init__.py
+-rw-r--r--   0        0        0     1286 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/violations/codes.py
+-rw-r--r--   0        0        0     1773 2023-04-29 20:16:42.220309 tryceratops-2.0.0/src/tryceratops/violations/violations.py
+-rw-r--r--   0        0        0     7358 1970-01-01 00:00:00.000000 tryceratops-2.0.0/PKG-INFO
```

### Comparing `tryceratops-1.2.0/LICENSE` & `tryceratops-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/README.md` & `tryceratops-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,18 +61,18 @@
 
 You can enable experimental analyzers by running:
 
 ```
 tryceratops --experimental [filename or dir...]
 ```
 
-You can ignore specific violations by using: `--ignore TCXXX` repeatedly:
+You can ignore specific violations by using: `--ignore TRYXXX` repeatedly:
 
 ```
-tryceratops --ignore TC201 --ignore TC202 [filename or dir...]
+tryceratops --ignore TRY201 --ignore TRY202 [filename or dir...]
 ```
 
 You can exclude dirs by using: `--exclude dir/path` repeatedly:
 
 ```
 tryceratops --exclude tests --exclude .venv [filename or dir...]
 ```
@@ -86,27 +86,27 @@
 ![example](https://raw.githubusercontent.com/guilatrova/tryceratops/main/img/tryceratops-example3.gif)
 
 ### [`flake8`](https://github.com/PyCQA/flake8) Plugin
 
 🦖 Tryceratops is also a plugin for `flake8`, so you can:
 
 ```
-❯ flake8 --select TC src/tests/samples/violations/call_raise_vanilla.py
-src/tests/samples/violations/call_raise_vanilla.py:13:9: TC002 Create your own exception
-src/tests/samples/violations/call_raise_vanilla.py:13:9: TC003 Avoid specifying long messages outside the exception class
-src/tests/samples/violations/call_raise_vanilla.py:21:9: TC201 Simply use 'raise' without specifying exception object again
+❯ flake8 --select TRY src/tests/samples/violations/call_raise_vanilla.py
+src/tests/samples/violations/call_raise_vanilla.py:13:9: TRY002 Create your own exception
+src/tests/samples/violations/call_raise_vanilla.py:13:9: TRY003 Avoid specifying long messages outside the exception class
+src/tests/samples/violations/call_raise_vanilla.py:21:9: TRY201 Simply use 'raise' without specifying exception object again
 ```
 
 ## Violations
 
 All violations and its descriptions can be found in [docs](https://github.com/guilatrova/tryceratops/tree/main/docs/violations).
 
 ### Autofix support
 
-So far, autofix only supports violations: [TC200](docs/violations/TC200.md), [TC201](docs/violations/TC201.md), and [TC400](docs/violations/TC400.md).
+So far, autofix only supports violations: [TRY200](docs/violations/TRY200.md), [TRY201](docs/violations/TRY201.md), and [TRY400](docs/violations/TRY400.md).
 
 ### Ignoring violations
 
 If you want to ignore a violation in a specific file, you can either:
 
 - Add a comment with `noqa` to the top of the file you want to ignore
 - Add a comment with `noqa` to the line you want to ignore
@@ -115,40 +115,40 @@
 Example:
 
 ```py
 def verbose_reraise_1():
     try:
         a = 1
     except Exception as ex:
-        raise ex  # noqa: TC202
+        raise ex  # noqa: TRY202
 ```
 
 ### Configuration
 
 You can set up a `pyproject.toml` file to set rules.
 This is useful to avoid reusing the same CLI flags over and over again and helps to define the structure of your project.
 
 Example:
 
 ```toml
 [tool.tryceratops]
 exclude = ["samples"]
-ignore = ["TC002", "TC200", "TC300"]
+ignore = ["TRY002", "TRY200", "TRY300"]
 experimental = true
 ```
 
 CLI flags always overwrite the config file.
 
 ## Pre-commit
 
 If you wish to use pre-commit, add this:
 
 ```yaml
   - repo: https://github.com/guilatrova/tryceratops
-    rev: v1.2.0
+    rev: v2.0.0
     hooks:
       - id: tryceratops
 ```
 
 ## Show your style
 
 [![try/except style: tryceratops](https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black)](https://github.com/guilatrova/tryceratops)
```

### Comparing `tryceratops-1.2.0/pyproject.toml` & `tryceratops-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tryceratops"
-version = "1.2.0"
+version = "2.0.0"
 description = "Prevent Exception Handling AntiPatterns"
 authors = ["Guilherme Latrova <hello@guilatrova.dev>"]
 license = "MIT"
 keywords = ["lint", "try", "except"]
 readme = "README.md"
 homepage = "https://github.com/guilatrova/tryceratops"
 repository = "https://github.com/guilatrova/tryceratops"
@@ -23,15 +23,15 @@
     { include = "tryceratops", from = "src" },
 ]
 
 [tool.poetry.scripts]
 tryceratops = 'tryceratops.__main__:main'
 
 [tool.poetry.plugins."flake8.extension"]
-TC = "tryceratops.flake_plugin:TryceratopsAdapterPlugin"
+TRY = "tryceratops.flake_plugin:TryceratopsAdapterPlugin"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/guilatrova/tryceratops/blob/main/CHANGELOG.md"
 
 [tool.semantic_release]
 version_variable = [
     "src/tryceratops/__init__.py:__version__"
@@ -52,17 +52,17 @@
 python = "^3.8"
 click = ">=7"
 toml = ">=0.10.2"
 rich = ">=10.14.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
-flake8 = "^3.9.2"
-black = "^20.8b1"
-isort = "^5.8.0"
+flake8 = "^5.0.4"
+black = "^22.12.0"
+isort = "^5.12.0"
 pre-commit = "^2.13.0"
 astpretty = "^2.1.0"
 pytest-cov = "^2.12.1"
 python-semantic-release = "^7.16.2"
 mypy = "^0.910"
 types-toml = "^0.1.3"
 flake8-annotations = "^2.9.0"
```

### Comparing `tryceratops-1.2.0/src/tryceratops/__main__.py` & `tryceratops-2.0.0/src/tryceratops/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 EXPERIMENTAL_FLAG_OPTION = dict(is_flag=True, help="Whether to enable experimental analyzers.")
 AUTOFIX_FLAG_OPTION = dict(
     is_flag=True, help="Whether to fix violations (that support it) automatically."
 )
 IGNORE_OPTION = dict(
     multiple=True,
-    help="A violation to be ignored. e.g. -i TC200 -i TC201",
+    help="A violation to be ignored. e.g. -i TRY200 -i TRY201",
     type=click.Choice(CODE_CHOICES),
 )
 EXCLUDE_OPTION = dict(multiple=True, help="A dir to be excluded. e.g. -x tests/ -x fixtures/")
 VERBOSE_OPTION = dict(is_flag=True, help="Will print more logging messages.")
 
 
 @click.command()
```

### Comparing `tryceratops-1.2.0/src/tryceratops/analyzers/__init__.py` & `tryceratops-2.0.0/src/tryceratops/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/analyzers/base.py` & `tryceratops-2.0.0/src/tryceratops/analyzers/base.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/analyzers/call.py` & `tryceratops-2.0.0/src/tryceratops/analyzers/call.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/analyzers/conditional.py` & `tryceratops-2.0.0/src/tryceratops/analyzers/conditional.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/analyzers/exception_block.py` & `tryceratops-2.0.0/src/tryceratops/analyzers/exception_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/analyzers/try_block.py` & `tryceratops-2.0.0/src/tryceratops/analyzers/try_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/files/discovery.py` & `tryceratops-2.0.0/src/tryceratops/files/discovery.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/files/parser.py` & `tryceratops-2.0.0/src/tryceratops/files/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 import tokenize
 from typing import Generator, Iterable, TextIO, Tuple
 
 from tryceratops.filters import FileFilter, IgnoreViolation
 
 IGNORE_TRYCERATOPS_TOKEN = "noqa"
-IGNORE_TOKEN_PATT = r"noqa(: ?((TC\d{3},? ?)+))?"
+IGNORE_TOKEN_PATT = r"noqa(: ?((TRY\d{3},? ?)+))?"
 
 
 def _build_ignore_line(match: re.Match, location: Tuple[int, int]) -> IgnoreViolation:
     lineno, _ = location
     if match.group(2) is not None:
         codes = [raw.strip() for raw in match.group(2).split(",")]
         return IgnoreViolation(lineno, codes)
```

### Comparing `tryceratops-1.2.0/src/tryceratops/filters.py` & `tryceratops-2.0.0/src/tryceratops/filters.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/fixers/__init__.py` & `tryceratops-2.0.0/src/tryceratops/fixers/__init__.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/fixers/base.py` & `tryceratops-2.0.0/src/tryceratops/fixers/base.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/fixers/exception_block.py` & `tryceratops-2.0.0/src/tryceratops/fixers/exception_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/flake_plugin.py` & `tryceratops-2.0.0/src/tryceratops/flake_plugin.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/interfaces.py` & `tryceratops-2.0.0/src/tryceratops/interfaces.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/runners.py` & `tryceratops-2.0.0/src/tryceratops/runners.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/settings.py` & `tryceratops-2.0.0/src/tryceratops/settings.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/src/tryceratops/types.py` & `tryceratops-2.0.0/src/tryceratops/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ParsedFilesType = Collection[ParsedFileType]
 
 
 class PyprojectConfig(TypedDict):
     """
     Represents the expected pyproject config to be loaded
         exclude: a list of path patterns to be excluded e.g. [/tests, /fixtures]
-        ignore: a list of violations to be completely ignored e.g. [TC002, TC300]
+        ignore: a list of violations to be completely ignored e.g. [TRY002, TRY300]
         experimental: whether to enable experimental analyzers
     """
 
     exclude: List[str]
     ignore: List[str]
     experimental: bool
     autofix: bool
```

### Comparing `tryceratops-1.2.0/src/tryceratops/violations/violations.py` & `tryceratops-2.0.0/src/tryceratops/violations/violations.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.2.0/PKG-INFO` & `tryceratops-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tryceratops
-Version: 1.2.0
+Version: 2.0.0
 Summary: Prevent Exception Handling AntiPatterns
 Home-page: https://github.com/guilatrova/tryceratops
 License: MIT
 Keywords: lint,try,except
 Author: Guilherme Latrova
 Author-email: hello@guilatrova.dev
 Requires-Python: >=3.8,<4.0
@@ -90,18 +90,18 @@
 
 You can enable experimental analyzers by running:
 
 ```
 tryceratops --experimental [filename or dir...]
 ```
 
-You can ignore specific violations by using: `--ignore TCXXX` repeatedly:
+You can ignore specific violations by using: `--ignore TRYXXX` repeatedly:
 
 ```
-tryceratops --ignore TC201 --ignore TC202 [filename or dir...]
+tryceratops --ignore TRY201 --ignore TRY202 [filename or dir...]
 ```
 
 You can exclude dirs by using: `--exclude dir/path` repeatedly:
 
 ```
 tryceratops --exclude tests --exclude .venv [filename or dir...]
 ```
@@ -115,27 +115,27 @@
 ![example](https://raw.githubusercontent.com/guilatrova/tryceratops/main/img/tryceratops-example3.gif)
 
 ### [`flake8`](https://github.com/PyCQA/flake8) Plugin
 
 🦖 Tryceratops is also a plugin for `flake8`, so you can:
 
 ```
-❯ flake8 --select TC src/tests/samples/violations/call_raise_vanilla.py
-src/tests/samples/violations/call_raise_vanilla.py:13:9: TC002 Create your own exception
-src/tests/samples/violations/call_raise_vanilla.py:13:9: TC003 Avoid specifying long messages outside the exception class
-src/tests/samples/violations/call_raise_vanilla.py:21:9: TC201 Simply use 'raise' without specifying exception object again
+❯ flake8 --select TRY src/tests/samples/violations/call_raise_vanilla.py
+src/tests/samples/violations/call_raise_vanilla.py:13:9: TRY002 Create your own exception
+src/tests/samples/violations/call_raise_vanilla.py:13:9: TRY003 Avoid specifying long messages outside the exception class
+src/tests/samples/violations/call_raise_vanilla.py:21:9: TRY201 Simply use 'raise' without specifying exception object again
 ```
 
 ## Violations
 
 All violations and its descriptions can be found in [docs](https://github.com/guilatrova/tryceratops/tree/main/docs/violations).
 
 ### Autofix support
 
-So far, autofix only supports violations: [TC200](docs/violations/TC200.md), [TC201](docs/violations/TC201.md), and [TC400](docs/violations/TC400.md).
+So far, autofix only supports violations: [TRY200](docs/violations/TRY200.md), [TRY201](docs/violations/TRY201.md), and [TRY400](docs/violations/TRY400.md).
 
 ### Ignoring violations
 
 If you want to ignore a violation in a specific file, you can either:
 
 - Add a comment with `noqa` to the top of the file you want to ignore
 - Add a comment with `noqa` to the line you want to ignore
@@ -144,40 +144,40 @@
 Example:
 
 ```py
 def verbose_reraise_1():
     try:
         a = 1
     except Exception as ex:
-        raise ex  # noqa: TC202
+        raise ex  # noqa: TRY202
 ```
 
 ### Configuration
 
 You can set up a `pyproject.toml` file to set rules.
 This is useful to avoid reusing the same CLI flags over and over again and helps to define the structure of your project.
 
 Example:
 
 ```toml
 [tool.tryceratops]
 exclude = ["samples"]
-ignore = ["TC002", "TC200", "TC300"]
+ignore = ["TRY002", "TRY200", "TRY300"]
 experimental = true
 ```
 
 CLI flags always overwrite the config file.
 
 ## Pre-commit
 
 If you wish to use pre-commit, add this:
 
 ```yaml
   - repo: https://github.com/guilatrova/tryceratops
-    rev: v1.2.0
+    rev: v2.0.0
     hooks:
       - id: tryceratops
 ```
 
 ## Show your style
 
 [![try/except style: tryceratops](https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black)](https://github.com/guilatrova/tryceratops)
```


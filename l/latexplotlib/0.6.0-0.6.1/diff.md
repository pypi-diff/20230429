# Comparing `tmp/latexplotlib-0.6.0.tar.gz` & `tmp/latexplotlib-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latexplotlib-0.6.0.tar", last modified: Thu Apr  6 16:00:05 2023, max compression
+gzip compressed data, was "latexplotlib-0.6.1.tar", last modified: Sat Apr 29 20:42:05 2023, max compression
```

## Comparing `latexplotlib-0.6.0.tar` & `latexplotlib-0.6.1.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:00:05.524983 latexplotlib-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-04-06 16:00:05.520983 latexplotlib-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 16:00:05.524983 latexplotlib-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:00:05.516982 latexplotlib-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:00:05.520983 latexplotlib-0.6.0/src/latexplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/src/latexplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/src/latexplotlib/_latexplotlib.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/src/latexplotlib/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:00:05.520983 latexplotlib-0.6.0/src/latexplotlib/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/src/latexplotlib/styles/latex10pt-minimal.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/src/latexplotlib/styles/latex10pt.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/src/latexplotlib/styles/latex11pt-minimal.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/src/latexplotlib/styles/latex11pt.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/src/latexplotlib/styles/latex12pt-minimal.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/src/latexplotlib/styles/latex12pt.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/src/latexplotlib/styles/latex9pt-minimal.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/src/latexplotlib/styles/latex9pt.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:00:05.520983 latexplotlib-0.6.0/src/latexplotlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-04-06 16:00:05.000000 latexplotlib-0.6.0/src/latexplotlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-06 16:00:05.000000 latexplotlib-0.6.0/src/latexplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 16:00:05.000000 latexplotlib-0.6.0/src/latexplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-06 16:00:05.000000 latexplotlib-0.6.0/src/latexplotlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-06 16:00:05.000000 latexplotlib-0.6.0/src/latexplotlib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:00:05.520983 latexplotlib-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/tests/test_latexplotlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/tests/test_styles.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-06 15:59:48.000000 latexplotlib-0.6.0/tests/test_styles_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:42:05.064110 latexplotlib-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-29 20:42:05.064110 latexplotlib-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 20:42:05.064110 latexplotlib-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:42:05.060110 latexplotlib-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:42:05.060110 latexplotlib-0.6.1/src/latexplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/_latexplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/_styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:42:05.064110 latexplotlib-0.6.1/src/latexplotlib/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex10pt-minimal.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex10pt.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex11pt-minimal.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex11pt.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex12pt-minimal.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex12pt.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex9pt-minimal.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex9pt.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:42:05.060110 latexplotlib-0.6.1/src/latexplotlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-29 20:42:05.000000 latexplotlib-0.6.1/src/latexplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-29 20:42:05.000000 latexplotlib-0.6.1/src/latexplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 20:42:05.000000 latexplotlib-0.6.1/src/latexplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-29 20:42:05.000000 latexplotlib-0.6.1/src/latexplotlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 20:42:05.000000 latexplotlib-0.6.1/src/latexplotlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:42:05.064110 latexplotlib-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/tests/test_00_styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/tests/test_10_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/tests/test_20_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/tests/test_30_latexplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/tests/test_styles_available.py
```

### Comparing `latexplotlib-0.6.0/LICENSE` & `latexplotlib-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.0/PKG-INFO` & `latexplotlib-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latexplotlib
-Version: 0.6.0
+Version: 0.6.1
 Summary: Perfect matplotlib figures for latex
 Author-email: Constantin Gahr <latexplotlib.gvxel@aleeas.com>
 License: MIT
 Project-URL: Homepage, https://github.com/cgahr/latexplotlib
 Project-URL: Issues, https://github.com/cgahr/latexplotlib/issues
 Keywords: latex,matplotlib-figures,matplotlib-style-sheets,matplotlib-styles,python
 Classifier: Programming Language :: Python :: 3.7
@@ -13,23 +13,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 Provides-Extra: tests
-Provides-Extra: linters
 License-File: LICENSE
 
 # latexplotlib
 
 [![image](https://img.shields.io/pypi/v/latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib)
 [![image](https://img.shields.io/pypi/l/latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib)
 [![image](https://img.shields.io/pypi/pyversions/latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib)
 [![Actions status](https://github.com/cgahr/latexplotlib/actions/workflows/main.yml/badge.svg)](https://github.com/cgahr/latexplotlib/actions)
+[![Coverage Status](https://coveralls.io/repos/github/cgahr/latexplotlib/badge.svg?branch=main)](https://coveralls.io/github/cgahr/latexplotlib?branch=main)
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 Perfect matplotlib figures for latex.
 
 
 ## Quickstart
```

#### html2text {}

```diff
@@ -1,26 +1,28 @@
-Metadata-Version: 2.1 Name: latexplotlib Version: 0.6.0 Summary: Perfect
+Metadata-Version: 2.1 Name: latexplotlib Version: 0.6.1 Summary: Perfect
 matplotlib figures for latex Author-email: Constantin Gahr
 gvxel@aleeas.com> License: MIT Project-URL: Homepage, https://github.com/cgahr/
 latexplotlib Project-URL: Issues, https://github.com/cgahr/latexplotlib/issues
 Keywords: latex,matplotlib-figures,matplotlib-style-sheets,matplotlib-
 styles,python Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
->=3.7.1 Description-Content-Type: text/markdown Provides-Extra: tests Provides-
-Extra: linters License-File: LICENSE # latexplotlib [![image](https://
-img.shields.io/pypi/v/latexplotlib.svg)](https://pypi.python.org/pypi/
-latexplotlib) [![image](https://img.shields.io/pypi/l/latexplotlib.svg)](https:
-//pypi.python.org/pypi/latexplotlib) [![image](https://img.shields.io/pypi/
-pyversions/latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib) [!
-[Actions status](https://github.com/cgahr/latexplotlib/actions/workflows/
-main.yml/badge.svg)](https://github.com/cgahr/latexplotlib/actions) [Code
-style:_black] [![Ruff](https://img.shields.io/endpoint?url=https://
+>=3.7.1 Description-Content-Type: text/markdown Provides-Extra: tests License-
+File: LICENSE # latexplotlib [![image](https://img.shields.io/pypi/v/
+latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib) [![image](https:/
+/img.shields.io/pypi/l/latexplotlib.svg)](https://pypi.python.org/pypi/
+latexplotlib) [![image](https://img.shields.io/pypi/pyversions/
+latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib) [![Actions
+status](https://github.com/cgahr/latexplotlib/actions/workflows/main.yml/
+badge.svg)](https://github.com/cgahr/latexplotlib/actions) [![Coverage Status]
+(https://coveralls.io/repos/github/cgahr/latexplotlib/badge.svg?branch=main)]
+(https://coveralls.io/github/cgahr/latexplotlib?branch=main) [Code_style:
+black] [![Ruff](https://img.shields.io/endpoint?url=https://
 raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https:
 //github.com/charliermarsh/ruff) Perfect matplotlib figures for latex. ##
 Quickstart 1. install `latexplotlib`: ```python pip install latexplotlib ``` 2.
 import latexplotlib and use latexplotlib style ```python import latexplotlib as
 lpl plt.style.use('latex10pt') # lpl.style.use('latex10pt-minimal') ``` 3.
 replace all `plt.subplots` with `lpl.subplots`: ```python # fig, axes =
 plt.subplots(2, 3) fig, axes = lpl.subplots(2, 3) ``` Optional: 4. get size of
```

### Comparing `latexplotlib-0.6.0/README.md` & `latexplotlib-0.6.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # latexplotlib
 
 [![image](https://img.shields.io/pypi/v/latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib)
 [![image](https://img.shields.io/pypi/l/latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib)
 [![image](https://img.shields.io/pypi/pyversions/latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib)
 [![Actions status](https://github.com/cgahr/latexplotlib/actions/workflows/main.yml/badge.svg)](https://github.com/cgahr/latexplotlib/actions)
+[![Coverage Status](https://coveralls.io/repos/github/cgahr/latexplotlib/badge.svg?branch=main)](https://coveralls.io/github/cgahr/latexplotlib?branch=main)
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 Perfect matplotlib figures for latex.
 
 
 ## Quickstart
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
 # latexplotlib [![image](https://img.shields.io/pypi/v/latexplotlib.svg)]
 (https://pypi.python.org/pypi/latexplotlib) [![image](https://img.shields.io/
 pypi/l/latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib) [![image]
 (https://img.shields.io/pypi/pyversions/latexplotlib.svg)](https://
 pypi.python.org/pypi/latexplotlib) [![Actions status](https://github.com/cgahr/
 latexplotlib/actions/workflows/main.yml/badge.svg)](https://github.com/cgahr/
-latexplotlib/actions) [Code_style:_black] [![Ruff](https://img.shields.io/
+latexplotlib/actions) [![Coverage Status](https://coveralls.io/repos/github/
+cgahr/latexplotlib/badge.svg?branch=main)](https://coveralls.io/github/cgahr/
+latexplotlib?branch=main) [Code_style:_black] [![Ruff](https://img.shields.io/
 endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/
 badge/v1.json)](https://github.com/charliermarsh/ruff) Perfect matplotlib
 figures for latex. ## Quickstart 1. install `latexplotlib`: ```python pip
 install latexplotlib ``` 2. import latexplotlib and use latexplotlib style
 ```python import latexplotlib as lpl plt.style.use('latex10pt') # lpl.style.use
 ('latex10pt-minimal') ``` 3. replace all `plt.subplots` with `lpl.subplots`:
 ```python # fig, axes = plt.subplots(2, 3) fig, axes = lpl.subplots(2, 3) ```
```

### Comparing `latexplotlib-0.6.0/pyproject.toml` & `latexplotlib-0.6.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,62 @@
 [build-system]
 build-backend = "setuptools.build_meta"
-requires = ["setuptools", "matplotlib"]
+requires = ["matplotlib", "setuptools"]
 
 [project]
 authors = [
-    {name = "Constantin Gahr", email = "latexplotlib.gvxel@aleeas.com"},
+    {email = "latexplotlib.gvxel@aleeas.com", name = "Constantin Gahr"}
 ]
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+    "Operating System :: OS Independent"
 ]
 dependencies = [
     "appdirs",
-    "matplotlib",
+    "matplotlib"
 ]
 description = "Perfect matplotlib figures for latex"
 dynamic = ["version"]
 keywords = [
     "latex",
     "matplotlib-figures",
     "matplotlib-style-sheets",
     "matplotlib-styles",
-    "python",
+    "python"
 ]
 license = {text = "MIT"}
 name = "latexplotlib"
 readme = "README.md"
 requires-python = ">=3.7.1"
 
 [project.optional-dependencies]
 tests = [
     "coverage",
     "pytest",
-    "pytest-console-scripts",
     "pytest-cov",
-    "pytest-env",
-    "pytest-mock",
-]
-linters =  [
-    "black",
-    "isort",
-    "mypy",
-    "ruff",
-    "types-appdirs",
+    "pytest-mock"
 ]
 
 [project.urls]
 Homepage = "https://github.com/cgahr/latexplotlib"
 Issues = "https://github.com/cgahr/latexplotlib/issues"
 
-[tool.setuptools.dynamic]
-version = {attr = "latexplotlib._version.__version__"}
+[tool.black]
+line_length = 88
 
-[tool.setuptools.package-data]
-opinf =  ["py.typed"]
+[tool.coverage.report]
+exclude_lines = ["if TYPE_CHECKING:"]
 
-[tool.setuptools.packages.find]
-where = ["src"]
-
-[tool.pytest.ini_options]
-addopts = "--cov=src --cov-report=html --cov-report=term"
-testpaths = [
-    "tests",
-]
+[tool.coverage.run]
+source = ["src"]
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 check_untyped_defs = true
 exclude = [
@@ -79,47 +64,58 @@
     ".git",
     ".ipynb_checkpoints",
     "__pycache__",
     "build",
     "dist",
     "examples",
     "setup*",
-    "tests",
+    "tests"
 ]
 mypy_path = "src"
 no_implicit_optional = true
 no_implicit_reexport = true
 show_error_codes = true
 strict_equality = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 
 [[tool.mypy.overrides]]
+ignore_missing_imports = true
 module = [
-    "matplotlib.*",
+    "matplotlib.*"
+]
+
+[tool.pytest.ini_options]
+addopts = "--cov --cov-report=html --cov-report=term"
+testpaths = [
+    "tests"
 ]
-ignore_missing_imports = true
 
 [tool.ruff]
+fix = true
+fixable = ["I"]
+ignore = [
+    "ANN101"  # missing-type-self
+]
 select = [
     "F",
     "E",
     "W",
     "C90",
     "I",
     "N",
     # "D",
     "UP",
     "YTT",
     "ANN",
     "S",
     "BLE",
-    "FBT", # unclear if good or not
+    "FBT",  # unclear if good or not
     "B",
     "A",
     "C4",
     "DTZ",
     "T10",
     "EM",
     "EXE",
@@ -140,34 +136,50 @@
     "ARG",
     "PTH",
     "ERA",
     "PGH",
     "PL",
     "TRY",
     "NPY",
-    "RUF",
+    "RUF"
 ]
 target-version = "py38"
-ignore = [
-    "ANN002",
-    "ANN003",
-    "ANN101",
-    "ANN102",
-    "ANN401",
-    "I001",
-]
-unfixable = ["I001"]
+
+[tool.ruff.flake8-annotations]
+suppress-dummy-args = true
 
 [tool.ruff.per-file-ignores]
-"__init__.py" = ["F401", 'F403']
 "examples/*" = [
-    "INP",
-    "ERA001",
+    "ERA001",  # commented-out-code
+    "INP"  # implicit-namespace-package
 ]
 "tests/*" = [
     "ANN",
-    "ARG002",
-    "INP",
+    "ARG002",  # unused-method-argument
+    "INP",  # implicit-namespace-package
     "PLR0913",  # too-many-arguments
-    "S101",
-    "SLF001",
+    "S101",  # assert
+    "SLF001"  # private-member-access
 ]
+
+[tool.ruff.pylint]
+max-args = 5
+
+[tool.setuptools.dynamic]
+version = {attr = "latexplotlib._version.__version__"}
+
+[tool.setuptools.package-data]
+latexplotlib = ["py.typed"]
+"latexplotlib.styles" = ["*.mplstyle"]
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.tomlsort]
+all = true
+in_place = true
+spaces_before_inline_comment = 2
+spaces_indent_inline_array = 4
+
+[tool.tomlsort.overrides]
+"project.classifiers".inline_arrays = false
+"tool.ruff.select".inline_arrays = false
```

### Comparing `latexplotlib-0.6.0/src/latexplotlib/styles/latex10pt.mplstyle` & `latexplotlib-0.6.1/src/latexplotlib/styles/latex10pt.mplstyle`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.0/src/latexplotlib/styles/latex11pt.mplstyle` & `latexplotlib-0.6.1/src/latexplotlib/styles/latex11pt.mplstyle`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.0/src/latexplotlib/styles/latex12pt.mplstyle` & `latexplotlib-0.6.1/src/latexplotlib/styles/latex12pt.mplstyle`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.0/src/latexplotlib/styles/latex9pt.mplstyle` & `latexplotlib-0.6.1/src/latexplotlib/styles/latex9pt.mplstyle`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.0/src/latexplotlib.egg-info/PKG-INFO` & `latexplotlib-0.6.1/src/latexplotlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latexplotlib
-Version: 0.6.0
+Version: 0.6.1
 Summary: Perfect matplotlib figures for latex
 Author-email: Constantin Gahr <latexplotlib.gvxel@aleeas.com>
 License: MIT
 Project-URL: Homepage, https://github.com/cgahr/latexplotlib
 Project-URL: Issues, https://github.com/cgahr/latexplotlib/issues
 Keywords: latex,matplotlib-figures,matplotlib-style-sheets,matplotlib-styles,python
 Classifier: Programming Language :: Python :: 3.7
@@ -13,23 +13,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 Provides-Extra: tests
-Provides-Extra: linters
 License-File: LICENSE
 
 # latexplotlib
 
 [![image](https://img.shields.io/pypi/v/latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib)
 [![image](https://img.shields.io/pypi/l/latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib)
 [![image](https://img.shields.io/pypi/pyversions/latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib)
 [![Actions status](https://github.com/cgahr/latexplotlib/actions/workflows/main.yml/badge.svg)](https://github.com/cgahr/latexplotlib/actions)
+[![Coverage Status](https://coveralls.io/repos/github/cgahr/latexplotlib/badge.svg?branch=main)](https://coveralls.io/github/cgahr/latexplotlib?branch=main)
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 Perfect matplotlib figures for latex.
 
 
 ## Quickstart
```

#### html2text {}

```diff
@@ -1,26 +1,28 @@
-Metadata-Version: 2.1 Name: latexplotlib Version: 0.6.0 Summary: Perfect
+Metadata-Version: 2.1 Name: latexplotlib Version: 0.6.1 Summary: Perfect
 matplotlib figures for latex Author-email: Constantin Gahr
 gvxel@aleeas.com> License: MIT Project-URL: Homepage, https://github.com/cgahr/
 latexplotlib Project-URL: Issues, https://github.com/cgahr/latexplotlib/issues
 Keywords: latex,matplotlib-figures,matplotlib-style-sheets,matplotlib-
 styles,python Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
->=3.7.1 Description-Content-Type: text/markdown Provides-Extra: tests Provides-
-Extra: linters License-File: LICENSE # latexplotlib [![image](https://
-img.shields.io/pypi/v/latexplotlib.svg)](https://pypi.python.org/pypi/
-latexplotlib) [![image](https://img.shields.io/pypi/l/latexplotlib.svg)](https:
-//pypi.python.org/pypi/latexplotlib) [![image](https://img.shields.io/pypi/
-pyversions/latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib) [!
-[Actions status](https://github.com/cgahr/latexplotlib/actions/workflows/
-main.yml/badge.svg)](https://github.com/cgahr/latexplotlib/actions) [Code
-style:_black] [![Ruff](https://img.shields.io/endpoint?url=https://
+>=3.7.1 Description-Content-Type: text/markdown Provides-Extra: tests License-
+File: LICENSE # latexplotlib [![image](https://img.shields.io/pypi/v/
+latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib) [![image](https:/
+/img.shields.io/pypi/l/latexplotlib.svg)](https://pypi.python.org/pypi/
+latexplotlib) [![image](https://img.shields.io/pypi/pyversions/
+latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib) [![Actions
+status](https://github.com/cgahr/latexplotlib/actions/workflows/main.yml/
+badge.svg)](https://github.com/cgahr/latexplotlib/actions) [![Coverage Status]
+(https://coveralls.io/repos/github/cgahr/latexplotlib/badge.svg?branch=main)]
+(https://coveralls.io/github/cgahr/latexplotlib?branch=main) [Code_style:
+black] [![Ruff](https://img.shields.io/endpoint?url=https://
 raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https:
 //github.com/charliermarsh/ruff) Perfect matplotlib figures for latex. ##
 Quickstart 1. install `latexplotlib`: ```python pip install latexplotlib ``` 2.
 import latexplotlib and use latexplotlib style ```python import latexplotlib as
 lpl plt.style.use('latex10pt') # lpl.style.use('latex10pt-minimal') ``` 3.
 replace all `plt.subplots` with `lpl.subplots`: ```python # fig, axes =
 plt.subplots(2, 3) fig, axes = lpl.subplots(2, 3) ``` Optional: 4. get size of
```

### Comparing `latexplotlib-0.6.0/src/latexplotlib.egg-info/SOURCES.txt` & `latexplotlib-0.6.1/src/latexplotlib.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 LICENSE
-MANIFEST.in
 README.md
 pyproject.toml
 src/latexplotlib/__init__.py
+src/latexplotlib/_cleanup.py
+src/latexplotlib/_config.py
 src/latexplotlib/_latexplotlib.py
+src/latexplotlib/_styles.py
 src/latexplotlib/_version.py
+src/latexplotlib/py.typed
 src/latexplotlib.egg-info/PKG-INFO
 src/latexplotlib.egg-info/SOURCES.txt
 src/latexplotlib.egg-info/dependency_links.txt
 src/latexplotlib.egg-info/requires.txt
 src/latexplotlib.egg-info/top_level.txt
 src/latexplotlib/styles/latex10pt-minimal.mplstyle
 src/latexplotlib/styles/latex10pt.mplstyle
 src/latexplotlib/styles/latex11pt-minimal.mplstyle
 src/latexplotlib/styles/latex11pt.mplstyle
 src/latexplotlib/styles/latex12pt-minimal.mplstyle
 src/latexplotlib/styles/latex12pt.mplstyle
 src/latexplotlib/styles/latex9pt-minimal.mplstyle
 src/latexplotlib/styles/latex9pt.mplstyle
-tests/test_latexplotlib.py
-tests/test_styles.py
+tests/test_00_styles.py
+tests/test_10_config.py
+tests/test_20_cleanup.py
+tests/test_30_latexplotlib.py
 tests/test_styles_available.py
```

### Comparing `latexplotlib-0.6.0/tests/test_styles.py` & `latexplotlib-0.6.1/tests/test_00_styles.py`

 * *Files identical despite different names*


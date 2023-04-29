# Comparing `tmp/pyshotgrid-0.8.0.tar.gz` & `tmp/pyshotgrid-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pyshotgrid/pyshotgrid/dist/.tmp-fdo6wi6h/pyshotgrid-0.8.0.tar", last modified: Mon Nov 28 13:20:35 2022, max compression
+gzip compressed data, was "/home/runner/work/pyshotgrid/pyshotgrid/dist/.tmp-opqngv8_/pyshotgrid-0.9.1.tar", last modified: Sun Jan  1 22:39:19 2023, max compression
```

## Comparing `pyshotgrid-0.8.0.tar` & `pyshotgrid-0.9.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 13:20:35.000000 pyshotgrid-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      170 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6613 2022-11-28 13:20:35.000000 pyshotgrid-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5485 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 13:20:35.000000 pyshotgrid-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      324 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/docs/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5608 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3777 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1231 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/docs/how_it_works.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4365 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/docs/how_to_add_custom_entities.rst
--rw-r--r--   0 runner    (1001) docker     (122)      421 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1112 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 13:20:35.000000 pyshotgrid-0.8.0/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (122)      150 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/docs/modules/core.rst
--rw-r--r--   0 runner    (1001) docker     (122)      154 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/docs/modules/field.rst
--rw-r--r--   0 runner    (1001) docker     (122)      210 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/docs/modules/sg_default_entities.rst
--rw-r--r--   0 runner    (1001) docker     (122)      170 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/docs/modules/sg_entity.rst
--rw-r--r--   0 runner    (1001) docker     (122)      162 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/docs/modules/sg_site.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1485 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/docs/pyshotgrid_vs_shotgun_api3.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2083 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/docs/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2272 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 13:20:35.000000 pyshotgrid-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       84 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 13:20:35.000000 pyshotgrid-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 13:20:35.000000 pyshotgrid-0.8.0/src/pyshotgrid/
--rw-r--r--   0 runner    (1001) docker     (122)      972 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/src/pyshotgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9375 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/src/pyshotgrid/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     9428 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/src/pyshotgrid/field.py
--rw-r--r--   0 runner    (1001) docker     (122)    20358 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/src/pyshotgrid/sg_default_entities.py
--rw-r--r--   0 runner    (1001) docker     (122)    10738 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/src/pyshotgrid/sg_entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     7488 2022-11-28 13:20:15.000000 pyshotgrid-0.8.0/src/pyshotgrid/sg_site.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 13:20:35.000000 pyshotgrid-0.8.0/src/pyshotgrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6613 2022-11-28 13:20:35.000000 pyshotgrid-0.8.0/src/pyshotgrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      714 2022-11-28 13:20:35.000000 pyshotgrid-0.8.0/src/pyshotgrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 13:20:35.000000 pyshotgrid-0.8.0/src/pyshotgrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-11-28 13:20:35.000000 pyshotgrid-0.8.0/src/pyshotgrid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 22:39:19.000000 pyshotgrid-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-01-01 22:39:19.000000 pyshotgrid-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 22:39:19.000000 pyshotgrid-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/docs/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/docs/how_it_works.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/docs/how_to_add_custom_entities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 22:39:19.000000 pyshotgrid-0.9.1/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/docs/modules/core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/docs/modules/field.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/docs/modules/sg_default_entities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/docs/modules/sg_entity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/docs/modules/sg_site.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/docs/pyshotgrid_vs_shotgun_api3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/docs/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-01 22:39:19.000000 pyshotgrid-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 22:39:19.000000 pyshotgrid-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 22:39:19.000000 pyshotgrid-0.9.1/src/pyshotgrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/src/pyshotgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/src/pyshotgrid/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/src/pyshotgrid/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20358 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/src/pyshotgrid/sg_default_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/src/pyshotgrid/sg_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-01-01 22:39:07.000000 pyshotgrid-0.9.1/src/pyshotgrid/sg_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 22:39:19.000000 pyshotgrid-0.9.1/src/pyshotgrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-01-01 22:39:19.000000 pyshotgrid-0.9.1/src/pyshotgrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-01-01 22:39:19.000000 pyshotgrid-0.9.1/src/pyshotgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-01 22:39:19.000000 pyshotgrid-0.9.1/src/pyshotgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-01 22:39:19.000000 pyshotgrid-0.9.1/src/pyshotgrid.egg-info/top_level.txt
```

### Comparing `pyshotgrid-0.8.0/LICENSE` & `pyshotgrid-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyshotgrid-0.8.0/PKG-INFO` & `pyshotgrid-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshotgrid
-Version: 0.8.0
+Version: 0.9.1
 Summary: A pythonic and object oriented way to talk to Autodesk ShotGrid.
 Author-email: Fabian Geisler <info@fasbue.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fabiangeisler/pyshotgrid
 Project-URL: Documentation, https://fabiangeisler.github.io/pyshotgrid
 Project-URL: Bug Tracker, https://github.com/fabiangeisler/pyshotgrid/issues
 Keywords: shotgrid
@@ -21,19 +21,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<p align="center">
+  <img src="https://github.com/fabiangeisler/pyshotgrid/blob/main/icons/pysg_logo.png?raw=true" />
+</p>
+
 [![pypi](https://img.shields.io/pypi/v/pyshotgrid.svg)](https://pypi.python.org/pypi/pyshotgrid)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyshotgrid.svg)](https://pypi.python.org/pypi/pyshotgrid/)
 [![Tests](https://github.com/fabiangeisler/pyshotgrid/actions/workflows/Tests.yml/badge.svg)](https://github.com/fabiangeisler/pyshotgrid/actions/workflows/Tests.yml)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![linter: ruff](https://img.shields.io/static/v1?label=linter&message=ruff&color=green)](https://github.com/charliermarsh/ruff)
+[![type checker: mypy](https://img.shields.io/badge/%20type_checker-my[py]-%231674b1?style=flat)](https://github.com/python/mypy)
 
 `pyshotgrid` is a python package that gives you a pythonic and
 object oriented way to talk to [Autodesk ShotGrid](https://www.autodesk.com/products/shotgrid/overview).
 
 > **Warning**
 > This python library is still in early development and the API is not yet stable.
 > Please be cautious in a production environment.
```

### Comparing `pyshotgrid-0.8.0/README.md` & `pyshotgrid-0.9.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+<p align="center">
+  <img src="https://github.com/fabiangeisler/pyshotgrid/blob/main/icons/pysg_logo.png?raw=true" />
+</p>
+
 [![pypi](https://img.shields.io/pypi/v/pyshotgrid.svg)](https://pypi.python.org/pypi/pyshotgrid)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyshotgrid.svg)](https://pypi.python.org/pypi/pyshotgrid/)
 [![Tests](https://github.com/fabiangeisler/pyshotgrid/actions/workflows/Tests.yml/badge.svg)](https://github.com/fabiangeisler/pyshotgrid/actions/workflows/Tests.yml)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![linter: ruff](https://img.shields.io/static/v1?label=linter&message=ruff&color=green)](https://github.com/charliermarsh/ruff)
+[![type checker: mypy](https://img.shields.io/badge/%20type_checker-my[py]-%231674b1?style=flat)](https://github.com/python/mypy)
 
 `pyshotgrid` is a python package that gives you a pythonic and
 object oriented way to talk to [Autodesk ShotGrid](https://www.autodesk.com/products/shotgrid/overview).
 
 > **Warning**
 > This python library is still in early development and the API is not yet stable.
 > Please be cautious in a production environment.
```

### Comparing `pyshotgrid-0.8.0/docs/conf.py` & `pyshotgrid-0.9.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "sphinx_rtd_theme"
+html_logo = "../icons/pysg_logo.png"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
```

### Comparing `pyshotgrid-0.8.0/docs/contributing.rst` & `pyshotgrid-0.9.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `pyshotgrid-0.8.0/docs/how_it_works.rst` & `pyshotgrid-0.9.1/docs/how_it_works.rst`

 * *Files identical despite different names*

### Comparing `pyshotgrid-0.8.0/docs/how_to_add_custom_entities.rst` & `pyshotgrid-0.9.1/docs/how_to_add_custom_entities.rst`

 * *Files identical despite different names*

### Comparing `pyshotgrid-0.8.0/docs/installation.rst` & `pyshotgrid-0.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyshotgrid-0.8.0/docs/pyshotgrid_vs_shotgun_api3.rst` & `pyshotgrid-0.9.1/docs/pyshotgrid_vs_shotgun_api3.rst`

 * *Files identical despite different names*

### Comparing `pyshotgrid-0.8.0/docs/user_guide.rst` & `pyshotgrid-0.9.1/docs/user_guide.rst`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 After you made `pyshotgrid` accessible in ShotGrid Toolkit the best way to use it is to convert
 any entity to a `pyshotgrid` object instance. What you need for this is:
 
 - a shotgun_api3.Shotgun instance (which conveniently is present almost everywhere in SGTK)
 - the type of the entity
 - the id of the entity
+
 These parameters will be passed to the `pyshotgrid.new_entity` method, which returns the
 object you want to work with.
 The method accepts 3 ways of passing arguments to it:
 
 .. code-block:: python
 
     import pyshotgrid as pysg
```

### Comparing `pyshotgrid-0.8.0/pyproject.toml` & `pyshotgrid-0.9.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -41,50 +41,63 @@
 [tool.setuptools.dynamic]
 version = {attr = "pyshotgrid.VERSION"}
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 skip_missing_interpreters = true
-envlist = py27, py37, py38, py39, py310, py310-flake8
+envlist = py27, py37, py38, py39, py310
 
 [gh-actions]
 python =
     2.7: py27
     3.7: py37
     3.8: py38
     3.9: py39
-    3.10: py310, py310-flake8
-
-[testenv:py310-flake8]
-exclude = docs
-deps = flake8
-commands = flake8 src tests --max-line-length=100
+    3.10: py310
 
 [testenv:docs]
 description=Documentation generation
 basepython=python3
 changedir=docs
 deps=
     -rrequirements_docs.txt
 commands=
     sphinx-build -b html -d {envtmpdir}/doctrees . _builds
 
 [testenv]
 deps =
     -rrequirements.txt
-commands = nose2 -v --with-coverage --coverage ./src --coverage-report html --coverage-report term
+commands = nose2 -v --with-coverage --coverage ./src --coverage-report term
 """
 
-[tool.mypy]
+[[tool.mypy.overrides]]
+module = [
+    "shotgun_api3.*",
+]
 ignore_missing_imports = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.8.0"
+version = "0.9.1"
 tag_format = "v$version"
 update_changelog_on_bump = true
 annotated_tag = true
 major_version_zero = true
 version_files = [
     "src/pyshotgrid/__init__.py:VERSION",
 ]
+
+[tool.ruff]
+line-length = 100
+select = [
+    "E",  # pycodestyle
+    "W",
+    "F",  # PyFlakes
+    "B",  # flake8-bugbear
+    "T20",  # "print" in code
+    "N",  # pep8 naming convention
+    "I",  # isort
+    "RUF",  # Bad unicode characters in code
+]
+
+src = ["src", "tests"]
```

### Comparing `pyshotgrid-0.8.0/src/pyshotgrid/__init__.py` & `pyshotgrid-0.9.1/src/pyshotgrid/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 Use it like::
 
     >>> import pyshotgrid
 
 """
 
 from . import sg_default_entities as sde
-from .core import new_entity  # noqa: F401
-from .core import new_site  # noqa: F401
 from .core import (
+    new_entity,  # noqa: F401
+    new_site,  # noqa: F401
     register_fallback_pysg_class,
     register_pysg_class,
     register_sg_site_class,
 )
 from .sg_entity import Field, SGEntity  # noqa: F401
-from .sg_site import SGSite  # noqa: F401
+from .sg_site import SGSite
 
 #: The pyshotgrid version number as string
-VERSION = "0.8.0"
+VERSION = "0.9.1"
 
 register_sg_site_class(SGSite)
 register_fallback_pysg_class(SGEntity)
 # Register default pysg plugins
 register_pysg_class("Project", sde.SGProject)
 register_pysg_class("Shot", sde.SGShot)
 register_pysg_class("Asset", sde.SGAsset)
```

### Comparing `pyshotgrid-0.8.0/src/pyshotgrid/core.py` & `pyshotgrid-0.9.1/src/pyshotgrid/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,23 @@
+import typing
 from typing import Any, Dict, List, Type  # noqa: F401
 
 import shotgun_api3
 import shotgun_api3.lib.mockgun
 
+if typing.TYPE_CHECKING:
+    from pyshotgrid.sg_entity import SGEntity  # noqa: F401
+    from pyshotgrid.sg_site import SGSite  # noqa: F401
+
 #: Entity plugins that are registered to pyshotgrid.
 __ENTITY_PLUGINS = []  # type: List[Dict[str,Any]]
 #: Fallback entity class that is used when no match in the __ENTITY_PLUGINS is found.
-__ENTITY_FALLBACK_CLASS = None  # type: Type|None
+__ENTITY_FALLBACK_CLASS = None  # type: Type[SGEntity]|None
 #: The class that represents the ShotGrid site.
-__SG_SITE_CLASS = None  # type: Type|None
+__SG_SITE_CLASS = None  # type: Type[SGSite]|None
 
 
 def new_entity(sg, *args, **kwargs):
     """
     Create a new instance of a pyshotgrid class that represents a ShotGrid entity.
     This function is meant to be used as the main way to create new pyshotgrid instances
     and will always return the correct entity instance that you should work with.
@@ -212,15 +217,16 @@
 
 def convert_filters_to_dict(filters):
     """
     Convert any pysg objects form the given shotgun_api3 filter to simple dictionaries.
 
     Example::
 
-        >>> convert_filters_to_dict([['user', 'is', SGHumanUser(sg, id=5)]])
+        >>> person = SGEntity(shotgun_api3.Shotgun('...'), entity_type='HumanUser', entity_id=5)
+        >>> convert_filters_to_dict([['user', 'is', person]])
         [['user', 'is', {'type': 'HumanUser', 'id': 5}]]
 
     :param list[list] filters: The filters to convert
     :return: The filter with all pysg objects converted to dictionaries.
     :rtype: list[list]
     """
     for f in filters:
```

### Comparing `pyshotgrid-0.8.0/src/pyshotgrid/field.py` & `pyshotgrid-0.9.1/src/pyshotgrid/sg_entity.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,271 +1,324 @@
-import os
+from .core import convert_fields_to_dicts, convert_fields_to_pysg, new_entity, new_site
+from .field import Field, FieldSchema
 
-from .core import convert_value_to_dict, convert_value_to_pysg, new_entity
 
-
-class Field(object):
+class SGEntity(object):
     """
-    This class represents a field on a ShotGrid entity.
-    It provides an interface to manage various aspects of a field.
+    An instance of this class represents a single entity in ShotGrid.
+
+    .. Note::
+
+        Try to avoid creating instances of this class in production code and
+        use the :py:meth:`pyshotgrid.new_entity <pyshotgrid.core.new_entity>`
+        method instead. This will make sure that you always get the correct
+        entity class to work with.
     """
 
-    # Note to developers:
-    # The naming convention of this class intentionally leaves out the "SG" in front,
-    # since there is a ShotGrid entity that is called "Field".
+    def __init__(self, sg, entity_type, entity_id):
+        """
+        :param shotgun_api3.shotgun.Shotgun sg:
+            A fully initialized instance of shotgun_api3.Shotgun.
+        :param str entity_type: The ShotGrid type of the entity.
+        :param int entity_id: The ID of the ShotGrid entity.
+        """
+        self._sg = sg  # :type: shotgun_api3.shotgun.Shotgun
+        self._type = entity_type
+        self._id = entity_id
+
+    def __str__(self):
+        return "{} - Type: {} - ID: {} - URL: {}".format(
+            self.__class__.__name__, self._type, self._id, self.url
+        )
 
-    def __init__(self, name, entity):
+    @property
+    def id(self):
         """
-        :param str name: The name of the field.
-        :param SGEntity entity: The entity that this field is attached to.
+        :return: The ID of the ShotGrid entity.
+        :rtype: int
         """
-        self._name = name
-        self._entity = entity
+        return self._id
 
     @property
-    def name(self):
+    def type(self):
         """
-        :return: The name of the field.
+        :return: The type of the ShotGrid entity.
         :rtype: str
         """
-        return self._name
+        return self._type
 
     @property
-    def entity(self):
+    def sg(self):
         """
-        :return: The entity that this field is attached to.
-        :rtype: SGEntity
+        :return: The Shotgun instance that the entity belongs to.
+        :rtype: shotgun_api3.shotgun.Shotgun
         """
-        return self._entity
+        return self._sg
 
-    def get(self, raw_values=False):
+    @property
+    def site(self):
         """
-        :param bool raw_values: Whether to return the raw dict values or the values converted to
-                                pyshotgrid objects.
-        :return: The value of the field. Any entities will be automatically converted to
-                 pyshotgrid objects.
-        :rtype: Any
+        :return: The pyshotgrid site for this entity.
+        :rtype: SGSite
         """
-        value = self._entity.sg.find_one(
-            entity_type=self._entity.type,
-            filters=[["id", "is", self._entity.id]],
-            fields=[self._name],
-        ).get(self._name)
-        return value if raw_values else convert_value_to_pysg(self._entity.sg, value)
+        return new_site(self._sg)
 
-    def set(self, value):
+    @property
+    def url(self):
         """
-        Set the field to the given value in ShotGrid.
+        :return: The ShotGrid URL for this entity.
 
-        :param Any value: The value to set the field to.
+            .. note::
+
+               This will only work on entities that have a detail view enabled
+               in the system settings.
+        :rtype: str
         """
-        self._entity.sg.update(
-            self._entity.type,
-            self._entity.id,
-            data={self._name: convert_value_to_dict(value)},
-        )
+        return "{}/detail/{}/{}".format(self.sg.base_url, self._type, self._id)
 
-    def add(self, values):
+    def __eq__(self, other):
         """
-        Add some values to this field
+        Compare SGEntities against each other.
+        We consider the entities equal if all these are true:
+          - the other instance is a (sub-)class of SGEntity
+          - the ID's match
+          - the entity types match
+          - the base URL of the Shotgun instances is the same.
 
-        :param list[Any] values: The value to add to this field.
+        :param Any other: The other python object to compare to.
+        :return: Whether the 2 instances represent the same entity in ShotGrid.
+        :rtype: bool
         """
-        self._entity.sg.update(
-            self._entity.type,
-            self._entity.id,
-            data={self._name: convert_value_to_dict(values)},
-            multi_entity_update_modes="add",
+        return all(
+            (
+                isinstance(other, SGEntity),
+                self._id == other.id,
+                self._type == other.type,
+                self._sg.base_url == other.sg.base_url,
+            )
         )
 
-    def remove(self, values):
+    def __getitem__(self, field):
         """
-        Remove some values from this field.
+        Enabling dict notation to query fields of the entity from ShotGrid.
 
-        :param list[Any] values: The values to remove from this field.
+        :param str field: The field to query.
+        :return: The value of the field. Any entities will be automatically converted to
+                 pyshotgrid objects.
         """
-        self._entity.sg.update(
-            self._entity.type,
-            self._entity.id,
-            data={self._name: convert_value_to_dict(values)},
-            multi_entity_update_modes="remove",
-        )
+        return Field(name=field, entity=self)
 
-    def upload(self, path, display_name=None):
+    def fields(self, project_entity=None):
         """
-        Upload a file to this field.
+        :param dict[str,Any]|SGEntity|None project_entity: A project entity to filter by.
+        :return: All fields from this entity. If a project entity is given
+                 only fields that are visible to the project are returned.
+        :rtype: list[Field]
+        """
+        if project_entity is not None and not isinstance(project_entity, dict):
+            project_entity = project_entity.to_dict()
 
-        :param str path: The path to the file to upload.
-        :param str display_name: The display name of the file in ShotGrid.
-        :return: The Attachment entity that was created for the uploaded file.
-        :rtype: SGEntity
-        """
-        sg_attachment_id = self._entity.sg.upload(
-            entity_type=self._entity.type,
-            entity_id=self._entity.id,
-            path=path,
-            field_name=self._name,
-            display_name=display_name,
+        sg_entity_fields = self.sg.schema_field_read(
+            self._type, project_entity=project_entity
         )
-        return new_entity(self._entity.sg, "Attachment", sg_attachment_id)
+        fields = [
+            field
+            for field, schema in sg_entity_fields.items()
+            if schema["visible"]["value"]
+        ]
 
-    def download(self, path):
-        """
-        Download a file from a field.
+        return [Field(name=field, entity=self) for field in fields]
 
-        :param str path: The path to download to.
-        :return:
-        :raises:
-            :RuntimeError: When nothing was uploaded to this field.
+    def all_field_values(self, project_entity=None, raw_values=False):
         """
-        sg_attachment = self._entity.sg.find_one(
-            self._entity.type, [["id", "is", self._entity.id]], [self._name]
-        )[self._name]
-
-        if sg_attachment is None:
-            raise RuntimeError(
-                'Cannot download file from field "{}" on entity "{}", because there'
-                "is nothing uploaded.".format(self.name, self.entity.to_dict())
-            )
-
-        # if we can split of a file extension from the given path we assume that the path is the
-        # full path with file name to download to. In the other case we assume that the path is
-        # the directory to download to and attach the attachment name as the file name to the
-        # directory path.
-        _, ext = os.path.splitext(path)
-        if ext:
-            local_file_path = os.path.join(path, sg_attachment["name"])
-        else:
-            local_file_path = path
+        :param dict[str,Any]|SGEntity project_entity: A project entity to filter by.
+        :param bool raw_values: Whether to convert entities to pysg objects or not.
+        :return: All fields and values from this entity in a dict. If a project entity is given
+                 only fields that are visible to the project are returned.
+        :rtype: dict[str,Any]
+        """
+        if project_entity is not None and not isinstance(project_entity, dict):
+            project_entity = project_entity.to_dict()
 
-        return self._entity.sg.download_attachment(
-            attachment=sg_attachment, file_path=local_file_path
+        sg_entity_fields = self.sg.schema_field_read(
+            self._type, project_entity=project_entity
         )
+        fields = [
+            field
+            for field, schema in sg_entity_fields.items()
+            if schema["visible"]["value"]
+        ]
+        all_fields = self.sg.find_one(self._type, [["id", "is", self._id]], fields)
 
-    def schema(self):
-        """
-        :return: The schema of this field.
-                 For example::
+        if raw_values:
+            return all_fields
+        else:
+            return convert_fields_to_pysg(self._sg, all_fields)
 
-                     {'custom_metadata': {'editable': True, 'value': ''},
-                      'data_type': {'editable': False, 'value': 'status_list'},
-                      'description': {'editable': True, 'value': ''},
-                      'editable': {'editable': False, 'value': True},
-                      'entity_type': {'editable': False, 'value': 'Shot'},
-                      'mandatory': {'editable': False, 'value': False},
-                      'name': {'editable': True, 'value': 'Sound delivery'},
-                      'properties': {'default_value': {'editable': True,
-                                                       'value': ''},
-                                     'display_values': {'editable': False,
-                                                        'value': {'dlvr': 'Delivered',
-                                                                  'wtg': 'Waiting '
-                                                                         'to '
-                                                                         'Start'}},
-                                     'hidden_values': {'editable': False,
-                                                       'value': []},
-                                     'summary_default': {'editable': True,
-                                                         'value': 'none'},
-                                     'valid_values': {'editable': True,
-                                                      'value': ['dlvr',
-                                                                'wtg']}},
-                      'ui_value_displayable': {'editable': False,
-                                               'value': True},
-                      'unique': {'editable': False, 'value': False},
-                      'visible': {'editable': True, 'value': True}}
+    def to_dict(self):
+        # noinspection PyUnresolvedReferences
         """
-        return self._entity.sg.schema_field_read(self._entity.type, self._name)[
-            self._name
-        ]
+        Creates a dict with just "type" and "id" (and does not call SG).
 
-    def _update_schema(self, prop, value, project_entity=None):
-        """
-        Update a property of the field.
+        Example::
 
-        :return: True when the update succeeded.
-        :rtype: bool
+            >>> sg_entity.to_dict()
+            {'type': 'CustomEntity01', 'id': 1}
+
+        :returns: The entity as a dict which is ready to consume by the shotgun_api3 methods.
+
+        :rtype: dict[str,Any]
         """
-        return self._entity.sg.schema_field_update(
-            self._entity.type,
-            self._name,
-            {prop: value},
-            project_entity=convert_value_to_dict(project_entity),
-        )
+        return {"id": self._id, "type": self._type}
 
-    @property
-    def data_type(self):
+    def batch_update_dict(self, data):
         """
-        :return: The data type of the field.
-        :rtype: str
+        :param dict[str,Any] data: A dict with the fields and values to set.
+        :returns: A dict that can be used in a shotgun.batch() call to update some fields.
+                  Useful when you want to collect field changes and set them in one go.
+        :rtype: dict[str,Any]
         """
-        return self.schema()["data_type"]["value"]
-
-    @data_type.setter
-    def data_type(self, value):
-        self._update_schema("data_type", value)
+        return {
+            "request_type": "update",
+            "entity_type": self._type,
+            "entity_id": self._id,
+            "data": convert_fields_to_dicts(data),
+        }
 
-    @property
-    def description(self):
+    def set(self, data, multi_entity_update_modes=None):
         """
-        :return: The description of the field.
-        :rtype: str
+        Set many fields at once on this entity.
+
+        :param dict[str,Any] data: A dict with the fields and values to set.
+        :param dict multi_entity_update_modes: Optional dict indicating what update mode to use
+            when updating a multi-entity link field. The keys in the dict are the fields to set
+            the mode for, and the values from the dict are one of ``set``, ``add``, or ``remove``.
+            Defaults to ``set``.
+            ::
+
+                multi_entity_update_modes={"shots": "add", "assets": "remove"}
+        :return:
         """
-        return self.schema()["description"]["value"]
+        return self.sg.update(
+            self._type,
+            self._id,
+            data=convert_fields_to_dicts(data),
+            multi_entity_update_modes=multi_entity_update_modes,
+        )
 
-    @property
-    def display_name(self):
+    def get(self, fields, raw_values=False):
         """
-        :return: The display name of the field.
-        :rtype: str
+        Set many fields at once on this entity.
+
+        :param list[str] fields: A list of fields to query from this entity.
+        :param bool raw_values: Any entities will be converted to pyshotgrid instances.
+                                If you set this parameter to True you can turn this behaviour off.
+        :return: A dict with the fields and their corresponding values.
+        :rtype: dict[str,Any]
         """
-        return self.schema()["name"]["value"]
+        sg_fields = self.sg.find_one(self._type, [["id", "is", self._id]], fields)
 
-    @display_name.setter
-    def display_name(self, value):
-        self._update_schema("name", value)
+        del sg_fields["id"]
+        del sg_fields["type"]
 
-    @property
-    def custom_metadata(self):
-        """
-        :return: Custom metadata attached to this field.
-        :rtype: str
+        if raw_values:
+            return sg_fields
+        else:
+            return convert_fields_to_pysg(self._sg, sg_fields)
+
+    def delete(self):
         """
-        return self.schema()["custom_metadata"]["value"]
+        Delete this entity.
 
-    @custom_metadata.setter
-    def custom_metadata(self, value):
-        self._update_schema("custom_metadata", value)
+        .. Note::
 
-    @property
-    def properties(self):
-        """
-        :return: The properties of the field. This strongly depends on the data type of the field.
-                 This can for example give you all the possible values of a status field.
-        :rtype: dict[str,dict[str,Any]]
-        """
-        return self.schema()["properties"]
+            The python object that represents this entity does not make sense any more after you
+            ran this method and will create errors if you keep calling functions on it.
 
-    @properties.setter
-    def properties(self, value):
-        self._update_schema("properties", value)
+        :return: Whether the entity was successfully deleted.
+        :rtype: bool
+        """
+        return self._sg.delete(self._type, self._id)
 
-    @property
-    def valid_types(self):
+    def schema(self):
         """
-        :return: The valid SG entity types for entity- and multi-entity-fields.
-        :rtype: list[str]
+        :return: The schema for the current entity.
         """
-        return self.schema()["properties"]["valid_types"]["value"]
+        return self.sg.schema_entity_read()[self._type]
 
-    def batch_update_dict(self, value):
+    def field_schemas(self):
         """
-        :param Any value: The value to set.
-        :returns: A dict that can be used in a shotgun.batch() call to update this field.
-                  Useful when you want to collect field changes and set them in one go.
-        :rtype: dict[str,Any]
+        :return: The schemas of all the entity fields.
+        :rtype: dict[str,FieldSchema]
         """
-        value = convert_value_to_dict(value)
         return {
-            "request_type": "update",
-            "entity_type": self._entity.type,
-            "entity_id": self._entity.id,
-            "data": {self._name: value},
+            field: FieldSchema(self._sg, self._type, field)
+            for field in self.sg.schema_field_read(self._type)
         }
+
+    def _publishes(
+        self, base_filter=None, pub_types=None, latest=False, additional_sg_filter=None
+    ):
+        """
+        This function is meant as a base for a "publishes" function on a sub class. Publishes
+        are stored in different fields for each entity and not every entity has a published file.
+        This is why this function is hidden by default.
+
+        :param base_filter: The basic sg filter to get the publishes that are associated with
+                            this entity.
+        :param str|list[str]|None pub_types: The names of the Publish File Types to return.
+        :param bool latest: Whether to get the "latest" publishes or not. This uses the
+                            same logic as the tk-multi-loader2 app which is as follows:
+                             - group all publishes with the same "name" field together
+                             - from these get the publishes with the highest "version_number" field
+                             - if there are publishes with the same "name" and "version_number" the
+                               newest one wins.
+        :param additional_sg_filter:
+        :return: All published files from this shot.
+        :rtype: list[SGPublishedFile]
+        """
+        base_filter = base_filter or []
+        if pub_types is not None:
+            if isinstance(pub_types, list):
+                pub_types_filter = {"filter_operator": "any", "filters": []}
+                for pub_type in pub_types:
+                    pub_types_filter["filters"].append(
+                        ["published_file_type.PublishedFileType.code", "is", pub_type]
+                    )
+            else:
+                pub_types_filter = [
+                    "published_file_type.PublishedFileType.code",
+                    "is",
+                    pub_types,
+                ]
+            base_filter.append(pub_types_filter)
+
+        additional_sg_filter = additional_sg_filter or []
+        result_filter = base_filter + additional_sg_filter
+
+        sg_publishes = self.sg.find(
+            "PublishedFile", result_filter, ["name", "version_number", "created_at"]
+        )
+        if latest:
+            # group publishes by "name"
+            tmp = {}
+            for sg_publish in sg_publishes:
+                if sg_publish["name"] in tmp:
+                    tmp[sg_publish["name"]].append(sg_publish)
+                else:
+                    tmp[sg_publish["name"]] = [sg_publish]
+
+            # sort them by date and than by version_number which sorts the latest publish to the
+            # last position.
+            result = []
+            for publishes in tmp.values():
+                publishes.sort(
+                    key=lambda pub: (pub["created_at"], pub["version_number"])
+                )
+                result.append(publishes[-1])
+
+            # Sort one more time by name.
+            result.sort(key=lambda pub: pub["name"])
+
+            sg_publishes = result
+
+        return [new_entity(self._sg, sg_publish) for sg_publish in sg_publishes]
```

### Comparing `pyshotgrid-0.8.0/src/pyshotgrid/sg_default_entities.py` & `pyshotgrid-0.9.1/src/pyshotgrid/sg_default_entities.py`

 * *Files identical despite different names*

### Comparing `pyshotgrid-0.8.0/src/pyshotgrid/sg_entity.py` & `pyshotgrid-0.9.1/src/pyshotgrid/sg_site.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,298 +1,218 @@
-from .core import convert_fields_to_dicts, convert_fields_to_pysg, new_entity, new_site
-from .field import Field
+from .core import convert_fields_to_dicts, convert_filters_to_dict, new_entity
 
 
-class SGEntity(object):
+class SGSite(object):
     """
-    An instance of this class represents a single entity in ShotGrid.
+    An instance of this class represents a ShotGrid site as a whole.
 
     .. Note::
 
         Try to avoid creating instances of this class in production code and
-        use the :py:meth:`pyshotgrid.new_entity <pyshotgrid.core.new_entity>`
-        method instead. This will make sure that you always get the correct
-        entity class to work with.
+        use the :py:meth:`pyshotgrid.new_site <pyshotgrid.core.new_site>`
+        method instead. This gives you more ways to initialize the this class
+        and ensures that the plugin system is correctly used.
     """
 
-    def __init__(self, sg, entity_type, entity_id):
+    def __init__(self, sg):
         """
         :param shotgun_api3.shotgun.Shotgun sg:
             A fully initialized instance of shotgun_api3.Shotgun.
-        :param str entity_type: The ShotGrid type of the entity.
-        :param int entity_id: The ID of the ShotGrid entity.
         """
-        self._sg = sg  # :type: shotgun_api3.shotgun.Shotgun
-        self._type = entity_type
-        self._id = entity_id
-
-    def __str__(self):
-        return "{} - Type: {} - ID: {} - URL: {}".format(
-            self.__class__.__name__, self._type, self._id, self.url
-        )
-
-    @property
-    def id(self):
-        """
-        :return: The ID of the ShotGrid entity.
-        :rtype: int
-        """
-        return self._id
-
-    @property
-    def type(self):
-        """
-        :return: The type of the ShotGrid entity.
-        :rtype: str
-        """
-        return self._type
+        self._sg = sg
 
     @property
     def sg(self):
         """
         :return: The Shotgun instance that the entity belongs to.
         :rtype: shotgun_api3.shotgun.Shotgun
         """
         return self._sg
 
-    @property
-    def site(self):
-        """
-        :return: The pyshotgrid site for this entity.
-        :rtype: SGSite
-        """
-        return new_site(self._sg)
-
-    @property
-    def url(self):
-        """
-        :return: The ShotGrid URL for this entity.
-
-            .. note::
-
-               This will only work on entities that have a detail view enabled
-               in the system settings.
-        :rtype: str
-        """
-        return "{}/detail/{}/{}".format(self.sg.base_url, self._type, self._id)
-
-    def __getitem__(self, field):
+    def create(self, entity_type, data):
         """
-        Enabling dict notation to query fields of the entity from ShotGrid.
-
-        :param str field: The field to query.
-        :return: The value of the field. Any entities will be automatically converted to
-                 pyshotgrid objects.
-        """
-        return Field(name=field, entity=self)
-
-    def fields(self, project_entity=None):
-        """
-        :param dict[str,Any]|SGEntity|None project_entity: A project entity to filter by.
-        :return: All fields from this entity. If a project entity is given
-                 only fields that are visible to the project are returned.
-        :rtype: list[Field]
-        """
-        if project_entity is not None and not isinstance(project_entity, dict):
-            project_entity = project_entity.to_dict()
-
-        sg_entity_fields = self.sg.schema_field_read(
-            self._type, project_entity=project_entity
+        The same function as
+        :py:meth:`Shotgun.create <shotgun_api3:shotgun_api3.shotgun.Shotgun.create>`,
+        but it accepts and returns a pyshotgrid object.
+
+        :param str entity_type: The type of the entity to create.
+        :param dict[str,Any]|None data: dict of fields and values to set on creation.
+                                        The values can contain pysg objects.
+        :return: The new created entity.
+        :rtype: SGEntity
+        """
+        # noinspection PyTypeChecker
+        return new_entity(
+            self._sg,
+            self._sg.create(
+                entity_type=entity_type,
+                data=convert_fields_to_dicts(data),
+                return_fields=None,
+            ),
         )
-        fields = [
-            field
-            for field, schema in sg_entity_fields.items()
-            if schema["visible"]["value"]
-        ]
 
-        return [Field(name=field, entity=self) for field in fields]
-
-    def all_field_values(self, project_entity=None, raw_values=False):
+    def find(
+        self,
+        entity_type,
+        filters,
+        order=None,
+        filter_operator=None,
+        limit=0,
+        retired_only=False,
+        page=0,
+        include_archived_projects=True,
+        additional_filter_presets=None,
+    ):
         """
-        :param dict[str,Any]|SGEntity project_entity: A project entity to filter by.
-        :param bool raw_values: Whether to convert entities to pysg objects or not.
-        :return: All fields and values from this entity in a dict. If a project entity is given
-                 only fields that are visible to the project are returned.
-        :rtype: dict[str,Any]
+        The same function as
+        :py:meth:`Shotgun.find <shotgun_api3:shotgun_api3.shotgun.Shotgun.find>`, but it
+        accepts and returns pyshotgrid objects.
+
+        :param entity_type:
+        :param filters:
+        :param order:
+        :param filter_operator:
+        :param limit:
+        :param retired_only:
+        :param page:
+        :param include_archived_projects:
+        :param additional_filter_presets:
+        :return:
         """
-        if project_entity is not None and not isinstance(project_entity, dict):
-            project_entity = project_entity.to_dict()
-
-        sg_entity_fields = self.sg.schema_field_read(
-            self._type, project_entity=project_entity
-        )
-        fields = [
-            field
-            for field, schema in sg_entity_fields.items()
-            if schema["visible"]["value"]
+        # noinspection PyTypeChecker
+        return [
+            new_entity(self._sg, sg_entity)
+            for sg_entity in self._sg.find(
+                entity_type=entity_type,
+                filters=convert_filters_to_dict(filters),
+                fields=None,
+                order=order,
+                filter_operator=filter_operator,
+                limit=limit,
+                retired_only=retired_only,
+                page=page,
+                include_archived_projects=include_archived_projects,
+                additional_filter_presets=additional_filter_presets,
+            )
         ]
-        all_fields = self.sg.find_one(self._type, [["id", "is", self._id]], fields)
-
-        if raw_values:
-            return all_fields
-        else:
-            return convert_fields_to_pysg(self._sg, all_fields)
-
-    def to_dict(self):
-        # noinspection PyUnresolvedReferences
-        """
-        Creates a dict with just "type" and "id" (and does not call SG).
-
-        Example::
-
-            >>> sg_entity.to_dict()
-            {'type': 'CustomEntity01', 'id': 1}
-
-        :returns: The entity as a dict which is ready to consume by the shotgun_api3 methods.
 
-        :rtype: dict[str,Any]
-        """
-        return {"id": self._id, "type": self._type}
-
-    def batch_update_dict(self, data):
-        """
-        :param dict[str,Any] data: A dict with the fields and values to set.
-        :returns: A dict that can be used in a shotgun.batch() call to update some fields.
-                  Useful when you want to collect field changes and set them in one go.
-        :rtype: dict[str,Any]
-        """
-        return {
-            "request_type": "update",
-            "entity_type": self._type,
-            "entity_id": self._id,
-            "data": convert_fields_to_dicts(data),
-        }
-
-    def set(self, data, multi_entity_update_modes=None):
-        """
-        Set many fields at once on this entity.
-
-        :param dict[str,Any] data: A dict with the fields and values to set.
-        :param dict multi_entity_update_modes: Optional dict indicating what update mode to use
-            when updating a multi-entity link field. The keys in the dict are the fields to set
-            the mode for, and the values from the dict are one of ``set``, ``add``, or ``remove``.
-            Defaults to ``set``.
-            ::
-
-                multi_entity_update_modes={"shots": "add", "assets": "remove"}
-        :return:
+    def find_one(
+        self,
+        entity_type,
+        filters,
+        order=None,
+        filter_operator=None,
+        limit=0,
+        retired_only=False,
+        page=0,
+        include_archived_projects=True,
+        additional_filter_presets=None,
+    ):
         """
-        return self.sg.update(
-            self._type,
-            self._id,
-            data=convert_fields_to_dicts(data),
-            multi_entity_update_modes=multi_entity_update_modes,
+        The same function as
+        :py:meth:`Shotgun.find_one <shotgun_api3:shotgun_api3.shotgun.Shotgun.find_one>` ,
+        but it accepts and returns pyshotgrid objects.
+        """
+        # TODO allow entering the display name for the entity_type
+        result = self.find(
+            entity_type=entity_type,
+            filters=filters,
+            order=order,
+            filter_operator=filter_operator,
+            limit=limit,
+            retired_only=retired_only,
+            page=page,
+            include_archived_projects=include_archived_projects,
+            additional_filter_presets=additional_filter_presets,
         )
+        if result:
+            return result[0]
 
-    def get(self, fields, raw_values=False):
+    def project(self, name_or_id):
         """
-        Set many fields at once on this entity.
+        :param int|str name_or_id: The name or id of the project to return.
+                                   The name can either match the "tank_name" (recommended)
+                                   or the "name" field.
+        :return: The found SG project or None.
+        :rtype: SGProject|None
+        """
+        sg_projects = self.projects(names_or_ids=[name_or_id], include_archived=True)
+        if sg_projects:
+            return sg_projects[0]
 
-        :param list[str] fields: A list of fields to query from this entity.
-        :param bool raw_values: Any entities will be converted to pyshotgrid instances.
-                                If you set this parameter to True you can turn this behaviour off.
-        :return: A dict with the fields and their corresponding values.
-        :rtype: dict[str,Any]
+    def projects(
+        self, names_or_ids=None, include_archived=False, template_projects=False
+    ):
         """
-        sg_fields = self.sg.find_one(self._type, [["id", "is", self._id]], fields)
+        :param list[int|str]|None names_or_ids: List of names or ids of the projects to return. The
+                                                names can either match the "tank_name" (recommended)
+                                                or the "name" field.
+        :param bool include_archived: Whether to include archived projects or not.
+        :param bool template_projects: Whether to return template projects or not.
+        :return: A list of SG projects.
+        :rtype: list[SGProject]
+        """
+        sg_projects = self._sg.find(
+            "Project",
+            [["is_template", "is", template_projects]],
+            ["tank_name", "name"],
+            include_archived_projects=include_archived,
+        )
 
-        del sg_fields["id"]
-        del sg_fields["type"]
+        if names_or_ids is not None:
+            if isinstance(names_or_ids[0], int):
+                sg_projects = [
+                    sg_project
+                    for sg_project in sg_projects
+                    if sg_project["id"] in names_or_ids
+                ]
+            else:
+                sg_projects = [
+                    sg_project
+                    for sg_project in sg_projects
+                    if (
+                        sg_project["tank_name"] in names_or_ids
+                        or sg_project["name"] in names_or_ids
+                    )
+                ]
 
-        if raw_values:
-            return sg_fields
-        else:
-            return convert_fields_to_pysg(self._sg, sg_fields)
+        return [new_entity(self._sg, sg_project) for sg_project in sg_projects]
 
-    def delete(self):
+    def pipeline_configuration(self, name_or_id=None, project=None):
         """
-        Delete this entity.
-
-        .. Note::
+        :param int|str|None name_or_id: Name or ID of the PipelineConfiguration.
+        :param dict|SGEntity|None project: The project that the PipelineConfiguration
+                                                 is attached to.
+        :return: The PipelineConfiguration.
+        :rtype: SGEntity|None
+        """
+        base_filter = []
+        if name_or_id is not None:
+            if isinstance(name_or_id, int):
+                return new_entity(
+                    self._sg, entity_type="PipelineConfiguration", entity_id=name_or_id
+                )
+            else:
+                base_filter = [["code", "is", name_or_id]]
 
-            The python object that represents this entity does not make sense any more after you
-            ran this method and will create errors if you keep calling functions on it.
+        if project is not None:
+            if isinstance(project, dict):
+                base_filter.append(["project", "is", project])
+            else:
+                base_filter.append(["project", "is", project.to_dict()])
 
-        :return: Whether the entity was successfully deleted.
-        :rtype: bool
-        """
-        return self._sg.delete(self._type, self._id)
+        sg_pipe_config = self._sg.find_one("PipelineConfiguration", base_filter)
 
-    def schema(self):
-        """
-        :return: The schema for the current entity.
-        """
-        return self.sg.schema_entity_read()[self._type]
+        if sg_pipe_config:
+            return new_entity(self._sg, sg_pipe_config)
 
-    def field_schemas(self):
+    def people(self, additional_sg_filter=None):
         """
-        :return: The schemas of all the entity fields.
+        :param list|None additional_sg_filter:
+        :return: All HumanUsers of this ShotGrid site.
+        :rtype: list[SGHumanUser]
         """
-        return self.sg.schema_field_read(self._type)
-
-    def _publishes(
-        self, base_filter=None, pub_types=None, latest=False, additional_sg_filter=None
-    ):
-        """
-        This function is meant as a base for a "publishes" function on a sub class. Publishes
-        are stored in different fields for each entity and not every entity has a published file.
-        This is why this function is hidden by default.
-
-        :param base_filter: The basic sg filter to get the publishes that are associated with
-                            this entity.
-        :param str|list[str]|None pub_types: The names of the Publish File Types to return.
-        :param bool latest: Whether to get the "latest" publishes or not. This uses the
-                            same logic as the tk-multi-loader2 app which is as follows:
-                             - group all publishes with the same "name" field together
-                             - from these get the publishes with the highest "version_number" field
-                             - if there are publishes with the same "name" and "version_number" the
-                               newest one wins.
-        :param additional_sg_filter:
-        :return: All published files from this shot.
-        :rtype: list[SGPublishedFile]
-        """
-        base_filter = base_filter or []
-        if pub_types is not None:
-            if isinstance(pub_types, list):
-                pub_types_filter = {"filter_operator": "any", "filters": []}
-                for pub_type in pub_types:
-                    pub_types_filter["filters"].append(
-                        ["published_file_type.PublishedFileType.code", "is", pub_type]
-                    )
-            else:
-                pub_types_filter = [
-                    "published_file_type.PublishedFileType.code",
-                    "is",
-                    pub_types,
-                ]
-            base_filter.append(pub_types_filter)
-
-        additional_sg_filter = additional_sg_filter or []
-        result_filter = base_filter + additional_sg_filter
-
-        sg_publishes = self.sg.find(
-            "PublishedFile", result_filter, ["name", "version_number", "created_at"]
-        )
-        if latest:
-            # group publishes by "name"
-            tmp = {}
-            for sg_publish in sg_publishes:
-                if sg_publish["name"] in tmp:
-                    tmp[sg_publish["name"]].append(sg_publish)
-                else:
-                    tmp[sg_publish["name"]] = [sg_publish]
-
-            # sort them by date and than by version_number which sorts the latest publish to the
-            # last position.
-            result = []
-            for publishes in tmp.values():
-                publishes.sort(
-                    key=lambda pub: (pub["created_at"], pub["version_number"])
-                )
-                result.append(publishes[-1])
-
-            # Sort one more time by name.
-            result.sort(key=lambda pub: pub["name"])
-
-            sg_publishes = result
-
-        return [new_entity(self._sg, sg_publish) for sg_publish in sg_publishes]
+        # TODO add "only_active" and "name_or_id" parameter
+        return [
+            new_entity(self._sg, sg_user)
+            for sg_user in self._sg.find("HumanUser", additional_sg_filter or [])
+        ]
```

### Comparing `pyshotgrid-0.8.0/src/pyshotgrid.egg-info/PKG-INFO` & `pyshotgrid-0.9.1/src/pyshotgrid.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshotgrid
-Version: 0.8.0
+Version: 0.9.1
 Summary: A pythonic and object oriented way to talk to Autodesk ShotGrid.
 Author-email: Fabian Geisler <info@fasbue.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fabiangeisler/pyshotgrid
 Project-URL: Documentation, https://fabiangeisler.github.io/pyshotgrid
 Project-URL: Bug Tracker, https://github.com/fabiangeisler/pyshotgrid/issues
 Keywords: shotgrid
@@ -21,19 +21,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<p align="center">
+  <img src="https://github.com/fabiangeisler/pyshotgrid/blob/main/icons/pysg_logo.png?raw=true" />
+</p>
+
 [![pypi](https://img.shields.io/pypi/v/pyshotgrid.svg)](https://pypi.python.org/pypi/pyshotgrid)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyshotgrid.svg)](https://pypi.python.org/pypi/pyshotgrid/)
 [![Tests](https://github.com/fabiangeisler/pyshotgrid/actions/workflows/Tests.yml/badge.svg)](https://github.com/fabiangeisler/pyshotgrid/actions/workflows/Tests.yml)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![linter: ruff](https://img.shields.io/static/v1?label=linter&message=ruff&color=green)](https://github.com/charliermarsh/ruff)
+[![type checker: mypy](https://img.shields.io/badge/%20type_checker-my[py]-%231674b1?style=flat)](https://github.com/python/mypy)
 
 `pyshotgrid` is a python package that gives you a pythonic and
 object oriented way to talk to [Autodesk ShotGrid](https://www.autodesk.com/products/shotgrid/overview).
 
 > **Warning**
 > This python library is still in early development and the API is not yet stable.
 > Please be cautious in a production environment.
```

### Comparing `pyshotgrid-0.8.0/src/pyshotgrid.egg-info/SOURCES.txt` & `pyshotgrid-0.9.1/src/pyshotgrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*


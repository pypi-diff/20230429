# Comparing `tmp/pyaud-6.2.1.tar.gz` & `tmp/pyaud-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaud-6.2.1.tar", max compression
+gzip compressed data, was "pyaud-6.2.2.tar", max compression
```

## Comparing `pyaud-6.2.1.tar` & `pyaud-6.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1073 2023-02-27 08:54:42.354367 pyaud-6.2.1/LICENSE
--rw-r--r--   0        0        0     4308 2023-02-28 08:57:40.004010 pyaud-6.2.1/README.rst
--rw-r--r--   0        0        0      327 2023-02-27 08:54:42.357974 pyaud-6.2.1/pyaud/__init__.py
--rw-r--r--   0        0        0      152 2023-02-27 08:54:42.358097 pyaud-6.2.1/pyaud/__main__.py
--rw-r--r--   0        0        0     2048 2023-02-27 08:54:42.358193 pyaud-6.2.1/pyaud/_builtins.py
--rw-r--r--   0        0        0     1817 2023-02-27 08:54:42.358385 pyaud-6.2.1/pyaud/_config.py
--rw-r--r--   0        0        0     3122 2023-02-27 08:54:42.358741 pyaud-6.2.1/pyaud/_core.py
--rw-r--r--   0        0        0      685 2023-02-27 08:54:42.359027 pyaud-6.2.1/pyaud/_main.py
--rw-r--r--   0        0        0     2744 2023-02-27 08:54:42.359156 pyaud-6.2.1/pyaud/_objects.py
--rw-r--r--   0        0        0      208 2023-02-28 08:58:44.170103 pyaud-6.2.1/pyaud/_version.py
--rw-r--r--   0        0        0      696 2023-02-27 08:54:42.359859 pyaud-6.2.1/pyaud/exceptions.py
--rw-r--r--   0        0        0      898 2023-02-27 08:54:42.360192 pyaud-6.2.1/pyaud/messages.py
--rw-r--r--   0        0        0    23867 2023-02-27 08:54:42.360680 pyaud-6.2.1/pyaud/plugins.py
--rw-r--r--   0        0        0        0 2023-02-27 08:54:42.360719 pyaud-6.2.1/pyaud/py.typed
--rw-r--r--   0        0        0     2248 2023-02-28 08:58:44.170397 pyaud-6.2.1/pyproject.toml
--rw-r--r--   0        0        0     5350 1970-01-01 00:00:00.000000 pyaud-6.2.1/setup.py
--rw-r--r--   0        0        0     5339 1970-01-01 00:00:00.000000 pyaud-6.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-04 05:11:58.984347 pyaud-6.2.2/LICENSE
+-rw-r--r--   0        0        0     4308 2023-04-29 03:17:29.436045 pyaud-6.2.2/README.rst
+-rw-r--r--   0        0        0      327 2023-03-04 05:31:45.479018 pyaud-6.2.2/pyaud/__init__.py
+-rw-r--r--   0        0        0      152 2023-03-04 05:11:59.012743 pyaud-6.2.2/pyaud/__main__.py
+-rw-r--r--   0        0        0     2048 2023-03-04 05:31:45.479122 pyaud-6.2.2/pyaud/_builtins.py
+-rw-r--r--   0        0        0     1817 2023-03-04 05:31:45.479339 pyaud-6.2.2/pyaud/_config.py
+-rw-r--r--   0        0        0     3122 2023-03-04 05:31:45.479900 pyaud-6.2.2/pyaud/_core.py
+-rw-r--r--   0        0        0      685 2023-03-04 05:31:45.480249 pyaud-6.2.2/pyaud/_main.py
+-rw-r--r--   0        0        0     2744 2023-03-04 05:31:45.480360 pyaud-6.2.2/pyaud/_objects.py
+-rw-r--r--   0        0        0      208 2023-04-29 03:27:36.582625 pyaud-6.2.2/pyaud/_version.py
+-rw-r--r--   0        0        0      696 2023-03-04 05:31:45.480459 pyaud-6.2.2/pyaud/exceptions.py
+-rw-r--r--   0        0        0      898 2023-03-04 05:31:45.480928 pyaud-6.2.2/pyaud/messages.py
+-rw-r--r--   0        0        0    23867 2023-03-04 05:31:45.481473 pyaud-6.2.2/pyaud/plugins.py
+-rw-r--r--   0        0        0        0 2023-03-04 05:11:59.011625 pyaud-6.2.2/pyaud/py.typed
+-rw-r--r--   0        0        0     2248 2023-04-29 03:27:36.582788 pyaud-6.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5350 1970-01-01 00:00:00.000000 pyaud-6.2.2/setup.py
+-rw-r--r--   0        0        0     5339 1970-01-01 00:00:00.000000 pyaud-6.2.2/PKG-INFO
```

### Comparing `pyaud-6.2.1/LICENSE` & `pyaud-6.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaud-6.2.1/README.rst` & `pyaud-6.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyaud-6.2.1/pyaud/_builtins.py` & `pyaud-6.2.2/pyaud/_builtins.py`

 * *Files identical despite different names*

### Comparing `pyaud-6.2.1/pyaud/_config.py` & `pyaud-6.2.2/pyaud/_config.py`

 * *Files identical despite different names*

### Comparing `pyaud-6.2.1/pyaud/_core.py` & `pyaud-6.2.2/pyaud/_core.py`

 * *Files identical despite different names*

### Comparing `pyaud-6.2.1/pyaud/_main.py` & `pyaud-6.2.2/pyaud/_main.py`

 * *Files identical despite different names*

### Comparing `pyaud-6.2.1/pyaud/_objects.py` & `pyaud-6.2.2/pyaud/_objects.py`

 * *Files identical despite different names*

### Comparing `pyaud-6.2.1/pyaud/exceptions.py` & `pyaud-6.2.2/pyaud/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyaud-6.2.1/pyaud/messages.py` & `pyaud-6.2.2/pyaud/messages.py`

 * *Files identical despite different names*

### Comparing `pyaud-6.2.1/pyaud/plugins.py` & `pyaud-6.2.2/pyaud/plugins.py`

 * *Files identical despite different names*

### Comparing `pyaud-6.2.1/pyproject.toml` & `pyaud-6.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 license = "MIT"
 maintainers = [
   "jshwi <stephen@jshwisolutions.com>"
 ]
 name = "pyaud"
 readme = "README.rst"
 repository = "https://github.com/jshwi/pyaud"
-version = "6.2.1"
+version = "6.2.2"
 
 [tool.poetry.dependencies]
 arcon = "^0.2.1"
 gitpython = "^3.1.30"
 lsfiles = ">=0.5"
 object-colors = "^2.0.1"
 pyaud-plugins = ">=0.14.0"
```

### Comparing `pyaud-6.2.1/setup.py` & `pyaud-6.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'spall>=0,<1']
 
 entry_points = \
 {'console_scripts': ['pyaud = pyaud.__main__:main']}
 
 setup_kwargs = {
     'name': 'pyaud',
-    'version': '6.2.1',
+    'version': '6.2.2',
     'description': 'Framework for writing Python package audits',
     'long_description': 'pyaud\n=====\n.. image:: https://img.shields.io/badge/License-MIT-yellow.svg\n    :target: https://opensource.org/licenses/MIT\n    :alt: License\n.. image:: https://img.shields.io/pypi/v/pyaud\n    :target: https://pypi.org/project/pyaud/\n    :alt: PyPI\n.. image:: https://github.com/jshwi/pyaud/actions/workflows/build.yaml/badge.svg\n    :target: https://github.com/jshwi/pyaud/actions/workflows/build.yaml\n    :alt: Build\n.. image:: https://github.com/jshwi/pyaud/actions/workflows/codeql-analysis.yml/badge.svg\n    :target: https://github.com/jshwi/pyaud/actions/workflows/codeql-analysis.yml\n    :alt: CodeQL\n.. image:: https://results.pre-commit.ci/badge/github/jshwi/pyaud/master.svg\n   :target: https://results.pre-commit.ci/latest/github/jshwi/pyaud/master\n   :alt: pre-commit.ci status\n.. image:: https://codecov.io/gh/jshwi/pyaud/branch/master/graph/badge.svg\n    :target: https://codecov.io/gh/jshwi/pyaud\n    :alt: codecov.io\n.. image:: https://readthedocs.org/projects/pyaud/badge/?version=latest\n    :target: https://pyaud.readthedocs.io/en/latest/?badge=latest\n    :alt: readthedocs.org\n.. image:: https://img.shields.io/badge/python-3.8-blue.svg\n    :target: https://www.python.org/downloads/release/python-380\n    :alt: python3.8\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n    :alt: Black\n.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336\n    :target: https://pycqa.github.io/isort/\n    :alt: isort\n.. image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n    :target: https://github.com/PyCQA/docformatter\n    :alt: docformatter\n.. image:: https://img.shields.io/badge/linting-pylint-yellowgreen\n    :target: https://github.com/PyCQA/pylint\n    :alt: pylint\n.. image:: https://img.shields.io/badge/security-bandit-yellow.svg\n    :target: https://github.com/PyCQA/bandit\n    :alt: Security Status\n.. image:: https://snyk.io/test/github/jshwi/pyaud/badge.svg\n    :target: https://snyk.io/test/github/jshwi/pyaud/badge.svg\n    :alt: Known Vulnerabilities\n.. image:: https://snyk.io/advisor/python/pyaud/badge.svg\n    :target: https://snyk.io/advisor/python/pyaud\n    :alt: pyaud\n\nFramework for writing Python package audits\n-------------------------------------------\n\nThe ``pyaud`` framework is designed for writing modular audits for Python packages\n\nAudits can be run to fail, such as when using CI, or include a fix\n\nFixes can be written for whole directories or individual files\n\nPlugins can be written for manipulating files\n\nSupports single script plugins\n\nInstallation\n------------\n\n.. code-block:: console\n\n    $ pip install pyaud\n\nUsage\n-----\n\nCommandline\n***********\n\n.. code-block:: console\n\n    usage: pyaud [-h] [-v] [-f] [-n] [-s] [--audit LIST] [--exclude EXCLUDE] MODULE\n\n    positional arguments:\n      MODULE             choice of module: [modules] to list all\n\n    optional arguments:\n      -h, --help         show this help message and exit\n      -v, --version      show program\'s version number and exit\n      -f, --fix          suppress and fix all fixable issues\n      -n, --no-cache     disable file caching\n      -s, --suppress     continue without stopping for errors\n      --audit LIST       comma separated list of plugins for audit\n      --exclude EXCLUDE  regex of paths to ignore\n\nPlugins\n*******\n\n``pyaud`` will search for a plugins package in the project root\n\nTo register a plugin package ensure it is importable and prefix the package with ``pyaud_``\n\nThe name ``pyaud_plugins`` is reserved and will be automatically imported\n\nTo view available plugins see ``pyaud-plugins`` `README <https://github.com/jshwi/pyaud-plugins/blob/master/README.rst>`_ or run ``pyaud modules all``\n\nFor writing plugins see `docs <https://jshwi.github.io/pyaud/pyaud.html#pyaud-plugins>`_\n\nConfigure\n*********\n\nConfiguration values are declared in the pyproject.toml file\n\n.. code-block:: toml\n\n    [tool.pyaud]\n    audit = [\n      "commit-policy",\n      "const",\n      "docs",\n      "files",\n      "format",\n      "format-docs",\n      "format-str",\n      "imports",\n      "lint",\n      "params",\n      "test",\n      "typecheck",\n      "unused"\n    ]\n    exclude = \'\'\'\n      (?x)^(\n        | docs\\/conf\\.py\n        | whitelist\\.py\n      )$\n    \'\'\'\n',
     'author': 'jshwi',
     'author_email': 'stephen@jshwisolutions.com',
     'maintainer': 'jshwi',
     'maintainer_email': 'stephen@jshwisolutions.com',
     'url': 'https://pypi.org/project/pyaud/',
```

### Comparing `pyaud-6.2.1/PKG-INFO` & `pyaud-6.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaud
-Version: 6.2.1
+Version: 6.2.2
 Summary: Framework for writing Python package audits
 Home-page: https://pypi.org/project/pyaud/
 License: MIT
 Keywords: audit,ci,fix,format,style
 Author: jshwi
 Author-email: stephen@jshwisolutions.com
 Maintainer: jshwi
```


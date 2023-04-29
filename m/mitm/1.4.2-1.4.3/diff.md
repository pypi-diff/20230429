# Comparing `tmp/mitm-1.4.2.tar.gz` & `tmp/mitm-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitm-1.4.2.tar", last modified: Fri Nov 25 20:30:28 2022, max compression
+gzip compressed data, was "mitm-1.4.3.tar", last modified: Sat Apr 29 16:11:24 2023, max compression
```

## Comparing `mitm-1.4.2.tar` & `mitm-1.4.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:28.030398 mitm-1.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:28.026398 mitm-1.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:28.026398 mitm-1.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1309 2022-11-25 20:30:14.000000 mitm-1.4.2/.github/workflows/docs-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      650 2022-11-25 20:30:14.000000 mitm-1.4.2/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      905 2022-11-25 20:30:14.000000 mitm-1.4.2/.github/workflows/pytest-cover-run.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      126 2022-11-25 20:30:14.000000 mitm-1.4.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)       56 2022-11-25 20:30:27.000000 mitm-1.4.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)       69 2022-11-25 20:30:27.000000 mitm-1.4.2/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2022-11-25 20:30:14.000000 mitm-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4880 2022-11-25 20:30:28.030398 mitm-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3979 2022-11-25 20:30:14.000000 mitm-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:28.026398 mitm-1.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      731 2022-11-25 20:30:14.000000 mitm-1.4.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      799 2022-11-25 20:30:14.000000 mitm-1.4.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)      159 2022-11-25 20:30:14.000000 mitm-1.4.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:28.026398 mitm-1.4.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     2491 2022-11-25 20:30:14.000000 mitm-1.4.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      305 2022-11-25 20:30:14.000000 mitm-1.4.2/docs/source/contents.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:28.030398 mitm-1.4.2/docs/source/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     6113 2022-11-25 20:30:14.000000 mitm-1.4.2/docs/source/docs/internals.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1686 2022-11-25 20:30:14.000000 mitm-1.4.2/docs/source/docs/trusting-mitm.rst
--rw-r--r--   0 runner    (1001) docker     (122)       26 2022-11-25 20:30:14.000000 mitm-1.4.2/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:28.030398 mitm-1.4.2/docs/source/introduction/
--rw-r--r--   0 runner    (1001) docker     (122)     6169 2022-11-25 20:30:14.000000 mitm-1.4.2/docs/source/introduction/how-mitm-works.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2022-11-25 20:30:14.000000 mitm-1.4.2/docs/source/introduction/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:28.030398 mitm-1.4.2/docs/source/module/
--rw-r--r--   0 runner    (1001) docker     (122)      437 2022-11-25 20:30:14.000000 mitm-1.4.2/docs/source/module/core.rst
--rw-r--r--   0 runner    (1001) docker     (122)      311 2022-11-25 20:30:14.000000 mitm-1.4.2/docs/source/module/crypto.rst
--rw-r--r--   0 runner    (1001) docker     (122)      327 2022-11-25 20:30:14.000000 mitm-1.4.2/docs/source/module/extension.rst
--rw-r--r--   0 runner    (1001) docker     (122)      842 2022-11-25 20:30:14.000000 mitm-1.4.2/docs/source/module/mitm.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:28.030398 mitm-1.4.2/mitm/
--rw-r--r--   0 runner    (1001) docker     (122)      848 2022-11-25 20:30:14.000000 mitm-1.4.2/mitm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11046 2022-11-25 20:30:14.000000 mitm-1.4.2/mitm/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    10113 2022-11-25 20:30:14.000000 mitm-1.4.2/mitm/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:28.030398 mitm-1.4.2/mitm/extension/
--rw-r--r--   0 runner    (1001) docker     (122)      190 2022-11-25 20:30:14.000000 mitm-1.4.2/mitm/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3444 2022-11-25 20:30:14.000000 mitm-1.4.2/mitm/extension/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     6372 2022-11-25 20:30:14.000000 mitm-1.4.2/mitm/extension/protocol.py
--rw-r--r--   0 runner    (1001) docker     (122)     6893 2022-11-25 20:30:14.000000 mitm-1.4.2/mitm/mitm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:28.030398 mitm-1.4.2/mitm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4880 2022-11-25 20:30:27.000000 mitm-1.4.2/mitm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1138 2022-11-25 20:30:27.000000 mitm-1.4.2/mitm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-25 20:30:27.000000 mitm-1.4.2/mitm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-25 20:30:22.000000 mitm-1.4.2/mitm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       47 2022-11-25 20:30:27.000000 mitm-1.4.2/mitm.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (122)      169 2022-11-25 20:30:27.000000 mitm-1.4.2/mitm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2022-11-25 20:30:27.000000 mitm-1.4.2/mitm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       31 2022-11-25 20:30:14.000000 mitm-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       72 2022-11-25 20:30:14.000000 mitm-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      992 2022-11-25 20:30:28.030398 mitm-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-25 20:30:14.000000 mitm-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:28.030398 mitm-1.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:14.000000 mitm-1.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1036 2022-11-25 20:30:14.000000 mitm-1.4.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:28.030398 mitm-1.4.2/tests/extension/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-25 20:30:14.000000 mitm-1.4.2/tests/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2022-11-25 20:30:14.000000 mitm-1.4.2/tests/extension/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     1231 2022-11-25 20:30:14.000000 mitm-1.4.2/tests/extension/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (122)       43 2022-11-25 20:30:14.000000 mitm-1.4.2/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      750 2022-11-25 20:30:14.000000 mitm-1.4.2/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2502 2022-11-25 20:30:14.000000 mitm-1.4.2/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (122)      916 2022-11-25 20:30:14.000000 mitm-1.4.2/tests/test_mitm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.114853 mitm-1.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-29 16:11:09.000000 mitm-1.4.3/.github/workflows/docs-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-29 16:11:09.000000 mitm-1.4.3/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-29 16:11:09.000000 mitm-1.4.3/.github/workflows/pytest-cover-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-29 16:11:09.000000 mitm-1.4.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-29 16:11:24.000000 mitm-1.4.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-29 16:11:24.000000 mitm-1.4.3/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-29 16:11:09.000000 mitm-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-29 16:11:24.118852 mitm-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-29 16:11:09.000000 mitm-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/contents.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/docs/source/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/docs/internals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/docs/trusting-mitm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/docs/source/introduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/introduction/how-mitm-works.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/introduction/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/docs/source/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/module/core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/module/crypto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/module/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/module/mitm.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/mitm/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-29 16:11:09.000000 mitm-1.4.3/mitm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-04-29 16:11:09.000000 mitm-1.4.3/mitm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-29 16:11:09.000000 mitm-1.4.3/mitm/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/mitm/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-29 16:11:09.000000 mitm-1.4.3/mitm/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-29 16:11:09.000000 mitm-1.4.3/mitm/extension/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-29 16:11:09.000000 mitm-1.4.3/mitm/extension/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-04-29 16:11:09.000000 mitm-1.4.3/mitm/mitm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/mitm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-29 16:11:24.000000 mitm-1.4.3/mitm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-29 16:11:24.000000 mitm-1.4.3/mitm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:11:24.000000 mitm-1.4.3/mitm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:11:19.000000 mitm-1.4.3/mitm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 16:11:24.000000 mitm-1.4.3/mitm.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-29 16:11:24.000000 mitm-1.4.3/mitm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 16:11:24.000000 mitm-1.4.3/mitm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 16:11:09.000000 mitm-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-29 16:11:09.000000 mitm-1.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-29 16:11:24.122852 mitm-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-29 16:11:09.000000 mitm-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/tests/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/extension/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/extension/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/test_mitm.py
```

### Comparing `mitm-1.4.2/.github/workflows/docs-publish.yaml` & `mitm-1.4.3/.github/workflows/docs-publish.yaml`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/.github/workflows/pypi-publish.yaml` & `mitm-1.4.3/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/.github/workflows/pytest-cover-run.yaml` & `mitm-1.4.3/.github/workflows/pytest-cover-run.yaml`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/LICENSE` & `mitm-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/PKG-INFO` & `mitm-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitm
-Version: 1.4.2
+Version: 1.4.3
 Summary: Man-in-the-middle proxy with customizable options.
 Home-page: https://github.com/synchronizing/mitm
 Author: Felipe Faria
 Author-email: felipefaria@me.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/synchronizing/mitm/issues
 Project-URL: Documentation, https://synchronizing.github.io/mitm/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mitm Version: 1.4.2 Summary: Man-in-the-middle
+Metadata-Version: 2.1 Name: mitm Version: 1.4.3 Summary: Man-in-the-middle
 proxy with customizable options. Home-page: https://github.com/synchronizing/
 mitm Author: Felipe Faria Author-email: felipefaria@me.com License: MIT
 Project-URL: Bug Tracker, https://github.com/synchronizing/mitm/issues Project-
 URL: Documentation, https://synchronizing.github.io/mitm/ Project-URL: Source
 Code, https://github.com/synchronizing/mitm/tree/master Keywords: mitm
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
```

### Comparing `mitm-1.4.2/README.md` & `mitm-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/docs/Makefile` & `mitm-1.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/docs/make.bat` & `mitm-1.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/docs/source/conf.py` & `mitm-1.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/docs/source/docs/internals.rst` & `mitm-1.4.3/docs/source/docs/internals.rst`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/docs/source/docs/trusting-mitm.rst` & `mitm-1.4.3/docs/source/docs/trusting-mitm.rst`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/docs/source/introduction/how-mitm-works.rst` & `mitm-1.4.3/docs/source/introduction/how-mitm-works.rst`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/docs/source/introduction/quickstart.rst` & `mitm-1.4.3/docs/source/introduction/quickstart.rst`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/docs/source/module/mitm.rst` & `mitm-1.4.3/docs/source/module/mitm.rst`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/mitm/__init__.py` & `mitm-1.4.3/mitm/__init__.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/mitm/core.py` & `mitm-1.4.3/mitm/core.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/mitm/crypto.py` & `mitm-1.4.3/mitm/crypto.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/mitm/extension/middleware.py` & `mitm-1.4.3/mitm/extension/middleware.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/mitm/extension/protocol.py` & `mitm-1.4.3/mitm/extension/protocol.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/mitm/mitm.py` & `mitm-1.4.3/mitm/mitm.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,17 @@
             proto = prtcl
             try:
                 # Attempts to resolve the protocol, and connect to the server.
                 host, port, tls = await proto.resolve(connection=connection, data=data)
                 await proto.connect(connection=connection, host=host, port=port, tls=tls, data=data)
             except InvalidProtocol:  # pragma: no cover
                 proto = None
+            else:
+                # Stop searching for working protocols.
+                break
 
         # Protocol was found, and we connected to a server.
         if proto and connection.server:
 
             # Sets the connection protocol.
             connection.protocol = proto
```

### Comparing `mitm-1.4.2/mitm.egg-info/PKG-INFO` & `mitm-1.4.3/mitm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitm
-Version: 1.4.2
+Version: 1.4.3
 Summary: Man-in-the-middle proxy with customizable options.
 Home-page: https://github.com/synchronizing/mitm
 Author: Felipe Faria
 Author-email: felipefaria@me.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/synchronizing/mitm/issues
 Project-URL: Documentation, https://synchronizing.github.io/mitm/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mitm Version: 1.4.2 Summary: Man-in-the-middle
+Metadata-Version: 2.1 Name: mitm Version: 1.4.3 Summary: Man-in-the-middle
 proxy with customizable options. Home-page: https://github.com/synchronizing/
 mitm Author: Felipe Faria Author-email: felipefaria@me.com License: MIT
 Project-URL: Bug Tracker, https://github.com/synchronizing/mitm/issues Project-
 URL: Documentation, https://synchronizing.github.io/mitm/ Project-URL: Source
 Code, https://github.com/synchronizing/mitm/tree/master Keywords: mitm
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
```

### Comparing `mitm-1.4.2/mitm.egg-info/SOURCES.txt` & `mitm-1.4.3/mitm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/setup.cfg` & `mitm-1.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/tests/conftest.py` & `mitm-1.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/tests/extension/test_middleware.py` & `mitm-1.4.3/tests/extension/test_middleware.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/tests/extension/test_protocol.py` & `mitm-1.4.3/tests/extension/test_protocol.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/tests/test_core.py` & `mitm-1.4.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/tests/test_crypto.py` & `mitm-1.4.3/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.2/tests/test_mitm.py` & `mitm-1.4.3/tests/test_mitm.py`

 * *Files identical despite different names*


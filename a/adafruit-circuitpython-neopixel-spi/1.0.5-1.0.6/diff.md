# Comparing `tmp/adafruit-circuitpython-neopixel-spi-1.0.5.tar.gz` & `tmp/adafruit-circuitpython-neopixel-spi-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-neopixel-spi-1.0.5.tar", last modified: Fri Aug 26 02:21:45 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-neopixel-spi-1.0.6.tar", last modified: Fri Apr 28 23:01:04 2023, max compression
```

## Comparing `adafruit-circuitpython-neopixel-spi-1.0.5.tar` & `adafruit-circuitpython-neopixel-spi-1.0.6.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:45.776004 adafruit-circuitpython-neopixel-spi-1.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:45.768004 adafruit-circuitpython-neopixel-spi-1.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:45.772004 adafruit-circuitpython-neopixel-spi-1.0.5/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:45.772004 adafruit-circuitpython-neopixel-spi-1.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:45.772004 adafruit-circuitpython-neopixel-spi-1.0.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3539 2022-08-26 02:21:45.776004 adafruit-circuitpython-neopixel-spi-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2782 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:45.772004 adafruit-circuitpython-neopixel-spi-1.0.5/adafruit_circuitpython_neopixel_spi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3539 2022-08-26 02:21:45.000000 adafruit-circuitpython-neopixel-spi-1.0.5/adafruit_circuitpython_neopixel_spi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-08-26 02:21:45.000000 adafruit-circuitpython-neopixel-spi-1.0.5/adafruit_circuitpython_neopixel_spi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:21:45.000000 adafruit-circuitpython-neopixel-spi-1.0.5/adafruit_circuitpython_neopixel_spi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-26 02:21:45.000000 adafruit-circuitpython-neopixel-spi-1.0.5/adafruit_circuitpython_neopixel_spi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-26 02:21:45.000000 adafruit-circuitpython-neopixel-spi-1.0.5/adafruit_circuitpython_neopixel_spi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:45.776004 adafruit-circuitpython-neopixel-spi-1.0.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:45.776004 adafruit-circuitpython-neopixel-spi-1.0.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5809 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:45.776004 adafruit-circuitpython-neopixel-spi-1.0.5/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-08-26 02:21:36.000000 adafruit-circuitpython-neopixel-spi-1.0.5/examples/neopixel_spi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4610 2022-08-26 02:21:36.000000 adafruit-circuitpython-neopixel-spi-1.0.5/neopixel_spi.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-08-26 02:21:36.000000 adafruit-circuitpython-neopixel-spi-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-26 02:21:27.000000 adafruit-circuitpython-neopixel-spi-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:21:45.776004 adafruit-circuitpython-neopixel-spi-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.950276 adafruit-circuitpython-neopixel-spi-1.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.950276 adafruit-circuitpython-neopixel-spi-1.0.6/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-28 23:01:04.000000 adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-28 23:01:04.000000 adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:01:04.000000 adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 23:01:04.000000 adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 23:01:04.000000 adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-28 23:00:56.000000 adafruit-circuitpython-neopixel-spi-1.0.6/examples/neopixel_spi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-28 23:00:56.000000 adafruit-circuitpython-neopixel-spi-1.0.6/neopixel_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-28 23:00:56.000000 adafruit-circuitpython-neopixel-spi-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/setup.cfg
```

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-neopixel-spi-1.0.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/.gitignore` & `adafruit-circuitpython-neopixel-spi-1.0.6/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/.pre-commit-config.yaml` & `adafruit-circuitpython-neopixel-spi-1.0.6/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.15.5
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/.pylintrc` & `adafruit-circuitpython-neopixel-spi-1.0.6/.pylintrc`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
```

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-neopixel-spi-1.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/LICENSE` & `adafruit-circuitpython-neopixel-spi-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-neopixel-spi-1.0.6/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/LICENSES/MIT.txt` & `adafruit-circuitpython-neopixel-spi-1.0.6/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/LICENSES/Unlicense.txt` & `adafruit-circuitpython-neopixel-spi-1.0.6/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/PKG-INFO` & `adafruit-circuitpython-neopixel-spi-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neopixel-spi
-Version: 1.0.5
+Version: 1.0.6
 Summary: SPI driven CircuitPython driver for neopixels.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel_SPI
 Keywords: adafruit,blinka,circuitpython,micropython,neopixel_spi,neopixel
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/README.rst` & `adafruit-circuitpython-neopixel-spi-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/adafruit_circuitpython_neopixel_spi.egg-info/PKG-INFO` & `adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neopixel-spi
-Version: 1.0.5
+Version: 1.0.6
 Summary: SPI driven CircuitPython driver for neopixels.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel_SPI
 Keywords: adafruit,blinka,circuitpython,micropython,neopixel_spi,neopixel
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/adafruit_circuitpython_neopixel_spi.egg-info/SOURCES.txt` & `adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 neopixel_spi.py
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_neopixel_spi.egg-info/PKG-INFO
 adafruit_circuitpython_neopixel_spi.egg-info/SOURCES.txt
 adafruit_circuitpython_neopixel_spi.egg-info/dependency_links.txt
 adafruit_circuitpython_neopixel_spi.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/docs/_static/favicon.ico` & `adafruit-circuitpython-neopixel-spi-1.0.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/docs/conf.py` & `adafruit-circuitpython-neopixel-spi-1.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/docs/index.rst` & `adafruit-circuitpython-neopixel-spi-1.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/examples/neopixel_spi_simpletest.py` & `adafruit-circuitpython-neopixel-spi-1.0.6/examples/neopixel_spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/neopixel_spi.py` & `adafruit-circuitpython-neopixel-spi-1.0.6/neopixel_spi.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,31 +21,35 @@
 **Software and Dependencies:**
 
 * Adafruit Blinka:
   https://github.com/adafruit/Adafruit_Blinka
 
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
+try:
+    from typing import Optional, Tuple, Union
 
-import adafruit_pixelbuf
+    from busio import SPI
+except ImportError:
+    pass
 
+import adafruit_pixelbuf
 from adafruit_bus_device.spi_device import SPIDevice
 
-
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel_SPI.git"
 
 # Pixel color order constants
-RGB = "RGB"
+RGB: str = "RGB"
 """Red Green Blue"""
-GRB = "GRB"
+GRB: str = "GRB"
 """Green Red Blue"""
-RGBW = "RGBW"
+RGBW: str = "RGBW"
 """Red Green Blue White"""
-GRBW = "GRBW"
+GRBW: str = "GRBW"
 """Green Red Blue White"""
 
 
 class NeoPixel_SPI(adafruit_pixelbuf.PixelBuf):
     """
     A sequence of neopixels.
 
@@ -53,14 +57,15 @@
     :param int n: The number of neopixels in the chain
     :param int bpp: Bytes per pixel. 3 for RGB and 4 for RGBW pixels.
     :param float brightness: Brightness of the pixels between 0.0 and 1.0 where 1.0 is full
       brightness
     :param bool auto_write: True if the neopixels should immediately change when set. If False,
       ``show`` must be called explicitly.
     :param tuple pixel_order: Set the pixel color channel order. GRBW is set by default.
+      pixel_order may be a string or a tuple of integers with values between 0 and 3.
     :param int frequency: SPI bus frequency. For 800kHz NeoPixels, use 6400000 (default).
       For 400kHz, use 3200000.
     :param float reset_time: Reset low level time in seconds. Default is 80e-6.
     :param byte bit0: Bit pattern to set timing for a NeoPixel 0 bit.
     :param byte bit1: Bit pattern to set timing for a NeoPixel 1 bit.
 
     Example:
@@ -72,27 +77,26 @@
 
         pixels = neopixel_spi.NeoPixel_SPI(board.SPI(), 10)
         pixels.fill(0xff0000)
     """
 
     def __init__(
         self,
-        spi,
-        n,
+        spi: SPI,
+        n: int,
         *,
-        bpp=3,
-        brightness=1.0,
-        auto_write=True,
-        pixel_order=None,
-        frequency=6400000,
-        reset_time=80e-6,
-        bit0=0b11000000,
-        bit1=0b11110000
-    ):
-
+        bpp: int = 3,
+        brightness: float = 1.0,
+        auto_write: bool = True,
+        pixel_order: Optional[Union[str, Tuple[int, ...]]] = None,
+        frequency: int = 6400000,
+        reset_time: float = 80e-6,
+        bit0: int = 0b11000000,
+        bit1: int = 0b11110000
+    ) -> None:
         # configure bpp and pixel_order
         if not pixel_order:
             pixel_order = GRB if bpp == 3 else GRBW
         else:
             bpp = len(pixel_order)
             if isinstance(pixel_order, tuple):
                 order_list = [RGBW[order] for order in pixel_order]
@@ -113,43 +117,43 @@
                 # use nominal
                 freq = frequency
         self._reset = bytes([0] * round(freq * self._trst / 8))
         self._spibuf = bytearray(8 * n * bpp)
 
         # everything else taken care of by base class
         super().__init__(
-            n, brightness=brightness, byteorder=pixel_order, auto_write=auto_write
+            size=n, brightness=brightness, byteorder=pixel_order, auto_write=auto_write
         )
 
-    def deinit(self):
+    def deinit(self) -> None:
         """Blank out the NeoPixels."""
         self.fill(0)
         self.show()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "[" + ", ".join([str(x) for x in self]) + "]"
 
     @property
-    def n(self):
+    def n(self) -> int:
         """
         The number of neopixels in the chain (read-only)
         """
         return len(self)
 
-    def _transmit(self, buffer):
+    def _transmit(self, buffer: bytearray) -> None:
         """Shows the new colors on the pixels themselves if they haven't already
         been autowritten."""
         self._transmogrify(buffer)
         # pylint: disable=no-member
         with self._spi as spi:
             # write out special byte sequence surrounded by RESET
             # leading RESET needed for cases where MOSI rests HI
             spi.write(self._reset + self._spibuf + self._reset)
 
-    def _transmogrify(self, buffer):
+    def _transmogrify(self, buffer: bytearray) -> None:
         """Turn every BIT of buf into a special BYTE pattern."""
         k = 0
         for byte in buffer:
             # MSB first
             for i in range(7, -1, -1):
                 if byte >> i & 0x01:
                     self._spibuf[k] = self._bit1  # A NeoPixel 1 bit
```

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.5/pyproject.toml` & `adafruit-circuitpython-neopixel-spi-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-neopixel-spi"
 description = "SPI driven CircuitPython driver for neopixels."
-version = "1.0.5"
+version = "1.0.6"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel_SPI"}
 keywords = [
     "adafruit",
```


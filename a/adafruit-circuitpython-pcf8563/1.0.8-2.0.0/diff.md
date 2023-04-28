# Comparing `tmp/adafruit-circuitpython-pcf8563-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-pcf8563-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pcf8563-1.0.8.tar", last modified: Fri Aug 26 02:32:43 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-pcf8563-2.0.0.tar", last modified: Fri Apr 28 23:36:27 2023, max compression
```

## Comparing `adafruit-circuitpython-pcf8563-1.0.8.tar` & `adafruit-circuitpython-pcf8563-2.0.0.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:43.589827 adafruit-circuitpython-pcf8563-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:43.585827 adafruit-circuitpython-pcf8563-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:43.589827 adafruit-circuitpython-pcf8563-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:43.589827 adafruit-circuitpython-pcf8563-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:43.589827 adafruit-circuitpython-pcf8563-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    17023 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5610 2022-08-26 02:32:43.589827 adafruit-circuitpython-pcf8563-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4842 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:43.589827 adafruit-circuitpython-pcf8563-1.0.8/adafruit_circuitpython_pcf8563.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5610 2022-08-26 02:32:43.000000 adafruit-circuitpython-pcf8563-1.0.8/adafruit_circuitpython_pcf8563.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-08-26 02:32:43.000000 adafruit-circuitpython-pcf8563-1.0.8/adafruit_circuitpython_pcf8563.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:32:43.000000 adafruit-circuitpython-pcf8563-1.0.8/adafruit_circuitpython_pcf8563.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-26 02:32:43.000000 adafruit-circuitpython-pcf8563-1.0.8/adafruit_circuitpython_pcf8563.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-26 02:32:43.000000 adafruit-circuitpython-pcf8563-1.0.8/adafruit_circuitpython_pcf8563.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3608 2022-08-26 02:32:35.000000 adafruit-circuitpython-pcf8563-1.0.8/adafruit_pcf8563.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/api.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:43.589827 adafruit-circuitpython-pcf8563-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:43.589827 adafruit-circuitpython-pcf8563-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)    10799 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:43.589827 adafruit-circuitpython-pcf8563-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1801 2022-08-26 02:32:35.000000 adafruit-circuitpython-pcf8563-1.0.8/examples/pcf8563_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-08-26 02:32:35.000000 adafruit-circuitpython-pcf8563-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-26 02:32:24.000000 adafruit-circuitpython-pcf8563-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:32:43.589827 adafruit-circuitpython-pcf8563-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.639472 adafruit-circuitpython-pcf8563-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.639472 adafruit-circuitpython-pcf8563-2.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.639472 adafruit-circuitpython-pcf8563-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17023 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-28 23:36:27.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-28 23:36:27.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:36:27.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 23:36:27.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 23:36:27.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/adafruit_pcf8563/
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-28 23:36:19.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_pcf8563/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-04-28 23:36:19.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_pcf8563/pcf8563.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-28 23:36:19.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_pcf8563/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/api.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-28 23:36:19.000000 adafruit-circuitpython-pcf8563-2.0.0/examples/pcf8563_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-28 23:36:19.000000 adafruit-circuitpython-pcf8563-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/setup.cfg
```

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pcf8563-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/.gitignore` & `adafruit-circuitpython-pcf8563-2.0.0/.gitignore`

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

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-pcf8563-2.0.0/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/.pylintrc` & `adafruit-circuitpython-pcf8563-2.0.0/.pylintrc`

 * *Files 24% similar despite different names*

```diff
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
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,pointless-string-statement,unspecified-encoding
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

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pcf8563-2.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/LICENSE` & `adafruit-circuitpython-pcf8563-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pcf8563-2.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-pcf8563-2.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pcf8563-2.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/PKG-INFO` & `adafruit-circuitpython-pcf8563-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pcf8563
-Version: 1.0.8
+Version: 2.0.0
 Summary: CircuitPython library for PCF8563 real time clock.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_PCF8563
 Keywords: adafruit,pcf8563,real,time,clock,rtc,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -89,15 +89,15 @@
 ------
 
 Of course, you must import the library to use it:
 
 .. code:: python
 
     import busio
-    import adafruit_pcf8563
+    from adafruit_pcf8563.pcf8563 import PCF8563
     import time
 
 All the Adafruit RTC libraries take an instantiated and active I2C object
 (from the `busio` library) as an argument to their constructor. The way to
 create an I2C object depends on the board you are using. For boards with labeled
 SCL and SDA pins, you can:
 
@@ -112,15 +112,15 @@
     i2c_bus = board.I2C()
 
 Once you have created the I2C interface object, you can use it to instantiate
 the RTC object:
 
 .. code:: python
 
-    rtc = adafruit_pcf8563.PCF8563(i2c_bus)
+    rtc = PCF8563(i2c_bus)
 
 Date and time
 -------------
 
 To set the time, you need to set ``datetime`` to a `time.struct_time` object:
 
 .. code:: python
```

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/README.rst` & `adafruit-circuitpython-pcf8563-2.0.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 ------
 
 Of course, you must import the library to use it:
 
 .. code:: python
 
     import busio
-    import adafruit_pcf8563
+    from adafruit_pcf8563.pcf8563 import PCF8563
     import time
 
 All the Adafruit RTC libraries take an instantiated and active I2C object
 (from the `busio` library) as an argument to their constructor. The way to
 create an I2C object depends on the board you are using. For boards with labeled
 SCL and SDA pins, you can:
 
@@ -94,15 +94,15 @@
     i2c_bus = board.I2C()
 
 Once you have created the I2C interface object, you can use it to instantiate
 the RTC object:
 
 .. code:: python
 
-    rtc = adafruit_pcf8563.PCF8563(i2c_bus)
+    rtc = PCF8563(i2c_bus)
 
 Date and time
 -------------
 
 To set the time, you need to set ``datetime`` to a `time.struct_time` object:
 
 .. code:: python
```

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/adafruit_circuitpython_pcf8563.egg-info/PKG-INFO` & `adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pcf8563
-Version: 1.0.8
+Version: 2.0.0
 Summary: CircuitPython library for PCF8563 real time clock.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_PCF8563
 Keywords: adafruit,pcf8563,real,time,clock,rtc,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -89,15 +89,15 @@
 ------
 
 Of course, you must import the library to use it:
 
 .. code:: python
 
     import busio
-    import adafruit_pcf8563
+    from adafruit_pcf8563.pcf8563 import PCF8563
     import time
 
 All the Adafruit RTC libraries take an instantiated and active I2C object
 (from the `busio` library) as an argument to their constructor. The way to
 create an I2C object depends on the board you are using. For boards with labeled
 SCL and SDA pins, you can:
 
@@ -112,15 +112,15 @@
     i2c_bus = board.I2C()
 
 Once you have created the I2C interface object, you can use it to instantiate
 the RTC object:
 
 .. code:: python
 
-    rtc = adafruit_pcf8563.PCF8563(i2c_bus)
+    rtc = PCF8563(i2c_bus)
 
 Date and time
 -------------
 
 To set the time, you need to set ``datetime`` to a `time.struct_time` object:
 
 .. code:: python
```

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/adafruit_circuitpython_pcf8563.egg-info/SOURCES.txt` & `adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
-adafruit_pcf8563.py
 api.rst.license
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
 adafruit_circuitpython_pcf8563.egg-info/PKG-INFO
 adafruit_circuitpython_pcf8563.egg-info/SOURCES.txt
 adafruit_circuitpython_pcf8563.egg-info/dependency_links.txt
 adafruit_circuitpython_pcf8563.egg-info/requires.txt
 adafruit_circuitpython_pcf8563.egg-info/top_level.txt
+adafruit_pcf8563/clock.py
+adafruit_pcf8563/pcf8563.py
+adafruit_pcf8563/timer.py
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
```

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/adafruit_pcf8563.py` & `adafruit-circuitpython-pcf8563-2.0.0/adafruit_pcf8563/pcf8563.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2016 Philip R. Moyer and Radomir Dopieralski for Adafruit Industries.
 # SPDX-FileCopyrightText: Copyright (c) 2021 Jeff Epler for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 """
-`adafruit_pcf8563` - PCF8563 Real Time Clock module
+`pcf8563` - PCF8563 Real Time Clock module
 ====================================================
 
 This library supports the use of the PCF8563-based RTC in CircuitPython. It
 contains a base RTC class used by all Adafruit RTC libraries. This base
 class is inherited by the chip-specific subclasses.
 
 Functions are included for reading and writing registers and manipulating
@@ -31,19 +31,21 @@
 * Adafruit CircuitPython firmware: https://github.com/adafruit/circuitpython/releases
 * Adafruit's Register library: https://github.com/adafruit/Adafruit_CircuitPython_Register
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 
 **Notes:**
 
 #. Milliseconds are not supported by this RTC.
+#. The alarm does not support seconds. It will always fire on full minutes.
+#. This RTC has a single timer. The class Timer implements the interface to timer-specfic registers.
+#. The class Clock implements the configuration of the clkout-pin.
 #. Datasheet: http://cache.nxp.com/documents/data_sheet/PCF8563.pdf
-
 """
 
-__version__ = "1.0.8"
+__version__ = "2.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PCF8563.git"
 
 import time
 
 from adafruit_bus_device.i2c_device import I2CDevice
 from adafruit_register import i2c_bit
 from adafruit_register import i2c_bcd_alarm
@@ -71,38 +73,40 @@
     """Current date and time."""
 
     # The False means that day and weekday share a register. The 0 is that the
     # first day of the week is value 0 and not 1.
     alarm = i2c_bcd_alarm.BCDAlarmTimeRegister(
         0x09, has_seconds=False, weekday_shared=False, weekday_start=0
     )
-    """Alarm time for the alarm."""
+    """Alarm time for the alarm. Note that the value of the seconds-fields
+    is ignored, i.e. alarms only fire at full minutes. For short-term
+    alarms, use a timer instead."""
 
     alarm_interrupt = i2c_bit.RWBit(0x01, 1)
     """True if the interrupt pin will output when alarm is alarming."""
 
     alarm_status = i2c_bit.RWBit(0x01, 3)
     """True if alarm is alarming. Set to False to reset."""
 
+    clockout_enabled = i2c_bit.RWBit(0x0D, 7)
+    """True if clockout is enabled (default). To disable clockout, set to False"""
+
     def __init__(self, i2c_bus: I2C) -> None:
         time.sleep(0.05)
         self.i2c_device = I2CDevice(i2c_bus, 0x51)
 
-        # Try and verify this is the RTC we expect by checking the timer B
-        # frequency control bits which are 1 on reset and shouldn't ever be
-        # changed.
-        buf = bytearray(2)
-        buf[0] = 0x12
-        with self.i2c_device as i2c:
-            i2c.write_then_readinto(buf, buf, out_end=1, in_start=1)
-
     @property
     def datetime(self) -> time.struct_time:
         """Gets the current date and time or sets the current date and time then starts the
         clock."""
         return self.datetime_register
 
     @datetime.setter
     def datetime(self, value: time.struct_time) -> None:
         # Automatically sets lost_power to false.
         self.datetime_register = value
         self.datetime_compromised = False
+
+    @property
+    def lost_power(self) -> bool:
+        """Compatibility property for PCF8523-lib"""
+        return self.datetime_compromised
```

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-pcf8563-2.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/docs/conf.py` & `adafruit-circuitpython-pcf8563-2.0.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = ["sphinx.ext.autodoc", "sphinx.ext.todo", "sphinx.ext.intersphinx"]
 
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
-# autodoc_mock_imports = ["adafruit_bus_device", "adafruit_register"]
+autodoc_mock_imports = ["adafruit_bus_device", "adafruit_register"]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
```

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/docs/index.rst` & `adafruit-circuitpython-pcf8563-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/examples/pcf8563_simpletest.py` & `adafruit-circuitpython-pcf8563-2.0.0/examples/pcf8563_simpletest.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 # print the current date and time every second.  Notice also comments to adjust
 # for working with hardware vs. software I2C.
 
 import time
 import board
 import busio
 
-import adafruit_pcf8563
+from adafruit_pcf8563.pcf8563 import PCF8563
 
 # Change to the appropriate I2C clock & data pins here!
 i2c_bus = busio.I2C(board.SCL, board.SDA)
 
 # Create the RTC instance:
-rtc = adafruit_pcf8563.PCF8563(i2c_bus)
+rtc = PCF8563(i2c_bus)
 
 # Lookup table for names of days (nicer printing).
 days = ("Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday")
 
 
 # pylint: disable-msg=using-constant-test
 if False:  # change to True if you want to set the time!
```

### Comparing `adafruit-circuitpython-pcf8563-1.0.8/pyproject.toml` & `adafruit-circuitpython-pcf8563-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-pcf8563"
 description = "CircuitPython library for PCF8563 real time clock."
-version = "1.0.8"
+version = "2.0.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_PCF8563"}
 keywords = [
     "adafruit",
@@ -38,12 +38,12 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["adafruit_pcf8563"]
+packages = ["adafruit_pcf8563"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 optional-dependencies = {optional = {file = ["optional_requirements.txt"]}}
```


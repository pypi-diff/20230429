# Comparing `tmp/citecheck-0.2.0.tar.gz` & `tmp/citecheck-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citecheck-0.2.0.tar", last modified: Fri Apr 21 10:30:43 2023, max compression
+gzip compressed data, was "citecheck-0.3.0.tar", last modified: Sat Apr 29 10:18:36 2023, max compression
```

## Comparing `citecheck-0.2.0.tar` & `citecheck-0.3.0.tar`

### file list

```diff
@@ -1,72 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-21 10:30:20.000000 citecheck-0.2.0/.env.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-21 10:30:20.000000 citecheck-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-21 10:30:20.000000 citecheck-0.2.0/.github/workflows/build_lint_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-21 10:30:20.000000 citecheck-0.2.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-21 10:30:20.000000 citecheck-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-21 10:30:20.000000 citecheck-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 10:30:20.000000 citecheck-0.2.0/.python-version
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-21 10:30:20.000000 citecheck-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-21 10:30:20.000000 citecheck-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-21 10:30:43.275886 citecheck-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-21 10:30:20.000000 citecheck-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.267886 citecheck-0.2.0/doc/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/doc/source/_static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/source/_static/logo/full_dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/source/_static/logo/full_light.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/source/_static/logo/icon_light.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/doc/source/whatsnew/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/source/whatsnew/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-21 10:30:20.000000 citecheck-0.2.0/doc/source/whatsnew/releasenotes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-21 10:30:20.000000 citecheck-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-21 10:30:20.000000 citecheck-0.2.0/requirements/ci-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-21 10:30:20.000000 citecheck-0.2.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-21 10:30:20.000000 citecheck-0.2.0/requirements.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-21 10:30:20.000000 citecheck-0.2.0/scripts/compile-requirements.sh
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-21 10:30:20.000000 citecheck-0.2.0/scripts/dev-setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:30:43.275886 citecheck-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.267886 citecheck-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.271886 citecheck-0.2.0/src/citecheck/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 10:30:43.000000 citecheck-0.2.0/src/citecheck/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/src/citecheck/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/cite.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/citeas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/cited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/citedmixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/src/citecheck/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/types/citable.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/core/types/citation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/src/citecheck/decorate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/decorate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-21 10:30:20.000000 citecheck-0.2.0/src/citecheck/decorate/check_citations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/src/citecheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-21 10:30:43.000000 citecheck-0.2.0/src/citecheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-21 10:30:43.000000 citecheck-0.2.0/src/citecheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:30:43.000000 citecheck-0.2.0/src/citecheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-21 10:30:43.000000 citecheck-0.2.0/src/citecheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 10:30:43.000000 citecheck-0.2.0/src/citecheck.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/tests/citecheck/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/tests/citecheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/tests/citecheck/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/tests/citecheck/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-21 10:30:20.000000 citecheck-0.2.0/tests/citecheck/core/test_citeas.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-21 10:30:20.000000 citecheck-0.2.0/tests/citecheck/core/test_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:43.275886 citecheck-0.2.0/tests/citecheck/decorate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:30:20.000000 citecheck-0.2.0/tests/citecheck/decorate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-21 10:30:20.000000 citecheck-0.2.0/tests/citecheck/decorate/test_check_citations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.310641 citecheck-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-29 10:18:15.000000 citecheck-0.3.0/.env.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.302641 citecheck-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-29 10:18:15.000000 citecheck-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.302641 citecheck-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-29 10:18:15.000000 citecheck-0.3.0/.github/workflows/build_lint_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-29 10:18:15.000000 citecheck-0.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-29 10:18:15.000000 citecheck-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-29 10:18:15.000000 citecheck-0.3.0/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-29 10:18:15.000000 citecheck-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 10:18:15.000000 citecheck-0.3.0/.python-version
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-29 10:18:15.000000 citecheck-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-29 10:18:15.000000 citecheck-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-29 10:18:36.310641 citecheck-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-29 10:18:15.000000 citecheck-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.302641 citecheck-0.3.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-29 10:18:15.000000 citecheck-0.3.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-29 10:18:15.000000 citecheck-0.3.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.302641 citecheck-0.3.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.294641 citecheck-0.3.0/doc/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.302641 citecheck-0.3.0/doc/source/_static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-04-29 10:18:15.000000 citecheck-0.3.0/doc/source/_static/logo/full_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-04-29 10:18:15.000000 citecheck-0.3.0/doc/source/_static/logo/full_light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-29 10:18:15.000000 citecheck-0.3.0/doc/source/_static/logo/icon_light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-29 10:18:15.000000 citecheck-0.3.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 10:18:15.000000 citecheck-0.3.0/doc/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.302641 citecheck-0.3.0/doc/source/whatsnew/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-29 10:18:15.000000 citecheck-0.3.0/doc/source/whatsnew/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-29 10:18:15.000000 citecheck-0.3.0/doc/source/whatsnew/releasenotes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-29 10:18:15.000000 citecheck-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.306641 citecheck-0.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-29 10:18:15.000000 citecheck-0.3.0/requirements/ci-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-29 10:18:15.000000 citecheck-0.3.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-29 10:18:15.000000 citecheck-0.3.0/requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.306641 citecheck-0.3.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-29 10:18:15.000000 citecheck-0.3.0/scripts/compile-requirements.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-29 10:18:15.000000 citecheck-0.3.0/scripts/dev-setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 10:18:36.310641 citecheck-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.298641 citecheck-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.306641 citecheck-0.3.0/src/citecheck/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-29 10:18:36.000000 citecheck-0.3.0/src/citecheck/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.306641 citecheck-0.3.0/src/citecheck/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/core/cite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/core/citeas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/core/cited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/core/citedmixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/core/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.306641 citecheck-0.3.0/src/citecheck/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/core/types/citable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/core/types/citation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/core/uncite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.306641 citecheck-0.3.0/src/citecheck/decorate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/decorate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/decorate/citedinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/decorate/citedreturn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-29 10:18:15.000000 citecheck-0.3.0/src/citecheck/decorate/enforcecite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.306641 citecheck-0.3.0/src/citecheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-29 10:18:36.000000 citecheck-0.3.0/src/citecheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-29 10:18:36.000000 citecheck-0.3.0/src/citecheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:18:36.000000 citecheck-0.3.0/src/citecheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-29 10:18:36.000000 citecheck-0.3.0/src/citecheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 10:18:36.000000 citecheck-0.3.0/src/citecheck.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.310641 citecheck-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:15.000000 citecheck-0.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.310641 citecheck-0.3.0/tests/citecheck/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:15.000000 citecheck-0.3.0/tests/citecheck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.310641 citecheck-0.3.0/tests/citecheck/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:15.000000 citecheck-0.3.0/tests/citecheck/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-29 10:18:15.000000 citecheck-0.3.0/tests/citecheck/core/test_citeas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-29 10:18:15.000000 citecheck-0.3.0/tests/citecheck/core/test_cited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-29 10:18:15.000000 citecheck-0.3.0/tests/citecheck/core/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-29 10:18:15.000000 citecheck-0.3.0/tests/citecheck/core/test_uncite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:36.310641 citecheck-0.3.0/tests/citecheck/decorate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:18:15.000000 citecheck-0.3.0/tests/citecheck/decorate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-29 10:18:15.000000 citecheck-0.3.0/tests/citecheck/decorate/test_check_citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-29 10:18:15.000000 citecheck-0.3.0/tests/citecheck/decorate/test_enforcecite.py
```

### Comparing `citecheck-0.2.0/.github/workflows/build_lint_test.yml` & `citecheck-0.3.0/.github/workflows/build_lint_test.yml`

 * *Files identical despite different names*

### Comparing `citecheck-0.2.0/.github/workflows/pypi-publish.yml` & `citecheck-0.3.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `citecheck-0.2.0/.gitignore` & `citecheck-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `citecheck-0.2.0/.pre-commit-config.yaml` & `citecheck-0.3.0/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -40,31 +40,36 @@
     rev: v4.4.0
     hooks:
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.262
+    rev: v0.0.263
     hooks:
       - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.2.0
     hooks:
-    -   id: mypy
+      - id: mypy
         args: ["."]
         pass_filenames: false
 
   - repo: https://github.com/pycqa/pylint
     rev: v3.0.0a6
     hooks:
       - id: pylint
         args: ["--disable", "fixme"]
 
+  - repo: https://github.com/igorshubovych/markdownlint-cli
+    rev: v0.33.0
+    hooks:
+      - id: markdownlint
+
   - repo: local
     hooks:
       - id: setuptools_scm
         name: setuptools_scm
         entry: python -m setuptools_scm -c
         additional_dependencies: [setuptools_scm]
         language: python
```

### Comparing `citecheck-0.2.0/LICENSE.txt` & `citecheck-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `citecheck-0.2.0/PKG-INFO` & `citecheck-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: citecheck
-Version: 0.2.0
+Version: 0.3.0
 Summary: Run-time protection of citation chains
 Author-email: Nathan McDougall <nathan.j.mcdougall@gmail.com>
 License: BSD-3-Clause
 Project-URL: Docs: User Guide, https://citecheck.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/nathanjmcdougall/citecheck
 Project-URL: homepage, https://github.com/nathanjmcdougall/citecheck
 Project-URL: What's New, https://citecheck.readthedocs.io/en/latest/whatsnew/releasenotes.html
 Project-URL: Bug Tracker, https://github.com/nathanjmcdougall/citecheck/issues
+Keywords: citations,cite,bibliography,annotations,references,bibtex,research,academic,methodology,equations
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -32,70 +33,79 @@
 Provides-Extra: doc
 Provides-Extra: dev
 Provides-Extra: check
 Provides-Extra: test
 Provides-Extra: notebook
 License-File: LICENSE.txt
 
-<div align="center">
+<h1 align="center">
   <img src="doc/source/_static/logo/full_dark.svg#gh-dark-mode-only"><br>
   <img src="doc/source/_static/logo/full_light.svg#gh-light-mode-only"><br>
-</div>
+</h1>
 
 # citecheck: like typechecks, but for citations 📖⛓️
 
 <!-- badges: start -->
 [![License](https://img.shields.io/github/license/nathanjmcdougall/citecheck)](https://github.com/nathanjmcdougall/citecheck/blob/main/LICENSE.txt)
 [![PyPI version](https://badge.fury.io/py/citecheck.svg)](https://badge.fury.io/py/citecheck)
 [![Documentation Status](https://readthedocs.org/projects/citecheck/badge/?version=latest)](https://citecheck.readthedocs.io/en/latest/?badge=latest)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Linting: Ruff](https://img.shields.io/badge/linting-ruff-yellowgreen)](https://github.com/charliermarsh/ruff)
 [![Linting: Pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/nathanjmcdougall/citecheck/main.svg)](https://results.pre-commit.ci/latest/github/nathanjmcdougall/citecheck/main)
 [![codecov](https://codecov.io/gh/nathanjmcdougall/citecheck/branch/develop/graph/badge.svg?token=OUHWT2NL8O)](https://codecov.io/gh/nathanjmcdougall/citecheck)
-<!-- [![Downloads](https://static.pepy.tech/badge/citecheck)](https://pepy.tech/project/citecheck) -->
+[![Downloads](https://static.pepy.tech/badge/citecheck)](https://pepy.tech/project/citecheck)
 <!-- badges: end -->
 
 ## Quick example
+
 Consider this example (all authors and quantities are fictitious):
 
 - Doe (2021) published a method for estimating $V_t$ as a function of $q_p$ and $t$.
-- Bloggs (2023) published a method for estimating $R_m$ as a function of $V_t$ and $\rho$, with the explicit requirement that $V_t$ be estimated using the method of Doe (2021) in particular.
+- Bloggs (2023) published a method for estimating $R_m$ as a function of $V_t$ and
+  $\rho$, with the explicit requirement that $V_t$ be estimated using the method of
+  Doe (2021) in particular.
 
 The goal for citecheck is that you could implement this as follows:
+
 ```Python
+from citecheck import enforcecite, Cite
+
 @enforcecite
 def calc_vt_doe2021(
   qt: float,
   t: float
 ) -> Annotated[float, Cite("doe2021")]:
     ...
 
 @enforcecite
 def calc_rm_bloggs2023(
-  vt: CiteAs[float, "doe2021"],
+  vt: Annotated[float, Cite("doe2021")],
   rho: float
 ) -> Annotated[float, Cite("bloggs2023")]:
     ...
 ```
 
-Now, if we try to pass a value for $V_t$ that was not estimated using the method of Doe (2021), we would get an error:
+Now, if we try to pass a value for $V_t$ that was not estimated using the method of Doe
+(2021), we would get an error:
 
 ```Python
 calc_rm_bloggs2023(vt=1.0, rho=1.0) # Error
 calc_rm_bloggs2023(vt=calc_vt_doe2021(1.0, 1.0), rho=1.0) # OK
 ```
 
 citecheck is still in development, but this is the general idea.
 
 ## When to use citecheck
 
-You should consider using citecheck when you are implementing functions corresponding to equations or methodologies in multiple papers which refer to one another.
+You should consider using citecheck when you are implementing functions corresponding to
+equations or methodologies in multiple papers which refer to one another.
 
 ## Getting Started with Development
 
-Use Linux, install [`pyenv`](https://github.com/pyenv/pyenv), and then run the setup script:
+Use Linux, install [`pyenv`](https://github.com/pyenv/pyenv), and then run the setup
+script:
 
 ```bash
 source .\scripts\dev-setup.sh
 ```
```

### Comparing `citecheck-0.2.0/README.md` & `citecheck-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,72 @@
-<div align="center">
+<h1 align="center">
   <img src="doc/source/_static/logo/full_dark.svg#gh-dark-mode-only"><br>
   <img src="doc/source/_static/logo/full_light.svg#gh-light-mode-only"><br>
-</div>
+</h1>
 
 # citecheck: like typechecks, but for citations 📖⛓️
 
 <!-- badges: start -->
 [![License](https://img.shields.io/github/license/nathanjmcdougall/citecheck)](https://github.com/nathanjmcdougall/citecheck/blob/main/LICENSE.txt)
 [![PyPI version](https://badge.fury.io/py/citecheck.svg)](https://badge.fury.io/py/citecheck)
 [![Documentation Status](https://readthedocs.org/projects/citecheck/badge/?version=latest)](https://citecheck.readthedocs.io/en/latest/?badge=latest)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Linting: Ruff](https://img.shields.io/badge/linting-ruff-yellowgreen)](https://github.com/charliermarsh/ruff)
 [![Linting: Pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/nathanjmcdougall/citecheck/main.svg)](https://results.pre-commit.ci/latest/github/nathanjmcdougall/citecheck/main)
 [![codecov](https://codecov.io/gh/nathanjmcdougall/citecheck/branch/develop/graph/badge.svg?token=OUHWT2NL8O)](https://codecov.io/gh/nathanjmcdougall/citecheck)
-<!-- [![Downloads](https://static.pepy.tech/badge/citecheck)](https://pepy.tech/project/citecheck) -->
+[![Downloads](https://static.pepy.tech/badge/citecheck)](https://pepy.tech/project/citecheck)
 <!-- badges: end -->
 
 ## Quick example
+
 Consider this example (all authors and quantities are fictitious):
 
 - Doe (2021) published a method for estimating $V_t$ as a function of $q_p$ and $t$.
-- Bloggs (2023) published a method for estimating $R_m$ as a function of $V_t$ and $\rho$, with the explicit requirement that $V_t$ be estimated using the method of Doe (2021) in particular.
+- Bloggs (2023) published a method for estimating $R_m$ as a function of $V_t$ and
+  $\rho$, with the explicit requirement that $V_t$ be estimated using the method of
+  Doe (2021) in particular.
 
 The goal for citecheck is that you could implement this as follows:
+
 ```Python
+from citecheck import enforcecite, Cite
+
 @enforcecite
 def calc_vt_doe2021(
   qt: float,
   t: float
 ) -> Annotated[float, Cite("doe2021")]:
     ...
 
 @enforcecite
 def calc_rm_bloggs2023(
-  vt: CiteAs[float, "doe2021"],
+  vt: Annotated[float, Cite("doe2021")],
   rho: float
 ) -> Annotated[float, Cite("bloggs2023")]:
     ...
 ```
 
-Now, if we try to pass a value for $V_t$ that was not estimated using the method of Doe (2021), we would get an error:
+Now, if we try to pass a value for $V_t$ that was not estimated using the method of Doe
+(2021), we would get an error:
 
 ```Python
 calc_rm_bloggs2023(vt=1.0, rho=1.0) # Error
 calc_rm_bloggs2023(vt=calc_vt_doe2021(1.0, 1.0), rho=1.0) # OK
 ```
 
 citecheck is still in development, but this is the general idea.
 
 ## When to use citecheck
 
-You should consider using citecheck when you are implementing functions corresponding to equations or methodologies in multiple papers which refer to one another.
+You should consider using citecheck when you are implementing functions corresponding to
+equations or methodologies in multiple papers which refer to one another.
 
 ## Getting Started with Development
 
-Use Linux, install [`pyenv`](https://github.com/pyenv/pyenv), and then run the setup script:
+Use Linux, install [`pyenv`](https://github.com/pyenv/pyenv), and then run the setup
+script:
 
 ```bash
 source .\scripts\dev-setup.sh
 ```
```

### Comparing `citecheck-0.2.0/doc/Makefile` & `citecheck-0.3.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `citecheck-0.2.0/doc/make.bat` & `citecheck-0.3.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `citecheck-0.2.0/doc/source/_static/logo/full_dark.svg` & `citecheck-0.3.0/doc/source/_static/logo/full_dark.svg`

 * *Files identical despite different names*

### Comparing `citecheck-0.2.0/doc/source/_static/logo/full_light.svg` & `citecheck-0.3.0/doc/source/_static/logo/full_light.svg`

 * *Files identical despite different names*

### Comparing `citecheck-0.2.0/doc/source/_static/logo/icon_light.svg` & `citecheck-0.3.0/doc/source/_static/logo/icon_light.svg`

 * *Files identical despite different names*

### Comparing `citecheck-0.2.0/doc/source/conf.py` & `citecheck-0.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `citecheck-0.2.0/doc/source/whatsnew/releasenotes.rst` & `citecheck-0.3.0/doc/source/whatsnew/releasenotes.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,69 @@
+v0.3.0 (2023-04-29)
+===================
+
+Features
+--------
+
+- An ``uncite`` function has been added to remove citations from cited objects, restoring
+  them to their original type. (#11)
+- The ``check_citations`` (now named ``citedinput``) decorator now automatically uncites
+  all inputs to the functions it decorates. (#13)
+- The ``enforcecite`` decorator has been implemented (as showcased in the README),
+  combining the ``citedinput`` decorator with the new ``citedreturn`` decorator,
+  which adds a citation to the return of the decorated function. (#54, #111)
+
+
+Bugfixes
+--------
+
+- The ``check_citations`` previously raised a warning as an error when ``warn=True``,
+  rather than using ``warnings.warn``. This has been fixed. (#125)
+
+
+Improved Documentation
+----------------------
+
+- More detailed docstrings have been added to the core classes. (#6)
+- Keywords have been added to pyproject.toml for PyPI metadata. (#90)
+- The simple example in the README had an outdated syntax using ``CiteAs`` rather than
+  ``typing.Annotated``. This has been corrected. (#103)
+- A badge showing the PyPI downloads count has been restored to the README. (#106)
+- The changelog entry for v0.2.0 had a typo of "pakcage". This has been corrected. (#114)
+
+
+Deprecations and Removals
+-------------------------
+
+- Using the ``CiteAs`` class's item-getting function i.e. ``CiteAs[..., ...]`` is no
+  longer allowed. For now ``_get_cited_class`` can be used instead.
+
+
+Renamings and Relocations
+-------------------------
+
+- The ``check_citations`` decorator has been renamed to ``citedinput``. (#126)
+
+
+Improved Test Suite
+-------------------
+
+- A few tests were incorrectly typed, using ``int`` values in place of ``float``. This
+  has been fixed.
+
+
+Development Configuration Changes
+---------------------------------
+
+- A linter (markdownlint) for Markdown files has been added as a pre-commit, and the
+  README is now compliant with it. (#104)
+- isort was previously removed in favour of ruff, however ruff had not been properly
+  configured to use its isort rules. This has been rectified. (#119)
+
+
 0.2.0 (2023-04-21)
 ==================
 
 Features
 --------
 
 - Mypy has been added to the project for static type checking, in strict mode.
@@ -19,15 +81,15 @@
 - Most parts of the core functionality have now been implemented, but also changed
   significantly; especially ``CiteAs`` and its dependents.
 
 
 Improved Documentation
 ----------------------
 
-- pyproject.toml has been configured with pakcage metadata for in PyPI. This includes
+- pyproject.toml has been configured with package metadata for in PyPI. This includes
   classifiers, project URLs, and the SPDX license identifier. (#5)
 - Badges in the README have been added and re-ordered. Also, one for the Python version
   used in development has been removed. (#43)
 - The README has been improved to include a logo (dark and light mode adaptive), a
   slogan, a quick example, basic guidance on when to use the package, and explicit
   reference to pyenv usage.
 - The changelog entry for v0.1.2 was incorrectly headered as v0.1.1. This used single
```

### Comparing `citecheck-0.2.0/pyproject.toml` & `citecheck-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,26 @@
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering",
   "Topic :: Software Development :: Documentation",
   "Topic :: Software Development :: Testing",
   "Topic :: Documentation",
   "Typing :: Typed",
 ]
+keywords = [
+  "citations",
+  "cite",
+  "bibliography",
+  "annotations",
+  "references",
+  "bibtex",
+  "research",
+  "academic",
+  "methodology",
+  "equations",
+]
 name = "citecheck"
 description = "Run-time protection of citation chains"
 authors = [
   { name = "Nathan McDougall", email = "nathan.j.mcdougall@gmail.com" },
 ]
 license = { text = "BSD-3-Clause" }
 readme = "README.md"
@@ -47,15 +59,15 @@
 ]
 dev = [
   "pip-tools",
   "setuptools_scm[toml]",
   # These three need to be synced with the versions in .pre-commit-config.yaml
   "black==23.3.0",
   "pylint==3.0.0a6",
-  "ruff==0.0.262",
+  "ruff==0.0.263",
   # ^^^
 ]
 check = [
   "pre-commit",
   "mypy==1.2.0", # Sync with the version in .pre-commit-config.yaml
 ]
 test = ["pytest", "coverage[toml]", "pytest-cov"]
@@ -118,14 +130,56 @@
 [[tool.towncrier.type]]
 directory = "config"
 name = "Development Configuration Changes"
 showcontent = true
 
 [tool.ruff]
 src = ["src"]
+select = [
+  # "A",
+  # "ANN",
+  # "ARG",
+  # "B",
+  # "BLE",
+  # "C90",
+  # "COM",
+  # "D",
+  # "DTZ",
+  "E",
+  # "EM",
+  # "ERA",
+  # "EXE",
+  "F",
+  # "FBT",
+  # "G",
+  "I",
+  # "ICN",
+  # "INP",
+  # "ISC",
+  # "N",
+  # "PD",
+  # "PGH",
+  # "PIE",
+  # "PL",
+  # "PT",
+  # "PTH",
+  # "Q",
+  # "RET",
+  # "RUF",
+  # "S",
+  # "SIM",
+  # "T10",
+  # "T20",
+  # "TCH",
+  # "TID",
+  # "TRY",
+  # "UP",
+  # "W",
+  # "YTT",
+]
 ignore = [
   "F403", # We often use * imports in __init__.py files, and other uses will be checked by pylint
 ]
 line-length = 88 # Sync with pylint
 target-version = "py311"
 
 [tool.pylint.messages_control]
@@ -153,18 +207,14 @@
 [tool.pytest]
 console_output_style = ['progress']
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 testpaths = ["tests"]
 
-[tool.isort]
-profile = "black"
-src_paths = ["src", "tests"]
-
 [tool.coverage.report]
 ignore_errors = true
 show_missing = true
 exclude_lines = [
   # Don't complain if tests don't hit defensive assertion code:
   "raise AssertionError",
   "raise NotImplementedError",
```

### Comparing `citecheck-0.2.0/requirements/ci-requirements.txt` & `citecheck-0.3.0/requirements/ci-requirements.txt`

 * *Files identical despite different names*

### Comparing `citecheck-0.2.0/requirements/requirements.txt` & `citecheck-0.3.0/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `citecheck-0.2.0/src/citecheck/core/citeas.py` & `citecheck-0.3.0/src/citecheck/core/citeas.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-"""Checking a citation of a citable object, or turning it into one"""
+"""A class for adding citation attributes to citable objects."""
 
 from citecheck.core.cited import _CitedT, _get_cited_class
-from citecheck.core.citedmixin import _CitedMixin
+from citecheck.core.citedmixin import _CitedMixinT
 from citecheck.core.types.citable import _CitableT
-from citecheck.core.types.citation import Citation, _CitationT
+from citecheck.core.types.citation import Citation
 
 
 class _CiteAsMeta(type):
     def __call__(
         cls, value: _CitableT, citation: Citation
-    ) -> _CitedT[_CitedMixin, _CitableT]:
+    ) -> _CitedT[_CitedMixinT, _CitableT]:
         citable_type = type(value)
         _cited_class = _get_cited_class(citable_type, citation)
         return _cited_class(value)
 
-    def __getitem__(
-        cls, item: tuple[type[_CitableT], _CitationT]
-    ) -> type[_CitedT[_CitedMixin, _CitableT]]:
-        citable_type, citation = item
-        return _get_cited_class(citable_type, citation)
-
 
 class CiteAs(metaclass=_CiteAsMeta):
-    """Checking a citation of a citable object, or turning it into one"""
+    """A class for adding citation attributes to citable objects.
+
+    Usage is `CiteAs(value, citation)`.
+    """
```

### Comparing `citecheck-0.2.0/src/citecheck/core/cited.py` & `citecheck-0.3.0/src/citecheck/core/citedmixin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,59 @@
-"""A dynamically-created type for objects cited with a citation."""
+"""A type for objects cited with a citation."""
 from functools import cache
-from typing import Any, Generic
+from typing import ClassVar, Protocol, TypeVar, runtime_checkable
 
-from citecheck.core.citedmixin import _CitedMixin, _CitedMixinT, _get_cited_mixin
-from citecheck.core.types.citable import _Citable, _CitableT
+from citecheck.core.types.citable import _Citable
 from citecheck.core.types.citation import Citation
 
+_T = TypeVar("_T", bound="_CitedMixin")
 
-class _CitedT(_CitedMixin, _Citable, Generic[_CitedMixinT, _CitableT]):
-    pass
+
+@runtime_checkable
+class _CitedMixin(Protocol):
+    _citation: ClassVar[Citation]
+
+    def __new__(cls: type[_T], value: _Citable) -> _T:
+        ...
+
+    def __hash__(self) -> int:
+        ...
+
+
+_CitedMixinT = TypeVar("_CitedMixinT", bound=_CitedMixin)
 
 
 @cache
-def _get_cited_class(
-    citable_type: type[_CitableT],
-    citation: Citation,
-) -> type[_CitedT[_CitedMixin, _CitableT]]:
-    # There seems to be a bug in mypy:
-    # https://github.com/python/mypy/issues/14458
-    # For now, we need to use Any with --allow-subclassing-any.
-    cited_mixin: Any = _get_cited_mixin(citation)
-    _citable_type: Any = citable_type
-
-    if not isinstance(citable_type, type):
-        raise TypeError(f"{citable_type} must be a type")
-
-    class _Cited(cited_mixin, _citable_type, metaclass=type):
-        def __repr__(self) -> str:
-            return f"{super().__repr__()} (cited as {self._citation})"
+def _get_cited_mixin(citation: Citation) -> type[_CitedMixin]:
+    _S = TypeVar("_S", bound="CitedMixin")
+
+    class CitedMixin:
+        """A Mixin class to add a fixed citation to another class"""
+
+        _citation: ClassVar[Citation] = citation
+
+        def __new__(cls: type[_S], value: _Citable) -> _S:
+            _super: _Citable = super()
+
+            # Clumsy syntax because of a bug in pylint:
+            # https://github.com/pylint-dev/pylint/issues/8554
+            if isinstance(_super, _Citable):
+                pass
+            else:
+                raise TypeError(f"""{_super} must follow the Citable protocol""")
+
+            xprsn = f"{_super}.__new__({cls}, {value})"
+            try:
+                self = _super.__new__(cls, value)
+            except TypeError as err:
+                raise TypeError(
+                    f"""{xprsn} must return a value. Likely, {cls}.__new__ does not
+                    accept exactly one argument.
+                    """
+                ) from err
+
+            if self != value:
+                raise ValueError(f"""{xprsn} must equal {value}""")
 
-        def __hash__(self) -> int:
-            return hash((super().__hash__(), self._citation))
+            return self
 
-    return _Cited
+    return CitedMixin
```

### Comparing `citecheck-0.2.0/src/citecheck/decorate/check_citations.py` & `citecheck-0.3.0/src/citecheck/decorate/citedinput.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,95 @@
 """A decorator to check citations of Cited objects in function annotations."""
 import inspect
-from typing import Annotated, Any, Callable, get_args, get_origin
+import warnings
+from collections.abc import Callable
+from functools import wraps
+from typing import Annotated, Any, get_args, get_origin
 
 from citecheck.core.cite import Cite
+from citecheck.core.cited import _CitedProtocol
 from citecheck.core.citedmixin import _CitedMixin
 from citecheck.core.errors import CitationError, CitationWarning
 from citecheck.core.types.citation import Citation, _CitationT
+from citecheck.core.uncite import uncite
 
 
 def _eq_compare(citation1: _CitationT, citation2: _CitationT) -> bool:
     return citation1 == citation2
 
 
 def _get_compare_func(
-    compare_func: Callable[[Citation, Citation], bool] | None
+    compare_func: Callable[[Citation, Citation], bool] | None,
 ) -> Callable[[Citation, Citation], bool]:
     if compare_func is None:
         return _eq_compare
     return compare_func
 
 
-def check_citations(
+def citedinput(
     warn: bool = False,
     compare_func: Callable[[Citation, Citation], bool] | None = None,
 ) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
     """A decorator to check citations of Cited objects in function annotations."""
-
     _compare_func = _get_compare_func(compare_func)
 
-    raiser = CitationWarning if warn else CitationError
-
     def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
         # Get the function signature
         sig = inspect.signature(func)
 
         # Get the function annotations
         anns = func.__annotations__
 
+        @wraps(func)
         def wrapper(*args: Any, **kwargs: Any) -> Any:
-            # Get the function arguments
-            bound_args = sig.bind(*args, **kwargs)
-
             # Iterate over the function arguments
-            for arg_name, arg_value in bound_args.arguments.items():
-                # Check if the argument is cited
-                if isinstance(arg_value, _CitedMixin):
-                    # Check if the argument is annotated
-                    if arg_name in anns:
-                        ann = anns[arg_name]
-
-                        # Check if the annotation is typing.Annotated
-                        if get_origin(ann) is Annotated:
-                            # Get the annotation arguments which are Cite type
-                            ann_args = [
-                                arg for arg in get_args(ann) if isinstance(arg, Cite)
-                            ]
-
-                            # Iterate over the annotation arguments
-                            any_match = False
-                            for ann_arg in ann_args:
-                                # pylint: disable=protected-access
-                                citation = arg_value._citation
-                                # pylint: enable=protected-access
-
-                                match = _compare_func(citation, ann_arg.citation)
-                                any_match = any_match or match
-
-                            # Check if the citation matches
-                            if not any_match:
-                                annotated_citations = [arg.citation for arg in ann_args]
-                                raise raiser(
-                                    f"Function {func.__name__} was called with "
-                                    f"an argument {arg_name} which has a "
-                                    f"citation {citation} which "
-                                    f"does not match any of the annotated citations "
-                                    f"{annotated_citations}"
-                                )
+            for arg_name, arg_value in sig.bind(*args, **kwargs).arguments.items():
+                # Check if the argument is cited and annotated
+                if isinstance(arg_value, _CitedMixin) and arg_name in anns:
+                    # Check if the annotation is typing.Annotated
+                    ann = anns[arg_name]
+                    if get_origin(ann) is Annotated:
+                        # Get the annotation arguments which are Cite type
+                        ann_args = [
+                            arg for arg in get_args(ann) if isinstance(arg, Cite)
+                        ]
+
+                        # Iterate over the annotation arguments
+                        # pylint: disable=protected-access
+                        any_match = any(
+                            _compare_func(arg_value._citation, ann_arg.citation)
+                            for ann_arg in ann_args
+                        )
+
+                        # Check if the citation matches
+                        if not any_match:
+                            annotated_citations = [arg.citation for arg in ann_args]
+                            msg = (
+                                f"Function {func.__name__} was called with "
+                                f"an argument {arg_name} which has a "
+                                f"citation {arg_value._citation} which "
+                                f"does not match any of the annotated citations "
+                                f"{annotated_citations}"
+                            )
+                            if warn:
+                                warnings.warn(msg, CitationWarning)
+                            else:
+                                raise CitationError(msg)
+
+                        # pylint: enable=protected-access
+
+            argslist = list(args)
+
+            for idx, arg in enumerate(argslist):
+                if isinstance(arg, _CitedProtocol):
+                    argslist[idx] = uncite(arg)
+
+            for key, value in kwargs.items():
+                if isinstance(value, _CitedProtocol):
+                    kwargs[key] = uncite(value)
 
             # Call the function
-            return func(*args, **kwargs)
+            return func(*argslist, **kwargs)
 
         return wrapper
 
     return decorator
```

### Comparing `citecheck-0.2.0/src/citecheck.egg-info/PKG-INFO` & `citecheck-0.3.0/src/citecheck.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: citecheck
-Version: 0.2.0
+Version: 0.3.0
 Summary: Run-time protection of citation chains
 Author-email: Nathan McDougall <nathan.j.mcdougall@gmail.com>
 License: BSD-3-Clause
 Project-URL: Docs: User Guide, https://citecheck.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/nathanjmcdougall/citecheck
 Project-URL: homepage, https://github.com/nathanjmcdougall/citecheck
 Project-URL: What's New, https://citecheck.readthedocs.io/en/latest/whatsnew/releasenotes.html
 Project-URL: Bug Tracker, https://github.com/nathanjmcdougall/citecheck/issues
+Keywords: citations,cite,bibliography,annotations,references,bibtex,research,academic,methodology,equations
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -32,70 +33,79 @@
 Provides-Extra: doc
 Provides-Extra: dev
 Provides-Extra: check
 Provides-Extra: test
 Provides-Extra: notebook
 License-File: LICENSE.txt
 
-<div align="center">
+<h1 align="center">
   <img src="doc/source/_static/logo/full_dark.svg#gh-dark-mode-only"><br>
   <img src="doc/source/_static/logo/full_light.svg#gh-light-mode-only"><br>
-</div>
+</h1>
 
 # citecheck: like typechecks, but for citations 📖⛓️
 
 <!-- badges: start -->
 [![License](https://img.shields.io/github/license/nathanjmcdougall/citecheck)](https://github.com/nathanjmcdougall/citecheck/blob/main/LICENSE.txt)
 [![PyPI version](https://badge.fury.io/py/citecheck.svg)](https://badge.fury.io/py/citecheck)
 [![Documentation Status](https://readthedocs.org/projects/citecheck/badge/?version=latest)](https://citecheck.readthedocs.io/en/latest/?badge=latest)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Linting: Ruff](https://img.shields.io/badge/linting-ruff-yellowgreen)](https://github.com/charliermarsh/ruff)
 [![Linting: Pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/nathanjmcdougall/citecheck/main.svg)](https://results.pre-commit.ci/latest/github/nathanjmcdougall/citecheck/main)
 [![codecov](https://codecov.io/gh/nathanjmcdougall/citecheck/branch/develop/graph/badge.svg?token=OUHWT2NL8O)](https://codecov.io/gh/nathanjmcdougall/citecheck)
-<!-- [![Downloads](https://static.pepy.tech/badge/citecheck)](https://pepy.tech/project/citecheck) -->
+[![Downloads](https://static.pepy.tech/badge/citecheck)](https://pepy.tech/project/citecheck)
 <!-- badges: end -->
 
 ## Quick example
+
 Consider this example (all authors and quantities are fictitious):
 
 - Doe (2021) published a method for estimating $V_t$ as a function of $q_p$ and $t$.
-- Bloggs (2023) published a method for estimating $R_m$ as a function of $V_t$ and $\rho$, with the explicit requirement that $V_t$ be estimated using the method of Doe (2021) in particular.
+- Bloggs (2023) published a method for estimating $R_m$ as a function of $V_t$ and
+  $\rho$, with the explicit requirement that $V_t$ be estimated using the method of
+  Doe (2021) in particular.
 
 The goal for citecheck is that you could implement this as follows:
+
 ```Python
+from citecheck import enforcecite, Cite
+
 @enforcecite
 def calc_vt_doe2021(
   qt: float,
   t: float
 ) -> Annotated[float, Cite("doe2021")]:
     ...
 
 @enforcecite
 def calc_rm_bloggs2023(
-  vt: CiteAs[float, "doe2021"],
+  vt: Annotated[float, Cite("doe2021")],
   rho: float
 ) -> Annotated[float, Cite("bloggs2023")]:
     ...
 ```
 
-Now, if we try to pass a value for $V_t$ that was not estimated using the method of Doe (2021), we would get an error:
+Now, if we try to pass a value for $V_t$ that was not estimated using the method of Doe
+(2021), we would get an error:
 
 ```Python
 calc_rm_bloggs2023(vt=1.0, rho=1.0) # Error
 calc_rm_bloggs2023(vt=calc_vt_doe2021(1.0, 1.0), rho=1.0) # OK
 ```
 
 citecheck is still in development, but this is the general idea.
 
 ## When to use citecheck
 
-You should consider using citecheck when you are implementing functions corresponding to equations or methodologies in multiple papers which refer to one another.
+You should consider using citecheck when you are implementing functions corresponding to
+equations or methodologies in multiple papers which refer to one another.
 
 ## Getting Started with Development
 
-Use Linux, install [`pyenv`](https://github.com/pyenv/pyenv), and then run the setup script:
+Use Linux, install [`pyenv`](https://github.com/pyenv/pyenv), and then run the setup
+script:
 
 ```bash
 source .\scripts\dev-setup.sh
 ```
```

### Comparing `citecheck-0.2.0/src/citecheck.egg-info/SOURCES.txt` & `citecheck-0.3.0/src/citecheck.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .env.template
 .gitignore
+.markdownlint.yaml
 .pre-commit-config.yaml
 .python-version
 .readthedocs.yaml
 LICENSE.txt
 README.md
 pyproject.toml
 requirements.in
@@ -32,19 +33,25 @@
 src/citecheck.egg-info/top_level.txt
 src/citecheck/core/__init__.py
 src/citecheck/core/cite.py
 src/citecheck/core/citeas.py
 src/citecheck/core/cited.py
 src/citecheck/core/citedmixin.py
 src/citecheck/core/errors.py
+src/citecheck/core/uncite.py
 src/citecheck/core/types/__init__.py
 src/citecheck/core/types/citable.py
 src/citecheck/core/types/citation.py
 src/citecheck/decorate/__init__.py
-src/citecheck/decorate/check_citations.py
+src/citecheck/decorate/citedinput.py
+src/citecheck/decorate/citedreturn.py
+src/citecheck/decorate/enforcecite.py
 tests/__init__.py
 tests/citecheck/__init__.py
 tests/citecheck/core/__init__.py
 tests/citecheck/core/test_citeas.py
+tests/citecheck/core/test_cited.py
 tests/citecheck/core/test_errors.py
+tests/citecheck/core/test_uncite.py
 tests/citecheck/decorate/__init__.py
-tests/citecheck/decorate/test_check_citations.py
+tests/citecheck/decorate/test_check_citations.py
+tests/citecheck/decorate/test_enforcecite.py
```

### Comparing `citecheck-0.2.0/tests/citecheck/core/test_errors.py` & `citecheck-0.3.0/tests/citecheck/core/test_errors.py`

 * *Files identical despite different names*


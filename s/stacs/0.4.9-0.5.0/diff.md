# Comparing `tmp/stacs-0.4.9.tar.gz` & `tmp/stacs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stacs-0.4.9.tar", last modified: Mon Oct  3 23:49:37 2022, max compression
+gzip compressed data, was "stacs-0.5.0.tar", last modified: Sat Apr 29 15:12:35 2023, max compression
```

## Comparing `stacs-0.4.9.tar` & `stacs-0.5.0.tar`

### file list

```diff
@@ -1,52 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 23:49:37.553469 stacs-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-10-03 23:49:23.000000 stacs-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8147 2022-10-03 23:49:37.553469 stacs-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7798 2022-10-03 23:49:23.000000 stacs-0.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-10-03 23:49:37.553469 stacs-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-10-03 23:49:23.000000 stacs-0.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 23:49:37.549469 stacs-0.4.9/stacs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 23:49:37.549469 stacs-0.4.9/stacs/native/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 23:49:37.549469 stacs-0.4.9/stacs/native/archive/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 23:49:37.549469 stacs-0.4.9/stacs/native/archive/src/
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/native/archive/src/archive.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 23:49:37.549469 stacs-0.4.9/stacs/scan/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 23:49:37.553469 stacs-0.4.9/stacs/scan/entrypoint/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/entrypoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5776 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/entrypoint/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 23:49:37.553469 stacs-0.4.9/stacs/scan/filter/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4496 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/filter/ignore_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 23:49:37.553469 stacs-0.4.9/stacs/scan/loader/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13404 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/loader/archive.py
--rw-r--r--   0 runner    (1001) docker     (121)     6313 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/loader/filepath.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 23:49:37.553469 stacs-0.4.9/stacs/scan/loader/format/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/loader/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6041 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/loader/format/xar.py
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/loader/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 23:49:37.553469 stacs-0.4.9/stacs/scan/model/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/model/finding.py
--rw-r--r--   0 runner    (1001) docker     (121)     3536 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/model/ignore_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/model/manifest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2348 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/model/pack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 23:49:37.553469 stacs-0.4.9/stacs/scan/output/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/output/markdown.py
--rw-r--r--   0 runner    (1001) docker     (121)     4088 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/output/pretty.py
--rw-r--r--   0 runner    (1001) docker     (121)     8154 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/output/sarif.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 23:49:37.553469 stacs-0.4.9/stacs/scan/scanner/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7432 2022-10-03 23:49:23.000000 stacs-0.4.9/stacs/scan/scanner/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 23:49:37.549469 stacs-0.4.9/stacs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8147 2022-10-03 23:49:37.000000 stacs-0.4.9/stacs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-10-03 23:49:37.000000 stacs-0.4.9/stacs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 23:49:37.000000 stacs-0.4.9/stacs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-03 23:49:37.000000 stacs-0.4.9/stacs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-10-03 23:49:37.000000 stacs-0.4.9/stacs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-03 23:49:37.000000 stacs-0.4.9/stacs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.401892 stacs-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-29 15:12:20.000000 stacs-0.5.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-29 15:12:20.000000 stacs-0.5.0/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-04-29 15:12:20.000000 stacs-0.5.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-29 15:12:20.000000 stacs-0.5.0/.github/workflows/publish_to_testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-29 15:12:20.000000 stacs-0.5.0/.github/workflows/update.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-29 15:12:20.000000 stacs-0.5.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-29 15:12:20.000000 stacs-0.5.0/.vscode/c_cpp_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-29 15:12:20.000000 stacs-0.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-29 15:12:20.000000 stacs-0.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-29 15:12:20.000000 stacs-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-29 15:12:35.401892 stacs-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-29 15:12:20.000000 stacs-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.389892 stacs-0.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/docs/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31469 2023-04-29 15:12:20.000000 stacs-0.5.0/docs/images/Human-Output-Example.png
+-rw-r--r--   0 runner    (1001) docker     (123)   605164 2023-04-29 15:12:20.000000 stacs-0.5.0/docs/images/SARIF-Viewer-Example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-04-29 15:12:20.000000 stacs-0.5.0/docs/images/STACS-Logo-RGB.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26956 2023-04-29 15:12:20.000000 stacs-0.5.0/docs/images/STACS-Logo-RGB.small.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-29 15:12:20.000000 stacs-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:12:35.401892 stacs-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-29 15:12:20.000000 stacs-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/stacs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.389892 stacs-0.5.0/stacs/native/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.389892 stacs-0.5.0/stacs/native/archive/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/stacs/native/archive/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/native/archive/src/archive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/native/archive/src/archiveentry.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/native/archive/src/archiveentry.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/native/archive/src/archivereader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/native/archive/src/archivereader.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/stacs/scan/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/stacs/scan/entrypoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/entrypoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/entrypoint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/stacs/scan/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/filter/ignore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/stacs/scan/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/loader/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/loader/filepath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/stacs/scan/loader/format/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/loader/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/loader/format/dmg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/loader/format/xar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/loader/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/stacs/scan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/model/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/model/ignore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/model/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/model/pack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/stacs/scan/output/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/output/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/output/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/output/sarif.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/stacs/scan/scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/scanner/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/stacs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-29 15:12:35.000000 stacs-0.5.0/stacs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-29 15:12:35.000000 stacs-0.5.0/stacs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:12:35.000000 stacs-0.5.0/stacs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-29 15:12:35.000000 stacs-0.5.0/stacs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-29 15:12:35.000000 stacs-0.5.0/stacs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 15:12:35.000000 stacs-0.5.0/stacs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/tests/fixtures/findings/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/findings/001.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/findings/002.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/findings/003.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/findings/004.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.401892 stacs-0.5.0/tests/fixtures/ignore_list/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/ignore_list/001-simple.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/ignore_list/002-framework.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/ignore_list/002-project.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/ignore_list/002-system.valid.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.401892 stacs-0.5.0/tests/fixtures/pack/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/pack/001-simple.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/pack/002-cloud.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/pack/002-parent.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/pack/002-pki-dsa.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/pack/002-pki-rsa.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/pack/002-pki.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/test_filter_ignore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/test_loader_filepath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/test_model_ignore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/test_model_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/test_output_sarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/test_scanner_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.401892 stacs-0.5.0/wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-04-29 15:12:20.000000 stacs-0.5.0/wrapper/stacs-scan
```

### Comparing `stacs-0.4.9/LICENSE` & `stacs-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stacs-0.4.9/PKG-INFO` & `stacs-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: stacs
-Version: 0.4.9
+Version: 0.5.0
 Summary: Static Token And Credential Scanner.
-Home-page: https://www.github.com/stacscan/stacs/
+Author: Peter Adkins
+License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: development
+Provides-Extra: tests
 License-File: LICENSE
 
-[![Shield](https://img.shields.io/github/workflow/status/stacscan/stacs/Check?label=Tests&style=flat-square)](https://github.com/stacscan/stacs/actions?workflow=Check)
-[![Shield](https://img.shields.io/github/workflow/status/stacscan/stacs/Publish?label=Deploy&style=flat-square)](https://github.com/stacscan/stacs/actions?workflow=Publish)
+[![Shield](https://img.shields.io/github/actions/workflow/status/stacscan/stacs/check.yml?label=Tests&style=flat-square)](https://github.com/stacscan/stacs/actions?workflow=Check)
+[![Shield](https://img.shields.io/github/actions/workflow/status/stacscan/stacs/publish.yml?label=Deploy&style=flat-square)](https://github.com/stacscan/stacs/actions?workflow=Publish)
 [![Shield](https://img.shields.io/docker/pulls/stacscan/stacs?style=flat-square)](https://hub.docker.com/r/stacscan/stacs)
 [![Shield](https://img.shields.io/docker/image-size/stacscan/stacs?style=flat-square)](https://hub.docker.com/r/stacscan/stacs/tags?page=1&ordering=last_updated)
 [![Shield](https://img.shields.io/twitter/follow/stacscan?style=flat-square)](https://twitter.com/stacscan)
 <p align="center">
     <br /><br />
     <img src="https://raw.githubusercontent.com/stacscan/stacs/main/docs/images/STACS-Logo-RGB.small.png">
 </p>
@@ -31,17 +32,17 @@
 which suports binary file formats, analysis of nested archives, composable rulesets
 and ignore lists, and SARIF reporting.
 
 ### What does STACS support?
 
 Currently, STACS supports recursive unpacking of:
 
-* 7z, ar, bz2, cab, cpio, gz, iso, rar, rpm, tar, xar, xz, zip
+* 7z, ar, bz2, cab, cpio, gz, iso, rar, rpm, tar, xar, xz, zip, dmg
 
-As STACS works on detected file types, propriatary file formats based and other
+As STACS works on detected file types, proprietary file formats based and other
 file-types which use these formats are automatically supported. This includes Docker
 images, Android APKs, Java JAR files, RPMs, Debian packages (`.deb`), macOS packages
 (`.pkg`), and more!
 
 ### Who should use STACS?
 
 STACS is designed for use by any teams who release binary artifacts. STACS provides
```

### Comparing `stacs-0.4.9/README.md` & `stacs-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-[![Shield](https://img.shields.io/github/workflow/status/stacscan/stacs/Check?label=Tests&style=flat-square)](https://github.com/stacscan/stacs/actions?workflow=Check)
-[![Shield](https://img.shields.io/github/workflow/status/stacscan/stacs/Publish?label=Deploy&style=flat-square)](https://github.com/stacscan/stacs/actions?workflow=Publish)
+[![Shield](https://img.shields.io/github/actions/workflow/status/stacscan/stacs/check.yml?label=Tests&style=flat-square)](https://github.com/stacscan/stacs/actions?workflow=Check)
+[![Shield](https://img.shields.io/github/actions/workflow/status/stacscan/stacs/publish.yml?label=Deploy&style=flat-square)](https://github.com/stacscan/stacs/actions?workflow=Publish)
 [![Shield](https://img.shields.io/docker/pulls/stacscan/stacs?style=flat-square)](https://hub.docker.com/r/stacscan/stacs)
 [![Shield](https://img.shields.io/docker/image-size/stacscan/stacs?style=flat-square)](https://hub.docker.com/r/stacscan/stacs/tags?page=1&ordering=last_updated)
 [![Shield](https://img.shields.io/twitter/follow/stacscan?style=flat-square)](https://twitter.com/stacscan)
 <p align="center">
     <br /><br />
     <img src="https://raw.githubusercontent.com/stacscan/stacs/main/docs/images/STACS-Logo-RGB.small.png">
 </p>
@@ -19,17 +19,17 @@
 which suports binary file formats, analysis of nested archives, composable rulesets
 and ignore lists, and SARIF reporting.
 
 ### What does STACS support?
 
 Currently, STACS supports recursive unpacking of:
 
-* 7z, ar, bz2, cab, cpio, gz, iso, rar, rpm, tar, xar, xz, zip
+* 7z, ar, bz2, cab, cpio, gz, iso, rar, rpm, tar, xar, xz, zip, dmg
 
-As STACS works on detected file types, propriatary file formats based and other
+As STACS works on detected file types, proprietary file formats based and other
 file-types which use these formats are automatically supported. This includes Docker
 images, Android APKs, Java JAR files, RPMs, Debian packages (`.deb`), macOS packages
 (`.pkg`), and more!
 
 ### Who should use STACS?
 
 STACS is designed for use by any teams who release binary artifacts. STACS provides
```

### Comparing `stacs-0.4.9/stacs/native/archive/src/archive.cpp` & `stacs-0.5.0/stacs/native/archive/src/archive.cpp`

 * *Files identical despite different names*

### Comparing `stacs-0.4.9/stacs/scan/constants.py` & `stacs-0.5.0/stacs/scan/constants.py`

 * *Files identical despite different names*

### Comparing `stacs-0.4.9/stacs/scan/entrypoint/cli.py` & `stacs-0.5.0/stacs/scan/entrypoint/cli.py`

 * *Files identical despite different names*

### Comparing `stacs-0.4.9/stacs/scan/exceptions.py` & `stacs-0.5.0/stacs/scan/exceptions.py`

 * *Files identical despite different names*

### Comparing `stacs-0.4.9/stacs/scan/filter/ignore_list.py` & `stacs-0.5.0/stacs/scan/filter/ignore_list.py`

 * *Files identical despite different names*

### Comparing `stacs-0.4.9/stacs/scan/helper.py` & `stacs-0.5.0/stacs/scan/helper.py`

 * *Files identical despite different names*

### Comparing `stacs-0.4.9/stacs/scan/loader/archive.py` & `stacs-0.5.0/stacs/scan/loader/archive.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 import hashlib
 import logging
 import lzma
 import os
 import shutil
 import tarfile
 import zipfile
+import zlib
+from typing import List, Tuple
 
 import zstandard
 from stacs.native import archive
 from stacs.scan.constants import CHUNK_SIZE
 from stacs.scan.exceptions import FileAccessException, InvalidFileException
-from stacs.scan.loader.format import xar
+from stacs.scan.loader.format import dmg, xar
 
 
 def path_hash(filepath: str) -> str:
     """Returns a hash of the filepath, for use with unique directory creation."""
     return hashlib.md5(bytes(filepath, "utf-8")).hexdigest()
 
 
@@ -82,17 +84,17 @@
         )
 
 
 def gzip_handler(filepath: str, directory: str) -> None:
     """Attempts to extract the provided gzip archive."""
     output = ".".join(os.path.basename(filepath).split(".")[:-1])
 
-    # Ensure that files with a proceeding dot are properly handled.
+    # No dots? Just use the name as is.
     if len(output) < 1:
-        output = os.path.basename(filepath).lstrip(".")
+        output = os.path.basename(filepath)
 
     # Although gzip files cannot contain more than one file, we'll still spool into
     # a subdirectory under the cache for consistency.
     try:
         os.mkdir(directory, mode=0o700)
     except OSError as err:
         raise FileAccessException(
@@ -111,14 +113,18 @@
         )
 
 
 def bzip2_handler(filepath: str, directory: str) -> None:
     """Attempts to extract the provided bzip2 archive."""
     output = ".".join(os.path.basename(filepath).split(".")[:-1])
 
+    # No dots? Just use the name as is.
+    if len(output) < 1:
+        output = os.path.basename(filepath)
+
     # Like gzip, bzip2 cannot support more than a single file. Again, we'll spool into
     # a subdirectory for consistency.
     try:
         os.mkdir(directory, mode=0o700)
     except OSError as err:
         raise FileAccessException(
             f"Unable to create unpack directory at {directory}: {err}"
@@ -136,14 +142,18 @@
         )
 
 
 def zstd_handler(filepath: str, directory: str) -> None:
     """Attempts to extract the provided zstd archive."""
     output = ".".join(os.path.basename(filepath).split(".")[:-1])
 
+    # No dots? Just use the name as is.
+    if len(output) < 1:
+        output = os.path.basename(filepath)
+
     # zstd does not appear to provide a native mechanism to compress multiple files,
     # and recommend 'to combine zstd with tar'.
     try:
         os.mkdir(directory, mode=0o700)
     except OSError as err:
         raise FileAccessException(
             f"Unable to create unpack directory at {directory}: {err}"
@@ -161,17 +171,17 @@
         )
 
 
 def lzma_handler(filepath: str, directory: str) -> None:
     """Attempts to extract the provided xz / lzma archive."""
     output = ".".join(os.path.basename(filepath).split(".")[:-1])
 
-    # Ensure that files with a proceeding dot are properly handled.
+    # No dots? Just use the name as is.
     if len(output) < 1:
-        output = os.path.basename(filepath).lstrip(".")
+        output = os.path.basename(filepath)
 
     # Although xz files cannot contain more than one file, we'll still spool into
     # a subdirectory under the cache for consistency.
     try:
         os.mkdir(directory, mode=0o700)
     except OSError as err:
         raise FileAccessException(
@@ -184,14 +194,42 @@
                 shutil.copyfileobj(fin, fout, CHUNK_SIZE)
     except lzma.LZMAError as err:
         raise InvalidFileException(
             f"Unable to extract archive {filepath} to {output}: {err}"
         )
 
 
+def zlib_handler(filepath: str, directory: str) -> None:
+    """Attempts to extract the provided zlib archive."""
+    output = ".".join(os.path.basename(filepath).split(".")[:-1])
+
+    # No dots? Just use the name as is.
+    if len(output) < 1:
+        output = os.path.basename(filepath)
+
+    try:
+        os.mkdir(directory, mode=0o700)
+    except OSError as err:
+        raise FileAccessException(
+            f"Unable to create unpack directory at {directory}: {err}"
+        )
+
+    try:
+        decompressor = zlib.decompressobj(wbits=zlib.MAX_WBITS)
+
+        with open(filepath, "rb") as fin:
+            with open(os.path.join(directory, output), "wb") as fout:
+                while compressed := fin.read(CHUNK_SIZE):
+                    fout.write(decompressor.decompress(compressed))
+    except zlib.error as err:
+        raise InvalidFileException(
+            f"Unable to extract archive {filepath} to {output}: {err}"
+        )
+
+
 def xar_handler(filepath: str, directory: str) -> None:
     """Attempts to extract the provided XAR archive."""
     try:
         os.mkdir(directory, mode=0o700)
     except OSError as err:
         raise FileAccessException(
             f"Unable to create unpack directory at {directory}: {err}"
@@ -207,14 +245,37 @@
         )
     except InvalidFileException as err:
         raise InvalidFileException(
             f"Unable to extract archive {filepath} to {directory}: {err}"
         )
 
 
+def dmg_handler(filepath: str, directory: str) -> None:
+    """Attempts to extract the provided DMG archive."""
+    try:
+        os.mkdir(directory, mode=0o700)
+    except OSError as err:
+        raise FileAccessException(
+            f"Unable to create unpack directory at {directory}: {err}"
+        )
+
+    # Attempt to unpack the archive.
+    try:
+        archive = dmg.DMG(filepath)
+        archive.extract(directory)
+    except FileAccessException as err:
+        raise FileAccessException(
+            f"Unable to extract archive {filepath} to {directory}: {err}"
+        )
+    except InvalidFileException as err:
+        raise InvalidFileException(
+            f"Unable to extract archive {filepath} to {directory}: {err}"
+        )
+
+
 def libarchive_handler(filepath: str, directory: str) -> None:
     """Attempts to extract the provided archive with libarchive."""
     try:
         os.mkdir(directory, mode=0o700)
     except OSError as err:
         raise FileAccessException(
             f"Unable to create unpack directory at {directory}: {err}"
@@ -260,136 +321,185 @@
                         break
     except archive.ArchiveError as err:
         raise InvalidFileException(
             f"Unable to extract archive {filepath} to {directory}: {err}"
         )
 
 
-def get_mimetype(chunk: bytes) -> str:
+def get_mimetype(chunk: bytes, start: bool) -> List[Tuple[int, str]]:
     """Attempts to locate the appropriate handler for a given file.
 
     This may fail if the required "magic" is at an offset greater than the CHUNK_SIZE.
     However, currently this is not an issue, but may need to be revisited later as more
     archive types are supported.
+
+    The start flag is used to indicate whether the current chunk is from the start of
+    the file, or the end of the file. Today we only support checking the first and last
+    chunk.
+
+    Returns a list of weights and MIME types as a tuple. This weight is specified by
+    handlers and is used to allow "container" formats, which may contain multiple other
+    files of various matching types, to "win" the match - due to a higher weight.
     """
     for name, options in MIME_TYPE_HANDLERS.items():
         offset = options["offset"]
         magic = options["magic"]
 
-        for candidate in magic:
-            if chunk[offset : (offset + len(candidate))] == candidate:  # noqa: E203
-                return name
+        # If looking at the last chunk, only use negative offsets. This is to prevent
+        # false positives as position 0 in the last chunk is actually N bytes into the
+        # file. This is especially problematic for formats with short magic numbers,
+        # such as zlib.
+        if not start and offset >= 0:
+            continue
+
+        # TODO: How to handle multiple matches in the same chunk? Is this this likely?
+        for format in magic:
+            if chunk[offset : (offset + len(format))] == format:  # noqa: E203
+                return (options["weight"], name)
 
-    return None
+    return (0, None)
 
 
 # Define all supported archives and their handlers. As we currently only support a small
 # list of types we can just define file magic directly here, rather than use an external
 # library. This removes the need for dependencies which may have other system
 # dependencies - such as libmagic. It should also provide a small a speed up during
 # unpacking, as we're only looking for a small number of types.
 MIME_TYPE_HANDLERS = {
     "application/x-tar": {
+        "weight": 1,
         "offset": 257,
         "magic": [
             bytearray([0x75, 0x73, 0x74, 0x61, 0x72]),
         ],
         "handler": tar_handler,
     },
     "application/gzip": {
+        "weight": 1,
         "offset": 0,
         "magic": [
             bytearray([0x1F, 0x8B]),
         ],
         "handler": gzip_handler,
     },
     "application/x-bzip2": {
+        "weight": 1,
         "offset": 0,
         "magic": [
             bytearray([0x42, 0x5A, 0x68]),
         ],
         "handler": bzip2_handler,
     },
     "application/zip": {
+        "weight": 1,
         "offset": 0,
         "magic": [
             bytearray([0x50, 0x4B, 0x03, 0x04]),
             bytearray([0x50, 0x4B, 0x05, 0x06]),
             bytearray([0x50, 0x4B, 0x07, 0x08]),
         ],
         "handler": zip_handler,
     },
+    "application/zlib": {
+        "weight": 1,
+        "offset": 0,
+        "magic": [
+            bytearray([0x78, 0x01]),
+            bytearray([0x78, 0x5E]),
+            bytearray([0x78, 0x9C]),
+            bytearray([0x78, 0xDA]),
+        ],
+        "handler": zlib_handler,
+    },
     "application/x-xz": {
+        "weight": 1,
         "offset": 0,
         "magic": [
             bytearray([0xFD, 0x37, 0x7A, 0x58, 0x5A, 0x00]),
         ],
         "handler": lzma_handler,
     },
     "application/x-rpm": {
+        "weight": 1,
         "offset": 0,
         "magic": [
             bytearray([0xED, 0xAB, 0xEE, 0xDB]),
         ],
         "handler": libarchive_handler,
     },
     "application/x-iso9660-image": {
+        "weight": 1,
         "offset": 0x8001,
         "magic": [
             bytearray([0x43, 0x44, 0x30, 0x30, 0x31]),
         ],
         "handler": libarchive_handler,
     },
     "application/x-7z-compressed": {
+        "weight": 1,
         "offset": 0,
         "magic": [
             bytearray([0x37, 0x7A, 0xBC, 0xAF, 0x27, 0x1C]),
         ],
         "handler": libarchive_handler,
     },
     "application/x-cpio": {
+        "weight": 1,
         "offset": 0,
         "magic": [
             bytearray([0xC7, 0x71]),  # 070707 in octal (Little Endian).
             bytearray([0x71, 0xC7]),  # 070707 in octal (Big Endian).
             bytearray([0x30, 0x37, 0x30, 0x37, 0x30, 0x31]),  # "070701"
             bytearray([0x30, 0x37, 0x30, 0x37, 0x30, 0x32]),  # "070702"
             bytearray([0x30, 0x37, 0x30, 0x37, 0x30, 0x37]),  # "070707"
         ],
         "handler": libarchive_handler,
     },
     "application/x-xar": {
+        "weight": 1,
         "offset": 0,
         "magic": [
             bytearray([0x78, 0x61, 0x72, 0x21]),
         ],
         "handler": xar_handler,
     },
     "application/vnd.ms-cab-compressed": {
+        "weight": 1,
         "offset": 0,
         "magic": [
             bytearray([0x4D, 0x53, 0x43, 0x46]),
         ],
         "handler": libarchive_handler,
     },
     "application/x-archive": {
+        "weight": 1,
         "offset": 0,
         "magic": [
             bytearray([0x21, 0x3C, 0x61, 0x72, 0x63, 0x68, 0x3E]),
         ],
         "handler": libarchive_handler,
     },
     "application/vnd.rar": {
+        "weight": 1,
         "offset": 0,
         "magic": [
             bytearray([0x52, 0x61, 0x72, 0x21, 0x1A, 0x07]),
         ],
         "handler": libarchive_handler,
     },
     "application/zstd": {
+        "weight": 1,
         "offset": 0,
         "magic": [
             bytearray([0x28, 0xB5, 0x2F, 0xFD]),
         ],
         "handler": zstd_handler,
     },
+    "application/x-apple-diskimage": {
+        "weight": 2,  # "container" formats are weighted higher.
+        "offset": -512,
+        "magic": [
+            bytearray([0x6B, 0x6F, 0x6C, 0x79]),
+        ],
+        "handler": dmg_handler,
+    },
 }
```

### Comparing `stacs-0.4.9/stacs/scan/loader/filepath.py` & `stacs-0.5.0/stacs/scan/loader/filepath.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,33 +19,44 @@
 logger = logging.getLogger(__name__)
 
 
 def metadata(filepath: str, overlay: str = None, parent: str = None) -> Entry:
     """Generates a hash and determines the mimetype of the input file."""
     md5 = hashlib.md5()
     mime = None
+    winner = 0
 
     # Read the file in chunks.
     try:
+        stat = os.stat(filepath)
+
         with open(filepath, "rb") as fin:
             while chunk := fin.read(CHUNK_SIZE):
                 md5.update(chunk)
 
-                # Only attempt to determine the filetype on the first chunk.
-                if not mime and fin.tell() <= CHUNK_SIZE:
-                    mime = archive.get_mimetype(chunk)
+                # Attempt to determine the mime-type using the first and last chunk.
+                # Note: This may need to change further in future.
+                if (not mime and fin.tell() <= CHUNK_SIZE) or len(chunk) < CHUNK_SIZE:
+                    start = False if len(chunk) < CHUNK_SIZE else True
+                    (score, candidate) = archive.get_mimetype(chunk, start)
+
+                    # Swap the winner if the score is higher.
+                    if score > winner:
+                        mime = candidate
+                        winner = score
     except OSError as err:
         raise FileAccessException(f"Unable to open file at {filepath}: {err}")
 
     return Entry(
         path=filepath,
         md5=md5.hexdigest(),
         mime=mime,
         overlay=overlay,
         parent=parent,
+        size=stat.st_size,
     )
 
 
 def walker(path: str, skip_on_eacces: bool) -> List[str]:
     """Recursively walk a file path, returning a list of all files."""
     entries = []
```

### Comparing `stacs-0.4.9/stacs/scan/loader/format/xar.py` & `stacs-0.5.0/stacs/scan/loader/format/xar.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,18 +57,15 @@
                 # Ensure the provided file is actually a XAR.
                 if fin.read(4) != XAR_MAGIC:
                     raise InvalidFileException("File does not appear to be a XAR")
 
                 # Rewind and attempt to read in header.
                 fin.seek(0)
                 self._header = XARHeader._make(
-                    struct.unpack(
-                        XAR_HEADER,
-                        fin.read(struct.calcsize(XAR_HEADER)),
-                    )
+                    struct.unpack(XAR_HEADER, fin.read(XAR_HEADER_SZ))
                 )
 
                 # Read and decompress the table-of-contents.
                 fin.seek(self._header.size)
 
                 self._toc = ET.fromstring(
                     str(
@@ -124,15 +121,15 @@
         candidates = []
 
         for entry in self._toc.findall("./toc/file"):
             candidates.extend(self._parse_entries(entry))
 
         return candidates
 
-    def extract(self, destination=None):
+    def extract(self, destination):
         """Extract all entries from the XAR to the optional destination directory."""
         # Offset must be adjusted by the size of the ToC and the header. This is as the
         # offset is from the first byte AFTER the header and compressed ToC.
         header_size = self._header.size + self._header.toc_length_compressed
 
         for entry in self.entries():
             parent = os.path.dirname(os.path.join(destination, entry.path))
```

### Comparing `stacs-0.4.9/stacs/scan/model/finding.py` & `stacs-0.5.0/stacs/scan/model/finding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Defines types to assist with reporting findings.
 
 SPDX-License-Identifier: BSD-3-Clause
 """
 
+from typing import List
+
 from pydantic import BaseModel, Extra, Field
 
 
 class Location(BaseModel, extra=Extra.forbid):
     """Defines data associated with a location of a finding."""
 
     line: int = Field(
@@ -26,15 +28,19 @@
         title="The STACS module which generated the finding.",
     )
     description: str = Field(
         None,
         title="A description of the finding",
     )
     reference: str = Field(
-        title="A reference to the element which generated the finding."
+        title="A reference to the element which generated the finding.",
+    )
+    tags: List[str] = Field(
+        [],
+        title="A list of tags associated with the finding.",
     )
     version: str = Field(
         None,
         title="The version of the element which generated the finding.",
     )
```

### Comparing `stacs-0.4.9/stacs/scan/model/ignore_list.py` & `stacs-0.5.0/stacs/scan/model/ignore_list.py`

 * *Files identical despite different names*

### Comparing `stacs-0.4.9/stacs/scan/model/manifest.py` & `stacs-0.5.0/stacs/scan/model/manifest.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,18 @@
         None,
         title="The MD5 sum of the file's parent.",
     )
     mime: str = Field(
         None,
         title="The mimetype of the file.",
     )
+    size: int = Field(
+        None,
+        title="The size of the file.",
+    )
 
 
 class Format(BaseModel, extra=Extra.forbid):
     """Defines the schema of a manifest file."""
 
     files: List[Entry] = Field(
         [],
```

### Comparing `stacs-0.4.9/stacs/scan/model/pack.py` & `stacs-0.5.0/stacs/scan/model/pack.py`

 * *Files identical despite different names*

### Comparing `stacs-0.4.9/stacs/scan/output/pretty.py` & `stacs-0.5.0/stacs/scan/output/pretty.py`

 * *Files identical despite different names*

### Comparing `stacs-0.4.9/stacs/scan/output/sarif.py` & `stacs-0.5.0/stacs/scan/output/sarif.py`

 * *Files identical despite different names*

### Comparing `stacs-0.4.9/stacs/scan/scanner/rules.py` & `stacs-0.5.0/stacs/scan/scanner/rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import base64
 import hashlib
 import os
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from typing import List
 
 import yara
+
 from stacs.scan.constants import CHUNK_SIZE, WINDOW_SIZE
 from stacs.scan.exceptions import FileAccessException, InvalidFormatException
 from stacs.scan.loader import archive
 from stacs.scan.model import finding, manifest, pack
 
 
 def is_binary(target: manifest.Entry) -> bool:
@@ -126,14 +127,20 @@
             while bytes_read < offset:
                 bytes_read += CHUNK_SIZE
 
                 if bytes_read > offset:
                     line_number += fin.read(offset).count("\n")
                 else:
                     line_number += fin.read(CHUNK_SIZE).count("\n")
+    except UnicodeDecodeError:
+        # It's possible to get into a state where the detected mime-type of a file is
+        # incorrect, resulting in unprocessable binary data making it here. In these
+        # cases we'll just bail early and report the number of bytes into the file of
+        # the finding. Exactly as we do for known binary files.
+        return finding.Location(offset=offset)
     except OSError as err:
         raise FileAccessException(err)
 
     return finding.Location(offset=offset, line=line_number)
 
 
 def generate_findings(target: manifest.Entry, match: yara.Match) -> List[finding.Entry]:
@@ -147,14 +154,15 @@
         location = generate_location(target, offset)
         sample = generate_sample(target, offset, len(entry))
 
         # Add on information about the origin of the finding (that's us!)
         source = finding.Source(
             module=__name__,
             reference=match.rule,
+            tags=match.tags,
             version=match.meta.get("version", "UNKNOWN"),
             description=match.meta.get("description"),
         )
         findings.append(
             finding.Entry(
                 md5=target.md5,
                 path=target.overlay if target.overlay else target.path,
```

### Comparing `stacs-0.4.9/stacs.egg-info/PKG-INFO` & `stacs-0.5.0/stacs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: stacs
-Version: 0.4.9
+Version: 0.5.0
 Summary: Static Token And Credential Scanner.
-Home-page: https://www.github.com/stacscan/stacs/
+Author: Peter Adkins
+License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: development
+Provides-Extra: tests
 License-File: LICENSE
 
-[![Shield](https://img.shields.io/github/workflow/status/stacscan/stacs/Check?label=Tests&style=flat-square)](https://github.com/stacscan/stacs/actions?workflow=Check)
-[![Shield](https://img.shields.io/github/workflow/status/stacscan/stacs/Publish?label=Deploy&style=flat-square)](https://github.com/stacscan/stacs/actions?workflow=Publish)
+[![Shield](https://img.shields.io/github/actions/workflow/status/stacscan/stacs/check.yml?label=Tests&style=flat-square)](https://github.com/stacscan/stacs/actions?workflow=Check)
+[![Shield](https://img.shields.io/github/actions/workflow/status/stacscan/stacs/publish.yml?label=Deploy&style=flat-square)](https://github.com/stacscan/stacs/actions?workflow=Publish)
 [![Shield](https://img.shields.io/docker/pulls/stacscan/stacs?style=flat-square)](https://hub.docker.com/r/stacscan/stacs)
 [![Shield](https://img.shields.io/docker/image-size/stacscan/stacs?style=flat-square)](https://hub.docker.com/r/stacscan/stacs/tags?page=1&ordering=last_updated)
 [![Shield](https://img.shields.io/twitter/follow/stacscan?style=flat-square)](https://twitter.com/stacscan)
 <p align="center">
     <br /><br />
     <img src="https://raw.githubusercontent.com/stacscan/stacs/main/docs/images/STACS-Logo-RGB.small.png">
 </p>
@@ -31,17 +32,17 @@
 which suports binary file formats, analysis of nested archives, composable rulesets
 and ignore lists, and SARIF reporting.
 
 ### What does STACS support?
 
 Currently, STACS supports recursive unpacking of:
 
-* 7z, ar, bz2, cab, cpio, gz, iso, rar, rpm, tar, xar, xz, zip
+* 7z, ar, bz2, cab, cpio, gz, iso, rar, rpm, tar, xar, xz, zip, dmg
 
-As STACS works on detected file types, propriatary file formats based and other
+As STACS works on detected file types, proprietary file formats based and other
 file-types which use these formats are automatically supported. This includes Docker
 images, Android APKs, Java JAR files, RPMs, Debian packages (`.deb`), macOS packages
 (`.pkg`), and more!
 
 ### Who should use STACS?
 
 STACS is designed for use by any teams who release binary artifacts. STACS provides
```


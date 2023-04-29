# Comparing `tmp/bandersnatch-6.2.0.tar.gz` & `tmp/bandersnatch-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bandersnatch-6.2.0.tar", last modified: Wed Mar  1 02:41:27 2023, max compression
+gzip compressed data, was "bandersnatch-6.3.0.tar", last modified: Sat Apr 29 18:43:56 2023, max compression
```

## Comparing `bandersnatch-6.2.0.tar` & `bandersnatch-6.3.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:41:27.648048 bandersnatch-6.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-03-01 02:41:27.648048 bandersnatch-6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-03-01 02:41:27.648048 bandersnatch-6.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:41:27.632047 bandersnatch-6.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:41:27.640047 bandersnatch-6.2.0/src/bandersnatch/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/default.conf
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/master.py
--rw-r--r--   0 runner    (1001) docker     (123)    41856 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:41:27.644048 bandersnatch-6.2.0/src/bandersnatch/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/mock_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/test_master.py
--rw-r--r--   0 runner    (1001) docker     (123)    37920 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/test_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/test_simple_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/tests/test_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/unittest.conf
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:41:27.640047 bandersnatch-6.2.0/src/bandersnatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-03-01 02:41:27.000000 bandersnatch-6.2.0/src/bandersnatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-03-01 02:41:27.000000 bandersnatch-6.2.0/src/bandersnatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 02:41:27.000000 bandersnatch-6.2.0/src/bandersnatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-03-01 02:41:27.000000 bandersnatch-6.2.0/src/bandersnatch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-01 02:41:27.000000 bandersnatch-6.2.0/src/bandersnatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-01 02:41:27.000000 bandersnatch-6.2.0/src/bandersnatch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:41:27.648048 bandersnatch-6.2.0/src/bandersnatch_filter_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch_filter_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch_filter_plugins/allowlist_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch_filter_plugins/blocklist_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch_filter_plugins/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch_filter_plugins/filename_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch_filter_plugins/latest_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch_filter_plugins/metadata_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch_filter_plugins/prerelease_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch_filter_plugins/regex_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:41:27.648048 bandersnatch-6.2.0/src/bandersnatch_storage_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch_storage_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch_storage_plugins/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    15486 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch_storage_plugins/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    35688 2023-03-01 02:41:11.000000 bandersnatch-6.2.0/src/bandersnatch_storage_plugins/swift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:43:56.898885 bandersnatch-6.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-04-29 18:43:56.898885 bandersnatch-6.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-29 18:43:56.898885 bandersnatch-6.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:43:56.890885 bandersnatch-6.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:43:56.894885 bandersnatch-6.3.0/src/bandersnatch/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/default.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41857 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:43:56.894885 bandersnatch-6.3.0/src/bandersnatch/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/mock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/test_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37068 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/test_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/test_simple_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/tests/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/unittest.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:43:56.894885 bandersnatch-6.3.0/src/bandersnatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-04-29 18:43:56.000000 bandersnatch-6.3.0/src/bandersnatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-29 18:43:56.000000 bandersnatch-6.3.0/src/bandersnatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:43:56.000000 bandersnatch-6.3.0/src/bandersnatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-29 18:43:56.000000 bandersnatch-6.3.0/src/bandersnatch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-29 18:43:56.000000 bandersnatch-6.3.0/src/bandersnatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-29 18:43:56.000000 bandersnatch-6.3.0/src/bandersnatch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:43:56.898885 bandersnatch-6.3.0/src/bandersnatch_filter_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch_filter_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch_filter_plugins/allowlist_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch_filter_plugins/blocklist_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch_filter_plugins/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch_filter_plugins/filename_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch_filter_plugins/latest_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch_filter_plugins/metadata_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch_filter_plugins/prerelease_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch_filter_plugins/regex_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:43:56.898885 bandersnatch-6.3.0/src/bandersnatch_storage_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch_storage_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch_storage_plugins/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15486 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch_storage_plugins/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35688 2023-04-29 18:43:43.000000 bandersnatch-6.3.0/src/bandersnatch_storage_plugins/swift.py
```

### Comparing `bandersnatch-6.2.0/LICENSE` & `bandersnatch-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/PKG-INFO` & `bandersnatch-6.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandersnatch
-Version: 6.2.0
+Version: 6.3.0
 Summary: Mirroring tool that implements the client (mirror) side of PEP 381
 Home-page: https://github.com/pypa/bandersnatch/
 Author: Christian Theune
 Author-email: ct@flyingcircus.io
 License: Academic Free License, version 3
 Project-URL: Source Code, https://github.com/pypa/bandersnatch
 Project-URL: Change Log, https://github.com/pypa/bandersnatch/blob/master/CHANGES.md
```

### Comparing `bandersnatch-6.2.0/README.md` & `bandersnatch-6.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/setup.cfg` & `bandersnatch-6.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 license = Academic Free License, version 3
 license_file = LICENSE
 name = bandersnatch
 project_urls = 
 	Source Code = https://github.com/pypa/bandersnatch
 	Change Log = https://github.com/pypa/bandersnatch/blob/master/CHANGES.md
 url = https://github.com/pypa/bandersnatch/
-version = 6.2.0
+version = 6.3.0
 
 [options]
 install_requires = 
 	aiohttp
 	aiohttp-socks
 	aiohttp-xmlrpc
 	filelock
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch/__init__.py` & `bandersnatch-6.3.0/src/bandersnatch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,13 +16,13 @@
     def version_str(self) -> str:
         release_level = f".{self.releaselevel}" if self.releaselevel else ""
         return f"{self.major}.{self.minor}.{self.micro}{release_level}"
 
 
 __version_info__ = _VersionInfo(
     major=6,
-    minor=2,
+    minor=3,
     micro=0,
     releaselevel="",
     serial=0,  # Not currently in use with Bandersnatch versioning
 )
 __version__ = __version_info__.version_str
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch/configuration.py` & `bandersnatch-6.3.0/src/bandersnatch/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import configparser
 import importlib.resources
 import logging
 from pathlib import Path
 from typing import Any, Dict, List, NamedTuple, Optional, Type
 
-from .simple import SimpleFormat, get_format_value
+from .simple import SimpleDigest, SimpleFormat, get_digest_value, get_format_value
 
 logger = logging.getLogger("bandersnatch")
 
 
 class SetConfigValues(NamedTuple):
     json_save: bool
     root_uri: str
@@ -127,23 +127,25 @@
         storage_backend_name = "filesystem"
         logger.debug(
             "Failed to find storage backend in config, falling back to default!"
         )
     logger.info(f"Selected storage backend: {storage_backend_name}")
 
     try:
-        digest_name = config.get("mirror", "digest_name")
+        digest_name = get_digest_value(config.get("mirror", "digest_name"))
     except configparser.NoOptionError:
-        digest_name = "sha256"
-    if digest_name not in ("md5", "sha256"):
-        raise ValueError(
-            f"Supplied digest_name {digest_name} is not supported! Please "
-            + "update digest_name to one of ('sha256', 'md5') in the [mirror] "
-            + "section."
+        digest_name = SimpleDigest.SHA256
+        logger.debug(f"Using digest {digest_name} by default ...")
+    except ValueError as e:
+        logger.error(
+            f"Supplied digest_name {config.get('mirror', 'digest_name')} is "
+            + "not supported! Please update the digest_name in the [mirror] "
+            + "section of your config to a supported digest value."
         )
+        raise e
 
     try:
         cleanup = config.getboolean("mirror", "cleanup")
     except configparser.NoOptionError:
         logger.debug(
             "bandersnatch is not cleaning up non PEP 503 normalized Simple "
             + "API directories"
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch/default.conf` & `bandersnatch-6.3.0/src/bandersnatch/default.conf`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch/delete.py` & `bandersnatch-6.3.0/src/bandersnatch/delete.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch/errors.py` & `bandersnatch-6.3.0/src/bandersnatch/errors.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch/filter.py` & `bandersnatch-6.3.0/src/bandersnatch/filter.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch/log.py` & `bandersnatch-6.3.0/src/bandersnatch/log.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch/main.py` & `bandersnatch-6.3.0/src/bandersnatch/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     uvloop.install()
 except ImportError:
     pass
 
 logger = logging.getLogger(__name__)  # pylint: disable=C0103
 
 
-# TODO: Workout why argparse.ArgumentParser causes type errors
 def _delete_parser(subparsers: argparse._SubParsersAction) -> None:
     d = subparsers.add_parser(
         "delete",
         help=(
             "Consulte metadata (locally or remotely) and delete "
             + "entire package artifacts."
         ),
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch/master.py` & `bandersnatch-6.3.0/src/bandersnatch/master.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch/mirror.py` & `bandersnatch-6.3.0/src/bandersnatch/mirror.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         # - others importing may not reset this like our main.py
         self.altered_packages = {}
 
         if specific_packages is None:
             # Changelog-based synchronization
             await self.determine_packages_to_sync()
         else:
-            # Synchronize specific packages. This method doesn't update the statusfile
+            # Synchronize specific packages. This method doesn't update the status file
             # Pass serial number 0 to bypass the stale serial check in Package class
             SERIAL_DONT_CARE = 0
             self.packages_to_sync = {
                 utils.bandersnatch_safe_name(name): SERIAL_DONT_CARE
                 for name in specific_packages
             }
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch/package.py` & `bandersnatch-6.3.0/src/bandersnatch/package.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch/simple.py` & `bandersnatch-6.3.0/src/bandersnatch/simple.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,108 @@
 import html
 import json
 import logging
+import sys
 from enum import Enum, auto
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, NamedTuple, Optional, Union
 from urllib.parse import urlparse
 
 from .package import Package
 
 if TYPE_CHECKING:
     from .storage import Storage
 
+if sys.version_info >= (3, 11):
+    from enum import StrEnum
+else:
+    from .utils import StrEnum
+
 
 class SimpleFormats(NamedTuple):
     html: str
     json: str
 
 
 class SimpleFormat(Enum):
     ALL = auto()
     HTML = auto()
     JSON = auto()
 
 
+class SimpleDigests(NamedTuple):
+    sha256: str
+    md5: str
+
+
+class SimpleDigest(StrEnum):
+    SHA256 = "sha256"
+    MD5 = "md5"
+
+
 logger = logging.getLogger(__name__)
 
 
 class InvalidSimpleFormat(KeyError):
     """We don't have a valid format choice from configuration"""
 
     pass
 
 
+class InvalidDigestFormat(ValueError):
+    """We don't have a valid digest choice from configuration"""
+
+    pass
+
+
 def get_format_value(format: str) -> SimpleFormat:
     try:
         return SimpleFormat[format.upper()]
     except KeyError:
-        valid_formats = [v.name for v in SimpleFormat].sort()
+        valid_formats = sorted([v.name for v in SimpleFormat])
         raise InvalidSimpleFormat(
             f"{format.upper()} is not a valid Simple API format. "
             + f"Valid Options: {valid_formats}"
         )
 
 
+def get_digest_value(digest: str) -> SimpleDigest:
+    try:
+        return SimpleDigest[digest.upper()]
+    except KeyError:
+        valid_digests = sorted([v.name for v in SimpleDigest])
+        raise InvalidDigestFormat(
+            f"{digest} is not a valid Simple API file hash digest. "
+            + f"Valid Options: {valid_digests}"
+        )
+
+
 class SimpleAPI:
     """Handle all Simple API file generation"""
 
     # PEP620 Simple API Version
     pypi_repository_version = "1.0"
     # PEP691 Simple API Version
     pypi_simple_api_version = "1.0"
 
     def __init__(
         self,
         storage_backend: "Storage",
         format: Union[SimpleFormat, str],
         diff_file_list: List[Path],
-        digest_name: str,
+        digest_name: Union[SimpleDigest, str],
         hash_index: bool,
         root_uri: Optional[str],
     ) -> None:
         self.diff_file_list = diff_file_list
-        self.digest_name = digest_name
+        self.digest_name = (
+            get_digest_value(digest_name)
+            if isinstance(digest_name, str)
+            else digest_name
+        )
         self.format = get_format_value(format) if isinstance(format, str) else format
         self.hash_index = hash_index
         self.root_uri = root_uri
         self.storage_backend = storage_backend
 
     def html_enabled(self) -> bool:
         return self.format in {SimpleFormat.ALL, SimpleFormat.HTML}
@@ -186,16 +223,15 @@
 
         # Add release files into the JSON dict
         for r in release_files:
             package_json["files"].append(
                 {
                     "filename": r["filename"],
                     "hashes": {
-                        digest_name: digest_hash
-                        for digest_name, digest_hash in r["digests"].items()
+                        self.digest_name: r["digests"][self.digest_name],
                     },
                     "requires-python": r.get("requires_python", ""),
                     "url": self._file_url_to_local_url(r["url"]),
                     "yanked": r.get("yanked", False),
                 }
             )
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch/storage.py` & `bandersnatch-6.3.0/src/bandersnatch/storage.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch/tests/conftest.py` & `bandersnatch-6.3.0/src/bandersnatch/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch/tests/test_configuration.py` & `bandersnatch-6.3.0/src/bandersnatch/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch/tests/test_delete.py` & `bandersnatch-6.3.0/src/bandersnatch/tests/test_delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,27 +33,23 @@
 pypi{0}unittest
 pypi{0}unittest{0}json
 simple
 simple{0}cooper
 simple{0}cooper{0}index.html
 simple{0}unittest
 simple{0}unittest{0}index.html\
-""".format(
-    os.sep
-)
+""".format(os.sep)
 EXPECTED_WEB_AFTER_DELETION = """\
 json
 packages
 packages{0}69
 packages{0}7b
 pypi
 simple\
-""".format(
-    os.sep
-)
+""".format(os.sep)
 MOCK_JSON_TEMPLATE = """{
     "releases": {
         "6.9": [
             {"url": "https://files.ph.org/packages/7b/PKGNAME-6.9-py3-none-any.whl"},
             {"url": "https://files.ph.org/packages/69/PKGNAME-6.9.tar.gz"}
         ]
     }
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch/tests/test_filter.py` & `bandersnatch-6.3.0/src/bandersnatch/tests/test_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,57 +34,51 @@
         if self.tempdir:
             assert self.cwd
             os.chdir(self.cwd)
             self.tempdir.cleanup()
             self.tempdir = None
 
     def test__filter_project_plugins__loads(self) -> None:
-        mock_config(
-            """\
+        mock_config("""\
 [plugins]
 enabled = all
-"""
-        )
+""")
         builtin_plugin_names = [
             "blocklist_project",
             "regex_project",
             "allowlist_project",
         ]
 
         plugins = LoadedFilters().filter_project_plugins()
         names = [plugin.name for plugin in plugins]
         for name in builtin_plugin_names:
             self.assertIn(name, names)
 
     def test__filter_release_plugins__loads(self) -> None:
-        mock_config(
-            """\
+        mock_config("""\
 [plugins]
 enabled = all
-"""
-        )
+""")
         builtin_plugin_names = [
             "blocklist_release",
             "prerelease_release",
             "regex_release",
             "latest_release",
         ]
 
         plugins = LoadedFilters().filter_release_plugins()
         names = [plugin.name for plugin in plugins]
         for name in builtin_plugin_names:
             self.assertIn(name, names)
 
     def test__filter_no_plugin(self) -> None:
-        mock_config(
-            """\
+        mock_config("""\
 [plugins]
 enabled =
-"""
-        )
+""")
 
         plugins = LoadedFilters().filter_release_plugins()
         self.assertEqual(len(plugins), 0)
 
         plugins = LoadedFilters().filter_project_plugins()
         self.assertEqual(len(plugins), 0)
 
@@ -130,32 +124,30 @@
         instance.config_file = "test.conf"
         instance.load_configuration()
         plugin = Filter()
         assert plugin.allowlist.name == "allowlist"
         assert plugin.blocklist.name == "blocklist"
 
     def test__filter_project_blocklist_allowlist__pep503_normalize(self) -> None:
-        mock_config(
-            """\
+        mock_config("""\
 [plugins]
 enabled =
     blocklist_project
     allowlist_project
 
 [blocklist]
 packages =
     SampleProject
     trove----classifiers
 
 [allowlist]
 packages =
     SampleProject
     trove----classifiers
-"""
-        )
+""")
 
         plugins = {
             plugin.name: plugin for plugin in LoadedFilters().filter_project_plugins()
         }
 
         self.assertTrue(plugins["blocklist_project"].check_match(name="sampleproject"))
         self.assertTrue(
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch/tests/test_main.py` & `bandersnatch-6.3.0/src/bandersnatch/tests/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     with open(conffile, "w") as fp:
         parser.write(fp)
     sys.argv = ["bandersnatch", "-c", conffile, "mirror"]
 
     with pytest.raises(ValueError) as e:
         main(asyncio.new_event_loop())
 
-    assert "foobar is not supported" in str(e.value)
+    assert "foobar is not a valid" in str(e.value)
 
 
 @pytest.fixture
 def customconfig(tmpdir: Path) -> Path:
     default_path = Path(bandersnatch.__file__).parent / "unittest.conf"
     with default_path.open("r") as dfp:
         config = dfp.read()
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch/tests/test_master.py` & `bandersnatch-6.3.0/src/bandersnatch/tests/test_master.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch/tests/test_mirror.py` & `bandersnatch-6.3.0/src/bandersnatch/tests/test_mirror.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,32 +225,25 @@
 last-modified
 local-stats
 local-stats{0}days
 packages
 simple
 simple{0}index.html
 simple{0}index.v1_html
-simple{0}index.v1_json""".format(
-        sep
-    ) == utils.find(
-        mirror.webdir
-    )
-    assert (
-        open("web{0}simple{0}index.html".format(sep)).read()
-        == """\
+simple{0}index.v1_json""".format(sep) == utils.find(mirror.webdir)
+    assert open("web{0}simple{0}index.html".format(sep)).read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Simple Index</title>
   </head>
   <body>
   </body>
 </html>"""
-    )
     assert open("status").read() == "0"
 
 
 @pytest.mark.asyncio
 async def test_mirror_empty_resume_from_todo_list(mirror: BandersnatchMirror) -> None:
     with open("todo", "w") as todo:
         todo.write("20\nfoobar 1")
@@ -277,35 +270,30 @@
 web{0}simple
 web{0}simple{0}foobar
 web{0}simple{0}foobar{0}index.html
 web{0}simple{0}foobar{0}index.v1_html
 web{0}simple{0}foobar{0}index.v1_json
 web{0}simple{0}index.html
 web{0}simple{0}index.v1_html
-web{0}simple{0}index.v1_json""".format(
-        sep
-    )
+web{0}simple{0}index.v1_json""".format(sep)
     if WINDOWS:
         expected = expected.replace(".lock\n", "")
     assert expected == utils.find(mirror.homedir)
 
-    assert (
-        open("web{0}simple{0}index.html".format(sep)).read()
-        == """\
+    assert open("web{0}simple{0}index.html".format(sep)).read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Simple Index</title>
   </head>
   <body>
     <a href="foobar/">foobar</a><br/>
   </body>
 </html>"""
-    )
     assert open("status").read() == "20"
 
 
 @pytest.mark.asyncio
 async def test_mirror_sync_package_skip_index(mirror: BandersnatchMirror) -> None:
     mirror.master.all_packages = mock.AsyncMock(return_value={"foo": 1})  # type: ignore
     mirror.json_save = True
@@ -317,19 +305,15 @@
 json{0}foo
 last-modified
 packages{0}2.7{0}f{0}foo{0}foo.whl
 packages{0}any{0}f{0}foo{0}foo.zip
 pypi{0}foo{0}json
 simple{0}foo{0}index.html
 simple{0}foo{0}index.v1_html
-simple{0}foo{0}index.v1_json""".format(
-        sep
-    ) == utils.find(
-        mirror.webdir, dirs=False
-    )
+simple{0}foo{0}index.v1_json""".format(sep) == utils.find(mirror.webdir, dirs=False)
     assert open("status", "rb").read() == b"1"
 
 
 @pytest.mark.asyncio
 async def test_mirror_sync_package(mirror: BandersnatchMirror) -> None:
     mirror.master.all_packages = mock.AsyncMock(return_value={"foo": 1})  # type: ignore
     mirror.json_save = True
@@ -344,33 +328,26 @@
 packages{0}any{0}f{0}foo{0}foo.zip
 pypi{0}foo{0}json
 simple{0}foo{0}index.html
 simple{0}foo{0}index.v1_html
 simple{0}foo{0}index.v1_json
 simple{0}index.html
 simple{0}index.v1_html
-simple{0}index.v1_json""".format(
-        sep
-    ) == utils.find(
-        mirror.webdir, dirs=False
-    )
-    assert (
-        open("web{0}simple{0}index.html".format(sep)).read()
-        == """\
+simple{0}index.v1_json""".format(sep) == utils.find(mirror.webdir, dirs=False)
+    assert open("web{0}simple{0}index.html".format(sep)).read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Simple Index</title>
   </head>
   <body>
     <a href="foo/">foo</a><br/>
   </body>
 </html>"""
-    )
     assert open("status", "rb").read() == b"1"
 
 
 @pytest.mark.asyncio
 async def test_mirror_sync_package_error_no_early_exit(
     mirror: BandersnatchMirror,
 ) -> None:
@@ -385,34 +362,29 @@
 web{0}packages{0}2.7{0}f{0}foo{0}foo.whl
 web{0}packages{0}any{0}f{0}foo{0}foo.zip
 web{0}simple{0}foo{0}index.html
 web{0}simple{0}foo{0}index.v1_html
 web{0}simple{0}foo{0}index.v1_json
 web{0}simple{0}index.html
 web{0}simple{0}index.v1_html
-web{0}simple{0}index.v1_json""".format(
-        sep
-    )
+web{0}simple{0}index.v1_json""".format(sep)
     if WINDOWS:
         expected = expected.replace(".lock\n", "")
     assert expected == utils.find(mirror.homedir, dirs=False)
-    assert (
-        open("web{0}simple{0}index.html".format(sep)).read()
-        == """\
+    assert open("web{0}simple{0}index.html".format(sep)).read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Simple Index</title>
   </head>
   <body>
     <a href="foo/">foo</a><br/>
   </body>
 </html>"""
-    )
 
     assert open("todo").read() == "1\n"
 
     # Check the returned dict is accurate
     expected_dict = {
         "foo": {
             "web{0}packages{0}2.7{0}f{0}foo{0}foo.whl".format(sep),
@@ -436,19 +408,15 @@
 
     assert """\
 .lock
 generation
 todo
 web{0}packages{0}any{0}f{0}foo{0}foo.zip
 web{0}simple{0}foo{0}index.html
-web{0}simple{0}index.html""".format(
-        sep
-    ) == utils.find(
-        mirror.homedir, dirs=False
-    )
+web{0}simple{0}index.html""".format(sep) == utils.find(mirror.homedir, dirs=False)
     assert open("web{0}simple{0}index.html".format(sep)).read() == "old index"
     assert open("todo").read() == "1\n"
 
 
 @pytest.mark.asyncio
 async def test_mirror_sync_package_with_hash(
     mirror_hash_index: BandersnatchMirror,
@@ -463,33 +431,28 @@
 packages{0}2.7{0}f{0}foo{0}foo.whl
 packages{0}any{0}f{0}foo{0}foo.zip
 simple{0}f{0}foo{0}index.html
 simple{0}f{0}foo{0}index.v1_html
 simple{0}f{0}foo{0}index.v1_json
 simple{0}index.html
 simple{0}index.v1_html
-simple{0}index.v1_json""".format(
-        sep
-    ) == utils.find(
+simple{0}index.v1_json""".format(sep) == utils.find(
         mirror_hash_index.webdir, dirs=False
     )
-    assert (
-        open("web{0}simple{0}index.html".format(sep)).read()
-        == """\
+    assert open("web{0}simple{0}index.html".format(sep)).read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Simple Index</title>
   </head>
   <body>
     <a href="foo/">foo</a><br/>
   </body>
 </html>"""
-    )
     assert open("status").read() == "1"
 
 
 @pytest.mark.asyncio
 async def test_mirror_sync_package_download_mirror(
     mirror: BandersnatchMirror,
 ) -> None:
@@ -509,33 +472,26 @@
 packages{0}any{0}f{0}foo{0}foo.zip
 pypi{0}foo{0}json
 simple{0}foo{0}index.html
 simple{0}foo{0}index.v1_html
 simple{0}foo{0}index.v1_json
 simple{0}index.html
 simple{0}index.v1_html
-simple{0}index.v1_json""".format(
-        sep
-    ) == utils.find(
-        mirror.webdir, dirs=False
-    )
-    assert (
-        open("web{0}simple{0}index.html".format(sep)).read()
-        == """\
+simple{0}index.v1_json""".format(sep) == utils.find(mirror.webdir, dirs=False)
+    assert open("web{0}simple{0}index.html".format(sep)).read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Simple Index</title>
   </head>
   <body>
     <a href="foo/">foo</a><br/>
   </body>
 </html>"""
-    )
     assert open("status", "rb").read() == b"1"
 
 
 @pytest.mark.asyncio
 async def test_mirror_sync_package_download_mirror_fallback(
     mirror: BandersnatchMirror,
 ) -> None:
@@ -554,33 +510,26 @@
 packages{0}any{0}f{0}foo{0}foo.zip
 pypi{0}foo{0}json
 simple{0}foo{0}index.html
 simple{0}foo{0}index.v1_html
 simple{0}foo{0}index.v1_json
 simple{0}index.html
 simple{0}index.v1_html
-simple{0}index.v1_json""".format(
-        sep
-    ) == utils.find(
-        mirror.webdir, dirs=False
-    )
-    assert (
-        open("web{0}simple{0}index.html".format(sep)).read()
-        == """\
+simple{0}index.v1_json""".format(sep) == utils.find(mirror.webdir, dirs=False)
+    assert open("web{0}simple{0}index.html".format(sep)).read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Simple Index</title>
   </head>
   <body>
     <a href="foo/">foo</a><br/>
   </body>
 </html>"""
-    )
 
 
 @pytest.mark.asyncio
 async def test_mirror_sync_package_download_mirror_fails(
     mirror: BandersnatchMirror,
 ) -> None:
     mirror.master.all_packages = mock.AsyncMock(return_value={"foo": 1})  # type: ignore
@@ -605,17 +554,15 @@
     mirror: BandersnatchMirror,
 ) -> None:
     mirror.master.changed_packages = mock.AsyncMock(return_value={})  # type: ignore
     mirror.synced_serial = 1
     await mirror.synchronize()
 
     assert """\
-last-modified""" == utils.find(
-        mirror.webdir, dirs=False
-    )
+last-modified""" == utils.find(mirror.webdir, dirs=False)
 
 
 def test_mirror_json_metadata(
     mirror: BandersnatchMirror, package_json: Dict[str, Any]
 ) -> None:
     package = Package("foo", serial=11)
     mirror.json_file(package.name).parent.mkdir(parents=True)
@@ -715,150 +662,125 @@
     mirror: BandersnatchMirror,
 ) -> None:
     mirror.packages_to_sync = {"foo": 1}
     await mirror.sync_packages()
 
     # Cross-check that simple directory hashing is disabled.
     assert not os.path.exists("web/simple/f/foo/index.html")
-    assert (
-        open("web/simple/foo/index.html").read()
-        == """\
+    assert open("web/simple/foo/index.html").read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Links for foo</title>
   </head>
   <body>
     <h1>Links for foo</h1>
     {}
   </body>
 </html>
 <!--SERIAL 654321-->\
-""".format(
-            EXPECTED_REL_HREFS
-        )
-    )
+""".format(EXPECTED_REL_HREFS)
 
 
 @pytest.mark.asyncio
 async def test_package_sync_with_release_no_files_syncs_simple_page_with_hash(
     mirror_hash_index: BandersnatchMirror,
 ) -> None:
     mirror_hash_index.packages_to_sync = {"foo": 1}
     await mirror_hash_index.sync_packages()
 
     assert not os.path.exists("web/simple/foo/index.html")
-    assert (
-        open("web/simple/f/foo/index.html").read()
-        == """\
+    assert open("web/simple/f/foo/index.html").read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Links for foo</title>
   </head>
   <body>
     <h1>Links for foo</h1>
     {}
   </body>
 </html>
 <!--SERIAL 654321-->\
-""".format(
-            EXPECTED_REL_HREFS
-        )
-    )
+""".format(EXPECTED_REL_HREFS)
 
 
 @pytest.mark.asyncio
 async def test_package_sync_with_canonical_simple_page(
     mirror: BandersnatchMirror,
 ) -> None:
     mirror.packages_to_sync = {"Foo": 1}
     await mirror.sync_packages()
 
     # Cross-check that simple directory hashing is disabled.
     assert not os.path.exists("web/simple/f/foo/index.html")
-    assert (
-        open("web/simple/foo/index.html").read()
-        == """\
+    assert open("web/simple/foo/index.html").read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Links for Foo</title>
   </head>
   <body>
     <h1>Links for Foo</h1>
     {}
   </body>
 </html>
 <!--SERIAL 654321-->\
-""".format(
-            EXPECTED_REL_HREFS
-        )
-    )
+""".format(EXPECTED_REL_HREFS)
 
 
 @pytest.mark.asyncio
 async def test_package_sync_with_canonical_simple_page_with_hash(
     mirror_hash_index: BandersnatchMirror,
 ) -> None:
     mirror_hash_index.packages_to_sync = {"Foo": 1}
     await mirror_hash_index.sync_packages()
 
     assert not os.path.exists("web/simple/foo/index.html")
-    assert (
-        open("web/simple/f/foo/index.html").read()
-        == """\
+    assert open("web/simple/f/foo/index.html").read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Links for Foo</title>
   </head>
   <body>
     <h1>Links for Foo</h1>
     {}
   </body>
 </html>
 <!--SERIAL 654321-->\
-""".format(
-            EXPECTED_REL_HREFS
-        )
-    )
+""".format(EXPECTED_REL_HREFS)
 
 
 @pytest.mark.asyncio
 async def test_package_sync_with_normalized_simple_page(
     mirror: BandersnatchMirror,
 ) -> None:
     mirror.packages_to_sync = {"Foo.bar-thing_other": 1}
     await mirror.sync_packages()
 
     # PEP 503 normalization
-    assert (
-        open("web/simple/foo-bar-thing-other/index.html").read()
-        == """\
+    assert open("web/simple/foo-bar-thing-other/index.html").read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Links for Foo.bar-thing_other</title>
   </head>
   <body>
     <h1>Links for Foo.bar-thing_other</h1>
     {}
   </body>
 </html>
 <!--SERIAL 654321-->\
-""".format(
-            EXPECTED_REL_HREFS
-        )
-    )
+""".format(EXPECTED_REL_HREFS)
 
 
 @pytest.mark.asyncio
 async def test_package_sync_simple_page_root_uri(mirror: BandersnatchMirror) -> None:
     mirror.packages_to_sync = {"foo": 1}
     mirror.simple_api.root_uri = "https://files.pythonhosted.org"
     await mirror.sync_packages()
@@ -868,124 +790,104 @@
         '<a href="https://files.pythonhosted.org/packages/2.7/f/foo/foo.whl#sha256=e3b'
         + '0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855">foo.whl</a>'
         + '<br/>\n    <a href="https://files.pythonhosted.org/packages/any/f/foo/foo.'
         + "zip#sha256=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855"
         + '">foo.zip</a><br/>'
     )
 
-    assert (
-        open("web/simple/foo/index.html").read()
-        == """\
+    assert open("web/simple/foo/index.html").read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Links for foo</title>
   </head>
   <body>
     <h1>Links for foo</h1>
     {}
   </body>
 </html>
 <!--SERIAL 654321-->\
-""".format(
-            expected_root_uri_hrefs
-        )
-    )
+""".format(expected_root_uri_hrefs)
 
 
 @pytest.mark.asyncio
 async def test_package_sync_simple_page_with_files(mirror: BandersnatchMirror) -> None:
     mirror.packages_to_sync = {"foo": 1}
     await mirror.sync_packages()
     assert not mirror.errors
 
-    assert (
-        open("web/simple/foo/index.html").read()
-        == """\
+    assert open("web/simple/foo/index.html").read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Links for foo</title>
   </head>
   <body>
     <h1>Links for foo</h1>
     {}
   </body>
 </html>
 <!--SERIAL 654321-->\
-""".format(
-            EXPECTED_REL_HREFS
-        )
-    )
+""".format(EXPECTED_REL_HREFS)
 
 
 @pytest.mark.asyncio
 async def test_package_sync_simple_page_with_existing_dir(
     mirror: BandersnatchMirror,
 ) -> None:
     mirror.packages_to_sync = {"foo": 1}
     package = Package("foo", serial=1)
     os.makedirs(mirror.simple_directory(package))
     await mirror.sync_packages()
     assert not mirror.errors
 
     # Cross-check that simple directory hashing is disabled.
     assert not os.path.exists("web/simple/f/foo/index.html")
-    assert (
-        open("web/simple/foo/index.html").read()
-        == """\
+    assert open("web/simple/foo/index.html").read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Links for foo</title>
   </head>
   <body>
     <h1>Links for foo</h1>
     {}
   </body>
 </html>
 <!--SERIAL 654321-->\
-""".format(
-            EXPECTED_REL_HREFS
-        )
-    )
+""".format(EXPECTED_REL_HREFS)
 
 
 @pytest.mark.asyncio
 async def test_package_sync_simple_page_with_existing_dir_with_hash(
     mirror_hash_index: BandersnatchMirror,
 ) -> None:
     mirror_hash_index.packages_to_sync = {"foo": 1}
     package = Package("foo", serial=1)
     os.makedirs(mirror_hash_index.simple_directory(package))
     await mirror_hash_index.sync_packages()
 
     assert not os.path.exists("web/simple/foo/index.html")
-    assert (
-        open("web/simple/f/foo/index.html").read()
-        == """\
+    assert open("web/simple/f/foo/index.html").read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Links for foo</title>
   </head>
   <body>
     <h1>Links for foo</h1>
     {}
   </body>
 </html>
 <!--SERIAL 654321-->\
-""".format(
-            EXPECTED_REL_HREFS
-        )
-    )
+""".format(EXPECTED_REL_HREFS)
 
 
 @pytest.mark.asyncio
 async def test_package_sync_with_error_keeps_it_on_todo_list(
     mirror: BandersnatchMirror,
 ) -> None:
     # Make packages_to_sync to generate an error
@@ -1155,33 +1057,28 @@
         raise OSError(errno.EBADF, "Some transient error?")
 
     mirror.packages_to_sync = {"Foo": 1}
     mirror.record_finished_package = record_finished_package  # type: ignore
 
     await mirror.sync_packages()
 
-    assert (
-        Path("web/simple/foo/index.html").open().read()
-        == """\
+    assert Path("web/simple/foo/index.html").open().read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Links for Foo</title>
   </head>
   <body>
     <h1>Links for Foo</h1>
     {}
   </body>
 </html>
 <!--SERIAL 654321-->\
-""".format(
-            EXPECTED_REL_HREFS
-        )
-    )
+""".format(EXPECTED_REL_HREFS)
     assert mirror.errors
 
 
 @freeze_time("2018-10-28")
 @pytest.mark.asyncio
 async def test_keep_index_versions_stores_one_prior_version(
     mirror: BandersnatchMirror,
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch/tests/test_package.py` & `bandersnatch-6.3.0/src/bandersnatch/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch/tests/test_simple_fixtures.py` & `bandersnatch-6.3.0/src/bandersnatch/tests/test_simple_fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,34 +105,32 @@
             "yanked_reason": None,
         }
     ],
     "vulnerabilities": [],
 }
 
 EXPECTED_SIMPLE_SIXTYNINE_JSON = """\
-{"files": [{"filename": "69-0.69.tar.gz", "hashes": {"md5": "4328d962656395fbd3e730c9d30bb48c", "sha256": "5c11f48399f9b1bca802751513f1f97bff6ce97e6facb576b7729e1351453c10"}, "requires-python": ">=3.6", "url": "../../packages/d3/cc/95dc5434362bd333a1fec275231775d748315b26edf1e7e568e6f8660238/69-0.69.tar.gz", "yanked": false}, {"filename": "69-6.9.tar.gz", "hashes": {"md5": "ff4bf804ef3722a1fd8853a8a32513d4", "sha256": "0c8deb7c8574787283c3fc08b714ee63fd6752a38d13515a9d8508798d428597"}, "requires-python": ">=3.6", "url": "../../packages/7b/6e/7c4ce77c6ca092e94e19b78282b459e7f8270362da655cbc6a75eeb9cdd7/69-6.9.tar.gz", "yanked": false}], "meta": {"api-version": "1.0", "_last-serial": "10333928"}, "name": "69"}\
+{"files": [{"filename": "69-0.69.tar.gz", "hashes": {"sha256": "5c11f48399f9b1bca802751513f1f97bff6ce97e6facb576b7729e1351453c10"}, "requires-python": ">=3.6", "url": "../../packages/d3/cc/95dc5434362bd333a1fec275231775d748315b26edf1e7e568e6f8660238/69-0.69.tar.gz", "yanked": false}, {"filename": "69-6.9.tar.gz", "hashes": {"sha256": "0c8deb7c8574787283c3fc08b714ee63fd6752a38d13515a9d8508798d428597"}, "requires-python": ">=3.6", "url": "../../packages/7b/6e/7c4ce77c6ca092e94e19b78282b459e7f8270362da655cbc6a75eeb9cdd7/69-6.9.tar.gz", "yanked": false}], "meta": {"api-version": "1.0", "_last-serial": "10333928"}, "name": "69"}\
 """
 
 EXPECTED_SIMPLE_SIXTYNINE_JSON_PRETTY = """\
 {
     "files": [
         {
             "filename": "69-0.69.tar.gz",
             "hashes": {
-                "md5": "4328d962656395fbd3e730c9d30bb48c",
                 "sha256": "5c11f48399f9b1bca802751513f1f97bff6ce97e6facb576b7729e1351453c10"
             },
             "requires-python": ">=3.6",
             "url": "../../packages/d3/cc/95dc5434362bd333a1fec275231775d748315b26edf1e7e568e6f8660238/69-0.69.tar.gz",
             "yanked": false
         },
         {
             "filename": "69-6.9.tar.gz",
             "hashes": {
-                "md5": "ff4bf804ef3722a1fd8853a8a32513d4",
                 "sha256": "0c8deb7c8574787283c3fc08b714ee63fd6752a38d13515a9d8508798d428597"
             },
             "requires-python": ">=3.6",
             "url": "../../packages/7b/6e/7c4ce77c6ca092e94e19b78282b459e7f8270362da655cbc6a75eeb9cdd7/69-6.9.tar.gz",
             "yanked": false
         }
     ],
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch/tests/test_sync.py` & `bandersnatch-6.3.0/src/bandersnatch/tests/test_sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,29 +26,22 @@
 packages{0}any{0}f{0}foo{0}foo.zip
 pypi{0}foo{0}json
 simple{0}foo{0}index.html
 simple{0}foo{0}index.v1_html
 simple{0}foo{0}index.v1_json
 simple{0}index.html
 simple{0}index.v1_html
-simple{0}index.v1_json""".format(
-        sep
-    ) == utils.find(
-        mirror.webdir, dirs=False
-    )
+simple{0}index.v1_json""".format(sep) == utils.find(mirror.webdir, dirs=False)
 
-    assert (
-        open("web{0}simple{0}index.html".format(sep)).read()
-        == """\
+    assert open("web{0}simple{0}index.html".format(sep)).read() == """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Simple Index</title>
   </head>
   <body>
     <a href="foo/">foo</a><br/>
   </body>
 </html>"""
-    )
     # The "sync" method shouldn't update the serial
     assert open("status", "rb").read() == FAKE_SERIAL
```

#### html2text {}

```diff
@@ -5,13 +5,13 @@
 as f: f.write(FAKE_SERIAL) # Package names should be normalized by synchronize
 () specific_packages = ["Foo"] mirror.master.all_packages = AsyncMock
 (return_value={"foo": 1}) # type: ignore mirror.json_save = True # Recall
 bootstrap so we have the json dirs mirror._bootstrap() await mirror.synchronize
 (specific_packages) assert """\ json{0}foo packages{0}2.7{0}f{0}foo{0}foo.whl
 packages{0}any{0}f{0}foo{0}foo.zip pypi{0}foo{0}json simple{0}foo{0}index.html
 simple{0}foo{0}index.v1_html simple{0}foo{0}index.v1_json simple{0}index.html
-simple{0}index.v1_html simple{0}index.v1_json""".format( sep ) == utils.find
-( mirror.webdir, dirs=False ) assert ( open("web{0}simple{0}index.html".format
+simple{0}index.v1_html simple{0}index.v1_json""".format(sep) == utils.find
+(mirror.webdir, dirs=False) assert open("web{0}simple{0}index.html".format
 (sep)).read() == """\
 foo
-""" ) # The "sync" method shouldn't update the serial assert open("status",
+""" # The "sync" method shouldn't update the serial assert open("status",
 "rb").read() == FAKE_SERIAL
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch/tests/test_utils.py` & `bandersnatch-6.3.0/src/bandersnatch/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch/tests/test_verify.py` & `bandersnatch-6.3.0/src/bandersnatch/tests/test_verify.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,17 +177,15 @@
 web{0}pypi{0}bandersnatch{0}json
 web{0}pypi{0}black
 web{0}pypi{0}black{0}json
 web{0}simple
 web{0}simple{0}bandersnatch
 web{0}simple{0}bandersnatch{0}index.html
 web{0}simple{0}black
-web{0}simple{0}black{0}index.html""".format(
-        os.sep
-    )
+web{0}simple{0}black{0}index.html""".format(os.sep)
     fm = FakeMirror("_mirror_base_test")
     assert expected_mirror_layout == find(str(fm.mirror_base), True)
     fm.clean_up()
 
 
 @pytest.mark.asyncio
 async def test_delete_unowned_files() -> None:
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch/unittest.conf` & `bandersnatch-6.3.0/src/bandersnatch/unittest.conf`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch/utils.py` & `bandersnatch-6.3.0/src/bandersnatch/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os.path
 import platform
 import re
 import shutil
 import sys
 import tempfile
 from datetime import datetime
+from enum import Enum
 from pathlib import Path
 from typing import IO, Any, Generator, List, Set, Union
 from urllib.parse import urlparse
 
 import aiohttp
 from packaging.tags import INTERPRETER_SHORT_NAMES
 
@@ -33,14 +34,23 @@
 
 
 SAFE_NAME_REGEX = re.compile(r"[^A-Za-z0-9.]+")
 USER_AGENT = user_agent()
 WINDOWS = bool(platform.system() == "Windows")
 
 
+class StrEnum(str, Enum):
+    """Enumeration class where members can be treated as strings."""
+
+    value: str
+
+    def __str__(self) -> str:
+        return self.value
+
+
 def make_time_stamp() -> str:
     """Helper function that returns a timestamp suitable for use
     in a filename on any OS"""
     return f"{datetime.utcnow().isoformat()}Z".replace(":", "")
 
 
 def convert_url_to_path(url: str) -> str:
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch/verify.py` & `bandersnatch-6.3.0/src/bandersnatch/verify.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch.egg-info/PKG-INFO` & `bandersnatch-6.3.0/src/bandersnatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandersnatch
-Version: 6.2.0
+Version: 6.3.0
 Summary: Mirroring tool that implements the client (mirror) side of PEP 381
 Home-page: https://github.com/pypa/bandersnatch/
 Author: Christian Theune
 Author-email: ct@flyingcircus.io
 License: Academic Free License, version 3
 Project-URL: Source Code, https://github.com/pypa/bandersnatch
 Project-URL: Change Log, https://github.com/pypa/bandersnatch/blob/master/CHANGES.md
```

### Comparing `bandersnatch-6.2.0/src/bandersnatch.egg-info/SOURCES.txt` & `bandersnatch-6.3.0/src/bandersnatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch.egg-info/entry_points.txt` & `bandersnatch-6.3.0/src/bandersnatch.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch_filter_plugins/allowlist_name.py` & `bandersnatch-6.3.0/src/bandersnatch_filter_plugins/allowlist_name.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch_filter_plugins/blocklist_name.py` & `bandersnatch-6.3.0/src/bandersnatch_filter_plugins/blocklist_name.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch_filter_plugins/encoding.py` & `bandersnatch-6.3.0/src/bandersnatch_filter_plugins/encoding.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch_filter_plugins/filename_name.py` & `bandersnatch-6.3.0/src/bandersnatch_filter_plugins/filename_name.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch_filter_plugins/latest_name.py` & `bandersnatch-6.3.0/src/bandersnatch_filter_plugins/latest_name.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch_filter_plugins/metadata_filter.py` & `bandersnatch-6.3.0/src/bandersnatch_filter_plugins/metadata_filter.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch_filter_plugins/prerelease_name.py` & `bandersnatch-6.3.0/src/bandersnatch_filter_plugins/prerelease_name.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch_filter_plugins/regex_name.py` & `bandersnatch-6.3.0/src/bandersnatch_filter_plugins/regex_name.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch_storage_plugins/filesystem.py` & `bandersnatch-6.3.0/src/bandersnatch_storage_plugins/filesystem.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch_storage_plugins/s3.py` & `bandersnatch-6.3.0/src/bandersnatch_storage_plugins/s3.py`

 * *Files identical despite different names*

### Comparing `bandersnatch-6.2.0/src/bandersnatch_storage_plugins/swift.py` & `bandersnatch-6.3.0/src/bandersnatch_storage_plugins/swift.py`

 * *Files identical despite different names*


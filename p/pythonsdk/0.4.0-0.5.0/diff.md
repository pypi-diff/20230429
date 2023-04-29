# Comparing `tmp/pythonsdk-0.4.0.tar.gz` & `tmp/pythonsdk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsdk-0.4.0.tar", last modified: Mon Apr 24 08:36:06 2023, max compression
+gzip compressed data, was "pythonsdk-0.5.0.tar", last modified: Sat Apr 29 21:37:37 2023, max compression
```

## Comparing `pythonsdk-0.4.0.tar` & `pythonsdk-0.5.0.tar`

### file list

```diff
@@ -1,93 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:36:06.697134 pythonsdk-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.685134 pythonsdk-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.685134 pythonsdk-0.4.0/src/python_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.689134 pythonsdk-0.4.0/src/python_sdk/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/_cli/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/_cli/_fmt.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/_cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.689134 pythonsdk-0.4.0/src/python_sdk/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/bin/_call.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.689134 pythonsdk-0.4.0/src/python_sdk/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_config_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_config_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_config_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_config_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_config_value_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_config_value_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_optional_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_string_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.689134 pythonsdk-0.4.0/src/python_sdk/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/encoding/_base64url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.689134 pythonsdk-0.4.0/src/python_sdk/log/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_log.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_log_levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.689134 pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/_structured_human_readable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/_structured_machine_readable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/_rotating_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/_stderr.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/python_sdk/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/python_sdk/sentinel/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/sentinel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/sentinel/_sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/python_sdk/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/testing/_prepackaged_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/python_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_which.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_zipfile.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 08:36:01.000000 pythonsdk-0.4.0/src/python_sdk/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/python_sdk/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/versioning/_version_file_based.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/pythonsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-24 08:36:06.000000 pythonsdk-0.4.0/src/pythonsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-24 08:36:06.000000 pythonsdk-0.4.0/src/pythonsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:36:06.000000 pythonsdk-0.4.0/src/pythonsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 08:36:06.000000 pythonsdk-0.4.0/src/pythonsdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 08:36:06.000000 pythonsdk-0.4.0/src/pythonsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 08:36:06.000000 pythonsdk-0.4.0/src/pythonsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.114232 pythonsdk-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.118232 pythonsdk-0.5.0/src/python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.118232 pythonsdk-0.5.0/src/python_sdk/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/_cli/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/_cli/_fmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/_cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.118232 pythonsdk-0.5.0/src/python_sdk/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/bin/_call.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.118232 pythonsdk-0.5.0/src/python_sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_config_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_config_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_config_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_config_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_config_value_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_config_value_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_optional_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_string_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.118232 pythonsdk-0.5.0/src/python_sdk/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/encoding/_base64url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.118232 pythonsdk-0.5.0/src/python_sdk/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.118232 pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_structured_human_readable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_structured_machine_readable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/_rotating_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/_stderr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/python_sdk/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/python_sdk/sentinel/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/sentinel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/sentinel/_sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/python_sdk/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/testing/_prepackaged_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/python_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/_file_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/_zipfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 21:37:31.000000 pythonsdk-0.5.0/src/python_sdk/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/python_sdk/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/versioning/_version_file_based.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/pythonsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-29 21:37:37.000000 pythonsdk-0.5.0/src/pythonsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-29 21:37:37.000000 pythonsdk-0.5.0/src/pythonsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:37:37.000000 pythonsdk-0.5.0/src/pythonsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-29 21:37:37.000000 pythonsdk-0.5.0/src/pythonsdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-29 21:37:37.000000 pythonsdk-0.5.0/src/pythonsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 21:37:37.000000 pythonsdk-0.5.0/src/pythonsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/version
```

### Comparing `pythonsdk-0.4.0/LICENSE` & `pythonsdk-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/PKG-INFO` & `pythonsdk-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonsdk
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python Software Dev Kit
 Author-email: lijok <lijok@pm.me>
 License: MIT License
         
         Copyright (c) 2023 Lijok
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pythonsdk-0.4.0/pyproject.toml` & `pythonsdk-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/_cli/_cli.py` & `pythonsdk-0.5.0/src/python_sdk/_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/_cli/_fmt.py` & `pythonsdk-0.5.0/src/python_sdk/_cli/_fmt.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/bin/_call.py` & `pythonsdk-0.5.0/src/python_sdk/bin/_call.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,124 @@
 import dataclasses
 import functools
 import logging
 import os
 import pathlib
+import shutil
 import subprocess
+import sys
 import typing
 
-from python_sdk import utils
 
-
-@dataclasses.dataclass
-class BinaryNotInstalled(FileNotFoundError):
+class BinaryNotInstalled(Exception):
+    message: str
     binary: str
 
+    def __init__(self, binary: str, message: str = "Binary not installed.") -> None:
+        super().__init__(message, binary)
+        self.message = message
+        self.binary = binary
+
     def __str__(self) -> str:
         return self.binary
 
 
 class CalledProcessError(Exception):
-    def __init__(self, message: str, output: str, exit_code: int) -> None:
+    message: str
+    output: str
+    exit_code: int
+
+    def __init__(self, output: str, exit_code: int, message: str = "Called process failure.") -> None:
         super().__init__(message, output, exit_code)
+        self.message = message
         self.output = output
         self.exit_code = exit_code
 
     def __str__(self) -> str:
         return f"{self.exit_code}\n{self.output}"
 
 
 def call(
     *args: typing.Any,
     sudo: bool = False,
     sudo_binary: str = "sudo",
     environment_variables: dict[str, str] | None = None,
     stream_output: bool = False,
-    stream_printer: typing.Callable[[str], None] = functools.partial(print, end="", flush=True),
+    stream_printer: typing.Callable[[str], None] = functools.partial(print, end="", file=sys.stderr, flush=True),
     force_arch: typing.Literal["amd64", "x86_64"] | None = None,
     stdin: typing.TextIO | None = None,
+    cwd: pathlib.Path | None = None,
 ) -> str:
     """
     Raises:
         BinaryNotInstalled: binary not installed
     """
     env = environment_variables if environment_variables is not None else dict(os.environ)
+    arguments = [str(argument) for argument in args]
+
+    if args[0] == "arch":
+        # Caller supplied arch in args, instead of the force_arch argument. Let's pull it out.
+        force_arch = args[1]
+        arguments = list(args[2:])
+
+    if args[0].endswith("sudo"):
+        # Caller supplied sudo in args, instead of the sudo argument. Let's pull it out.
+        sudo = True
+        sudo_binary = args[0]
+        arguments = list(args[1:])
+
+    if sudo:
+        path_to_sudo = shutil.which(sudo_binary)
+        if not path_to_sudo:
+            raise BinaryNotInstalled(binary=sudo_binary)
+        sudo_full_path = pathlib.Path(path_to_sudo)
+        if not sudo_full_path.exists():
+            raise BinaryNotInstalled(binary=str(sudo_full_path))
+        if not os.access(sudo_full_path, os.EX_OK):
+            raise PermissionError(f"{sudo_full_path} is not executable.")
 
     binary: str = args[0]
-    arguments: typing.Any = [str(argument) for argument in args[1:]]
+    arguments = list(args[1:])
 
-    try:
-        binary_full_path = utils.which(binary)
-        sudo_full_path = utils.which(sudo_binary)
-    except FileNotFoundError as e:
-        raise BinaryNotInstalled(binary=e.filename) from e
+    path_to_binary = shutil.which(binary)
+    if not path_to_binary:
+        raise BinaryNotInstalled(binary=binary)
+    binary_full_path = pathlib.Path(path_to_binary)
+    if not binary_full_path.exists():
+        raise BinaryNotInstalled(binary=str(binary_full_path))
+    if not os.access(binary_full_path, os.EX_OK):
+        raise PermissionError(f"{binary_full_path} is not executable.")
 
     command: list[str | pathlib.Path] = [binary_full_path] + arguments
     if sudo:
         command.insert(0, sudo_full_path)
     if force_arch:
         command.insert(0, "arch")
         command.insert(1, f"-{force_arch}")
 
     logging.debug(f"Calling command. binary={binary_full_path} {command=}")
     process = subprocess.Popen(
-        command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, stdin=stdin, text=True, env=env
+        command,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+        stdin=stdin,
+        text=True,
+        env=env,
+        cwd=cwd,
     )
 
     output = ""
-    for line in iter(process.stdout.readline, ""):  # type: ignore
-        output += line
+    for char in iter(functools.partial(process.stdout.read, 1), ""):  # type: ignore
+        output += char
         if stream_output:
-            stream_printer(line)
+            stream_printer(char)
 
     logging.debug(
         f"Called command output. binary={binary_full_path} {command=} {output=} exit_code={process.returncode}"
     )
 
     process.wait()
 
     if process.returncode:
-        raise CalledProcessError("Called process failure.", output=output, exit_code=process.returncode)
+        raise CalledProcessError(output=output, exit_code=process.returncode)
 
     return output.strip()
```

### Comparing `pythonsdk-0.4.0/src/python_sdk/config/__init__.py` & `pythonsdk-0.5.0/src/python_sdk/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/config/_config.py` & `pythonsdk-0.5.0/src/python_sdk/config/_config.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/config/_config_option.py` & `pythonsdk-0.5.0/src/python_sdk/config/_config_option.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/config/_config_sources.py` & `pythonsdk-0.5.0/src/python_sdk/config/_config_sources.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/config/_config_value_types.py` & `pythonsdk-0.5.0/src/python_sdk/config/_config_value_types.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/config/_config_value_validators.py` & `pythonsdk-0.5.0/src/python_sdk/config/_config_value_validators.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/config/_string_decoder.py` & `pythonsdk-0.5.0/src/python_sdk/config/_string_decoder.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/encoding/_base64url.py` & `pythonsdk-0.5.0/src/python_sdk/encoding/_base64url.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/log/__init__.py` & `pythonsdk-0.5.0/src/python_sdk/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/log/_base.py` & `pythonsdk-0.5.0/src/python_sdk/log/_base.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/log/_config.py` & `pythonsdk-0.5.0/src/python_sdk/log/_config.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/log/_context.py` & `pythonsdk-0.5.0/src/python_sdk/log/_context.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/log/_log.py` & `pythonsdk-0.5.0/src/python_sdk/log/_log.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/log/_logger.py` & `pythonsdk-0.5.0/src/python_sdk/log/_logger.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/_factory.py` & `pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_factory.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/_protocol.py` & `pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_protocol.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/_structured_human_readable.py` & `pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_structured_human_readable.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/_structured_machine_readable.py` & `pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_structured_machine_readable.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/_factory.py` & `pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/_factory.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/_rotating_file.py` & `pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/_rotating_file.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/secrets/__init__.py` & `pythonsdk-0.5.0/src/python_sdk/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/secrets/_config.py` & `pythonsdk-0.5.0/src/python_sdk/secrets/_config.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py` & `pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py` & `pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py` & `pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_factory.py` & `pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_factory.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_protocol.py` & `pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_protocol.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/sentinel/_sentinel.py` & `pythonsdk-0.5.0/src/python_sdk/sentinel/_sentinel.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/testing/_prepackaged_tests.py` & `pythonsdk-0.5.0/src/python_sdk/testing/_prepackaged_tests.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/utils/__init__.py` & `pythonsdk-0.5.0/src/python_sdk/utils/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from python_sdk.utils._ansi import remove_ansi_escape_sequences as remove_ansi_escape_sequences
 from python_sdk.utils._checksum import get_file_sha1 as get_file_sha1
 from python_sdk.utils._connectivity import is_connected as is_connected
 from python_sdk.utils._file_watcher import FileStats as FileStats
 from python_sdk.utils._file_watcher import file_watcher as file_watcher
 from python_sdk.utils._flag import BoolFlag as BoolFlag
 from python_sdk.utils._templates import render_template as render_template
-from python_sdk.utils._which import which as which
 from python_sdk.utils._zipfile import ZipFileWithPermissions as ZipFileWithPermissions
```

### Comparing `pythonsdk-0.4.0/src/python_sdk/utils/_file_watcher.py` & `pythonsdk-0.5.0/src/python_sdk/utils/_file_watcher.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/python_sdk/utils/_zipfile.py` & `pythonsdk-0.5.0/src/python_sdk/utils/_zipfile.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.4.0/src/pythonsdk.egg-info/PKG-INFO` & `pythonsdk-0.5.0/src/pythonsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonsdk
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python Software Dev Kit
 Author-email: lijok <lijok@pm.me>
 License: MIT License
         
         Copyright (c) 2023 Lijok
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pythonsdk-0.4.0/src/pythonsdk.egg-info/SOURCES.txt` & `pythonsdk-0.5.0/src/pythonsdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 src/python_sdk/utils/__init__.py
 src/python_sdk/utils/_ansi.py
 src/python_sdk/utils/_checksum.py
 src/python_sdk/utils/_connectivity.py
 src/python_sdk/utils/_file_watcher.py
 src/python_sdk/utils/_flag.py
 src/python_sdk/utils/_templates.py
-src/python_sdk/utils/_which.py
 src/python_sdk/utils/_zipfile.py
 src/python_sdk/versioning/__init__.py
 src/python_sdk/versioning/_version_file_based.py
 src/pythonsdk.egg-info/PKG-INFO
 src/pythonsdk.egg-info/SOURCES.txt
 src/pythonsdk.egg-info/dependency_links.txt
 src/pythonsdk.egg-info/entry_points.txt
```


# Comparing `tmp/invoke-2.0.1.tar.gz` & `tmp/invoke-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpew24n5pc/dist/invoke-2.0.1.tar", last modified: Sat Apr 29 18:09:35 2023, max compression
+gzip compressed data, was "/tmp/tmpgntf1yl8/dist/invoke-2.1.0.tar", last modified: Fri Apr 28 20:11:51 2023, max compression
```

## Comparing `invoke-2.0.1.tar` & `invoke-2.1.0.tar`

### file list

```diff
@@ -1,215 +1,214 @@
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/
--rw-r--r--   0 jforcier  (1000) users      (100)     1314 2021-12-23 21:30:34.000000 invoke-2.0.1/LICENSE
--rw-r--r--   0 jforcier  (1000) users      (100)      393 2023-04-29 17:40:06.000000 invoke-2.0.1/dev-requirements.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      273 2022-03-18 21:53:07.000000 invoke-2.0.1/MANIFEST.in
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/sites/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/sites/docs/
--rw-r--r--   0 jforcier  (1000) users      (100)      445 2023-02-16 19:54:15.000000 invoke-2.0.1/sites/docs/conf.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/sites/docs/api/
--rw-r--r--   0 jforcier  (1000) users      (100)      157 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/api/util.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       68 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/api/program.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      229 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/api/loader.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      156 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/api/collection.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       96 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/api/runners.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       63 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/api/__init__.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       76 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/api/terminals.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       64 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/api/config.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      401 2023-01-12 23:12:21.000000 invoke-2.0.1/sites/docs/api/parser.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       60 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/api/tasks.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       68 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/api/context.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/api/exceptions.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/api/executor.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       72 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/api/watchers.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    12466 2022-05-11 15:59:13.000000 invoke-2.0.1/sites/docs/invoke.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     7640 2022-05-11 15:59:13.000000 invoke-2.0.1/sites/docs/getting-started.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      943 2022-05-11 15:59:13.000000 invoke-2.0.1/sites/docs/index.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/sites/docs/_static/
--rw-r--r--   0 jforcier  (1000) users      (100)    15260 2021-12-23 21:30:34.000000 invoke-2.0.1/sites/docs/_static/rtd.css
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/sites/docs/concepts/
--rw-r--r--   0 jforcier  (1000) users      (100)    16705 2023-01-07 00:40:53.000000 invoke-2.0.1/sites/docs/concepts/invoking-tasks.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    11750 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/concepts/namespaces.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     9234 2023-02-17 20:13:42.000000 invoke-2.0.1/sites/docs/concepts/library.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    10180 2023-01-07 00:40:50.000000 invoke-2.0.1/sites/docs/concepts/testing.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2917 2022-05-11 15:59:13.000000 invoke-2.0.1/sites/docs/concepts/loading.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2424 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/docs/concepts/watchers.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    17701 2023-01-07 00:40:50.000000 invoke-2.0.1/sites/docs/concepts/configuration.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1367 2023-02-16 19:54:15.000000 invoke-2.0.1/sites/shared_conf.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/sites/www/
--rw-r--r--   0 jforcier  (1000) users      (100)     1218 2022-05-11 15:59:13.000000 invoke-2.0.1/sites/www/contact.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    76317 2023-04-29 18:09:34.000000 invoke-2.0.1/sites/www/changelog.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      753 2023-01-07 00:40:50.000000 invoke-2.0.1/sites/www/installing.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1791 2022-05-11 15:59:13.000000 invoke-2.0.1/sites/www/development.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2537 2022-03-25 22:40:47.000000 invoke-2.0.1/sites/www/prior-art.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2801 2022-05-11 15:59:13.000000 invoke-2.0.1/sites/www/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     8153 2023-01-07 00:40:50.000000 invoke-2.0.1/sites/www/faq.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      703 2023-02-16 19:54:15.000000 invoke-2.0.1/sites/www/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3290 2023-04-29 18:09:35.000000 invoke-2.0.1/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)     1328 2022-05-11 15:59:13.000000 invoke-2.0.1/README.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/invoke.egg-info/
--rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-04-29 18:09:35.000000 invoke-2.0.1/invoke.egg-info/top_level.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       82 2023-04-29 18:09:35.000000 invoke-2.0.1/invoke.egg-info/entry_points.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     5100 2023-04-29 18:09:35.000000 invoke-2.0.1/invoke.egg-info/SOURCES.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-04-29 18:09:35.000000 invoke-2.0.1/invoke.egg-info/dependency_links.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     3290 2023-04-29 18:09:35.000000 invoke-2.0.1/invoke.egg-info/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)     3737 2023-04-29 17:40:06.000000 invoke-2.0.1/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2711 2023-02-17 20:13:42.000000 invoke-2.0.1/setup.py
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-04-29 18:09:35.000000 invoke-2.0.1/setup.cfg
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/
--rw-r--r--   0 jforcier  (1000) users      (100)    22668 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/parser_parser.py
--rw-r--r--   0 jforcier  (1000) users      (100)    33509 2023-02-17 20:13:42.000000 invoke-2.0.1/tests/collection.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12116 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/parser_context.py
--rw-r--r--   0 jforcier  (1000) users      (100)    29680 2023-02-17 20:13:42.000000 invoke-2.0.1/tests/context.py
--rw-r--r--   0 jforcier  (1000) users      (100)    44633 2023-02-17 20:13:42.000000 invoke-2.0.1/tests/config.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2895 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/conftest.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3261 2023-02-17 20:13:42.000000 invoke-2.0.1/tests/concurrency.py
--rw-r--r--   0 jforcier  (1000) users      (100)    56042 2023-04-28 19:58:26.000000 invoke-2.0.1/tests/program.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7179 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/parser_argument.py
--rw-r--r--   0 jforcier  (1000) users      (100)    70584 2023-04-29 18:01:39.000000 invoke-2.0.1/tests/runners.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4239 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/watchers.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1661 2023-02-17 20:13:42.000000 invoke-2.0.1/tests/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)    17268 2023-02-17 20:13:42.000000 invoke-2.0.1/tests/task.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12415 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7687 2023-02-17 20:13:42.000000 invoke-2.0.1/tests/completion.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4550 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/merge_dicts.py
--rw-r--r--   0 jforcier  (1000) users      (100)     9820 2023-02-17 20:13:42.000000 invoke-2.0.1/tests/_util.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/branch/
--rw-r--r--   0 jforcier  (1000) users      (100)       73 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/branch/explicit.py
--rw-r--r--   0 jforcier  (1000) users      (100)       86 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/branch/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)       96 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/tasks.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/configs/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/configs/yaml/
--rw-r--r--   0 jforcier  (1000) users      (100)       89 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/configs/yaml/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)      127 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/configs/yaml/explicit.py
--rw-r--r--   0 jforcier  (1000) users      (100)       35 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/configs/yaml/invoke.yaml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/configs/underscores/
--rw-r--r--   0 jforcier  (1000) users      (100)       68 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/configs/underscores/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)       32 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/configs/underscores/invoke.yaml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/configs/all-four/
--rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/configs/all-four/invoke.py
--rw-r--r--   0 jforcier  (1000) users      (100)       40 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/configs/all-four/invoke.yaml
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/configs/all-four/invoke.yml
--rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/configs/all-four/invoke.json
--rw-r--r--   0 jforcier  (1000) users      (100)       89 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/configs/runtime.py
--rw-r--r--   0 jforcier  (1000) users      (100)       19 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/configs/no-echo.yaml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/configs/nested/
--rw-r--r--   0 jforcier  (1000) users      (100)       35 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/configs/nested/invoke.yaml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/configs/python/
--rw-r--r--   0 jforcier  (1000) users      (100)       40 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/configs/python/invoke.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/configs/json/
--rw-r--r--   0 jforcier  (1000) users      (100)       41 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/configs/json/invoke.json
--rw-r--r--   0 jforcier  (1000) users      (100)       18 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/configs/echo.yaml
--rw-r--r--   0 jforcier  (1000) users      (100)       23 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/configs/no-dedupe.yaml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/configs/yml/
--rw-r--r--   0 jforcier  (1000) users      (100)       34 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/configs/yml/invoke.yml
--rw-r--r--   0 jforcier  (1000) users      (100)      126 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/configs/yml/explicit.py
--rw-r--r--   0 jforcier  (1000) users      (100)       88 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/configs/yml/tasks.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/configs/three-of-em/
--rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/configs/three-of-em/invoke.py
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/configs/three-of-em/invoke.yml
--rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/configs/three-of-em/invoke.json
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/configs/json-and-python/
--rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/configs/json-and-python/invoke.json
--rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/configs/json-and-python/invoke.py
--rw-r--r--   0 jforcier  (1000) users      (100)      173 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/configs/collection.py
--rw-r--r--   0 jforcier  (1000) users      (100)      157 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/sudo_prompt.py
--rw-r--r--   0 jforcier  (1000) users      (100)       85 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/subcollection_task_name.py
--rw-r--r--   0 jforcier  (1000) users      (100)      121 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/empty_subcollection.py
--rw-r--r--   0 jforcier  (1000) users      (100)      178 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/simple_ns_list.py
--rw-r--r--   0 jforcier  (1000) users      (100)       57 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/custom_executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/oops.py
--rw-r--r--   0 jforcier  (1000) users      (100)      194 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/deeper_ns_list.py
--rw-r--r--   0 jforcier  (1000) users      (100)      276 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/docstrings.py
--rw-r--r--   0 jforcier  (1000) users      (100)       78 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/alias_sorting.py
--rw-r--r--   0 jforcier  (1000) users      (100)      919 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/decorators.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/ignoreme/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/ignoreme/ignoremetoo/
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/ignoreme/ignoremetoo/.no
--rw-r--r--   0 jforcier  (1000) users      (100)      226 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/foo.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/tree/
--rw-r--r--   0 jforcier  (1000) users      (100)      653 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/tree/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)      301 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/tree/deploy.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/tree/build/
--rw-r--r--   0 jforcier  (1000) users      (100)      274 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/tree/build/docs.py
--rw-r--r--   0 jforcier  (1000) users      (100)      421 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/tree/build/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)      278 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/tree/build/python.py
--rw-r--r--   0 jforcier  (1000) users      (100)      171 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/tree/provision.py
--rw-r--r--   0 jforcier  (1000) users      (100)      365 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/autoprint.py
--rw-r--r--   0 jforcier  (1000) users      (100)       35 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/has_modules.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/tests/_support/package/
--rw-r--r--   0 jforcier  (1000) users      (100)       56 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/package/module.py
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/package/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)      264 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/explicit_root.py
--rw-r--r--   0 jforcier  (1000) users      (100)      511 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/depth_first.py
--rw-r--r--   0 jforcier  (1000) users      (100)      116 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/decorator_multi_default.py
--rw-r--r--   0 jforcier  (1000) users      (100)      395 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/contextualized.py
--rw-r--r--   0 jforcier  (1000) users      (100)      425 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/nontrivial_docstrings.py
--rw-r--r--   0 jforcier  (1000) users      (100)      188 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/namespacing.py
--rw-r--r--   0 jforcier  (1000) users      (100)      666 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/integration.py
--rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/empty.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4146 2021-12-23 21:30:34.000000 invoke-2.0.1/tests/_support/tree.json
--rw-r--r--   0 jforcier  (1000) users      (100)       99 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/_support/debugging.py
--rw-r--r--   0 jforcier  (1000) users      (100)    94208 2023-04-29 18:01:32.000000 invoke-2.0.1/tests/.runners.py.swp
--rw-r--r--   0 jforcier  (1000) users      (100)     3820 2023-04-29 17:40:06.000000 invoke-2.0.1/tests/loader.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5361 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/cli.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4053 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/init.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2945 2023-02-16 19:54:15.000000 invoke-2.0.1/tests/terminals.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/invoke/
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-04-29 18:07:09.000000 invoke-2.0.1/invoke/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4882 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/watchers.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2135 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     8277 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)    48310 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/config.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7511 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/terminals.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/invoke/completion/
--rw-r--r--   0 jforcier  (1000) users      (100)     4830 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/completion/complete.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1356 2021-12-23 21:30:34.000000 invoke-2.0.1/invoke/completion/bash.completion
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/completion/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)      382 2021-12-23 21:30:34.000000 invoke-2.0.1/invoke/completion/fish.completion
--rw-r--r--   0 jforcier  (1000) users      (100)     1429 2021-12-23 21:30:34.000000 invoke-2.0.1/invoke/completion/zsh.completion
--rw-r--r--   0 jforcier  (1000) users      (100)    24760 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/context.py
--rw-r--r--   0 jforcier  (1000) users      (100)    11615 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/exceptions.py
--rw-r--r--   0 jforcier  (1000) users      (100)    36900 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/program.py
--rw-r--r--   0 jforcier  (1000) users      (100)     9376 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)      235 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/main.py
--rw-r--r--   0 jforcier  (1000) users      (100)    62747 2023-04-29 18:01:39.000000 invoke-2.0.1/invoke/runners.py
--rw-r--r--   0 jforcier  (1000) users      (100)    21970 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/collection.py
--rw-r--r--   0 jforcier  (1000) users      (100)       47 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/__main__.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/invoke/parser/
--rw-r--r--   0 jforcier  (1000) users      (100)      181 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/parser/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     9314 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/parser/context.py
--rw-r--r--   0 jforcier  (1000) users      (100)    19053 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/parser/parser.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5567 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/parser/argument.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4027 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/env.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4770 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/loader.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/invoke/vendor/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/invoke/vendor/fluidity/
--rw-r--r--   0 jforcier  (1000) users      (100)     8686 2023-02-16 19:54:22.000000 invoke-2.0.1/invoke/vendor/fluidity/machine.py
--rw-r--r--   0 jforcier  (1000) users      (100)      135 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/fluidity/backwardscompat.py
--rw-r--r--   0 jforcier  (1000) users      (100)      196 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/fluidity/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)    15649 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/vendor/decorator.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/invoke/vendor/yaml/
--rw-r--r--   0 jforcier  (1000) users      (100)    14184 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/yaml/representer.py
--rw-r--r--   0 jforcier  (1000) users      (100)     8999 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/yaml/resolver.py
--rw-r--r--   0 jforcier  (1000) users      (100)    13170 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/yaml/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)    25495 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/yaml/parser.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4883 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/yaml/composer.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3851 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/yaml/cyaml.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4165 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/yaml/serializer.py
--rw-r--r--   0 jforcier  (1000) users      (100)    51277 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/yaml/scanner.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2533 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/yaml/error.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2445 2023-02-16 19:54:22.000000 invoke-2.0.1/invoke/vendor/yaml/events.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2573 2023-02-16 19:54:22.000000 invoke-2.0.1/invoke/vendor/yaml/tokens.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2061 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/yaml/loader.py
--rw-r--r--   0 jforcier  (1000) users      (100)    28639 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/yaml/constructor.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6794 2023-02-16 19:54:22.000000 invoke-2.0.1/invoke/vendor/yaml/reader.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1440 2023-02-16 19:54:22.000000 invoke-2.0.1/invoke/vendor/yaml/nodes.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2837 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/yaml/dumper.py
--rw-r--r--   0 jforcier  (1000) users      (100)    43006 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/yaml/emitter.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:09:35.000000 invoke-2.0.1/invoke/vendor/lexicon/
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/lexicon/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1133 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/lexicon/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3223 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/lexicon/alias_dict.py
--rw-r--r--   0 jforcier  (1000) users      (100)      407 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/lexicon/attribute_dict.py
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.0.1/invoke/vendor/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)    19676 2023-04-29 17:40:06.000000 invoke-2.0.1/invoke/tasks.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke/
+-rw-r--r--   0 jforcier  (1000) users      (100)     5229 2023-04-28 20:11:24.000000 invoke-2.1.0/invoke/loader.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke/parser/
+-rw-r--r--   0 jforcier  (1000) users      (100)    19809 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/parser/parser.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      181 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/parser/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     9815 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/parser/context.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6045 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/parser/argument.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4394 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/env.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    10018 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      235 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/main.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke/vendor/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke/vendor/lexicon/
+-rw-r--r--   0 jforcier  (1000) users      (100)      407 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/lexicon/attribute_dict.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/lexicon/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3223 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/lexicon/alias_dict.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1133 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/lexicon/__init__.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke/vendor/yaml/
+-rw-r--r--   0 jforcier  (1000) users      (100)     4883 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/composer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    43006 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/emitter.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    25495 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/parser.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    13170 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2533 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/error.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    14184 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/representer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3851 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/cyaml.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8999 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/resolver.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4165 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/serializer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6794 2023-02-16 19:54:22.000000 invoke-2.1.0/invoke/vendor/yaml/reader.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    51277 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/scanner.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2837 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/dumper.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1440 2023-02-16 19:54:22.000000 invoke-2.1.0/invoke/vendor/yaml/nodes.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2445 2023-02-16 19:54:22.000000 invoke-2.1.0/invoke/vendor/yaml/events.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2573 2023-02-16 19:54:22.000000 invoke-2.1.0/invoke/vendor/yaml/tokens.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    28639 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/constructor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2061 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/loader.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke/vendor/fluidity/
+-rw-r--r--   0 jforcier  (1000) users      (100)      135 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/fluidity/backwardscompat.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      196 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/fluidity/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8686 2023-02-16 19:54:22.000000 invoke-2.1.0/invoke/vendor/fluidity/machine.py
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/__init__.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke/completion/
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/completion/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5222 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/completion/complete.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1356 2021-12-23 21:30:34.000000 invoke-2.1.0/invoke/completion/bash.completion
+-rw-r--r--   0 jforcier  (1000) users      (100)     1429 2021-12-23 21:30:34.000000 invoke-2.1.0/invoke/completion/zsh.completion
+-rw-r--r--   0 jforcier  (1000) users      (100)      382 2021-12-23 21:30:34.000000 invoke-2.1.0/invoke/completion/fish.completion
+-rw-r--r--   0 jforcier  (1000) users      (100)       47 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/__main__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    23060 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/collection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    50005 2023-04-28 20:11:24.000000 invoke-2.1.0/invoke/config.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-04-28 20:11:50.000000 invoke-2.1.0/invoke/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12227 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/exceptions.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    25486 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/context.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8065 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/terminals.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    38177 2023-04-28 19:58:26.000000 invoke-2.1.0/invoke/program.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    65307 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/runners.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5097 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/watchers.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2229 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    19946 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8855 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3290 2023-04-28 20:11:51.000000 invoke-2.1.0/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)     1314 2021-12-23 21:30:34.000000 invoke-2.1.0/LICENSE
+-rw-r--r--   0 jforcier  (1000) users      (100)     4061 2023-04-28 19:57:26.000000 invoke-2.1.0/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1250 2023-04-28 19:57:26.000000 invoke-2.1.0/pyproject.toml
+-rw-r--r--   0 jforcier  (1000) users      (100)     2711 2023-02-17 20:13:42.000000 invoke-2.1.0/setup.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke.egg-info/
+-rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-04-28 20:11:50.000000 invoke-2.1.0/invoke.egg-info/top_level.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     3290 2023-04-28 20:11:50.000000 invoke-2.1.0/invoke.egg-info/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)       82 2023-04-28 20:11:50.000000 invoke-2.1.0/invoke.egg-info/entry_points.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-04-28 20:11:50.000000 invoke-2.1.0/invoke.egg-info/dependency_links.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     5066 2023-04-28 20:11:50.000000 invoke-2.1.0/invoke.egg-info/SOURCES.txt
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/
+-rw-r--r--   0 jforcier  (1000) users      (100)    17268 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/task.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    33509 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/collection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4100 2023-04-28 20:11:24.000000 invoke-2.1.0/tests/loader.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1661 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     9820 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/_util.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/empty.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      264 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/explicit_root.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      178 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/simple_ns_list.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/oops.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      226 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/foo.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       99 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/debugging.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       57 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/custom_executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      157 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/sudo_prompt.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      194 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/deeper_ns_list.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/ignoreme/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/ignoreme/ignoremetoo/
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/ignoreme/ignoremetoo/.no
+-rw-r--r--   0 jforcier  (1000) users      (100)      116 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/decorator_multi_default.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      365 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/autoprint.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/
+-rw-r--r--   0 jforcier  (1000) users      (100)       18 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/echo.yaml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/underscores/
+-rw-r--r--   0 jforcier  (1000) users      (100)       68 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/underscores/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       32 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/underscores/invoke.yaml
+-rw-r--r--   0 jforcier  (1000) users      (100)       19 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/no-echo.yaml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/json/
+-rw-r--r--   0 jforcier  (1000) users      (100)       41 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/json/invoke.json
+-rw-r--r--   0 jforcier  (1000) users      (100)       23 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/no-dedupe.yaml
+-rw-r--r--   0 jforcier  (1000) users      (100)       89 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/runtime.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/three-of-em/
+-rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/three-of-em/invoke.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/three-of-em/invoke.json
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/three-of-em/invoke.yml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/json-and-python/
+-rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/json-and-python/invoke.json
+-rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/json-and-python/invoke.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      173 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/collection.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/yaml/
+-rw-r--r--   0 jforcier  (1000) users      (100)       89 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/yaml/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      127 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/yaml/explicit.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       35 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/yaml/invoke.yaml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/yml/
+-rw-r--r--   0 jforcier  (1000) users      (100)       88 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/yml/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      126 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/yml/explicit.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       34 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/yml/invoke.yml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/nested/
+-rw-r--r--   0 jforcier  (1000) users      (100)       35 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/nested/invoke.yaml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/all-four/
+-rw-r--r--   0 jforcier  (1000) users      (100)       40 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/all-four/invoke.yaml
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/all-four/invoke.yml
+-rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/all-four/invoke.json
+-rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/all-four/invoke.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/python/
+-rw-r--r--   0 jforcier  (1000) users      (100)       40 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/python/invoke.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/package/
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/package/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       56 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/package/module.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4146 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/tree.json
+-rw-r--r--   0 jforcier  (1000) users      (100)       78 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/alias_sorting.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      395 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/contextualized.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       35 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/has_modules.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/branch/
+-rw-r--r--   0 jforcier  (1000) users      (100)       73 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/branch/explicit.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       86 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/branch/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      919 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/decorators.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      276 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/docstrings.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      511 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/depth_first.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      425 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/nontrivial_docstrings.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      188 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/namespacing.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      666 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/integration.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      121 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/empty_subcollection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       85 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/subcollection_task_name.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/tree/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/tree/build/
+-rw-r--r--   0 jforcier  (1000) users      (100)      274 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/tree/build/docs.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      278 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/tree/build/python.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      421 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/tree/build/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      301 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/tree/deploy.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      171 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/tree/provision.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      653 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/tree/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       96 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12415 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12116 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/parser_context.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4239 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/watchers.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2895 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/conftest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3261 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/concurrency.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    44633 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/config.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    70272 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/runners.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4053 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/init.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4550 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/merge_dicts.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5361 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/cli.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    29680 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/context.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7687 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/completion.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    56042 2023-04-28 19:58:26.000000 invoke-2.1.0/tests/program.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2945 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/terminals.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    22668 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/parser_parser.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7179 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/parser_argument.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      437 2023-04-28 19:58:12.000000 invoke-2.1.0/dev-requirements.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     1328 2022-05-11 15:59:13.000000 invoke-2.1.0/README.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-04-28 20:11:51.000000 invoke-2.1.0/setup.cfg
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/sites/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/sites/www/
+-rw-r--r--   0 jforcier  (1000) users      (100)     2537 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/www/prior-art.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      753 2023-01-07 00:40:50.000000 invoke-2.1.0/sites/www/installing.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1791 2022-05-11 15:59:13.000000 invoke-2.1.0/sites/www/development.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1218 2022-05-11 15:59:13.000000 invoke-2.1.0/sites/www/contact.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     8153 2023-01-07 00:40:50.000000 invoke-2.1.0/sites/www/faq.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      703 2023-02-16 19:54:15.000000 invoke-2.1.0/sites/www/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2801 2022-05-11 15:59:13.000000 invoke-2.1.0/sites/www/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    76512 2023-04-28 20:11:47.000000 invoke-2.1.0/sites/www/changelog.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1367 2023-02-16 19:54:15.000000 invoke-2.1.0/sites/shared_conf.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/sites/docs/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/sites/docs/concepts/
+-rw-r--r--   0 jforcier  (1000) users      (100)    16705 2023-01-07 00:40:53.000000 invoke-2.1.0/sites/docs/concepts/invoking-tasks.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     9234 2023-02-17 20:13:42.000000 invoke-2.1.0/sites/docs/concepts/library.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2424 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/concepts/watchers.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    17701 2023-01-07 00:40:50.000000 invoke-2.1.0/sites/docs/concepts/configuration.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2917 2022-05-11 15:59:13.000000 invoke-2.1.0/sites/docs/concepts/loading.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    10180 2023-01-07 00:40:50.000000 invoke-2.1.0/sites/docs/concepts/testing.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    11750 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/concepts/namespaces.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     7640 2022-05-11 15:59:13.000000 invoke-2.1.0/sites/docs/getting-started.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      445 2023-02-16 19:54:15.000000 invoke-2.1.0/sites/docs/conf.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/sites/docs/_static/
+-rw-r--r--   0 jforcier  (1000) users      (100)    15260 2021-12-23 21:30:34.000000 invoke-2.1.0/sites/docs/_static/rtd.css
+-rw-r--r--   0 jforcier  (1000) users      (100)      943 2022-05-11 15:59:13.000000 invoke-2.1.0/sites/docs/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    12466 2022-05-11 15:59:13.000000 invoke-2.1.0/sites/docs/invoke.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/sites/docs/api/
+-rw-r--r--   0 jforcier  (1000) users      (100)       96 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/runners.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       68 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/program.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       60 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/tasks.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/executor.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      157 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/util.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       72 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/watchers.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/exceptions.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       63 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/__init__.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       68 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/context.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      229 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/loader.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      156 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/collection.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      401 2023-01-12 23:12:21.000000 invoke-2.1.0/sites/docs/api/parser.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       76 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/terminals.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       64 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/config.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      273 2022-03-18 21:53:07.000000 invoke-2.1.0/MANIFEST.in
```

### Comparing `invoke-2.0.1/LICENSE` & `invoke-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/docs/invoke.rst` & `invoke-2.1.0/sites/docs/invoke.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/docs/getting-started.rst` & `invoke-2.1.0/sites/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/docs/index.rst` & `invoke-2.1.0/sites/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/docs/_static/rtd.css` & `invoke-2.1.0/sites/docs/_static/rtd.css`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/docs/concepts/invoking-tasks.rst` & `invoke-2.1.0/sites/docs/concepts/invoking-tasks.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/docs/concepts/namespaces.rst` & `invoke-2.1.0/sites/docs/concepts/namespaces.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/docs/concepts/library.rst` & `invoke-2.1.0/sites/docs/concepts/library.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/docs/concepts/testing.rst` & `invoke-2.1.0/sites/docs/concepts/testing.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/docs/concepts/loading.rst` & `invoke-2.1.0/sites/docs/concepts/loading.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/docs/concepts/watchers.rst` & `invoke-2.1.0/sites/docs/concepts/watchers.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/docs/concepts/configuration.rst` & `invoke-2.1.0/sites/docs/concepts/configuration.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/shared_conf.py` & `invoke-2.1.0/sites/shared_conf.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/www/contact.rst` & `invoke-2.1.0/sites/www/contact.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/www/changelog.rst` & `invoke-2.1.0/sites/www/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 =========
 Changelog
 =========
 
-- :release:`2.0.1 <2023-04-29>`
-- :bug:`910` Add more rigor around subprocess/runner shutdown to avoid spurious
-  exceptions & also fix downstream issues in libraries like Fabric. Reported by
-  Orlando Rodríguez.
+- :release:`2.1.0 <2023-04-28>`
+- :support:`675` Implement `importlib` and deprecate `imp` module. Patches
+  provided by Jesse P. Johnson
+- :bug:`376` Resolve equality comparison bug for non-collections. Patch via
+  Jesse P. Johnson
+- :support:`906` Implement type hints and type checking tests with mypy to
+  reduce errors and impove code documentation. Patches by Jesse P. Johnson and
+  review by Sam Bull.
 - :support:`901 backported` (via :issue:`903`) Tweak test suite ``setup``
   methods to be named ``setup_method`` so pytest stops whining about it. Patch
   via Jesse P. Johnson.
 - :release:`2.0.0 <2023-01-16>`
 - :support:`-` Remove support for, and imports related to, all Python versions
   less than 3.6 - including Python 2. This also includes updates to vendored
   packages, such as removing ``six`` and upgrading ``lexicon`` to the latest
```

### Comparing `invoke-2.0.1/sites/www/installing.rst` & `invoke-2.1.0/sites/www/installing.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/www/development.rst` & `invoke-2.1.0/sites/www/development.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/www/prior-art.rst` & `invoke-2.1.0/sites/www/prior-art.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/www/index.rst` & `invoke-2.1.0/sites/www/index.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/www/faq.rst` & `invoke-2.1.0/sites/www/faq.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/sites/www/conf.py` & `invoke-2.1.0/sites/www/conf.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/PKG-INFO` & `invoke-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoke
-Version: 2.0.1
+Version: 2.1.0
 Summary: Pythonic task execution
 Home-page: https://pyinvoke.org
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Docs, https://docs.pyinvoke.org
 Project-URL: Source, https://github.com/pyinvoke/invoke
```

### Comparing `invoke-2.0.1/README.rst` & `invoke-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke.egg-info/SOURCES.txt` & `invoke-2.1.0/invoke.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.rst
 dev-requirements.txt
+pyproject.toml
 setup.py
 tasks.py
 invoke/__init__.py
 invoke/__main__.py
 invoke/_version.py
 invoke/collection.py
 invoke/config.py
@@ -32,15 +33,14 @@
 invoke/completion/fish.completion
 invoke/completion/zsh.completion
 invoke/parser/__init__.py
 invoke/parser/argument.py
 invoke/parser/context.py
 invoke/parser/parser.py
 invoke/vendor/__init__.py
-invoke/vendor/decorator.py
 invoke/vendor/fluidity/__init__.py
 invoke/vendor/fluidity/backwardscompat.py
 invoke/vendor/fluidity/machine.py
 invoke/vendor/lexicon/__init__.py
 invoke/vendor/lexicon/_version.py
 invoke/vendor/lexicon/alias_dict.py
 invoke/vendor/lexicon/attribute_dict.py
@@ -92,15 +92,14 @@
 sites/www/conf.py
 sites/www/contact.rst
 sites/www/development.rst
 sites/www/faq.rst
 sites/www/index.rst
 sites/www/installing.rst
 sites/www/prior-art.rst
-tests/.runners.py.swp
 tests/_util.py
 tests/cli.py
 tests/collection.py
 tests/completion.py
 tests/concurrency.py
 tests/config.py
 tests/conftest.py
```

### Comparing `invoke-2.0.1/invoke.egg-info/PKG-INFO` & `invoke-2.1.0/invoke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoke
-Version: 2.0.1
+Version: 2.1.0
 Summary: Pythonic task execution
 Home-page: https://pyinvoke.org
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Docs, https://docs.pyinvoke.org
 Project-URL: Source, https://github.com/pyinvoke/invoke
```

### Comparing `invoke-2.0.1/tasks.py` & `invoke-2.1.0/tasks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,66 @@
 import os
+from typing import TYPE_CHECKING, Optional
 
 from invoke import Collection, task, Exit
 
 from invocations import ci, checks
 from invocations.docs import docs, www, sites, watch_docs
 from invocations.pytest import coverage as coverage_, test as test_
 from invocations.packaging import vendorize, release
 
+if TYPE_CHECKING:
+    from invoke import Context
+
 
 @task
 def test(
-    c,
-    verbose=False,
-    color=True,
-    capture="no",
-    module=None,
-    k=None,
-    x=False,
-    opts="",
-    pty=True,
-):
+    c: "Context",
+    verbose: bool = False,
+    color: bool = True,
+    capture: str = "no",
+    module: Optional[str] = None,
+    k: Optional[str] = None,
+    x: bool = False,
+    opts: str = "",
+    pty: bool = True,
+) -> None:
     """
     Run pytest. See `invocations.pytest.test` for details.
 
     This is a simple wrapper around the abovementioned task, which makes a
     couple minor defaults changes appropriate for this particular test suite,
     such as:
 
     - setting ``capture=no`` instead of ``capture=sys``, as we do a very large
       amount of subprocess IO testing that even the ``sys``  capture screws up
     - setting ``verbose=False`` because we have a large number of tests and
       skipping verbose output by default is a ~20% time savings.)
     """
     # TODO: update test suite to use c.config.run.in_stream = False globally.
     # somehow.
-    return test_(
+    test_(
         c,
         verbose=verbose,
         color=color,
         capture=capture,
         module=module,
         k=k,
         x=x,
         opts=opts,
         pty=pty,
     )
 
 
 # TODO: replace with invocations' once the "call truly local tester" problem is
 # solved (see other TODOs). For now this is just a copy/paste/modify.
-@task(help=test.help)
-def integration(c, opts=None, pty=True):
+@task(help=test.help)  # type: ignore
+def integration(
+    c: "Context", opts: Optional[str] = None, pty: bool = True
+) -> None:
     """
     Run the integration test suite. May be slow!
     """
     # Abort if no default shell on this system - implies some unusual dev
     # environment. Certain entirely-standalone tests will fail w/o it, even if
     # tests honoring config overrides (like the unit-test suite) don't.
     shell = c.config.global_defaults()["run"]["shell"]
@@ -63,15 +69,17 @@
         raise Exit(err.format(shell))
     opts = opts or ""
     opts += " integration/"
     test(c, opts=opts, pty=pty)
 
 
 @task
-def coverage(c, report="term", opts="", codecov=False):
+def coverage(
+    c: "Context", report: str = "term", opts: str = "", codecov: bool = False
+) -> None:
     """
     Run pytest in coverage mode. See `invocations.pytest.coverage` for details.
     """
     # Use our own test() instead of theirs.
     # Also add integration test so this always hits both.
     # (Not regression, since that's "weird" / doesn't really hit any new
     # coverage points)
@@ -82,15 +90,15 @@
         tester=test,
         additional_testers=[integration],
         codecov=codecov,
     )
 
 
 @task
-def regression(c, jobs=8):
+def regression(c: "Context", jobs: int = 8) -> None:
     """
     Run an expensive, hard-to-test-in-pytest run() regression checker.
 
     :param int jobs: Number of jobs to run, in total. Ideally num of CPUs.
     """
     os.chdir("integration/_support")
     cmd = "seq {} | parallel -n0 --halt=now,fail=1 inv -c regression check"
```

### Comparing `invoke-2.0.1/setup.py` & `invoke-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/parser_parser.py` & `invoke-2.1.0/tests/parser_parser.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/collection.py` & `invoke-2.1.0/tests/collection.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/parser_context.py` & `invoke-2.1.0/tests/parser_context.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/context.py` & `invoke-2.1.0/tests/context.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/config.py` & `invoke-2.1.0/tests/config.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/conftest.py` & `invoke-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/concurrency.py` & `invoke-2.1.0/tests/concurrency.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/program.py` & `invoke-2.1.0/tests/program.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/parser_argument.py` & `invoke-2.1.0/tests/parser_argument.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/runners.py` & `invoke-2.1.0/tests/runners.py`

 * *Files 0% similar despite different names*

```diff
@@ -1398,14 +1398,19 @@
         def run_always_stops_timer(self):
             runner = _GenericExceptingRunner(Context())
             runner._timer = Mock()
             with raises(_GenericException):
                 runner.run(_)
             runner._timer.cancel.assert_called_once_with()
 
+        def stop_cancels_timer(self):
+            runner = self._mocked_timer()
+            runner.stop()
+            runner._timer.cancel.assert_called_once_with()
+
         def timer_aliveness_is_test_of_timing_out(self):
             # Might be redundant, but easy enough to unit test
             runner = Runner(Context())
             runner._timer = Mock()
             runner._timer.is_alive.return_value = False
             assert runner.timed_out
             runner._timer.is_alive.return_value = True
@@ -1421,20 +1426,14 @@
         def always_runs_no_matter_what(self):
             runner = _GenericExceptingRunner(context=Context())
             runner.stop = Mock()
             with raises(_GenericException):
                 runner.run(_)
             runner.stop.assert_called_once_with()
 
-        def cancels_timer(self):
-            runner = self._runner()
-            runner._timer = Mock()
-            runner.stop()
-            runner._timer.cancel.assert_called_once_with()
-
     class asynchronous:
         def returns_Promise_immediately_and_finishes_on_join(self):
             # Dummy subclass with controllable process_is_finished flag
             class _Finisher(_Dummy):
                 _finished = False
 
                 @property
@@ -1531,23 +1530,14 @@
 class Local_:
     def _run(self, *args, **kwargs):
         return _run(*args, **dict(kwargs, klass=_FastLocal))
 
     def _runner(self, *args, **kwargs):
         return _runner(*args, **dict(kwargs, klass=_FastLocal))
 
-    class stop:
-        @mock_subprocess()
-        def calls_super(self):
-            # Re #910
-            runner = self._runner()
-            runner._timer = Mock()  # twiddled by parent class stop()
-            runner.run(_)
-            runner._timer.cancel.assert_called_once_with()
-
     class pty:
         @mock_pty()
         def when_pty_True_we_use_pty_fork_and_os_exec(self):
             "when pty=True, we use pty.fork and os.exec*"
             self._run(_, pty=True)
             # @mock_pty's asserts check os/pty calls for us.
```

### Comparing `invoke-2.0.1/tests/watchers.py` & `invoke-2.1.0/tests/watchers.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/util.py` & `invoke-2.1.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/task.py` & `invoke-2.1.0/tests/task.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/executor.py` & `invoke-2.1.0/tests/executor.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/completion.py` & `invoke-2.1.0/tests/completion.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/merge_dicts.py` & `invoke-2.1.0/tests/merge_dicts.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/_util.py` & `invoke-2.1.0/tests/_util.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/_support/decorators.py` & `invoke-2.1.0/tests/_support/decorators.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/_support/tree/__init__.py` & `invoke-2.1.0/tests/_support/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/_support/integration.py` & `invoke-2.1.0/tests/_support/integration.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/_support/tree.json` & `invoke-2.1.0/tests/_support/tree.json`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/loader.py` & `invoke-2.1.0/tests/loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import imp
 import os
 import sys
-import types
+from importlib.util import spec_from_file_location
+from types import ModuleType
 
 from pytest import raises
 
 from invoke import Config
 from invoke.loader import Loader, FilesystemLoader as FSLoader
 from invoke.exceptions import CollectionNotFound
 
@@ -17,27 +17,32 @@
     Tests top level Loader behavior with basic finder stub.
 
     Used when we want to make sure we're testing Loader.load and not e.g.
     FilesystemLoader's specific implementation.
     """
 
     def find(self, name):
-        self.fd, self.path, self.desc = t = imp.find_module(name, [support])
-        return t
+        path = os.path.join(support, name)
+        if os.path.exists(f"{path}.py"):
+            path = f"{path}.py"
+        elif os.path.exists(path):
+            path = os.path.join(path, "__init__.py")
+        spec = spec_from_file_location(name, path)
+        return spec
 
 
 class Loader_:
     def exhibits_default_config_object(self):
         loader = _BasicLoader()
         assert isinstance(loader.config, Config)
         assert loader.config.tasks.collection_name == "tasks"
 
     def returns_module_and_location(self):
         mod, path = _BasicLoader().load("namespacing")
-        assert isinstance(mod, types.ModuleType)
+        assert isinstance(mod, ModuleType)
         assert path == support
 
     def may_configure_config_via_constructor(self):
         config = Config({"tasks": {"collection_name": "mytasks"}})
         loader = _BasicLoader(config=config)
         assert loader.config.tasks.collection_name == "mytasks"
 
@@ -48,19 +53,14 @@
     def doesnt_dupliate_parent_dir_addition(self):
         _BasicLoader().load("namespacing")
         _BasicLoader().load("namespacing")
         # If the bug is present, this will be 2 at least (and often more, since
         # other tests will pollute it (!).
         assert sys.path.count(support) == 1
 
-    def closes_opened_file_object(self):
-        loader = _BasicLoader()
-        loader.load("foo")
-        assert loader.fd.closed
-
     def can_load_package(self):
         loader = _BasicLoader()
         # make sure it doesn't explode
         loader.load("package")
 
     def load_name_defaults_to_config_tasks_collection_name(self):
         "load() name defaults to config.tasks.collection_name"
@@ -85,30 +85,34 @@
     def discovery_start_point_defaults_to_cwd(self):
         assert FSLoader().start == os.getcwd()
 
     def exposes_start_point_as_attribute(self):
         assert FSLoader().start == os.getcwd()
 
     def start_point_is_configurable_via_kwarg(self):
-        start = "/tmp/"
+        start = "/tmp"
         assert FSLoader(start=start).start == start
 
     def start_point_is_configurable_via_config(self):
         config = Config({"tasks": {"search_root": "nowhere"}})
         assert FSLoader(config=config).start == "nowhere"
 
     def raises_CollectionNotFound_if_not_found(self):
         with raises(CollectionNotFound):
             self.loader.load("nope")
 
     def raises_ImportError_if_found_collection_cannot_be_imported(self):
         # Instead of masking with a CollectionNotFound
-        with raises(ImportError):
+        with raises(ModuleNotFoundError):
             self.loader.load("oops")
 
+    # TODO: Need CollectionImportError here
+
     def searches_towards_root_of_filesystem(self):
         # Loaded while root is in same dir as .py
         directly = self.loader.load("foo")
         # Loaded while root is multiple dirs deeper than the .py
         deep = os.path.join(support, "ignoreme", "ignoremetoo")
         indirectly = FSLoader(start=deep).load("foo")
-        assert directly == indirectly
+        assert directly[0].__file__ == indirectly[0].__file__
+        assert directly[0].__spec__ == indirectly[0].__spec__
+        assert directly[1] == indirectly[1]
```

### Comparing `invoke-2.0.1/tests/cli.py` & `invoke-2.1.0/tests/cli.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/init.py` & `invoke-2.1.0/tests/init.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/tests/terminals.py` & `invoke-2.1.0/tests/terminals.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/watchers.py` & `invoke-2.1.0/invoke/watchers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import threading
+from typing import Generator, Iterable
 
 from .exceptions import ResponseNotAccepted
 
 
 class StreamWatcher(threading.local):
     """
     A class whose subclasses may act on seen stream data from subprocesses.
@@ -30,15 +31,15 @@
         `StreamWatcher` subclasses `threading.local` so that its instances can
         be used to 'watch' both subprocess stdout and stderr in separate
         threads.
 
     .. versionadded:: 1.0
     """
 
-    def submit(self, stream):
+    def submit(self, stream: str) -> Iterable[str]:
         """
         Act on ``stream`` data, potentially returning responses.
 
         :param str stream:
             All data read on this stream since the beginning of the session.
 
         :returns:
@@ -54,15 +55,15 @@
     A parameterizable object that submits responses to specific patterns.
 
     Commonly used to implement password auto-responds for things like ``sudo``.
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, pattern, response):
+    def __init__(self, pattern: str, response: str) -> None:
         r"""
         Imprint this `Responder` with necessary parameters.
 
         :param pattern:
             A raw string (e.g. ``r"\[sudo\] password for .*:"``) which will be
             turned into a regular expression.
 
@@ -71,15 +72,17 @@
             detected.
         """
         # TODO: precompile the keys into regex objects
         self.pattern = pattern
         self.response = response
         self.index = 0
 
-    def pattern_matches(self, stream, pattern, index_attr):
+    def pattern_matches(
+        self, stream: str, pattern: str, index_attr: str
+    ) -> Iterable[str]:
         """
         Generic "search for pattern in stream, using index" behavior.
 
         Used here and in some subclasses that want to track multiple patterns
         concurrently.
 
         :param str stream: The same data passed to ``submit``.
@@ -89,23 +92,23 @@
 
         .. versionadded:: 1.0
         """
         # NOTE: generifies scanning so it can be used to scan for >1 pattern at
         # once, e.g. in FailingResponder.
         # Only look at stream contents we haven't seen yet, to avoid dupes.
         index = getattr(self, index_attr)
-        new_ = stream[index:]
+        new = stream[index:]
         # Search, across lines if necessary
-        matches = re.findall(pattern, new_, re.S)
+        matches = re.findall(pattern, new, re.S)
         # Update seek index if we've matched
         if matches:
-            setattr(self, index_attr, index + len(new_))
+            setattr(self, index_attr, index + len(new))
         return matches
 
-    def submit(self, stream):
+    def submit(self, stream: str) -> Generator[str, None, None]:
         # Iterate over findall() response in case >1 match occurred.
         for _ in self.pattern_matches(stream, self.pattern, "index"):
             yield self.response
 
 
 class FailingResponder(Responder):
     """
@@ -114,21 +117,21 @@
     This class adds a ``sentinel`` parameter to ``__init__``, and its
     ``submit`` will raise `.ResponseNotAccepted` if it detects that sentinel
     value in the stream.
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, pattern, response, sentinel):
+    def __init__(self, pattern: str, response: str, sentinel: str) -> None:
         super().__init__(pattern, response)
         self.sentinel = sentinel
         self.failure_index = 0
         self.tried = False
 
-    def submit(self, stream):
+    def submit(self, stream: str) -> Generator[str, None, None]:
         # Behave like regular Responder initially
         response = super().submit(stream)
         # Also check stream for our failure sentinel
         failed = self.pattern_matches(stream, self.sentinel, "failure_index")
         # Error out if we seem to have failed after a previous response.
         if self.tried and failed:
             err = 'Auto-response to r"{}" failed with {!r}!'.format(
```

### Comparing `invoke-2.0.1/invoke/__init__.py` & `invoke-2.1.0/invoke/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any, Optional
+
 from ._version import __version_info__, __version__  # noqa
 from .collection import Collection  # noqa
 from .config import Config  # noqa
 from .context import Context, MockContext  # noqa
 from .exceptions import (  # noqa
     AmbiguousEnvVar,
     AuthFailure,
@@ -25,15 +27,15 @@
 from .program import Program  # noqa
 from .runners import Runner, Local, Failure, Result, Promise  # noqa
 from .tasks import task, call, Call, Task  # noqa
 from .terminals import pty_size  # noqa
 from .watchers import FailingResponder, Responder, StreamWatcher  # noqa
 
 
-def run(command, **kwargs):
+def run(command: str, **kwargs: Any) -> Optional[Result]:
     """
     Run ``command`` in a subprocess and return a `.Result` object.
 
     See `.Runner.run` for API details.
 
     .. note::
         This function is a convenience wrapper around Invoke's `.Context` and
@@ -44,15 +46,15 @@
         runner subclass for command execution.
 
     .. versionadded:: 1.0
     """
     return Context().run(command, **kwargs)
 
 
-def sudo(command, **kwargs):
+def sudo(command: str, **kwargs: Any) -> Optional[Result]:
     """
     Run ``command`` in a ``sudo`` subprocess and return a `.Result` object.
 
     See `.Context.sudo` for API details, such as the ``password`` kwarg.
 
     .. note::
         This function is a convenience wrapper around Invoke's `.Context` and
```

### Comparing `invoke-2.0.1/invoke/executor.py` & `invoke-2.1.0/invoke/executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,36 @@
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
+
 from .config import Config
 from .parser import ParserContext
 from .util import debug
 from .tasks import Call, Task
 
+if TYPE_CHECKING:
+    from .collection import Collection
+    from .runners import Result
+    from .parser import ParseResult
+
 
 class Executor:
     """
     An execution strategy for Task objects.
 
     Subclasses may override various extension points to change, add or remove
     behavior.
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, collection, config=None, core=None):
+    def __init__(
+        self,
+        collection: "Collection",
+        config: Optional["Config"] = None,
+        core: Optional["ParseResult"] = None,
+    ) -> None:
         """
         Initialize executor with handles to necessary data structures.
 
         :param collection:
             A `.Collection` used to look up requested tasks (and their default
             config data, if any) by name during execution.
 
@@ -30,15 +42,17 @@
             An optional `.ParseResult` holding parsed core program arguments.
             Defaults to ``None``.
         """
         self.collection = collection
         self.config = config if config is not None else Config()
         self.core = core
 
-    def execute(self, *tasks):
+    def execute(
+        self, *tasks: Union[str, Tuple[str, Dict[str, Any]], ParserContext]
+    ) -> Dict["Task", "Result"]:
         """
         Execute one or more ``tasks`` in sequence.
 
         :param tasks:
             An all-purpose iterable of "tasks to execute", each member of which
             may take one of the following forms:
 
@@ -102,15 +116,14 @@
         # Execute
         results = {}
         # TODO: maybe clone initial config here? Probably not necessary,
         # especially given Executor is not designed to execute() >1 time at the
         # moment...
         for call in calls:
             autoprint = call in direct and call.autoprint
-            args = call.args
             debug("Executing {!r}".format(call))
             # Hand in reference to our config, which will preserve user
             # modifications across the lifetime of the session.
             config = self.config
             # But make sure we reset its task-sensitive levels each time
             # (collection & shell env)
             # TODO: load_collection needs to be skipped if task is anonymous
@@ -119,48 +132,54 @@
             config.load_collection(collection_config)
             config.load_shell_env()
             debug("Finished loading collection & shell env configs")
             # Get final context from the Call (which will know how to generate
             # an appropriate one; e.g. subclasses might use extra data from
             # being parameterized), handing in this config for use there.
             context = call.make_context(config)
-            args = (context,) + args
+            args = (context, *call.args)
             result = call.task(*args, **call.kwargs)
             if autoprint:
                 print(result)
             # TODO: handle the non-dedupe case / the same-task-different-args
             # case, wherein one task obj maps to >1 result.
             results[call.task] = result
         return results
 
-    def normalize(self, tasks):
+    def normalize(
+        self,
+        tasks: Tuple[
+            Union[str, Tuple[str, Dict[str, Any]], ParserContext], ...
+        ],
+    ) -> List["Call"]:
         """
         Transform arbitrary task list w/ various types, into `.Call` objects.
 
         See docstring for `~.Executor.execute` for details.
 
         .. versionadded:: 1.0
         """
         calls = []
         for task in tasks:
-            name, kwargs = None, {}
+            name: Optional[str]
             if isinstance(task, str):
                 name = task
+                kwargs = {}
             elif isinstance(task, ParserContext):
                 name = task.name
                 kwargs = task.as_kwargs
             else:
                 name, kwargs = task
-            c = Call(task=self.collection[name], kwargs=kwargs, called_as=name)
+            c = Call(self.collection[name], kwargs=kwargs, called_as=name)
             calls.append(c)
         if not tasks and self.collection.default is not None:
-            calls = [Call(task=self.collection[self.collection.default])]
+            calls = [Call(self.collection[self.collection.default])]
         return calls
 
-    def dedupe(self, calls):
+    def dedupe(self, calls: List["Call"]) -> List["Call"]:
         """
         Deduplicate a list of `tasks <.Call>`.
 
         :param calls: An iterable of `.Call` objects representing tasks.
 
         :returns: A list of `.Call` objects.
 
@@ -172,15 +191,15 @@
             if call not in deduped:
                 debug("{!r}: no duplicates found, ok".format(call))
                 deduped.append(call)
             else:
                 debug("{!r}: found in list already, skipping".format(call))
         return deduped
 
-    def expand_calls(self, calls):
+    def expand_calls(self, calls: List["Call"]) -> List["Call"]:
         """
         Expand a list of `.Call` objects into a near-final list of same.
 
         The default implementation of this method simply adds a task's
         pre/post-task list before/after the task itself, as necessary.
 
         Subclasses may wish to do other things in addition (or instead of) the
@@ -190,15 +209,15 @@
         .. versionadded:: 1.0
         """
         ret = []
         for call in calls:
             # Normalize to Call (this method is sometimes called with pre/post
             # task lists, which may contain 'raw' Task objects)
             if isinstance(call, Task):
-                call = Call(task=call)
+                call = Call(call)
             debug("Expanding task-call {!r}".format(call))
             # TODO: this is where we _used_ to call Executor.config_for(call,
             # config)...
             # TODO: now we may need to preserve more info like where the call
             # came from, etc, but I feel like that shit should go _on the call
             # itself_ right???
             # TODO: we _probably_ don't even want the config in here anymore,
```

### Comparing `invoke-2.0.1/invoke/config.py` & `invoke-2.1.0/invoke/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 import copy
 import json
 import os
 import types
+from importlib.util import spec_from_loader
+from os import PathLike
 from os.path import join, splitext, expanduser
+from types import ModuleType
+from typing import Any, Dict, Iterator, Optional, Tuple, Type, Union
 
 from .env import Environment
 from .exceptions import UnknownFileType, UnpicklableConfigMember
 from .runners import Local
 from .terminals import WINDOWS
 from .util import debug, yaml
 
 
 try:
     from importlib.machinery import SourceFileLoader
 except ImportError:  # PyPy3
-    from importlib._bootstrap import _SourceFileLoader as SourceFileLoader
+    from importlib._bootstrap import (  # type: ignore[no-redef]
+        _SourceFileLoader as SourceFileLoader,
+    )
 
 
-def load_source(name, path):
+def load_source(name: str, path: str) -> Dict[str, Any]:
     if not os.path.exists(path):
         return {}
-    return vars(SourceFileLoader("mod", path).load_module())
+    loader = SourceFileLoader("mod", path)
+    mod = ModuleType("mod")
+    mod.__spec__ = spec_from_loader("mod", loader)
+    loader.exec_module(mod)
+    return vars(mod)
 
 
 class DataProxy:
     """
     Helper class implementing nested dict+attr access for `.Config`.
 
     Specifically, is used both for `.Config` itself, and to wrap any other
@@ -60,15 +70,20 @@
         iter
         sizeof
     """.split()
         )
     )
 
     @classmethod
-    def from_data(cls, data, root=None, keypath=tuple()):
+    def from_data(
+        cls,
+        data: Dict[str, Any],
+        root: Optional["DataProxy"] = None,
+        keypath: Tuple[str, ...] = tuple(),
+    ) -> "DataProxy":
         """
         Alternate constructor for 'baby' DataProxies used as sub-dict values.
 
         Allows creating standalone DataProxy objects while also letting
         subclasses like `.Config` define their own ``__init__`` without
         muddling the two.
 
@@ -89,15 +104,15 @@
         """
         obj = cls()
         obj._set(_config=data)
         obj._set(_root=root)
         obj._set(_keypath=keypath)
         return obj
 
-    def __getattr__(self, key):
+    def __getattr__(self, key: str) -> Any:
         # NOTE: due to default Python attribute-lookup semantics, "real"
         # attributes will always be yielded on attribute access and this method
         # is skipped. That behavior is good for us (it's more intuitive than
         # having a config key accidentally shadow a real attribute or method).
         try:
             return self._get(key)
         except KeyError:
@@ -109,54 +124,54 @@
             attrs = [x for x in dir(self.__class__) if not x.startswith("_")]
             err += "\n\nValid keys: {!r}".format(
                 sorted(list(self._config.keys()))
             )
             err += "\n\nValid real attributes: {!r}".format(attrs)
             raise AttributeError(err)
 
-    def __setattr__(self, key, value):
+    def __setattr__(self, key: str, value: Any) -> None:
         # Turn attribute-sets into config updates anytime we don't have a real
         # attribute with the given name/key.
         has_real_attr = key in dir(self)
         if not has_real_attr:
             # Make sure to trigger our own __setitem__ instead of going direct
             # to our internal dict/cache
             self[key] = value
         else:
             super().__setattr__(key, value)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Dict[str, Any]]:
         # For some reason Python is ignoring our __hasattr__ when determining
         # whether we support __iter__. BOO
         return iter(self._config)
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         # NOTE: Can't proxy __eq__ because the RHS will always be an obj of the
         # current class, not the proxied-to class, and that causes
         # NotImplemented.
         # Try comparing to other objects like ourselves, falling back to a not
         # very comparable value (None) so comparison fails.
         other_val = getattr(other, "_config", None)
         # But we can compare to vanilla dicts just fine, since our _config is
         # itself just a dict.
         if isinstance(other, dict):
             other_val = other
-        return self._config == other_val
+        return bool(self._config == other_val)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._config)
 
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: str, value: str) -> None:
         self._config[key] = value
         self._track_modification_of(key, value)
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str) -> Any:
         return self._get(key)
 
-    def _get(self, key):
+    def _get(self, key: str) -> Any:
         # Short-circuit if pickling/copying mechanisms are asking if we've got
         # __setstate__ etc; they'll ask this w/o calling our __init__ first, so
         # we'd be in a RecursionError-causing catch-22 otherwise.
         if key in ("__setstate__",):
             raise AttributeError(key)
         # At this point we should be able to assume a self._config...
         value = self._config[key]
@@ -168,15 +183,15 @@
                 keypath = self._keypath + keypath
             # If we have no _root, we must be the root, so it's us. Otherwise,
             # pass along our handle on the root.
             root = getattr(self, "_root", self)
             value = DataProxy.from_data(data=value, root=root, keypath=keypath)
         return value
 
-    def _set(self, *args, **kwargs):
+    def _set(self, *args: Any, **kwargs: Any) -> None:
         """
         Convenience workaround of default 'attrs are config keys' behavior.
 
         Uses `object.__setattr__` to work around the class' normal proxying
         behavior, but is less verbose than using that directly.
 
         Has two modes (which may be combined if you really want):
@@ -185,68 +200,68 @@
         - ``self._set(attname=value)`` (i.e. kwargs), even less typing.
         """
         if args:
             object.__setattr__(self, *args)
         for key, value in kwargs.items():
             object.__setattr__(self, key, value)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "<{}: {}>".format(self.__class__.__name__, self._config)
 
-    def __contains__(self, key):
+    def __contains__(self, key: str) -> bool:
         return key in self._config
 
     @property
-    def _is_leaf(self):
+    def _is_leaf(self) -> bool:
         return hasattr(self, "_root")
 
     @property
-    def _is_root(self):
+    def _is_root(self) -> bool:
         return hasattr(self, "_modify")
 
-    def _track_removal_of(self, key):
+    def _track_removal_of(self, key: str) -> None:
         # Grab the root object responsible for tracking removals; either the
         # referenced root (if we're a leaf) or ourselves (if we're not).
         # (Intermediate nodes never have anything but __getitem__ called on
         # them, otherwise they're by definition being treated as a leaf.)
         target = None
         if self._is_leaf:
             target = self._root
         elif self._is_root:
             target = self
         if target is not None:
             target._remove(getattr(self, "_keypath", tuple()), key)
 
-    def _track_modification_of(self, key, value):
+    def _track_modification_of(self, key: str, value: str) -> None:
         target = None
         if self._is_leaf:
             target = self._root
         elif self._is_root:
             target = self
         if target is not None:
             target._modify(getattr(self, "_keypath", tuple()), key, value)
 
-    def __delitem__(self, key):
+    def __delitem__(self, key: str) -> None:
         del self._config[key]
         self._track_removal_of(key)
 
-    def __delattr__(self, name):
+    def __delattr__(self, name: str) -> None:
         # Make sure we don't screw up true attribute deletion for the
         # situations that actually want it. (Uncommon, but not rare.)
         if name in self:
             del self[name]
         else:
             object.__delattr__(self, name)
 
-    def clear(self):
+    def clear(self) -> None:
         keys = list(self.keys())
         for key in keys:
             del self[key]
 
-    def pop(self, *args):
+    def pop(self, *args: Any) -> Any:
         # Must test this up front before (possibly) mutating self._config
         key_existed = args and args[0] in self._config
         # We always have a _config (whether it's a real dict or a cache of
         # merged levels) so we can fall back to it for all the corner case
         # handling re: args (arity, handling a default, raising KeyError, etc)
         ret = self._config.pop(*args)
         # If it looks like no popping occurred (key wasn't there), presumably
@@ -255,35 +270,35 @@
         if not key_existed:
             return ret
         # Here, we can assume at least the 1st posarg (key) existed.
         self._track_removal_of(args[0])
         # In all cases, return the popped value.
         return ret
 
-    def popitem(self):
+    def popitem(self) -> Any:
         ret = self._config.popitem()
         self._track_removal_of(ret[0])
         return ret
 
-    def setdefault(self, *args):
+    def setdefault(self, *args: Any) -> Any:
         # Must test up front whether the key existed beforehand
         key_existed = args and args[0] in self._config
         # Run locally
         ret = self._config.setdefault(*args)
         # Key already existed -> nothing was mutated, short-circuit
         if key_existed:
             return ret
         # Here, we can assume the key did not exist and thus user must have
         # supplied a 'default' (if they did not, the real setdefault() above
         # would have excepted.)
         key, default = args
         self._track_modification_of(key, default)
         return ret
 
-    def update(self, *args, **kwargs):
+    def update(self, *args: Any, **kwargs: Any) -> None:
         if kwargs:
             for key, value in kwargs.items():
                 self[key] = value
         elif args:
             # TODO: complain if arity>1
             arg = args[0]
             if isinstance(arg, dict):
@@ -408,15 +423,15 @@
     """
 
     prefix = "invoke"
     file_prefix = None
     env_prefix = None
 
     @staticmethod
-    def global_defaults():
+    def global_defaults() -> Dict[str, Any]:
         """
         Return the core default settings for Invoke.
 
         Generally only for use by `.Config` internals. For descriptions of
         these values, see :ref:`default-values`.
 
         Subclasses may choose to override this method, calling
@@ -492,21 +507,21 @@
                 "search_root": None,
             },
             "timeouts": {"command": None},
         }
 
     def __init__(
         self,
-        overrides=None,
-        defaults=None,
-        system_prefix=None,
-        user_prefix=None,
-        project_location=None,
-        runtime_path=None,
-        lazy=False,
+        overrides: Optional[Dict[str, Any]] = None,
+        defaults: Optional[Dict[str, Any]] = None,
+        system_prefix: Optional[str] = None,
+        user_prefix: Optional[str] = None,
+        project_location: Optional[PathLike] = None,
+        runtime_path: Optional[PathLike] = None,
+        lazy: bool = False,
     ):
         """
         Creates a new config object.
 
         :param dict defaults:
             A dict containing default (lowest level) config data. Default:
             `global_defaults`.
@@ -635,20 +650,20 @@
         # other levels in order to function.
         if not lazy:
             self.load_base_conf_files()
         # Always merge, otherwise defaults, etc are not usable until creator or
         # a subroutine does so.
         self.merge()
 
-    def load_base_conf_files(self):
+    def load_base_conf_files(self) -> None:
         # Just a refactor of something done in unlazy init or in clone()
         self.load_system(merge=False)
         self.load_user(merge=False)
 
-    def load_defaults(self, data, merge=True):
+    def load_defaults(self, data: Dict[str, Any], merge: bool = True) -> None:
         """
         Set or replace the 'defaults' configuration level, from ``data``.
 
         :param dict data: The config data to load as the defaults level.
 
         :param bool merge:
             Whether to merge the loaded data into the central config. Default:
@@ -658,15 +673,15 @@
 
         .. versionadded:: 1.0
         """
         self._set(_defaults=data)
         if merge:
             self.merge()
 
-    def load_overrides(self, data, merge=True):
+    def load_overrides(self, data: Dict[str, Any], merge: bool = True) -> None:
         """
         Set or replace the 'overrides' configuration level, from ``data``.
 
         :param dict data: The config data to load as the overrides level.
 
         :param bool merge:
             Whether to merge the loaded data into the central config. Default:
@@ -676,15 +691,15 @@
 
         .. versionadded:: 1.0
         """
         self._set(_overrides=data)
         if merge:
             self.merge()
 
-    def load_system(self, merge=True):
+    def load_system(self, merge: bool = True) -> None:
         """
         Load a system-level config file, if possible.
 
         Checks the configured ``_system_prefix`` path, which defaults to
         ``/etc``, and will thus load files like ``/etc/invoke.yml``.
 
         :param bool merge:
@@ -693,15 +708,15 @@
 
         :returns: ``None``.
 
         .. versionadded:: 1.0
         """
         self._load_file(prefix="system", merge=merge)
 
-    def load_user(self, merge=True):
+    def load_user(self, merge: bool = True) -> None:
         """
         Load a user-level config file, if possible.
 
         Checks the configured ``_user_prefix`` path, which defaults to ``~/.``,
         and will thus load files like ``~/.invoke.yml``.
 
         :param bool merge:
@@ -710,15 +725,15 @@
 
         :returns: ``None``.
 
         .. versionadded:: 1.0
         """
         self._load_file(prefix="user", merge=merge)
 
-    def load_project(self, merge=True):
+    def load_project(self, merge: bool = True) -> None:
         """
         Load a project-level config file, if possible.
 
         Checks the configured ``_project_prefix`` value derived from the path
         given to `set_project_location`, which is typically set to the
         directory containing the loaded task collection.
 
@@ -732,29 +747,29 @@
 
         :returns: ``None``.
 
         .. versionadded:: 1.0
         """
         self._load_file(prefix="project", merge=merge)
 
-    def set_runtime_path(self, path):
+    def set_runtime_path(self, path: Optional[PathLike]) -> None:
         """
         Set the runtime config file path.
 
         .. versionadded:: 1.0
         """
         # Path to the user-specified runtime config file.
         self._set(_runtime_path=path)
         # Data loaded from the runtime config file.
         self._set(_runtime={})
         # Whether the runtime config file has been loaded or not (or ``None``
         # if no loading has been attempted yet.)
         self._set(_runtime_found=None)
 
-    def load_runtime(self, merge=True):
+    def load_runtime(self, merge: bool = True) -> None:
         """
         Load a runtime-level config file, if one was specified.
 
         When the CLI framework creates a `Config`, it sets ``_runtime_path``,
         which is a full path to the requested config file. This method attempts
         to load that file.
 
@@ -764,15 +779,15 @@
 
         :returns: ``None``.
 
         .. versionadded:: 1.0
         """
         self._load_file(prefix="runtime", absolute=True, merge=merge)
 
-    def load_shell_env(self):
+    def load_shell_env(self) -> None:
         """
         Load values from the shell environment.
 
         `.load_shell_env` is intended for execution late in a `.Config`
         object's lifecycle, once all other sources (such as a runtime config
         file or per-collection configurations) have been loaded. Loading from
         the shell is not terrifically expensive, but must be done at a specific
@@ -789,30 +804,32 @@
         self.merge()
         debug("Done with pre-merge.")
         loader = Environment(config=self._config, prefix=self._env_prefix)
         self._set(_env=loader.load())
         debug("Loaded shell environment, triggering final merge")
         self.merge()
 
-    def load_collection(self, data, merge=True):
+    def load_collection(
+        self, data: Dict[str, Any], merge: bool = True
+    ) -> None:
         """
         Update collection-driven config data.
 
         `.load_collection` is intended for use by the core task execution
         machinery, which is responsible for obtaining collection-driven data.
         See :ref:`collection-configuration` for details.
 
         .. versionadded:: 1.0
         """
         debug("Loading collection configuration")
         self._set(_collection=data)
         if merge:
             self.merge()
 
-    def set_project_location(self, path):
+    def set_project_location(self, path: Union[PathLike, str, None]) -> None:
         """
         Set the directory path where a project-level config file may be found.
 
         Does not do any file loading on its own; for that, see `load_project`.
 
         .. versionadded:: 1.0
         """
@@ -826,15 +843,17 @@
         self._set(_project_path=None)
         # Whether the project config file has been loaded or not (or ``None``
         # if no loading has been attempted yet.)
         self._set(_project_found=None)
         # Data loaded from the per-project config file.
         self._set(_project={})
 
-    def _load_file(self, prefix, absolute=False, merge=True):
+    def _load_file(
+        self, prefix: str, absolute: bool = False, merge: bool = True
+    ) -> None:
         # Setup
         found = "_{}_found".format(prefix)
         path = "_{}_path".format(prefix)
         data = "_{}".format(prefix)
         midfix = self.file_prefix
         if midfix is None:
             midfix = self.prefix
@@ -887,26 +906,25 @@
         # Still None -> no suffixed paths were found, record this fact
         if getattr(self, path) is None:
             self._set(found, False)
         # Merge loaded data in if any was found
         elif merge:
             self.merge()
 
-    def _load_yaml(self, path):
+    def _load_yaml(self, path: PathLike) -> Any:
         with open(path) as fd:
             return yaml.safe_load(fd)
 
-    def _load_yml(self, path):
-        return self._load_yaml(path)
+    _load_yml = _load_yaml
 
-    def _load_json(self, path):
+    def _load_json(self, path: PathLike) -> Any:
         with open(path) as fd:
             return json.load(fd)
 
-    def _load_py(self, path):
+    def _load_py(self, path: str) -> Dict[str, Any]:
         data = {}
         for key, value in (load_source("mod", path)).items():
             # Strip special members, as these are always going to be builtins
             # and other special things a user will not want in their config.
             if key.startswith("__"):
                 continue
             # Raise exceptions on module values; they are unpicklable.
@@ -916,15 +934,15 @@
             # code and not in a "config file"...right?
             if isinstance(value, types.ModuleType):
                 err = "'{}' is a module, which can't be used as a config value. (Are you perhaps giving a tasks file instead of a config file by mistake?)"  # noqa
                 raise UnpicklableConfigMember(err.format(key))
             data[key] = value
         return data
 
-    def merge(self):
+    def merge(self) -> None:
         """
         Merge all config sources, in order.
 
         .. versionadded:: 1.0
         """
         debug("Merging config sources in order onto new empty _config...")
         self._set(_config={})
@@ -941,15 +959,15 @@
         debug("Overrides: {!r}".format(self._overrides))
         merge_dicts(self._config, self._overrides)
         debug("Modifications: {!r}".format(self._modifications))
         merge_dicts(self._config, self._modifications)
         debug("Deletions: {!r}".format(self._deletions))
         obliterate(self._config, self._deletions)
 
-    def _merge_file(self, name, desc):
+    def _merge_file(self, name: str, desc: str) -> None:
         # Setup
         desc += " config file"  # yup
         found = getattr(self, "_{}_found".format(name))
         path = getattr(self, "_{}_path".format(name))
         data = getattr(self, "_{}".format(name))
         # None -> no loading occurred yet
         if found is None:
@@ -960,15 +978,15 @@
             merge_dicts(self._config, data)
         # False -> did try, did not succeed
         else:
             # TODO: how to preserve what was tried for each case but only for
             # the negative? Just a branch here based on 'name'?
             debug("{} not found, skipping".format(desc))
 
-    def clone(self, into=None):
+    def clone(self, into: Optional[Type["Config"]] = None) -> "Config":
         """
         Return a copy of this configuration object.
 
         The new object will be identical in terms of configured sources and any
         loaded (or user-manipulated) data, but will be a distinct object with
         as little shared mutable state as possible.
 
@@ -1056,15 +1074,17 @@
         # conf files.
         new.load_base_conf_files()
         # Finally, merge() for reals (_load_base_conf_files doesn't do so
         # internally, so that data wouldn't otherwise show up.)
         new.merge()
         return new
 
-    def _clone_init_kwargs(self, into=None):
+    def _clone_init_kwargs(
+        self, into: Optional[Type["Config"]] = None
+    ) -> Dict[str, Any]:
         """
         Supply kwargs suitable for initializing a new clone of this object.
 
         Note that most of the `.clone` process involves copying data between
         two instances instead of passing init kwargs; however, sometimes you
         really do want init kwargs, which is why this method exists.
 
@@ -1083,15 +1103,15 @@
             defaults=new_defaults,
             # TODO: consider making this 'hardcoded' on the calling end (ie
             # inside clone()) to make sure nobody accidentally nukes it via
             # subclassing?
             lazy=True,
         )
 
-    def _modify(self, keypath, key, value):
+    def _modify(self, keypath: Tuple[str, ...], key: str, value: str) -> None:
         """
         Update our user-modifications config level with new data.
 
         :param tuple keypath:
             The key path identifying the sub-dict being updated. May be an
             empty tuple if the update is occurring at the topmost level.
 
@@ -1102,37 +1122,37 @@
             The value being written.
         """
         # First, ensure we wipe the keypath from _deletions, in case it was
         # previously deleted.
         excise(self._deletions, keypath + (key,))
         # Now we can add it to the modifications structure.
         data = self._modifications
-        keypath = list(keypath)
-        while keypath:
-            subkey = keypath.pop(0)
+        keypath_list = list(keypath)
+        while keypath_list:
+            subkey = keypath_list.pop(0)
             # TODO: could use defaultdict here, but...meh?
             if subkey not in data:
                 # TODO: generify this and the subsequent 3 lines...
                 data[subkey] = {}
             data = data[subkey]
         data[key] = value
         self.merge()
 
-    def _remove(self, keypath, key):
+    def _remove(self, keypath: Tuple[str, ...], key: str) -> None:
         """
         Like `._modify`, but for removal.
         """
         # NOTE: because deletions are processed in merge() last, we do not need
         # to remove things from _modifications on removal; but we *do* do the
         # inverse - remove from _deletions on modification.
         # TODO: may be sane to push this step up to callers?
         data = self._deletions
-        keypath = list(keypath)
-        while keypath:
-            subkey = keypath.pop(0)
+        keypath_list = list(keypath)
+        while keypath_list:
+            subkey = keypath_list.pop(0)
             if subkey in data:
                 data = data[subkey]
                 # If we encounter None, it means something higher up than our
                 # requested keypath is already marked as deleted; so we don't
                 # have to do anything or go further.
                 if data is None:
                     return
@@ -1149,15 +1169,17 @@
         self.merge()
 
 
 class AmbiguousMergeError(ValueError):
     pass
 
 
-def merge_dicts(base, updates):
+def merge_dicts(
+    base: Dict[str, Any], updates: Dict[str, Any]
+) -> Dict[str, Any]:
     """
     Recursively merge dict ``updates`` into dict ``base`` (mutating ``base``.)
 
     * Values which are themselves dicts will be recursed into.
     * Values which are a dict in one input and *not* a dict in the other input
       (e.g. if our inputs were ``{'foo': 5}`` and ``{'foo': {'bar': 5}}``) are
       irreconciliable and will generate an exception.
@@ -1206,58 +1228,58 @@
                 base[key] = value
             # Non-dict values just get set straight
             else:
                 base[key] = copy.copy(value)
     return base
 
 
-def _merge_error(orig, new_):
+def _merge_error(orig: object, new: object) -> AmbiguousMergeError:
     return AmbiguousMergeError(
         "Can't cleanly merge {} with {}".format(
-            _format_mismatch(orig), _format_mismatch(new_)
+            _format_mismatch(orig), _format_mismatch(new)
         )
     )
 
 
-def _format_mismatch(x):
+def _format_mismatch(x: object) -> str:
     return "{} ({!r})".format(type(x), x)
 
 
-def copy_dict(source):
+def copy_dict(source: Dict[str, Any]) -> Dict[str, Any]:
     """
     Return a fresh copy of ``source`` with as little shared state as possible.
 
     Uses `merge_dicts` under the hood, with an empty ``base`` dict; see its
     documentation for details on behavior.
 
     .. versionadded:: 1.0
     """
     return merge_dicts({}, source)
 
 
-def excise(dict_, keypath):
+def excise(dict_: Dict[str, Any], keypath: Tuple[str, ...]) -> None:
     """
     Remove key pointed at by ``keypath`` from nested dict ``dict_``, if exists.
 
     .. versionadded:: 1.0
     """
     data = dict_
-    keypath = list(keypath)
-    leaf_key = keypath.pop()
-    while keypath:
-        key = keypath.pop(0)
+    keypath_list = list(keypath)
+    leaf_key = keypath_list.pop()
+    while keypath_list:
+        key = keypath_list.pop(0)
         if key not in data:
             # Not there, nothing to excise
             return
         data = data[key]
     if leaf_key in data:
         del data[leaf_key]
 
 
-def obliterate(base, deletions):
+def obliterate(base: Dict[str, Any], deletions: Dict[str, Any]) -> None:
     """
     Remove all (nested) keys mentioned in ``deletions``, from ``base``.
 
     .. versionadded:: 1.0
     """
     for key, value in deletions.items():
         if isinstance(value, dict):
```

### Comparing `invoke-2.0.1/invoke/terminals.py` & `invoke-2.1.0/invoke/terminals.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Much of this code performs platform-sensitive branching, e.g. Windows support.
 
 This is its own module to abstract away what would otherwise be distracting
 logic-flow interruptions.
 """
 
 from contextlib import contextmanager
+from typing import Generator, IO, Optional, Tuple
 import os
 import select
 import sys
 
 # TODO: move in here? They're currently platform-agnostic...
 from .util import has_fileno, isatty
 
@@ -23,103 +24,114 @@
 Note that Cygwin's Python is actually close enough to "real" UNIXes that it
 doesn't need (or want!) to use PyWin32 -- so we only test for literal Win32
 setups (vanilla Python, ActiveState etc) here.
 
 .. versionadded:: 1.0
 """
 
-if WINDOWS:
+if sys.platform == "win32":
     import msvcrt
-    from ctypes import Structure, c_ushort, windll, POINTER, byref
+    from ctypes import (
+        Structure,
+        c_ushort,
+        windll,
+        POINTER,
+        byref,
+    )
     from ctypes.wintypes import HANDLE, _COORD, _SMALL_RECT
 else:
     import fcntl
     import struct
     import termios
     import tty
 
 
-def pty_size():
+if sys.platform == "win32":
+
+    def _pty_size() -> Tuple[Optional[int], Optional[int]]:
+        class CONSOLE_SCREEN_BUFFER_INFO(Structure):
+            _fields_ = [
+                ("dwSize", _COORD),
+                ("dwCursorPosition", _COORD),
+                ("wAttributes", c_ushort),
+                ("srWindow", _SMALL_RECT),
+                ("dwMaximumWindowSize", _COORD),
+            ]
+
+        GetStdHandle = windll.kernel32.GetStdHandle
+        GetConsoleScreenBufferInfo = windll.kernel32.GetConsoleScreenBufferInfo
+        GetStdHandle.restype = HANDLE
+        GetConsoleScreenBufferInfo.argtypes = [
+            HANDLE,
+            POINTER(CONSOLE_SCREEN_BUFFER_INFO),
+        ]
+
+        hstd = GetStdHandle(-11)  # STD_OUTPUT_HANDLE = -11
+        csbi = CONSOLE_SCREEN_BUFFER_INFO()
+        ret = GetConsoleScreenBufferInfo(hstd, byref(csbi))
+
+        if ret:
+            sizex = csbi.srWindow.Right - csbi.srWindow.Left + 1
+            sizey = csbi.srWindow.Bottom - csbi.srWindow.Top + 1
+            return sizex, sizey
+        else:
+            return (None, None)
+
+else:
+
+    def _pty_size() -> Tuple[Optional[int], Optional[int]]:
+        """
+        Suitable for most POSIX platforms.
+
+        .. versionadded:: 1.0
+        """
+        # Sentinel values to be replaced w/ defaults by caller
+        size = (None, None)
+        # We want two short unsigned integers (rows, cols)
+        fmt = "HH"
+        # Create an empty (zeroed) buffer for ioctl to map onto. Yay for C!
+        buf = struct.pack(fmt, 0, 0)
+        # Call TIOCGWINSZ to get window size of stdout, returns our filled
+        # buffer
+        try:
+            result = fcntl.ioctl(sys.stdout, termios.TIOCGWINSZ, buf)
+            # Unpack buffer back into Python data types
+            # NOTE: this unpack gives us rows x cols, but we return the
+            # inverse.
+            rows, cols = struct.unpack(fmt, result)
+            return (cols, rows)
+        # Fallback to emptyish return value in various failure cases:
+        # * sys.stdout being monkeypatched, such as in testing, and lacking
+        # * .fileno
+        # * sys.stdout having a .fileno but not actually being attached to a
+        # * TTY
+        # * termios not having a TIOCGWINSZ attribute (happens sometimes...)
+        # * other situations where ioctl doesn't explode but the result isn't
+        #   something unpack can deal with
+        except (struct.error, TypeError, IOError, AttributeError):
+            pass
+        return size
+
+
+def pty_size() -> Tuple[int, int]:
     """
     Determine current local pseudoterminal dimensions.
 
     :returns:
         A ``(num_cols, num_rows)`` two-tuple describing PTY size. Defaults to
         ``(80, 24)`` if unable to get a sensible result dynamically.
 
     .. versionadded:: 1.0
     """
-    cols, rows = _pty_size() if not WINDOWS else _win_pty_size()
+    cols, rows = _pty_size()
     # TODO: make defaults configurable?
-    return ((cols or 80), (rows or 24))
-
-
-def _pty_size():
-    """
-    Suitable for most POSIX platforms.
-
-    .. versionadded:: 1.0
-    """
-    # Sentinel values to be replaced w/ defaults by caller
-    size = (None, None)
-    # We want two short unsigned integers (rows, cols)
-    fmt = "HH"
-    # Create an empty (zeroed) buffer for ioctl to map onto. Yay for C!
-    buf = struct.pack(fmt, 0, 0)
-    # Call TIOCGWINSZ to get window size of stdout, returns our filled
-    # buffer
-    try:
-        result = fcntl.ioctl(sys.stdout, termios.TIOCGWINSZ, buf)
-        # Unpack buffer back into Python data types
-        # NOTE: this unpack gives us rows x cols, but we return the
-        # inverse.
-        rows, cols = struct.unpack(fmt, result)
-        return (cols, rows)
-    # Fallback to emptyish return value in various failure cases:
-    # * sys.stdout being monkeypatched, such as in testing, and lacking .fileno
-    # * sys.stdout having a .fileno but not actually being attached to a TTY
-    # * termios not having a TIOCGWINSZ attribute (happens sometimes...)
-    # * other situations where ioctl doesn't explode but the result isn't
-    #   something unpack can deal with
-    except (struct.error, TypeError, IOError, AttributeError):
-        pass
-    return size
-
-
-def _win_pty_size():
-    class CONSOLE_SCREEN_BUFFER_INFO(Structure):
-        _fields_ = [
-            ("dwSize", _COORD),
-            ("dwCursorPosition", _COORD),
-            ("wAttributes", c_ushort),
-            ("srWindow", _SMALL_RECT),
-            ("dwMaximumWindowSize", _COORD),
-        ]
-
-    GetStdHandle = windll.kernel32.GetStdHandle
-    GetConsoleScreenBufferInfo = windll.kernel32.GetConsoleScreenBufferInfo
-    GetStdHandle.restype = HANDLE
-    GetConsoleScreenBufferInfo.argtypes = [
-        HANDLE,
-        POINTER(CONSOLE_SCREEN_BUFFER_INFO),
-    ]
-
-    hstd = GetStdHandle(-11)  # STD_OUTPUT_HANDLE = -11
-    csbi = CONSOLE_SCREEN_BUFFER_INFO()
-    ret = GetConsoleScreenBufferInfo(hstd, byref(csbi))
-
-    if ret:
-        sizex = csbi.srWindow.Right - csbi.srWindow.Left + 1
-        sizey = csbi.srWindow.Bottom - csbi.srWindow.Top + 1
-        return sizex, sizey
-    else:
-        return (None, None)
+    return (cols or 80, rows or 24)
 
 
-def stdin_is_foregrounded_tty(stream):
+def stdin_is_foregrounded_tty(stream: IO) -> bool:
     """
     Detect if given stdin ``stream`` seems to be in the foreground of a TTY.
 
     Specifically, compares the current Python process group ID to that of the
     stream's file descriptor to see if they match; if they do not match, it is
     likely that the process has been placed in the background.
 
@@ -135,15 +147,15 @@
     .. versionadded:: 1.0
     """
     if not has_fileno(stream):
         return False
     return os.getpgrp() == os.tcgetpgrp(stream.fileno())
 
 
-def cbreak_already_set(stream):
+def cbreak_already_set(stream: IO) -> bool:
     # Explicitly not docstringed to remain private, for now. Eh.
     # Checks whether tty.setcbreak appears to have already been run against
     # ``stream`` (or if it would otherwise just not do anything).
     # Used to effect idempotency for character-buffering a stream, which also
     # lets us avoid multiple capture-then-restore cycles.
     attrs = termios.tcgetattr(stream)
     lflags, cc = attrs[3], attrs[6]
@@ -158,15 +170,17 @@
         cc[termios.VMIN] in [1, b"\x01"],
         cc[termios.VTIME] in [0, b"\x00"],
     )
     return all(sentinels)
 
 
 @contextmanager
-def character_buffered(stream):
+def character_buffered(
+    stream: IO,
+) -> Generator[None, None, None]:
     """
     Force local terminal ``stream`` be character, not line, buffered.
 
     Only applies to Unix-based systems; on Windows this is a no-op.
 
     .. versionadded:: 1.0
     """
@@ -182,15 +196,15 @@
         tty.setcbreak(stream)
         try:
             yield
         finally:
             termios.tcsetattr(stream, termios.TCSADRAIN, old_settings)
 
 
-def ready_for_reading(input_):
+def ready_for_reading(input_: IO) -> bool:
     """
     Test ``input_`` to determine whether a read action will succeed.
 
     :param input_: Input stream object (file-like).
 
     :returns: ``True`` if a read should succeed, ``False`` otherwise.
 
@@ -198,22 +212,22 @@
     """
     # A "real" terminal stdin needs select/kbhit to tell us when it's ready for
     # a nonblocking read().
     # Otherwise, assume a "safer" file-like object that can be read from in a
     # nonblocking fashion (e.g. a StringIO or regular file).
     if not has_fileno(input_):
         return True
-    if WINDOWS:
+    if sys.platform == "win32":
         return msvcrt.kbhit()
     else:
         reads, _, _ = select.select([input_], [], [], 0.0)
         return bool(reads and reads[0] is input_)
 
 
-def bytes_to_read(input_):
+def bytes_to_read(input_: IO) -> int:
     """
     Query stream ``input_`` to see how many bytes may be readable.
 
     .. note::
         If we are unable to tell (e.g. if ``input_`` isn't a true file
         descriptor or isn't a valid TTY) we fall back to suggesting reading 1
         byte only.
@@ -224,10 +238,10 @@
 
     .. versionadded:: 1.0
     """
     # NOTE: we have to check both possibilities here; situations exist where
     # it's not a tty but has a fileno, or vice versa; neither is typically
     # going to work re: ioctl().
     if not WINDOWS and isatty(input_) and has_fileno(input_):
-        fionread = fcntl.ioctl(input_, termios.FIONREAD, "  ")
-        return struct.unpack("h", fionread)[0]
+        fionread = fcntl.ioctl(input_, termios.FIONREAD, b"  ")
+        return int(struct.unpack("h", fionread)[0])
     return 1
```

### Comparing `invoke-2.0.1/invoke/completion/complete.py` & `invoke-2.1.0/invoke/completion/complete.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 """
 Command-line completion mechanisms, executed by the core ``--complete`` flag.
 """
 
+from typing import List
 import glob
 import os
 import re
 import shlex
+from typing import TYPE_CHECKING
 
 from ..exceptions import Exit, ParseError
 from ..util import debug, task_name_sort_key
 
+if TYPE_CHECKING:
+    from ..collection import Collection
+    from ..parser import Parser, ParseResult, ParserContext
 
-def complete(names, core, initial_context, collection, parser):
+
+def complete(
+    names: List[str],
+    core: "ParseResult",
+    initial_context: "ParserContext",
+    collection: "Collection",
+    parser: "Parser",
+) -> Exit:
     # Strip out program name (scripts give us full command line)
     # TODO: this may not handle path/to/script though?
     invocation = re.sub(r"^({}) ".format("|".join(names)), "", core.remainder)
     debug("Completing for invocation: {!r}".format(invocation))
     # Tokenize (shlex will have to do)
     tokens = shlex.split(invocation)
     # Handle flags (partial or otherwise)
     if tokens and tokens[-1].startswith("-"):
         tail = tokens[-1]
         debug("Invocation's tail {!r} is flag-like".format(tail))
         # Gently parse invocation to obtain 'current' context.
         # Use last seen context in case of failure (required for
         # otherwise-invalid partial invocations being completed).
+
+        contexts: List[ParserContext]
         try:
             debug("Seeking context name in tokens: {!r}".format(tokens))
             contexts = parser.parse_argv(tokens)
         except ParseError as e:
             msg = "Got parser error ({!r}), grabbing its last-seen context {!r}"  # noqa
             debug(msg.format(e, e.context))
-            contexts = [e.context]
+            contexts = [e.context] if e.context is not None else []
         # Fall back to core context if no context seen.
         debug("Parsed invocation, contexts: {!r}".format(contexts))
         if not contexts or not contexts[-1]:
             context = initial_context
         else:
             context = contexts[-1]
         debug("Selected context: {!r}".format(context))
@@ -76,24 +90,24 @@
     # task names.
     else:
         debug("Last token isn't flag-like, just printing task names")
         print_task_names(collection)
     raise Exit
 
 
-def print_task_names(collection):
+def print_task_names(collection: "Collection") -> None:
     for name in sorted(collection.task_names, key=task_name_sort_key):
         print(name)
         # Just stick aliases after the thing they're aliased to. Sorting isn't
         # so important that it's worth bending over backwards here.
         for alias in collection.task_names[name]:
             print(alias)
 
 
-def print_completion_script(shell, names):
+def print_completion_script(shell: str, names: List[str]) -> None:
     # Grab all .completion files in invoke/completion/. (These used to have no
     # suffix, but surprise, that's super fragile.
     completions = {
         os.path.splitext(os.path.basename(x))[0]: x
         for x in glob.glob(
             os.path.join(
                 os.path.dirname(os.path.realpath(__file__)), "*.completion"
```

### Comparing `invoke-2.0.1/invoke/completion/bash.completion` & `invoke-2.1.0/invoke/completion/bash.completion`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/completion/zsh.completion` & `invoke-2.1.0/invoke/completion/zsh.completion`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/context.py` & `invoke-2.1.0/invoke/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 import os
 import re
 from contextlib import contextmanager
 from itertools import cycle
+from os import PathLike
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Generator,
+    Iterator,
+    List,
+    Optional,
+    Union,
+)
 from unittest.mock import Mock
 
 from .config import Config, DataProxy
 from .exceptions import Failure, AuthFailure, ResponseNotAccepted
 from .runners import Result
 from .watchers import FailingResponder
 
+if TYPE_CHECKING:
+    from invoke.runners import Runner
+
 
 class Context(DataProxy):
     """
     Context-aware API wrapper & state-passing object.
 
     `.Context` objects are created during command-line parsing (or, if desired,
     by hand) and used to share parser and configuration state with executed
@@ -26,15 +39,15 @@
     Instances of `.Context` may be shared between tasks when executing
     sub-tasks - either the same context the caller was given, or an altered
     copy thereof (or, theoretically, a brand new one).
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, config=None):
+    def __init__(self, config: Optional[Config] = None) -> None:
         """
         :param config:
             `.Config` object to use as the base configuration.
 
             Defaults to an anonymous/default `.Config` instance.
         """
         #: The fully merged `.Config` object appropriate for this context.
@@ -47,38 +60,38 @@
         #: ``config`` attribute in the same way - e.g. ``c['foo']`` or
         #: ``c.foo`` returns the same value as ``c.config['foo']``.
         config = config if config is not None else Config()
         self._set(_config=config)
         #: A list of commands to run (via "&&") before the main argument to any
         #: `run` or `sudo` calls. Note that the primary API for manipulating
         #: this list is `prefix`; see its docs for details.
-        command_prefixes = list()
+        command_prefixes: List[str] = list()
         self._set(command_prefixes=command_prefixes)
         #: A list of directories to 'cd' into before running commands with
         #: `run` or `sudo`; intended for management via `cd`, please see its
         #: docs for details.
-        command_cwds = list()
+        command_cwds: List[str] = list()
         self._set(command_cwds=command_cwds)
 
     @property
-    def config(self):
+    def config(self) -> Config:
         # Allows Context to expose a .config attribute even though DataProxy
         # otherwise considers it a config key.
         return self._config
 
     @config.setter
-    def config(self, value):
+    def config(self, value: Config) -> None:
         # NOTE: mostly used by client libraries needing to tweak a Context's
         # config at execution time; i.e. a Context subclass that bears its own
         # unique data may want to be stood up when parameterizing/expanding a
         # call list at start of a session, with the final config filled in at
         # runtime.
         self._set(_config=value)
 
-    def run(self, command, **kwargs):
+    def run(self, command: str, **kwargs: Any) -> Optional[Result]:
         """
         Execute a local shell command, honoring config options.
 
         Specifically, this method instantiates a `.Runner` subclass (according
         to the ``runner`` config option; default is `.Local`) and calls its
         ``.run`` method with ``command`` and ``kwargs``.
 
@@ -89,19 +102,21 @@
         """
         runner = self.config.runners.local(self)
         return self._run(runner, command, **kwargs)
 
     # NOTE: broken out of run() to allow for runner class injection in
     # Fabric/etc, which needs to juggle multiple runner class types (local and
     # remote).
-    def _run(self, runner, command, **kwargs):
+    def _run(
+        self, runner: "Runner", command: str, **kwargs: Any
+    ) -> Optional[Result]:
         command = self._prefix_commands(command)
         return runner.run(command, **kwargs)
 
-    def sudo(self, command, **kwargs):
+    def sudo(self, command: str, **kwargs: Any) -> Optional[Result]:
         """
         Execute a shell command via ``sudo`` with password auto-response.
 
         **Basics**
 
         This method is identical to `run` but adds a handful of
         convenient behaviors around invoking the ``sudo`` program. It doesn't
@@ -166,15 +181,17 @@
 
         .. versionadded:: 1.0
         """
         runner = self.config.runners.local(self)
         return self._sudo(runner, command, **kwargs)
 
     # NOTE: this is for runner injection; see NOTE above _run().
-    def _sudo(self, runner, command, **kwargs):
+    def _sudo(
+        self, runner: "Runner", command: str, **kwargs: Any
+    ) -> Optional[Result]:
         prompt = self.config.sudo.prompt
         password = kwargs.pop("password", self.config.sudo.password)
         user = kwargs.pop("user", self.config.sudo.user)
         env = kwargs.get("env", {})
         # TODO: allow subclassing for 'get the password' so users who REALLY
         # want lazy runtime prompting can have it easily implemented.
         # TODO: want to print a "cleaner" echo with just 'sudo <command>'; but
@@ -228,30 +245,30 @@
             # Reraise for any other error so it bubbles up normally.
             else:
                 raise
 
     # TODO: wonder if it makes sense to move this part of things inside Runner,
     # which would grow a `prefixes` and `cwd` init kwargs or similar. The less
     # that's stuffed into Context, probably the better.
-    def _prefix_commands(self, command):
+    def _prefix_commands(self, command: str) -> str:
         """
         Prefixes ``command`` with all prefixes found in ``command_prefixes``.
 
         ``command_prefixes`` is a list of strings which is modified by the
         `prefix` context manager.
         """
         prefixes = list(self.command_prefixes)
         current_directory = self.cwd
         if current_directory:
             prefixes.insert(0, "cd {}".format(current_directory))
 
         return " && ".join(prefixes + [command])
 
     @contextmanager
-    def prefix(self, command):
+    def prefix(self, command: str) -> Generator[None, None, None]:
         """
         Prefix all nested `run`/`sudo` commands with given command plus ``&&``.
 
         Most of the time, you'll want to be using this alongside a shell script
         which alters shell state, such as ones which export or alter shell
         environment variables.
 
@@ -299,15 +316,15 @@
         self.command_prefixes.append(command)
         try:
             yield
         finally:
             self.command_prefixes.pop()
 
     @property
-    def cwd(self):
+    def cwd(self) -> str:
         """
         Return the current working directory, accounting for uses of `cd`.
 
         .. versionadded:: 1.0
         """
         if not self.command_cwds:
             # TODO: should this be None? Feels cleaner, though there may be
@@ -319,18 +336,18 @@
         for i, path in reversed(list(enumerate(self.command_cwds))):
             if path.startswith("~") or path.startswith("/"):
                 break
 
         # TODO: see if there's a stronger "escape this path" function somewhere
         # we can reuse. e.g., escaping tildes or slashes in filenames.
         paths = [path.replace(" ", r"\ ") for path in self.command_cwds[i:]]
-        return os.path.join(*paths)
+        return str(os.path.join(*paths))
 
     @contextmanager
-    def cd(self, path):
+    def cd(self, path: Union[PathLike, str]) -> Generator[None, None, None]:
         """
         Context manager that keeps directory state when executing commands.
 
         Any calls to `run`, `sudo`, within the wrapped block will implicitly
         have a string similar to ``"cd <path> && "`` prefixed in order to give
         the sense that there is actually statefulness involved.
 
@@ -397,15 +414,15 @@
         real underlying method - typically undesirable when mocking.)
 
     .. versionadded:: 1.0
     .. versionchanged:: 1.5
         Added ``Mock`` wrapping of ``run`` and ``sudo``.
     """
 
-    def __init__(self, config=None, **kwargs):
+    def __init__(self, config: Optional[Config] = None, **kwargs: Any) -> None:
         """
         Create a ``Context``-like object whose methods yield `.Result` objects.
 
         :param config:
             A Configuration object to use. Identical in behavior to `.Context`.
 
         :param run:
@@ -477,15 +494,15 @@
                 err = "Not sure how to yield results from a {!r}"
                 raise TypeError(err.format(type(results)))
             # Save results for use by the method
             self._set("__{}".format(method), results)
             # Wrap the method in a Mock
             self._set(method, Mock(wraps=getattr(self, method)))
 
-    def _normalize(self, value):
+    def _normalize(self, value: Any) -> Iterator[Any]:
         # First turn everything into an iterable
         if not hasattr(value, "__iter__") or isinstance(value, str):
             value = [value]
         # Then turn everything within into a Result
         results = []
         for obj in value:
             if isinstance(obj, bool):
@@ -497,15 +514,15 @@
         return cycle(results) if getattr(self, "__repeat") else iter(results)
 
     # TODO: _maybe_ make this more metaprogrammy/flexible (using __call__ etc)?
     # Pretty worried it'd cause more hard-to-debug issues than it's presently
     # worth. Maybe in situations where Context grows a _lot_ of methods (e.g.
     # in Fabric 2; though Fabric could do its own sub-subclass in that case...)
 
-    def _yield_result(self, attname, command):
+    def _yield_result(self, attname: str, command: str) -> Result:
         try:
             obj = getattr(self, attname)
             # Dicts need to try direct lookup or regex matching
             if isinstance(obj, dict):
                 try:
                     obj = obj[command]
                 except KeyError:
@@ -517,39 +534,41 @@
                             break
                     else:
                         # Nope, nothing did match.
                         raise KeyError
             # Here, the value was either never a dict or has been extracted
             # from one, so we can assume it's an iterable of Result objects due
             # to work done by __init__.
-            result = next(obj)
+            result: Result = next(obj)
             # Populate Result's command string with what matched unless
             # explicitly given
             if not result.command:
                 result.command = command
             return result
         except (AttributeError, IndexError, KeyError, StopIteration):
             # raise_from(NotImplementedError(command), None)
             raise NotImplementedError(command)
 
-    def run(self, command, *args, **kwargs):
+    def run(self, command: str, *args: Any, **kwargs: Any) -> Result:
         # TODO: perform more convenience stuff associating args/kwargs with the
         # result? E.g. filling in .command, etc? Possibly useful for debugging
         # if one hits unexpected-order problems with what they passed in to
         # __init__.
         return self._yield_result("__run", command)
 
-    def sudo(self, command, *args, **kwargs):
+    def sudo(self, command: str, *args: Any, **kwargs: Any) -> Result:
         # TODO: this completely nukes the top-level behavior of sudo(), which
         # could be good or bad, depending. Most of the time I think it's good.
         # No need to supply dummy password config, etc.
         # TODO: see the TODO from run() re: injecting arg/kwarg values
         return self._yield_result("__sudo", command)
 
-    def set_result_for(self, attname, command, result):
+    def set_result_for(
+        self, attname: str, command: str, result: Result
+    ) -> None:
         """
         Modify the stored mock results for given ``attname`` (e.g. ``run``).
 
         This is similar to how one instantiates `MockContext` with a ``run`` or
         ``sudo`` dict kwarg. For example, this::
 
             mc = MockContext(run={'mycommand': Result("mystdout")})
```

### Comparing `invoke-2.0.1/invoke/exceptions.py` & `invoke-2.1.0/invoke/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 Custom exception classes.
 
 These vary in use case from "we needed a specific data structure layout in
 exceptions used for message-passing" to simply "we needed to express an error
 condition in a way easily told apart from other, truly unexpected errors".
 """
 
-from traceback import format_exception
 from pprint import pformat
+from traceback import format_exception
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
+
+if TYPE_CHECKING:
+    from .parser import ParserContext
+    from .runners import Result
+    from .util import ExceptionWrapper
 
 
 class CollectionNotFound(Exception):
-    def __init__(self, name, start):
+    def __init__(self, name: str, start: str) -> None:
         self.name = name
         self.start = start
 
 
 class Failure(Exception):
     """
     Exception subclass representing failure of a command execution.
@@ -37,19 +43,21 @@
     This class is only rarely raised by itself; most of the time `.Runner.run`
     (or a wrapper of same, such as `.Context.sudo`) will raise a specific
     subclass like `UnexpectedExit` or `AuthFailure`.
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, result, reason=None):
+    def __init__(
+        self, result: "Result", reason: Optional["WatcherError"] = None
+    ) -> None:
         self.result = result
         self.reason = reason
 
-    def streams_for_display(self):
+    def streams_for_display(self) -> Tuple[str, str]:
         """
         Return stdout/err streams as necessary for error display.
 
         Subject to the following rules:
 
         - If a given stream was *not* hidden during execution, a placeholder is
           used instead, to avoid printing it twice.
@@ -71,18 +79,18 @@
         else:
             if "stderr" not in self.result.hide:
                 stderr = already_printed
             else:
                 stderr = self.result.tail("stderr")
         return stdout, stderr
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self._repr()
 
-    def _repr(self, **kwargs):
+    def _repr(self, **kwargs: Any) -> str:
         """
         Return ``__repr__``-like value from inner result + any kwargs.
         """
         # TODO: expand?
         # TODO: truncate command?
         template = "<{}: cmd={!r}{}>"
         rest = ""
@@ -106,15 +114,15 @@
     - The last 10 lines of stdout, if it was hidden;
     - The last 10 lines of stderr, if it was hidden and non-empty (e.g.
       pty=False; when pty=True, stderr never happens.)
 
     .. versionadded:: 1.0
     """
 
-    def __str__(self):
+    def __str__(self) -> str:
         stdout, stderr = self.streams_for_display()
         command = self.result.command
         exited = self.result.exited
         template = """Encountered a bad command exit code!
 
 Command: {!r}
 
@@ -123,32 +131,32 @@
 Stdout:{}
 
 Stderr:{}
 
 """
         return template.format(command, exited, stdout, stderr)
 
-    def _repr(self, **kwargs):
+    def _repr(self, **kwargs: Any) -> str:
         kwargs.setdefault("exited", self.result.exited)
         return super()._repr(**kwargs)
 
 
 class CommandTimedOut(Failure):
     """
     Raised when a subprocess did not exit within a desired timeframe.
     """
 
-    def __init__(self, result, timeout):
+    def __init__(self, result: "Result", timeout: int) -> None:
         super().__init__(result)
         self.timeout = timeout
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self._repr(timeout=self.timeout)
 
-    def __str__(self):
+    def __str__(self) -> str:
         stdout, stderr = self.streams_for_display()
         command = self.result.command
         template = """Command did not complete within {} seconds!
 
 Command: {!r}
 
 Stdout:{}
@@ -167,33 +175,35 @@
         `.Result` objects attached to these exceptions typically lack exit code
         information, since the command was never fully executed - the exception
         was raised instead.
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, result, prompt):
+    def __init__(self, result: "Result", prompt: str) -> None:
         self.result = result
         self.prompt = prompt
 
-    def __str__(self):
+    def __str__(self) -> str:
         err = "The password submitted to prompt {!r} was rejected."
         return err.format(self.prompt)
 
 
 class ParseError(Exception):
     """
     An error arising from the parsing of command-line flags/arguments.
 
     Ambiguous input, invalid task names, invalid flags, etc.
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, msg, context=None):
+    def __init__(
+        self, msg: str, context: Optional["ParserContext"] = None
+    ) -> None:
         super().__init__(msg)
         self.context = context
 
 
 class Exit(Exception):
     """
     Simple custom stand-in for SystemExit.
@@ -211,20 +221,22 @@
     If ``message`` (a string) given, it is printed to standard error, and the
     program exits with code ``1`` by default (unless overridden by also giving
     ``code`` explicitly.)
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, message=None, code=None):
+    def __init__(
+        self, message: Optional[str] = None, code: Optional[int] = None
+    ) -> None:
         self.message = message
         self._code = code
 
     @property
-    def code(self):
+    def code(self) -> int:
         if self._code is not None:
             return self._code
         return 1 if self.message else 0
 
 
 class PlatformError(Exception):
     """
@@ -285,15 +297,15 @@
 
     .. versionadded:: 1.0.2
     """
 
     pass
 
 
-def _printable_kwargs(kwargs):
+def _printable_kwargs(kwargs: Any) -> Dict[str, Any]:
     """
     Return print-friendly version of a thread-related ``kwargs`` dict.
 
     Extra care is taken with ``args`` members which are very long iterables -
     those need truncating to be useful.
     """
     printable = {}
@@ -333,20 +345,20 @@
     #: .. note::
     #:     The ordering of this attribute is not well-defined.
     #:
     #: .. note::
     #:     Thread kwargs which appear to be very long (e.g. IO
     #:     buffers) will be truncated when printed, to avoid huge
     #:     unreadable error display.
-    exceptions = tuple()
+    exceptions: Tuple["ExceptionWrapper", ...] = tuple()
 
-    def __init__(self, exceptions):
+    def __init__(self, exceptions: List["ExceptionWrapper"]) -> None:
         self.exceptions = tuple(exceptions)
 
-    def __str__(self):
+    def __str__(self) -> str:
         details = []
         for x in self.exceptions:
             # Build useful display
             detail = "Thread args: {}\n\n{}"
             details.append(
                 detail.format(
                     pformat(_printable_kwargs(x.kwargs)),
```

### Comparing `invoke-2.0.1/invoke/program.py` & `invoke-2.1.0/invoke/program.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 import getpass
 import inspect
 import json
 import os
 import sys
 import textwrap
 from importlib import import_module  # buffalo buffalo
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+)
 
 from . import Collection, Config, Executor, FilesystemLoader
 from .completion.complete import complete, print_completion_script
 from .parser import Parser, ParserContext, Argument
 from .exceptions import UnexpectedExit, CollectionNotFound, ParseError, Exit
 from .terminals import pty_size
 from .util import debug, enable_logging, helpline
 
+if TYPE_CHECKING:
+    from .loader import Loader
+    from .parser import ParseResult
+    from .util import Lexicon
+
 
 class Program:
     """
     Manages top-level CLI invocation, typically via ``setup.py`` entrypoints.
 
     Designed for distributing Invoke task collections as standalone programs,
     but also used internally to implement the ``invoke`` program itself.
@@ -24,15 +39,17 @@
     .. seealso::
         :ref:`reusing-as-a-binary` for a tutorial/walkthrough of this
         functionality.
 
     .. versionadded:: 1.0
     """
 
-    def core_args(self):
+    core: "ParseResult"
+
+    def core_args(self) -> List["Argument"]:
         """
         Return default core `.Argument` objects, as a list.
 
         .. versionadded:: 1.0
         """
         # Arguments present always, even when wrapped as a different binary
         return [
@@ -128,15 +145,15 @@
                 names=("write-pyc",),
                 kind=bool,
                 default=False,
                 help="Enable creation of .pyc files.",
             ),
         ]
 
-    def task_args(self):
+    def task_args(self) -> List["Argument"]:
         """
         Return default task-related `.Argument` objects, as a list.
 
         These are only added to the core args in "task runner" mode (the
         default for ``invoke`` itself) - they are omitted when the constructor
         is given a non-empty ``namespace`` argument ("bundled namespace" mode).
 
@@ -157,33 +174,34 @@
             ),
             Argument(
                 names=("search-root", "r"),
                 help="Change root directory used for finding task modules.",
             ),
         ]
 
+    argv: List[str]
     # Other class-level global variables a subclass might override sometime
     # maybe?
     leading_indent_width = 2
     leading_indent = " " * leading_indent_width
     indent_width = 4
     indent = " " * indent_width
     col_padding = 3
 
     def __init__(
         self,
-        version=None,
-        namespace=None,
-        name=None,
-        binary=None,
-        loader_class=None,
-        executor_class=None,
-        config_class=None,
-        binary_names=None,
-    ):
+        version: Optional[str] = None,
+        namespace: Optional["Collection"] = None,
+        name: Optional[str] = None,
+        binary: Optional[str] = None,
+        loader_class: Optional[Type["Loader"]] = None,
+        executor_class: Optional[Type["Executor"]] = None,
+        config_class: Optional[Type["Config"]] = None,
+        binary_names: Optional[List[str]] = None,
+    ) -> None:
         """
         Create a new, parameterized `.Program` instance.
 
         :param str version:
             The program's version, e.g. ``"0.1.0"``. Defaults to ``"unknown"``.
 
         :param namespace:
@@ -257,35 +275,35 @@
         self.version = "unknown" if version is None else version
         self.namespace = namespace
         self._name = name
         # TODO 3.0: rename binary to binary_help_name or similar. (Or write
         # code to autogenerate it from binary_names.)
         self._binary = binary
         self._binary_names = binary_names
-        self.argv = None
+        self.argv = []
         self.loader_class = loader_class or FilesystemLoader
         self.executor_class = executor_class or Executor
         self.config_class = config_class or Config
 
-    def create_config(self):
+    def create_config(self) -> None:
         """
         Instantiate a `.Config` (or subclass, depending) for use in task exec.
 
         This Config is fully usable but will lack runtime-derived data like
         project & runtime config files, CLI arg overrides, etc. That data is
         added later in `update_config`. See `.Config` docstring for lifecycle
         details.
 
         :returns: ``None``; sets ``self.config`` instead.
 
         .. versionadded:: 1.0
         """
         self.config = self.config_class()
 
-    def update_config(self, merge=True):
+    def update_config(self, merge: bool = True) -> None:
         """
         Update the previously instantiated `.Config` with parsed data.
 
         For example, this is how ``--echo`` is able to override the default
         config value for ``run.echo``.
 
         :param bool merge:
@@ -330,15 +348,15 @@
         if runtime_path is None:
             runtime_path = os.environ.get("INVOKE_RUNTIME_CONFIG", None)
         self.config.set_runtime_path(runtime_path)
         self.config.load_runtime(merge=False)
         if merge:
             self.config.merge()
 
-    def run(self, argv=None, exit=True):
+    def run(self, argv: Optional[List[str]] = None, exit: bool = True) -> None:
         """
         Execute main CLI logic, based on ``argv``.
 
         :param argv:
             The arguments to execute against. May be ``None``, a list of
             strings, or a string. See `.normalize_argv` for details.
 
@@ -399,15 +417,15 @@
                     code = 1
                 sys.exit(code)
             else:
                 debug("Invoked as run(..., exit=False), ignoring exception")
         except KeyboardInterrupt:
             sys.exit(1)  # Same behavior as Python itself outside of REPL
 
-    def parse_core(self, argv):
+    def parse_core(self, argv: Optional[List[str]]) -> None:
         debug("argv given to Program.run: {!r}".format(argv))
         self.normalize_argv(argv)
 
         # Obtain core args (sets self.core)
         self.parse_core_args()
         debug("Finished parsing core args")
 
@@ -429,15 +447,15 @@
         if self.args["print-completion-script"].value:
             print_completion_script(
                 shell=self.args["print-completion-script"].value,
                 names=self.binary_names,
             )
             raise Exit
 
-    def parse_collection(self):
+    def parse_collection(self) -> None:
         """
         Load a tasks collection & project-level config.
 
         .. versionadded:: 1.0
         """
         # Load a collection of tasks unless one was already set.
         if self.namespace is not None:
@@ -458,22 +476,22 @@
                 )
                 self.print_help()
                 raise Exit
             self.load_collection()
         # Set these up for potential use later when listing tasks
         # TODO: be nice if these came from the config...! Users would love to
         # say they default to nested for example. Easy 2.x feature-add.
-        self.list_root = None
-        self.list_depth = None
+        self.list_root: Optional[str] = None
+        self.list_depth: Optional[int] = None
         self.list_format = "flat"
         self.scoped_collection = self.collection
 
         # TODO: load project conf, if possible, gracefully
 
-    def parse_cleanup(self):
+    def parse_cleanup(self) -> None:
         """
         Post-parsing, pre-execution steps such as --help, --list, etc.
 
         .. versionadded:: 1.0
         """
         halp = self.args.help.value
 
@@ -527,22 +545,22 @@
         # Fallback behavior if no tasks were given & no default specified
         # (mostly a subroutine for overriding purposes)
         # NOTE: when there is a default task, Executor will select it when no
         # tasks were found in CLI parsing.
         if not self.tasks and not self.collection.default:
             self.no_tasks_given()
 
-    def no_tasks_given(self):
+    def no_tasks_given(self) -> None:
         debug(
             "No tasks specified for execution and no default task; printing global help as fallback"  # noqa
         )
         self.print_help()
         raise Exit
 
-    def execute(self):
+    def execute(self) -> None:
         """
         Hand off data & tasks-to-execute specification to an `.Executor`.
 
         .. note::
             Client code just wanting a different `.Executor` subclass can just
             set ``executor_class`` in `.__init__`, or override
             ``tasks.executor_class`` anywhere in the :ref:`config system
@@ -560,15 +578,15 @@
             # for cases where module exists but class name does not? More
             # "normal" but also its own possible source of bugs/confusion...
             module = import_module(module_path)
             klass = getattr(module, class_name)
         executor = klass(self.collection, self.config, self.core)
         executor.execute(*self.tasks)
 
-    def normalize_argv(self, argv):
+    def normalize_argv(self, argv: Optional[List[str]]) -> None:
         """
         Massages ``argv`` into a useful list of strings.
 
         **If None** (the default), uses `sys.argv`.
 
         **If a non-string iterable**, uses that in place of `sys.argv`.
 
@@ -584,116 +602,119 @@
             debug("argv was None; using sys.argv: {!r}".format(argv))
         elif isinstance(argv, str):
             argv = argv.split()
             debug("argv was string-like; splitting: {!r}".format(argv))
         self.argv = argv
 
     @property
-    def name(self):
+    def name(self) -> str:
         """
         Derive program's human-readable name based on `.binary`.
 
         .. versionadded:: 1.0
         """
         return self._name or self.binary.capitalize()
 
     @property
-    def called_as(self):
+    def called_as(self) -> str:
         """
         Returns the program name we were actually called as.
 
         Specifically, this is the (Python's os module's concept of a) basename
         of the first argument in the parsed argument vector.
 
         .. versionadded:: 1.2
         """
-        return os.path.basename(self.argv[0])
+        # XXX: defaults to empty string if 'argv' is '[]' or 'None'
+        return os.path.basename(self.argv[0]) if self.argv else ""
 
     @property
-    def binary(self):
+    def binary(self) -> str:
         """
         Derive program's help-oriented binary name(s) from init args & argv.
 
         .. versionadded:: 1.0
         """
         return self._binary or self.called_as
 
     @property
-    def binary_names(self):
+    def binary_names(self) -> List[str]:
         """
         Derive program's completion-oriented binary name(s) from args & argv.
 
         .. versionadded:: 1.2
         """
         return self._binary_names or [self.called_as]
 
     # TODO 3.0: ugh rename this or core_args, they are too confusing
     @property
-    def args(self):
+    def args(self) -> "Lexicon":
         """
         Obtain core program args from ``self.core`` parse result.
 
         .. versionadded:: 1.0
         """
         return self.core[0].args
 
     @property
-    def initial_context(self):
+    def initial_context(self) -> ParserContext:
         """
         The initial parser context, aka core program flags.
 
         The specific arguments contained therein will differ depending on
         whether a bundled namespace was specified in `.__init__`.
 
         .. versionadded:: 1.0
         """
         args = self.core_args()
         if self.namespace is None:
             args += self.task_args()
         return ParserContext(args=args)
 
-    def print_version(self):
+    def print_version(self) -> None:
         print("{} {}".format(self.name, self.version or "unknown"))
 
-    def print_help(self):
+    def print_help(self) -> None:
         usage_suffix = "task1 [--task1-opts] ... taskN [--taskN-opts]"
         if self.namespace is not None:
             usage_suffix = "<subcommand> [--subcommand-opts] ..."
         print("Usage: {} [--core-opts] {}".format(self.binary, usage_suffix))
         print("")
         print("Core options:")
         print("")
         self.print_columns(self.initial_context.help_tuples())
         if self.namespace is not None:
             self.list_tasks()
 
-    def parse_core_args(self):
+    def parse_core_args(self) -> None:
         """
         Filter out core args, leaving any tasks or their args for later.
 
         Sets ``self.core`` to the `.ParseResult` from this step.
 
         .. versionadded:: 1.0
         """
         debug("Parsing initial context (core args)")
         parser = Parser(initial=self.initial_context, ignore_unknown=True)
         self.core = parser.parse_argv(self.argv[1:])
         msg = "Core-args parse result: {!r} & unparsed: {!r}"
         debug(msg.format(self.core, self.core.unparsed))
 
-    def load_collection(self):
+    def load_collection(self) -> None:
         """
         Load a task collection based on parsed core args, or die trying.
 
         .. versionadded:: 1.0
         """
         # NOTE: start, coll_name both fall back to configuration values within
         # Loader (which may, however, get them from our config.)
         start = self.args["search-root"].value
-        loader = self.loader_class(config=self.config, start=start)
+        loader = self.loader_class(  # type: ignore
+            config=self.config, start=start
+        )
         coll_name = self.args.collection.value
         try:
             module, parent = loader.load(coll_name)
             # This is the earliest we can load project config, so we should -
             # allows project config to affect the task parsing step!
             # TODO: is it worth merging these set- and load- methods? May
             # require more tweaking of how things behave in/after __init__.
@@ -703,32 +724,34 @@
                 module,
                 loaded_from=parent,
                 auto_dash_names=self.config.tasks.auto_dash_names,
             )
         except CollectionNotFound as e:
             raise Exit("Can't find any collection named {!r}!".format(e.name))
 
-    def _update_core_context(self, context, new_args):
+    def _update_core_context(
+        self, context: ParserContext, new_args: Dict[str, Any]
+    ) -> None:
         # Update core context w/ core_via_task args, if and only if the
         # via-task version of the arg was truly given a value.
         # TODO: push this into an Argument-aware Lexicon subclass and
         # .update()?
         for key, arg in new_args.items():
             if arg.got_value:
                 context.args[key]._value = arg._value
 
-    def _make_parser(self):
+    def _make_parser(self) -> Parser:
         return Parser(
             initial=self.initial_context,
             contexts=self.collection.to_contexts(
                 ignore_unknown_help=self.config.tasks.ignore_unknown_help
             ),
         )
 
-    def parse_tasks(self):
+    def parse_tasks(self) -> None:
         """
         Parse leftover args, which are typically tasks & per-task args.
 
         Sets ``self.parser`` to the parser used, ``self.tasks`` to the
         parsed per-task contexts, and ``self.core_via_tasks`` to a context
         holding any core flags seen within the task contexts.
 
@@ -744,15 +767,15 @@
         self.core_via_tasks = result.pop(0)
         self._update_core_context(
             context=self.core[0], new_args=self.core_via_tasks.args
         )
         self.tasks = result
         debug("Resulting task contexts: {!r}".format(self.tasks))
 
-    def print_task_help(self, name):
+    def print_task_help(self, name: str) -> None:
         """
         Print help for a specific task, e.g. ``inv --help <taskname>``.
 
         .. versionadded:: 1.0
         """
         # Setup
         ctx = self.parser.contexts[name]
@@ -777,34 +800,38 @@
         print("Options:")
         if tuples:
             self.print_columns(tuples)
         else:
             print(self.leading_indent + "none")
             print("")
 
-    def list_tasks(self):
+    def list_tasks(self) -> None:
         # Short circuit if no tasks to show (Collection now implements bool)
         focus = self.scoped_collection
         if not focus:
             msg = "No tasks found in collection '{}'!"
             raise Exit(msg.format(focus.name))
         # TODO: now that flat/nested are almost 100% unified, maybe rethink
         # this a bit?
         getattr(self, "list_{}".format(self.list_format))()
 
-    def list_flat(self):
+    def list_flat(self) -> None:
         pairs = self._make_pairs(self.scoped_collection)
         self.display_with_columns(pairs=pairs)
 
-    def list_nested(self):
+    def list_nested(self) -> None:
         pairs = self._make_pairs(self.scoped_collection)
         extra = "'*' denotes collection defaults"
         self.display_with_columns(pairs=pairs, extra=extra)
 
-    def _make_pairs(self, coll, ancestors=None):
+    def _make_pairs(
+        self,
+        coll: "Collection",
+        ancestors: Optional[List[str]] = None,
+    ) -> List[Tuple[str, Optional[str]]]:
         if ancestors is None:
             ancestors = []
         pairs = []
         indent = len(ancestors) * self.indent
         ancestor_path = ".".join(x for x in ancestors)
         for name, task in sorted(coll.tasks.items()):
             is_default = name == coll.default
@@ -861,15 +888,15 @@
             if not truncate:
                 recursed_pairs = self._make_pairs(
                     coll=subcoll, ancestors=ancestors + [name]
                 )
                 pairs.extend(recursed_pairs)
         return pairs
 
-    def list_json(self):
+    def list_json(self) -> None:
         # Sanity: we can't cleanly honor the --list-depth argument without
         # changing the data schema or otherwise acting strangely; and it also
         # doesn't make a ton of sense to limit depth when the output is for a
         # script to handle. So we just refuse, for now. TODO: find better way
         if self.list_depth:
             raise Exit(
                 "The --list-depth option is not supported with JSON format!"
@@ -877,15 +904,15 @@
         # TODO: consider using something more formal re: the format this emits,
         # eg json-schema or whatever. Would simplify the
         # relatively-concise-but-only-human docs that currently describe this.
         coll = self.scoped_collection
         data = coll.serialized()
         print(json.dumps(data))
 
-    def task_list_opener(self, extra=""):
+    def task_list_opener(self, extra: str = "") -> str:
         root = self.list_root
         depth = self.list_depth
         specifier = " '{}'".format(root) if root else ""
         tail = ""
         if depth or extra:
             depthstr = "depth={}".format(depth) if depth else ""
             joiner = "; " if (depth and extra) else ""
@@ -893,30 +920,34 @@
         text = "Available{} tasks{}".format(specifier, tail)
         # TODO: do use cases w/ bundled namespace want to display things like
         # root and depth too? Leaving off for now...
         if self.namespace is not None:
             text = "Subcommands"
         return text
 
-    def display_with_columns(self, pairs, extra=""):
+    def display_with_columns(
+        self, pairs: Sequence[Tuple[str, Optional[str]]], extra: str = ""
+    ) -> None:
         root = self.list_root
         print("{}:\n".format(self.task_list_opener(extra=extra)))
         self.print_columns(pairs)
         # TODO: worth stripping this out for nested? since it's signified with
         # asterisk there? ugggh
         default = self.scoped_collection.default
         if default:
             specific = ""
             if root:
                 specific = " '{}'".format(root)
                 default = ".{}".format(default)
             # TODO: trim/prefix dots
             print("Default{} task: {}\n".format(specific, default))
 
-    def print_columns(self, tuples):
+    def print_columns(
+        self, tuples: Sequence[Tuple[str, Optional[str]]]
+    ) -> None:
         """
         Print tabbed columns from (name, help) ``tuples``.
 
         Useful for listing tasks + docstrings, flags + help strings, etc.
 
         .. versionadded:: 1.0
         """
```

### Comparing `invoke-2.0.1/invoke/util.py` & `invoke-2.1.0/invoke/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from collections import namedtuple
 from contextlib import contextmanager
+from types import TracebackType
+from typing import Any, Generator, List, IO, Optional, Tuple, Type, Union
 import io
 import logging
 import os
 import threading
 import sys
 
 # NOTE: This is the canonical location for commonly-used vendored modules,
@@ -15,37 +17,36 @@
 # TODO: would this make more sense to put _into_ invoke.vendor? That way, the
 # import lines which now read 'from .util import <third party stuff>' would be
 # more obvious. Requires packagers to leave invoke/vendor/__init__.py alone tho
 try:
     from .vendor.lexicon import Lexicon  # noqa
     from .vendor import yaml  # noqa
 except ImportError:
-    from lexicon import Lexicon  # noqa
-    import yaml  # noqa
+    from lexicon import Lexicon  # type: ignore[no-redef] # noqa
+    import yaml  # type: ignore[no-redef] # noqa
 
 
 LOG_FORMAT = "%(name)s.%(module)s.%(funcName)s: %(message)s"
 
 
-def enable_logging():
+def enable_logging() -> None:
     logging.basicConfig(level=logging.DEBUG, format=LOG_FORMAT)
 
 
 # Allow from-the-start debugging (vs toggled during load of tasks module) via
 # shell env var.
 if os.environ.get("INVOKE_DEBUG"):
     enable_logging()
 
 # Add top level logger functions to global namespace. Meh.
 log = logging.getLogger("invoke")
-for x in ("debug",):
-    globals()[x] = getattr(log, x)
+debug = log.debug
 
 
-def task_name_sort_key(name):
+def task_name_sort_key(name: str) -> Tuple[List[str], str]:
     """
     Return key tuple for use sorting dotted task names, via e.g. `sorted`.
 
     .. versionadded:: 1.0
     """
     parts = name.split(".")
     return (
@@ -56,24 +57,24 @@
         # Then we sort lexicographically by the actual task name
         parts[-1],
     )
 
 
 # TODO: Make part of public API sometime
 @contextmanager
-def cd(where):
+def cd(where: str) -> Generator[None, None, None]:
     cwd = os.getcwd()
     os.chdir(where)
     try:
         yield
     finally:
         os.chdir(cwd)
 
 
-def has_fileno(stream):
+def has_fileno(stream: IO) -> bool:
     """
     Cleanly determine whether ``stream`` has a useful ``.fileno()``.
 
     .. note::
         This function helps determine if a given file-like object can be used
         with various terminal-oriented modules and functions such as `select`,
         `termios`, and `tty`. For most of those, a fileno is all that is
@@ -89,15 +90,15 @@
     """
     try:
         return isinstance(stream.fileno(), int)
     except (AttributeError, io.UnsupportedOperation):
         return False
 
 
-def isatty(stream):
+def isatty(stream: IO) -> Union[bool, Any]:
     """
     Cleanly determine whether ``stream`` is a TTY.
 
     Specifically, first try calling ``stream.isatty()``, and if that fails
     (e.g. due to lacking the method entirely) fallback to `os.isatty`.
 
     .. note::
@@ -122,15 +123,15 @@
     elif has_fileno(stream):
         return os.isatty(stream.fileno())
     # If we got here, none of the above worked, so it's reasonable to assume
     # the darn thing isn't a real TTY.
     return False
 
 
-def helpline(obj):
+def helpline(obj: object) -> Optional[str]:
     """
     Yield an object's first docstring line, or None if there was no docstring.
 
     .. versionadded:: 1.0
     """
     docstring = obj.__doc__
     if (
@@ -157,52 +158,59 @@
     This is because this thread's entire point is to wrap behavior around the
     thread's execution; subclasses could not redefine ``run()`` without
     breaking that functionality.
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """
         Create a new exception-handling thread instance.
 
         Takes all regular `threading.Thread` keyword arguments, via
         ``**kwargs`` for easier display of thread identity when raising
         captured exceptions.
         """
         super().__init__(**kwargs)
         # No record of why, but Fabric used daemon threads ever since the
         # switch from select.select, so let's keep doing that.
         self.daemon = True
         # Track exceptions raised in run()
         self.kwargs = kwargs
-        self.exc_info = None
+        # TODO: legacy cruft that needs to be removed
+        self.exc_info: Optional[
+            Union[
+                Tuple[Type[BaseException], BaseException, TracebackType],
+                Tuple[None, None, None],
+            ]
+        ] = None
 
-    def run(self):
+    def run(self) -> None:
         try:
             # Allow subclasses implemented using the "override run()'s body"
             # approach to work, by using _run() instead of run(). If that
             # doesn't appear to be the case, then assume we're being used
             # directly and just use super() ourselves.
-            if hasattr(self, "_run") and callable(self._run):
+            # XXX https://github.com/python/mypy/issues/1424
+            if hasattr(self, "_run") and callable(self._run):  # type: ignore
                 # TODO: this could be:
                 # - io worker with no 'result' (always local)
                 # - tunnel worker, also with no 'result' (also always local)
                 # - threaded concurrent run(), sudo(), put(), etc, with a
                 # result (not necessarily local; might want to be a subproc or
                 # whatever eventually)
                 # TODO: so how best to conditionally add a "capture result
                 # value of some kind"?
                 # - update so all use cases use subclassing, add functionality
                 # alongside self.exception() that is for the result of _run()
                 # - split out class that does not care about result of _run()
                 # and let it continue acting like a normal thread (meh)
                 # - assume the run/sudo/etc case will use a queue inside its
                 # worker body, orthogonal to how exception handling works
-                self._run()
+                self._run()  # type: ignore
             else:
                 super().run()
         except BaseException:
             # Store for actual reraising later
             self.exc_info = sys.exc_info()
             # And log now, in case we never get to later (e.g. if executing
             # program is hung waiting for us to do something)
@@ -210,15 +218,15 @@
             # Name is either target function's dunder-name, or just "_run" if
             # we were run subclass-wise.
             name = "_run"
             if "target" in self.kwargs:
                 name = self.kwargs["target"].__name__
             debug(msg.format(self.exc_info[1], name))  # noqa
 
-    def exception(self):
+    def exception(self) -> Optional["ExceptionWrapper"]:
         """
         If an exception occurred, return an `.ExceptionWrapper` around it.
 
         :returns:
             An `.ExceptionWrapper` managing the result of `sys.exc_info`, if an
             exception was raised during thread execution. If no exception
             occurred, returns ``None`` instead.
@@ -226,30 +234,30 @@
         .. versionadded:: 1.0
         """
         if self.exc_info is None:
             return None
         return ExceptionWrapper(self.kwargs, *self.exc_info)
 
     @property
-    def is_dead(self):
+    def is_dead(self) -> bool:
         """
         Returns ``True`` if not alive and has a stored exception.
 
         Used to detect threads that have excepted & shut down.
 
         .. versionadded:: 1.0
         """
         # NOTE: it seems highly unlikely that a thread could still be
         # is_alive() but also have encountered an exception. But hey. Why not
         # be thorough?
         return (not self.is_alive()) and self.exc_info is not None
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         # TODO: beef this up more
-        return self.kwargs["target"].__name__
+        return str(self.kwargs["target"].__name__)
 
 
 # NOTE: ExceptionWrapper defined here, not in exceptions.py, to avoid circular
 # dependency issues (e.g. Failure subclasses need to use some bits from this
 # module...)
 #: A namedtuple wrapping a thread-borne exception & that thread's arguments.
 #: Mostly used as an intermediate between `.ExceptionHandlingThread` (which
```

### Comparing `invoke-2.0.1/invoke/runners.py` & `invoke-2.1.0/invoke/runners.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 import errno
 import locale
 import os
 import struct
-from subprocess import Popen, PIPE
 import sys
 import threading
 import time
 import signal
+from subprocess import Popen, PIPE
+from types import TracebackType
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Generator,
+    IO,
+    List,
+    Optional,
+    Tuple,
+    Type,
+)
 
 # Import some platform-specific things at top level so they can be mocked for
 # tests.
 try:
     import pty
 except ImportError:
-    pty = None
+    pty = None  # type: ignore[assignment]
 try:
     import fcntl
 except ImportError:
-    fcntl = None
+    fcntl = None  # type: ignore[assignment]
 try:
     import termios
 except ImportError:
-    termios = None
+    termios = None  # type: ignore[assignment]
 
 from .exceptions import (
     UnexpectedExit,
     Failure,
     ThreadException,
     WatcherError,
     SubprocessPipeError,
@@ -36,30 +49,36 @@
     pty_size,
     character_buffered,
     ready_for_reading,
     bytes_to_read,
 )
 from .util import has_fileno, isatty, ExceptionHandlingThread
 
+if TYPE_CHECKING:
+    from .context import Context
+    from .watchers import StreamWatcher
+
 
 class Runner:
     """
     Partially-abstract core command-running API.
 
     This class is not usable by itself and must be subclassed, implementing a
     number of methods such as `start`, `wait` and `returncode`. For a subclass
     implementation example, see the source code for `.Local`.
 
     .. versionadded:: 1.0
     """
 
+    opts: Dict[str, Any]
+    using_pty: bool
     read_chunk_size = 1000
     input_sleep = 0.01
 
-    def __init__(self, context):
+    def __init__(self, context: "Context") -> None:
         """
         Create a new runner with a handle on some `.Context`.
 
         :param context:
             a `.Context` instance, used to transmit default options and provide
             access to other contextualized information (e.g. a remote-oriented
             `.Runner` might want a `.Context` subclass holding info about
@@ -91,23 +110,23 @@
         #: How many seconds to sleep on each iteration of the stdin read loop
         #: and other otherwise-fast loops.
         self.input_sleep = self.__class__.input_sleep
         #: Whether pty fallback warning has been emitted.
         self.warned_about_pty_fallback = False
         #: A list of `.StreamWatcher` instances for use by `respond`. Is filled
         #: in at runtime by `run`.
-        self.watchers = []
+        self.watchers: List["StreamWatcher"] = []
         # Optional timeout timer placeholder
-        self._timer = None
+        self._timer: Optional[threading.Timer] = None
         # Async flags (initialized for 'finally' referencing in case something
         # goes REAL bad during options parsing)
         self._asynchronous = False
         self._disowned = False
 
-    def run(self, command, **kwargs):
+    def run(self, command: str, **kwargs: Any) -> Optional["Result"]:
         """
         Execute ``command``, returning an instance of `Result` once complete.
 
         By default, this method is synchronous (it only returns once the
         subprocess has completed), and allows interactive keyboard
         communication with the subprocess.
 
@@ -374,18 +393,18 @@
         """
         try:
             return self._run_body(command, **kwargs)
         finally:
             if not (self._asynchronous or self._disowned):
                 self.stop()
 
-    def echo(self, command):
+    def echo(self, command: str) -> None:
         print(self.opts["echo_format"].format(command=command))
 
-    def _setup(self, command, kwargs):
+    def _setup(self, command: str, kwargs: Any) -> None:
         """
         Prepare data on ``self`` so we're ready to start running.
         """
         # Normalize kwargs w/ config; sets self.opts, self.streams
         self._unify_kwargs_with_config(kwargs)
         # Environment setup
         self.env = self.generate_env(
@@ -405,45 +424,45 @@
             shell=self.opts["shell"],
             env=self.env,
             pty=self.using_pty,
             hide=self.opts["hide"],
             encoding=self.encoding,
         )
 
-    def _run_body(self, command, **kwargs):
+    def _run_body(self, command: str, **kwargs: Any) -> Optional["Result"]:
         # Prepare all the bits n bobs.
         self._setup(command, kwargs)
         # If dry-run, stop here.
         if self.opts["dry"]:
             return self.generate_result(
                 **dict(self.result_kwargs, stdout="", stderr="", exited=0)
             )
         # Start executing the actual command (runs in background)
         self.start(command, self.opts["shell"], self.env)
         # If disowned, we just stop here - no threads, no timer, no error
         # checking, nada.
         if self._disowned:
-            return
+            return None
         # Stand up & kick off IO, timer threads
         self.start_timer(self.opts["timeout"])
         self.threads, self.stdout, self.stderr = self.create_io_threads()
         for thread in self.threads.values():
             thread.start()
         # Wrap up or promise that we will, depending
         return self.make_promise() if self._asynchronous else self._finish()
 
-    def make_promise(self):
+    def make_promise(self) -> "Promise":
         """
         Return a `Promise` allowing async control of the rest of lifecycle.
 
         .. versionadded:: 1.4
         """
         return Promise(self)
 
-    def _finish(self):
+    def _finish(self) -> "Result":
         # Wait for subprocess to run, forwarding signals as we get them.
         try:
             while True:
                 try:
                     self.wait()
                     break  # done waiting!
                 # Don't locally stop on ^C, only forward it:
@@ -495,15 +514,15 @@
         timeout = self.opts["timeout"]
         if timeout is not None and self.timed_out:
             raise CommandTimedOut(result, timeout=timeout)
         if not (result or self.opts["warn"]):
             raise UnexpectedExit(result)
         return result
 
-    def _unify_kwargs_with_config(self, kwargs):
+    def _unify_kwargs_with_config(self, kwargs: Any) -> None:
         """
         Unify `run` kwargs with config options to arrive at local options.
 
         Sets:
 
         - ``self.opts`` - opts dict
         - ``self.streams`` - map of stream names to stream target values
@@ -555,15 +574,15 @@
         self.using_pty = self.should_use_pty(opts["pty"], opts["fallback"])
         if opts["watchers"]:
             self.watchers = opts["watchers"]
         # Set data
         self.opts = opts
         self.streams = {"out": out_stream, "err": err_stream, "in": in_stream}
 
-    def _collate_result(self, watcher_errors):
+    def _collate_result(self, watcher_errors: List[WatcherError]) -> "Result":
         # At this point, we had enough success that we want to be returning or
         # raising detailed info about our execution; so we generate a Result.
         stdout = "".join(self.stdout)
         stderr = "".join(self.stderr)
         if WINDOWS:
             # "Universal newlines" - replace all standard forms of
             # newline with \n. This is not technically Windows related
@@ -583,15 +602,15 @@
         result = self.generate_result(
             **dict(
                 self.result_kwargs, stdout=stdout, stderr=stderr, exited=exited
             )
         )
         return result
 
-    def _thread_join_timeout(self, target):
+    def _thread_join_timeout(self, target: Callable) -> Optional[int]:
         # Add a timeout to out/err thread joins when it looks like they're not
         # dead but their counterpart is dead; this indicates issue #351 (fixed
         # by #432) where the subproc may hang because its stdout (or stderr) is
         # no longer being consumed by the dead thread (and a pipe is filling
         # up.) In that case, the non-dead thread is likely to block forever on
         # a `recv` unless we add this timeout.
         if target == self.handle_stdin:
@@ -599,24 +618,27 @@
         opposite = self.handle_stderr
         if target == self.handle_stderr:
             opposite = self.handle_stdout
         if opposite in self.threads and self.threads[opposite].is_dead:
             return 1
         return None
 
-    def create_io_threads(self):
+    def create_io_threads(
+        self,
+    ) -> Tuple[Dict[Callable, ExceptionHandlingThread], List[str], List[str]]:
         """
         Create and return a dictionary of IO thread worker objects.
 
         Caller is expected to handle persisting and/or starting the wrapped
         threads.
         """
-        stdout, stderr = [], []
+        stdout: List[str] = []
+        stderr: List[str] = []
         # Set up IO thread parameters (format - body_func: {kwargs})
-        thread_args = {
+        thread_args: Dict[Callable, Any] = {
             self.handle_stdout: {
                 "buffer_": stdout,
                 "hide": "stdout" in self.opts["hide"],
                 "output": self.streams["out"],
             }
         }
         # After opt processing above, in_stream will be a real stream obj or
@@ -638,27 +660,27 @@
         # Kick off IO threads
         threads = {}
         for target, kwargs in thread_args.items():
             t = ExceptionHandlingThread(target=target, kwargs=kwargs)
             threads[target] = t
         return threads, stdout, stderr
 
-    def generate_result(self, **kwargs):
+    def generate_result(self, **kwargs: Any) -> "Result":
         """
         Create & return a suitable `Result` instance from the given ``kwargs``.
 
         Subclasses may wish to override this in order to manipulate things or
         generate a `Result` subclass (e.g. ones containing additional metadata
         besides the default).
 
         .. versionadded:: 1.0
         """
         return Result(**kwargs)
 
-    def read_proc_output(self, reader):
+    def read_proc_output(self, reader: Callable) -> Generator[str, None, None]:
         """
         Iteratively read & decode bytes from a subprocess' out/err stream.
 
         :param reader:
             A literal reader function/partial, wrapping the actual stream
             object in question, which takes a number of bytes to read, and
             returns that many bytes (or ``None``).
@@ -683,15 +705,15 @@
         # condition).
         while True:
             data = reader(self.read_chunk_size)
             if not data:
                 break
             yield self.decode(data)
 
-    def write_our_output(self, stream, string):
+    def write_our_output(self, stream: IO, string: str) -> None:
         """
         Write ``string`` to ``stream``.
 
         Also calls ``.flush()`` on ``stream`` to ensure that real terminal
         streams don't buffer.
 
         :param stream:
@@ -703,15 +725,21 @@
         :returns: ``None``.
 
         .. versionadded:: 1.0
         """
         stream.write(string)
         stream.flush()
 
-    def _handle_output(self, buffer_, hide, output, reader):
+    def _handle_output(
+        self,
+        buffer_: List[str],
+        hide: bool,
+        output: IO,
+        reader: Callable,
+    ) -> None:
         # TODO: store un-decoded/raw bytes somewhere as well...
         for data in self.read_proc_output(reader):
             # Echo to local stdout if necessary
             # TODO: should we rephrase this as "if you want to hide, give me a
             # dummy output stream, e.g. something like /dev/null"? Otherwise, a
             # combo of 'hide=stdout' + 'here is an explicit out_stream' means
             # out_stream is never written to, and that seems...odd.
@@ -721,15 +749,17 @@
             # result after execution completes.
             # NOTE: this is threadsafe insofar as no reading occurs until after
             # the thread is join()'d.
             buffer_.append(data)
             # Run our specific buffer through the autoresponder framework
             self.respond(buffer_)
 
-    def handle_stdout(self, buffer_, hide, output):
+    def handle_stdout(
+        self, buffer_: List[str], hide: bool, output: IO
+    ) -> None:
         """
         Read process' stdout, storing into a buffer & printing/parsing.
 
         Intended for use as a thread target. Only terminates when all stdout
         from the subprocess has been read.
 
         :param buffer_: The capture buffer shared with the main thread.
@@ -742,28 +772,30 @@
 
         .. versionadded:: 1.0
         """
         self._handle_output(
             buffer_, hide, output, reader=self.read_proc_stdout
         )
 
-    def handle_stderr(self, buffer_, hide, output):
+    def handle_stderr(
+        self, buffer_: List[str], hide: bool, output: IO
+    ) -> None:
         """
         Read process' stderr, storing into a buffer & printing/parsing.
 
         Identical to `handle_stdout` except for the stream read from; see its
         docstring for API details.
 
         .. versionadded:: 1.0
         """
         self._handle_output(
             buffer_, hide, output, reader=self.read_proc_stderr
         )
 
-    def read_our_stdin(self, input_):
+    def read_our_stdin(self, input_: IO) -> Optional[str]:
         """
         Read & decode bytes from a local stdin stream.
 
         :param input_:
             Actual stream object to read from. Maps to ``in_stream`` in `run`,
             so will often be ``sys.stdin``, but might be any stream-like
             object.
@@ -795,15 +827,20 @@
             # streams, usually yes; from file-like objects, often no.)
             if bytes_ and isinstance(bytes_, bytes):
                 # TODO: will decoding 1 byte at a time break multibyte
                 # character encodings? How to square interactivity with that?
                 bytes_ = self.decode(bytes_)
         return bytes_
 
-    def handle_stdin(self, input_, output, echo):
+    def handle_stdin(
+        self,
+        input_: IO,
+        output: IO,
+        echo: bool = False,
+    ) -> None:
         """
         Read local stdin, copying into process' stdin as necessary.
 
         Intended for use as a thread target.
 
         .. note::
             Because real terminal stdin streams have no well-defined "end", if
@@ -856,29 +893,29 @@
                 # stdin. (NOTE: If we only test the former, we may encounter
                 # race conditions re: unread stdin.)
                 if self.program_finished.is_set() and not data:
                     break
                 # Take a nap so we're not chewing CPU.
                 time.sleep(self.input_sleep)
 
-    def should_echo_stdin(self, input_, output):
+    def should_echo_stdin(self, input_: IO, output: IO) -> bool:
         """
         Determine whether data read from ``input_`` should echo to ``output``.
 
         Used by `handle_stdin`; tests attributes of ``input_`` and ``output``.
 
         :param input_: Input stream (file-like object).
         :param output: Output stream (file-like object).
         :returns: A ``bool``.
 
         .. versionadded:: 1.0
         """
         return (not self.using_pty) and isatty(input_)
 
-    def respond(self, buffer_):
+    def respond(self, buffer_: List[str]) -> None:
         """
         Write to the program's stdin in response to patterns in ``buffer_``.
 
         The patterns and responses are driven by the `.StreamWatcher` instances
         from the ``watchers`` kwarg of `run` - see :doc:`/concepts/watchers`
         for a conceptual overview.
 
@@ -897,30 +934,32 @@
         # StringIO or cStringIO (tho the latter doesn't do Unicode well?) which
         # is apparently even more efficient.
         stream = "".join(buffer_)
         for watcher in self.watchers:
             for response in watcher.submit(stream):
                 self.write_proc_stdin(response)
 
-    def generate_env(self, env, replace_env):
+    def generate_env(
+        self, env: Dict[str, Any], replace_env: bool
+    ) -> Dict[str, Any]:
         """
         Return a suitable environment dict based on user input & behavior.
 
         :param dict env: Dict supplying overrides or full env, depending.
         :param bool replace_env:
             Whether ``env`` updates, or is used in place of, the value of
             `os.environ`.
 
         :returns: A dictionary of shell environment vars.
 
         .. versionadded:: 1.0
         """
         return env if replace_env else dict(os.environ, **env)
 
-    def should_use_pty(self, pty, fallback):
+    def should_use_pty(self, pty: bool, fallback: bool) -> bool:
         """
         Should execution attempt to use a pseudo-terminal?
 
         :param bool pty:
             Whether the user explicitly asked for a pty.
         :param bool fallback:
             Whether falling back to non-pty execution should be allowed, in
@@ -928,15 +967,15 @@
 
         .. versionadded:: 1.0
         """
         # NOTE: fallback not used: no falling back implemented by default.
         return pty
 
     @property
-    def has_dead_threads(self):
+    def has_dead_threads(self) -> bool:
         """
         Detect whether any IO threads appear to have terminated unexpectedly.
 
         Used during process-completion waiting (in `wait`) to ensure we don't
         deadlock our child process if our IO processing threads have
         errored/died.
 
@@ -944,55 +983,55 @@
             ``True`` if any threads appear to have terminated with an
             exception, ``False`` otherwise.
 
         .. versionadded:: 1.0
         """
         return any(x.is_dead for x in self.threads.values())
 
-    def wait(self):
+    def wait(self) -> None:
         """
         Block until the running command appears to have exited.
 
         :returns: ``None``.
 
         .. versionadded:: 1.0
         """
         while True:
             proc_finished = self.process_is_finished
             dead_threads = self.has_dead_threads
             if proc_finished or dead_threads:
                 break
             time.sleep(self.input_sleep)
 
-    def write_proc_stdin(self, data):
+    def write_proc_stdin(self, data: str) -> None:
         """
         Write encoded ``data`` to the running process' stdin.
 
         :param data: A Unicode string.
 
         :returns: ``None``.
 
         .. versionadded:: 1.0
         """
         # Encode always, then request implementing subclass to perform the
         # actual write to subprocess' stdin.
         self._write_proc_stdin(data.encode(self.encoding))
 
-    def decode(self, data):
+    def decode(self, data: bytes) -> str:
         """
         Decode some ``data`` bytes, returning Unicode.
 
         .. versionadded:: 1.0
         """
         # NOTE: yes, this is a 1-liner. The point is to make it much harder to
         # forget to use 'replace' when decoding :)
         return data.decode(self.encoding, "replace")
 
     @property
-    def process_is_finished(self):
+    def process_is_finished(self) -> bool:
         """
         Determine whether our subprocess has terminated.
 
         .. note::
             The implementation of this method should be nonblocking, as it is
             used within a query/poll loop.
 
@@ -1000,15 +1039,15 @@
             ``True`` if the subprocess has finished running, ``False``
             otherwise.
 
         .. versionadded:: 1.0
         """
         raise NotImplementedError
 
-    def start(self, command, shell, env):
+    def start(self, command: str, shell: str, env: Dict[str, Any]) -> None:
         """
         Initiate execution of ``command`` (via ``shell``, with ``env``).
 
         Typically this means use of a forked subprocess or requesting start of
         execution on a remote system.
 
         In most cases, this method will also set subclass-specific member
@@ -1023,84 +1062,84 @@
         :param dict env:
             Environment dict used to prep shell environment.
 
         .. versionadded:: 1.0
         """
         raise NotImplementedError
 
-    def start_timer(self, timeout):
+    def start_timer(self, timeout: int) -> None:
         """
         Start a timer to `kill` our subprocess after ``timeout`` seconds.
         """
         if timeout is not None:
             self._timer = threading.Timer(timeout, self.kill)
             self._timer.start()
 
-    def read_proc_stdout(self, num_bytes):
+    def read_proc_stdout(self, num_bytes: int) -> Optional[bytes]:
         """
         Read ``num_bytes`` from the running process' stdout stream.
 
         :param int num_bytes: Number of bytes to read at maximum.
 
         :returns: A string/bytes object.
 
         .. versionadded:: 1.0
         """
         raise NotImplementedError
 
-    def read_proc_stderr(self, num_bytes):
+    def read_proc_stderr(self, num_bytes: int) -> Optional[bytes]:
         """
         Read ``num_bytes`` from the running process' stderr stream.
 
         :param int num_bytes: Number of bytes to read at maximum.
 
         :returns: A string/bytes object.
 
         .. versionadded:: 1.0
         """
         raise NotImplementedError
 
-    def _write_proc_stdin(self, data):
+    def _write_proc_stdin(self, data: bytes) -> None:
         """
         Write ``data`` to running process' stdin.
 
         This should never be called directly; it's for subclasses to implement.
         See `write_proc_stdin` for the public API call.
 
         :param data: Already-encoded byte data suitable for writing.
 
         :returns: ``None``.
 
         .. versionadded:: 1.0
         """
         raise NotImplementedError
 
-    def close_proc_stdin(self):
+    def close_proc_stdin(self) -> None:
         """
         Close running process' stdin.
 
         :returns: ``None``.
 
         .. versionadded:: 1.3
         """
         raise NotImplementedError
 
-    def default_encoding(self):
+    def default_encoding(self) -> str:
         """
         Return a string naming the expected encoding of subprocess streams.
 
         This return value should be suitable for use by encode/decode methods.
 
         .. versionadded:: 1.0
         """
         # TODO: probably wants to be 2 methods, one for local and one for
         # subprocess. For now, good enough to assume both are the same.
         return default_encoding()
 
-    def send_interrupt(self, interrupt):
+    def send_interrupt(self, interrupt: "KeyboardInterrupt") -> None:
         """
         Submit an interrupt signal to the running subprocess.
 
         In almost all implementations, the default behavior is what will be
         desired: submit ``\x03`` to the subprocess' stdin pipe. However, we
         leave this as a public method in case this default needs to be
         augmented or replaced.
@@ -1110,61 +1149,63 @@
 
         :returns: ``None``.
 
         .. versionadded:: 1.0
         """
         self.write_proc_stdin("\x03")
 
-    def returncode(self):
+    def returncode(self) -> Optional[int]:
         """
         Return the numeric return/exit code resulting from command execution.
 
-        :returns: `int`
+        :returns:
+            `int`, if any reasonable return code could be determined, or
+            ``None`` in corner cases where that was not possible.
 
         .. versionadded:: 1.0
         """
         raise NotImplementedError
 
-    def stop(self):
+    def stop(self) -> None:
         """
         Perform final cleanup, if necessary.
 
         This method is called within a ``finally`` clause inside the main `run`
         method. Depending on the subclass, it may be a no-op, or it may do
         things such as close network connections or open files.
 
         :returns: ``None``
 
         .. versionadded:: 1.0
         """
         if self._timer:
             self._timer.cancel()
 
-    def kill(self):
+    def kill(self) -> None:
         """
         Forcibly terminate the subprocess.
 
         Typically only used by the timeout functionality.
 
         This is often a "best-effort" attempt, e.g. remote subprocesses often
         must settle for simply shutting down the local side of the network
         connection and hoping the remote end eventually gets the message.
         """
         raise NotImplementedError
 
     @property
-    def timed_out(self):
+    def timed_out(self) -> bool:
         """
         Returns ``True`` if the subprocess stopped because it timed out.
 
         .. versionadded:: 1.3
         """
         # Timer expiry implies we did time out. (The timer itself will have
         # killed the subprocess, allowing us to even get to this point.)
-        return self._timer and not self._timer.is_alive()
+        return bool(self._timer and not self._timer.is_alive())
 
 
 class Local(Runner):
     """
     Execute a command on the local system in a subprocess.
 
     .. note::
@@ -1176,33 +1217,33 @@
         a warning to stderr.
 
         To disable this behavior, say ``fallback=False``.
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, context):
+    def __init__(self, context: "Context") -> None:
         super().__init__(context)
         # Bookkeeping var for pty use case
-        self.status = None
+        self.status = 0
 
-    def should_use_pty(self, pty=False, fallback=True):
+    def should_use_pty(self, pty: bool = False, fallback: bool = True) -> bool:
         use_pty = False
         if pty:
             use_pty = True
             # TODO: pass in & test in_stream, not sys.stdin
             if not has_fileno(sys.stdin) and fallback:
                 if not self.warned_about_pty_fallback:
                     err = "WARNING: stdin has no fileno; falling back to non-pty execution!\n"  # noqa
                     sys.stderr.write(err)
                     self.warned_about_pty_fallback = True
                 use_pty = False
         return use_pty
 
-    def read_proc_stdout(self, num_bytes):
+    def read_proc_stdout(self, num_bytes: int) -> Optional[bytes]:
         # Obtain useful read-some-bytes function
         if self.using_pty:
             # Need to handle spurious OSErrors on some Linux platforms.
             try:
                 data = os.read(self.parent_fd, num_bytes)
             except OSError as e:
                 # Only eat I/O specific OSErrors so we don't hide others
@@ -1215,44 +1256,60 @@
                 )
                 if not any(error in stringified for error in io_errors):
                     raise
                 # The bad OSErrors happen after all expected output has
                 # appeared, so we return a falsey value, which triggers the
                 # "end of output" logic in code using reader functions.
                 data = None
-        else:
+        elif self.process and self.process.stdout:
             data = os.read(self.process.stdout.fileno(), num_bytes)
+        else:
+            data = None
         return data
 
-    def read_proc_stderr(self, num_bytes):
+    def read_proc_stderr(self, num_bytes: int) -> Optional[bytes]:
         # NOTE: when using a pty, this will never be called.
         # TODO: do we ever get those OSErrors on stderr? Feels like we could?
-        return os.read(self.process.stderr.fileno(), num_bytes)
+        if self.process and self.process.stderr:
+            return os.read(self.process.stderr.fileno(), num_bytes)
+        return None
 
-    def _write_proc_stdin(self, data):
+    def _write_proc_stdin(self, data: bytes) -> None:
         # NOTE: parent_fd from os.fork() is a read/write pipe attached to our
         # forked process' stdout/stdin, respectively.
-        fd = self.parent_fd if self.using_pty else self.process.stdin.fileno()
+        if self.using_pty:
+            fd = self.parent_fd
+        elif self.process and self.process.stdin:
+            fd = self.process.stdin.fileno()
+        else:
+            raise SubprocessPipeError(
+                "Unable to write to missing subprocess or stdin!"
+            )
         # Try to write, ignoring broken pipes if encountered (implies child
         # process exited before the process piping stdin to us finished;
         # there's nothing we can do about that!)
         try:
-            return os.write(fd, data)
+            os.write(fd, data)
         except OSError as e:
             if "Broken pipe" not in str(e):
                 raise
 
-    def close_proc_stdin(self):
+    def close_proc_stdin(self) -> None:
         if self.using_pty:
             # there is no working scenario to tell the process that stdin
             # closed when using pty
             raise SubprocessPipeError("Cannot close stdin when pty=True")
-        self.process.stdin.close()
+        elif self.process and self.process.stdin:
+            self.process.stdin.close()
+        else:
+            raise SubprocessPipeError(
+                "Unable to close missing subprocess or stdin!"
+            )
 
-    def start(self, command, shell, env):
+    def start(self, command: str, shell: str, env: Dict[str, Any]) -> None:
         if self.using_pty:
             if pty is None:  # Encountered ImportError
                 err = "You indicated pty=True, but your platform doesn't support the 'pty' module!"  # noqa
                 sys.exit(err)
             cols, rows = pty_size()
             self.pid, self.parent_fd = pty.fork()
             # If we're the child process, load up the actual command in a
@@ -1283,39 +1340,34 @@
                 executable=shell,
                 env=env,
                 stdout=PIPE,
                 stderr=PIPE,
                 stdin=PIPE,
             )
 
-    def kill(self):
+    def kill(self) -> None:
         pid = self.pid if self.using_pty else self.process.pid
-        try:
-            os.kill(pid, signal.SIGKILL)
-        except ProcessLookupError:
-            # In odd situations where our subprocess is already dead, don't
-            # throw this upwards.
-            pass
+        os.kill(pid, signal.SIGKILL)
 
     @property
-    def process_is_finished(self):
+    def process_is_finished(self) -> bool:
         if self.using_pty:
             # NOTE:
             # https://github.com/pexpect/ptyprocess/blob/4058faa05e2940662ab6da1330aa0586c6f9cd9c/ptyprocess/ptyprocess.py#L680-L687
             # implies that Linux "requires" use of the blocking, non-WNOHANG
             # version of this call. Our testing doesn't verify this, however,
             # so...
             # NOTE: It does appear to be totally blocking on Windows, so our
             # issue #351 may be totally unsolvable there. Unclear.
             pid_val, self.status = os.waitpid(self.pid, os.WNOHANG)
             return pid_val != 0
         else:
             return self.process.poll() is not None
 
-    def returncode(self):
+    def returncode(self) -> Optional[int]:
         if self.using_pty:
             # No subprocess.returncode available; use WIFEXITED/WIFSIGNALED to
             # determine whch of WEXITSTATUS / WTERMSIG to use.
             # TODO: is it safe to just say "call all WEXITSTATUS/WTERMSIG and
             # return whichever one of them is nondefault"? Probably not?
             # NOTE: doing this in an arbitrary order should be safe since only
             # one of the WIF* methods ought to ever return True.
@@ -1328,16 +1380,15 @@
                 # 'exit code' integers.
                 code = -1 * code
             return code
             # TODO: do we care about WIFSTOPPED? Maybe someday?
         else:
             return self.process.returncode
 
-    def stop(self):
-        super().stop()
+    def stop(self) -> None:
         # If we opened a PTY for child communications, make sure to close() it,
         # otherwise long-running Invoke-using processes exhaust their file
         # descriptors eventually.
         if self.using_pty:
             try:
                 os.close(self.parent_fd)
             except Exception:
@@ -1411,49 +1462,49 @@
 
     .. versionadded:: 1.0
     """
 
     # TODO: inherit from namedtuple instead? heh (or: use attrs from pypi)
     def __init__(
         self,
-        stdout="",
-        stderr="",
-        encoding=None,
-        command="",
-        shell="",
-        env=None,
-        exited=0,
-        pty=False,
-        hide=tuple(),
+        stdout: str = "",
+        stderr: str = "",
+        encoding: Optional[str] = None,
+        command: str = "",
+        shell: str = "",
+        env: Optional[Dict[str, Any]] = None,
+        exited: int = 0,
+        pty: bool = False,
+        hide: Tuple[str, ...] = tuple(),
     ):
         self.stdout = stdout
         self.stderr = stderr
         if encoding is None:
             encoding = default_encoding()
         self.encoding = encoding
         self.command = command
         self.shell = shell
         self.env = {} if env is None else env
         self.exited = exited
         self.pty = pty
         self.hide = hide
 
     @property
-    def return_code(self):
+    def return_code(self) -> int:
         """
         An alias for ``.exited``.
 
         .. versionadded:: 1.0
         """
         return self.exited
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         return self.ok
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.exited is not None:
             desc = "Command exited with status {}.".format(self.exited)
         else:
             desc = "Command was not fully executed due to watcher error."
         ret = [desc]
         for x in ("stdout", "stderr"):
             val = getattr(self, x)
@@ -1464,43 +1515,43 @@
                     x, val.rstrip()
                 )
                 if val
                 else "(no {})".format(x)
             )
         return "\n".join(ret)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         # TODO: more? e.g. len of stdout/err? (how to represent cleanly in a
         # 'x=y' format like this? e.g. '4b' is ambiguous as to what it
         # represents
         template = "<Result cmd={!r} exited={}>"
         return template.format(self.command, self.exited)
 
     @property
-    def ok(self):
+    def ok(self) -> bool:
         """
         A boolean equivalent to ``exited == 0``.
 
         .. versionadded:: 1.0
         """
-        return self.exited == 0
+        return bool(self.exited == 0)
 
     @property
-    def failed(self):
+    def failed(self) -> bool:
         """
         The inverse of ``ok``.
 
         I.e., ``True`` if the program exited with a nonzero return code, and
         ``False`` otherwise.
 
         .. versionadded:: 1.0
         """
         return not self.ok
 
-    def tail(self, stream, count=10):
+    def tail(self, stream: str, count: int = 10) -> str:
         """
         Return the last ``count`` lines of ``stream``, plus leading whitespace.
 
         :param str stream:
             Name of some captured stream attribute, eg ``"stdout"``.
         :param int count:
             Number of lines to preserve.
@@ -1525,30 +1576,30 @@
     those that derive from `~Runner.run` kwargs and not the result of command
     execution. For example, ``command`` is replicated here, but ``stdout`` is
     not.
 
     .. versionadded:: 1.4
     """
 
-    def __init__(self, runner):
+    def __init__(self, runner: "Runner") -> None:
         """
         Create a new promise.
 
         :param runner:
             An in-flight `Runner` instance making this promise.
 
             Must already have started the subprocess and spun up IO threads.
         """
         self.runner = runner
         # Basically just want exactly this (recently refactored) kwargs dict.
         # TODO: consider proxying vs copying, but prob wait for refactor
         for key, value in self.runner.result_kwargs.items():
             setattr(self, key, value)
 
-    def join(self):
+    def join(self) -> Result:
         """
         Block until associated subprocess exits, returning/raising the result.
 
         This acts identically to the end of a synchronously executed ``run``,
         namely that:
 
         - various background threads (such as IO workers) are themselves
@@ -1562,22 +1613,31 @@
         details.
         """
         try:
             return self.runner._finish()
         finally:
             self.runner.stop()
 
-    def __enter__(self):
+    def __enter__(self) -> "Promise":
         return self
 
-    def __exit__(self, exc_type, exc_value, traceback):
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_value: BaseException,
+        exc_tb: Optional[TracebackType],
+    ) -> None:
         self.join()
 
 
-def normalize_hide(val, out_stream=None, err_stream=None):
+def normalize_hide(
+    val: Any,
+    out_stream: Optional[str] = None,
+    err_stream: Optional[str] = None,
+) -> Tuple[str, ...]:
     # Normalize to list-of-stream-names
     hide_vals = (None, False, "out", "stdout", "err", "stderr", "both", True)
     if val not in hide_vals:
         err = "'hide' got {!r} which is not in {!r}"
         raise ValueError(err.format(val, hide_vals))
     if val in (None, False):
         hide = []
@@ -1593,15 +1653,15 @@
     if out_stream is not None and "stdout" in hide:
         hide.remove("stdout")
     if err_stream is not None and "stderr" in hide:
         hide.remove("stderr")
     return tuple(hide)
 
 
-def default_encoding():
+def default_encoding() -> str:
     """
     Obtain apparent interpreter-local default text encoding.
 
     Often used as a baseline in situations where we must use SOME encoding for
     unknown-but-presumably-text bytes, and the user has not specified an
     override.
     """
```

### Comparing `invoke-2.0.1/invoke/collection.py` & `invoke-2.1.0/invoke/collection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
-import types
+from types import ModuleType
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from .util import Lexicon, helpline
 
 from .config import merge_dicts, copy_dict
 from .parser import Context as ParserContext
 from .tasks import Task
 
@@ -11,15 +12,15 @@
 class Collection:
     """
     A collection of executable tasks. See :doc:`/concepts/namespaces`.
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         """
         Create a new task collection/namespace.
 
         `.Collection` offers a set of methods for building a collection of
         tasks from scratch, plus a convenient constructor wrapping said API.
 
         In either case:
@@ -88,75 +89,72 @@
             ns.add_collection(docs, 'docs')
 
         See individual methods' API docs for details.
         """
         # Initialize
         self.tasks = Lexicon()
         self.collections = Lexicon()
-        self.default = None
+        self.default: Optional[str] = None
         self.name = None
-        self._configuration = {}
+        self._configuration: Dict[str, Any] = {}
         # Specific kwargs if applicable
         self.loaded_from = kwargs.pop("loaded_from", None)
         self.auto_dash_names = kwargs.pop("auto_dash_names", None)
         # splat-kwargs version of default value (auto_dash_names=True)
         if self.auto_dash_names is None:
             self.auto_dash_names = True
         # Name if applicable
-        args = list(args)
-        if args and isinstance(args[0], str):
-            self.name = self.transform(args.pop(0))
+        _args = list(args)
+        if _args and isinstance(args[0], str):
+            self.name = self.transform(_args.pop(0))
         # Dispatch args/kwargs
-        for arg in args:
+        for arg in _args:
             self._add_object(arg)
         # Dispatch kwargs
         for name, obj in kwargs.items():
             self._add_object(obj, name)
 
-    def _add_object(self, obj, name=None):
+    def _add_object(self, obj: Any, name: Optional[str] = None) -> None:
+        method: Callable
         if isinstance(obj, Task):
             method = self.add_task
-        elif isinstance(obj, (Collection, types.ModuleType)):
+        elif isinstance(obj, (Collection, ModuleType)):
             method = self.add_collection
         else:
             raise TypeError("No idea how to insert {!r}!".format(type(obj)))
-        return method(obj, name=name)
+        method(obj, name=name)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         task_names = list(self.tasks.keys())
         collections = ["{}...".format(x) for x in self.collections.keys()]
         return "<Collection {!r}: {}>".format(
             self.name, ", ".join(sorted(task_names) + sorted(collections))
         )
 
-    def __eq__(self, other):
-        return (
-            self.name == other.name
-            and self.tasks == other.tasks
-            and self.collections == other.collections
-        )
-
-    def __ne__(self, other):
-        return not self == other
-
-    def __nonzero__(self):
-        return self.__bool__()
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, Collection):
+            return (
+                self.name == other.name
+                and self.tasks == other.tasks
+                and self.collections == other.collections
+            )
+        return False
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         return bool(self.task_names)
 
     @classmethod
     def from_module(
         cls,
-        module,
-        name=None,
-        config=None,
-        loaded_from=None,
-        auto_dash_names=None,
-    ):
+        module: ModuleType,
+        name: Optional[str] = None,
+        config: Optional[Dict[str, Any]] = None,
+        loaded_from: Optional[str] = None,
+        auto_dash_names: Optional[bool] = None,
+    ) -> "Collection":
         """
         Return a new `.Collection` created from ``module``.
 
         Inspects ``module`` for any `.Task` instances and adds them to a new
         `.Collection`, returning it. If any explicit namespace collections
         exist (named ``ns`` or ``namespace``) a copy of that collection object
         is preferentially loaded instead.
@@ -194,15 +192,15 @@
             Identical to the same-named kwarg from the regular class
             constructor - determines whether emitted names are auto-dashed.
 
         .. versionadded:: 1.0
         """
         module_name = module.__name__.split(".")[-1]
 
-        def instantiate(obj_name=None):
+        def instantiate(obj_name: Optional[str] = None) -> "Collection":
             # Explicitly given name wins over root ns name (if applicable),
             # which wins over actual module name.
             args = [name or obj_name or module_name]
             kwargs = dict(
                 loaded_from=loaded_from, auto_dash_names=auto_dash_names
             )
             instance = cls(*args, **kwargs)
@@ -214,15 +212,17 @@
         for candidate in ("ns", "namespace"):
             obj = getattr(module, candidate, None)
             if obj and isinstance(obj, Collection):
                 # TODO: make this into Collection.clone() or similar?
                 ret = instantiate(obj_name=obj.name)
                 ret.tasks = ret._transform_lexicon(obj.tasks)
                 ret.collections = ret._transform_lexicon(obj.collections)
-                ret.default = ret.transform(obj.default)
+                ret.default = (
+                    ret.transform(obj.default) if obj.default else None
+                )
                 # Explicitly given config wins over root ns config
                 obj_config = copy_dict(obj._configuration)
                 if config:
                     merge_dicts(obj_config, config)
                 ret._configuration = obj_config
                 return ret
         # Failing that, make our own collection from the module's tasks.
@@ -231,15 +231,21 @@
         collection = instantiate()
         for task in tasks:
             collection.add_task(task)
         if config:
             collection.configure(config)
         return collection
 
-    def add_task(self, task, name=None, aliases=None, default=None):
+    def add_task(
+        self,
+        task: "Task",
+        name: Optional[str] = None,
+        aliases: Optional[Tuple[str, ...]] = None,
+        default: Optional[bool] = None,
+    ) -> None:
         """
         Add `.Task` ``task`` to this collection.
 
         :param task: The `.Task` object to add to this collection.
 
         :param name:
             Optional string name to bind to (overrides the task's own
@@ -254,16 +260,17 @@
         :param default: Whether this task should be the collection default.
 
         .. versionadded:: 1.0
         """
         if name is None:
             if task.name:
                 name = task.name
+            # XXX https://github.com/python/mypy/issues/1424
             elif hasattr(task.body, "func_name"):
-                name = task.body.func_name
+                name = task.body.func_name  # type: ignore
             elif hasattr(task.body, "__name__"):
                 name = task.__name__
             else:
                 raise ValueError("Could not obtain a name for this task!")
         name = self.transform(name)
         if name in self.collections:
             err = "Name conflict: this collection has a sub-collection named {!r} already"  # noqa
@@ -271,15 +278,20 @@
         self.tasks[name] = task
         for alias in list(task.aliases) + list(aliases or []):
             self.tasks.alias(self.transform(alias), to=name)
         if default is True or (default is None and task.is_default):
             self._check_default_collision(name)
             self.default = name
 
-    def add_collection(self, coll, name=None, default=None):
+    def add_collection(
+        self,
+        coll: "Collection",
+        name: Optional[str] = None,
+        default: Optional[bool] = None,
+    ) -> None:
         """
         Add `.Collection` ``coll`` as a sub-collection of this one.
 
         :param coll: The `.Collection` to add.
 
         :param str name:
             The name to attach the collection as. Defaults to the collection's
@@ -290,15 +302,15 @@
             be the default invocation of the parent collection.
 
         .. versionadded:: 1.0
         .. versionchanged:: 1.5
             Added the ``default`` parameter.
         """
         # Handle module-as-collection
-        if isinstance(coll, types.ModuleType):
+        if isinstance(coll, ModuleType):
             coll = Collection.from_module(coll)
         # Ensure we have a name, or die trying
         name = name or coll.name
         if not name:
             raise ValueError("Non-root collections must have a name!")
         name = self.transform(name)
         # Test for conflict
@@ -307,47 +319,47 @@
             raise ValueError(err.format(name))
         # Insert
         self.collections[name] = coll
         if default:
             self._check_default_collision(name)
             self.default = name
 
-    def _check_default_collision(self, name):
+    def _check_default_collision(self, name: str) -> None:
         if self.default:
             msg = "'{}' cannot be the default because '{}' already is!"
             raise ValueError(msg.format(name, self.default))
 
-    def _split_path(self, path):
+    def _split_path(self, path: str) -> Tuple[str, str]:
         """
         Obtain first collection + remainder, of a task path.
 
         E.g. for ``"subcollection.taskname"``, return ``("subcollection",
         "taskname")``; for ``"subcollection.nested.taskname"`` return
         ``("subcollection", "nested.taskname")``, etc.
 
         An empty path becomes simply ``('', '')``.
         """
         parts = path.split(".")
         coll = parts.pop(0)
         rest = ".".join(parts)
         return coll, rest
 
-    def subcollection_from_path(self, path):
+    def subcollection_from_path(self, path: str) -> "Collection":
         """
         Given a ``path`` to a subcollection, return that subcollection.
 
         .. versionadded:: 1.0
         """
         parts = path.split(".")
         collection = self
         while parts:
             collection = collection.collections[parts.pop(0)]
         return collection
 
-    def __getitem__(self, name=None):
+    def __getitem__(self, name: Optional[str] = None) -> Any:
         """
         Returns task named ``name``. Honors aliases and subcollections.
 
         If this collection has a default task, it is returned when ``name`` is
         empty or ``None``. If empty input is given and no task has been
         selected as the default, ValueError will be raised.
 
@@ -355,19 +367,23 @@
         'foo.bar'. Subcollection default tasks will be returned on the
         subcollection's name.
 
         .. versionadded:: 1.0
         """
         return self.task_with_config(name)[0]
 
-    def _task_with_merged_config(self, coll, rest, ours):
+    def _task_with_merged_config(
+        self, coll: str, rest: str, ours: Dict[str, Any]
+    ) -> Tuple[str, Dict[str, Any]]:
         task, config = self.collections[coll].task_with_config(rest)
         return task, dict(config, **ours)
 
-    def task_with_config(self, name):
+    def task_with_config(
+        self, name: Optional[str]
+    ) -> Tuple[str, Dict[str, Any]]:
         """
         Return task named ``name`` plus its configuration dict.
 
         E.g. in a deeply nested tree, this method returns the `.Task`, and a
         configuration dict created by merging that of this `.Collection` and
         any nested `Collections <.Collection>`, up through the one actually
         holding the `.Task`.
@@ -393,22 +409,24 @@
             return self._task_with_merged_config(coll, rest, ours)
         # Default task for subcollections (via empty-name lookup)
         if name in self.collections:
             return self._task_with_merged_config(name, "", ours)
         # Regular task lookup
         return self.tasks[name], ours
 
-    def __contains__(self, name):
+    def __contains__(self, name: str) -> bool:
         try:
             self[name]
             return True
         except KeyError:
             return False
 
-    def to_contexts(self, ignore_unknown_help=None):
+    def to_contexts(
+        self, ignore_unknown_help: Optional[bool] = None
+    ) -> List[ParserContext]:
         """
         Returns all contained tasks and subtasks as a list of parser contexts.
 
         :param bool ignore_unknown_help:
             Passed on to each task's ``get_arguments()`` method. See the config
             option by the same name for details.
 
@@ -426,20 +444,20 @@
                     args=task.get_arguments(
                         ignore_unknown_help=ignore_unknown_help
                     ),
                 )
             )
         return result
 
-    def subtask_name(self, collection_name, task_name):
+    def subtask_name(self, collection_name: str, task_name: str) -> str:
         return ".".join(
             [self.transform(collection_name), self.transform(task_name)]
         )
 
-    def transform(self, name):
+    def transform(self, name: str) -> str:
         """
         Transform ``name`` with the configured auto-dashes behavior.
 
         If the collection's ``auto_dash_names`` attribute is ``True``
         (default), all non leading/trailing underscores are turned into dashes.
         (Leading/trailing underscores tend to get stripped elsewhere in the
         stack.)
@@ -470,33 +488,33 @@
                 and name[i - 1] != "."
                 and name[i + 1] != "."
             ):
                 char = to
             replaced.append(char)
         return "".join(replaced)
 
-    def _transform_lexicon(self, old):
+    def _transform_lexicon(self, old: Lexicon) -> Lexicon:
         """
         Take a Lexicon and apply `.transform` to its keys and aliases.
 
         :returns: A new Lexicon.
         """
-        new_ = Lexicon()
+        new = Lexicon()
         # Lexicons exhibit only their real keys in most places, so this will
         # only grab those, not aliases.
         for key, value in old.items():
             # Deepcopy the value so we're not just copying a reference
-            new_[self.transform(key)] = copy.deepcopy(value)
+            new[self.transform(key)] = copy.deepcopy(value)
         # Also copy all aliases, which are string-to-string key mappings
         for key, value in old.aliases.items():
-            new_.alias(from_=self.transform(key), to=self.transform(value))
-        return new_
+            new.alias(from_=self.transform(key), to=self.transform(value))
+        return new
 
     @property
-    def task_names(self):
+    def task_names(self) -> Dict[str, List[str]]:
         """
         Return all task identifiers for this collection as a one-level dict.
 
         Specifically, a dict with the primary/"real" task names as the key, and
         any aliases as a list value.
 
         It basically collapses the namespace tree into a single
@@ -519,15 +537,15 @@
                 # Tack on collection name to alias list if this task is the
                 # collection's default.
                 if coll.default == task_name:
                     aliases += (coll_name,)
                 ret[self.subtask_name(coll_name, task_name)] = aliases
         return ret
 
-    def configuration(self, taskpath=None):
+    def configuration(self, taskpath: Optional[str] = None) -> Dict[str, Any]:
         """
         Obtain merged configuration values from collection & children.
 
         :param taskpath:
             (Optional) Task name/path, identical to that used for
             `~.Collection.__getitem__` (e.g. may be dotted for nested tasks,
             etc.) Used to decide which path to follow in the collection tree
@@ -537,15 +555,15 @@
 
         .. versionadded:: 1.0
         """
         if taskpath is None:
             return copy_dict(self._configuration)
         return self.task_with_config(taskpath)[1]
 
-    def configure(self, options):
+    def configure(self, options: Dict[str, Any]) -> None:
         """
         (Recursively) merge ``options`` into the current `.configuration`.
 
         Options configured this way will be available to all tasks. It is
         recommended to use unique keys to avoid potential clashes with other
         config options
 
@@ -556,15 +574,15 @@
         :param options: An object implementing the dictionary protocol.
         :returns: ``None``.
 
         .. versionadded:: 1.0
         """
         merge_dicts(self._configuration, options)
 
-    def serialized(self):
+    def serialized(self) -> Dict[str, Any]:
         """
         Return an appropriate-for-serialization version of this object.
 
         See the documentation for `.Program` and its ``json`` task listing
         format; this method is the driver for that functionality.
 
         .. versionadded:: 1.0
```

### Comparing `invoke-2.0.1/invoke/parser/context.py` & `invoke-2.1.0/invoke/parser/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import itertools
+from typing import Any, Dict, List, Iterable, Optional, Tuple, Union
 
 try:
     from ..vendor.lexicon import Lexicon
 except ImportError:
-    from lexicon import Lexicon
+    from lexicon import Lexicon  # type: ignore[no-redef]
 
 from .argument import Argument
 
 
-def translate_underscores(name):
+def translate_underscores(name: str) -> str:
     return name.lstrip("_").rstrip("_").replace("_", "-")
 
 
-def to_flag(name):
+def to_flag(name: str) -> str:
     name = translate_underscores(name)
     if len(name) == 1:
         return "-" + name
     return "--" + name
 
 
-def sort_candidate(arg):
+def sort_candidate(arg: Argument) -> str:
     names = arg.names
     # TODO: is there no "split into two buckets on predicate" builtin?
     shorts = {x for x in names if len(x.strip("-")) == 1}
     longs = {x for x in names if x not in shorts}
-    return sorted(shorts if shorts else longs)[0]
+    return str(sorted(shorts if shorts else longs)[0])
 
 
-def flag_key(x):
+def flag_key(arg: Argument) -> List[Union[int, str]]:
     """
     Obtain useful key list-of-ints for sorting CLI flags.
 
     .. versionadded:: 1.0
     """
     # Setup
-    ret = []
-    x = sort_candidate(x)
+    ret: List[Union[int, str]] = []
+    x = sort_candidate(arg)
     # Long-style flags win over short-style ones, so the first item of
     # comparison is simply whether the flag is a single character long (with
     # non-length-1 flags coming "first" [lower number])
     ret.append(1 if len(x) == 1 else 0)
     # Next item of comparison is simply the strings themselves,
     # case-insensitive. They will compare alphabetically if compared at this
     # stage.
@@ -63,15 +64,20 @@
 
     When run through a parser, will also hold runtime values filled in by the
     parser.
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, name=None, aliases=(), args=()):
+    def __init__(
+        self,
+        name: Optional[str] = None,
+        aliases: Iterable[str] = (),
+        args: Iterable[Argument] = (),
+    ) -> None:
         """
         Create a new ``ParserContext`` named ``name``, with ``aliases``.
 
         ``name`` is optional, and should be a string if given. It's used to
         tell ParserContext objects apart, and for use in a Parser when
         determining what chunk of input might belong to a given ParserContext.
 
@@ -79,31 +85,31 @@
         strings. Parsing will honor any aliases when trying to "find" a given
         context in its input.
 
         May give one or more ``args``, which is a quick alternative to calling
         ``for arg in args: self.add_arg(arg)`` after initialization.
         """
         self.args = Lexicon()
-        self.positional_args = []
+        self.positional_args: List[Argument] = []
         self.flags = Lexicon()
-        self.inverse_flags = {}  # No need for Lexicon here
+        self.inverse_flags: Dict[str, str] = {}  # No need for Lexicon here
         self.name = name
         self.aliases = aliases
         for arg in args:
             self.add_arg(arg)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         aliases = ""
         if self.aliases:
             aliases = " ({})".format(", ".join(self.aliases))
         name = (" {!r}{}".format(self.name, aliases)) if self.name else ""
         args = (": {!r}".format(self.args)) if self.args else ""
         return "<parser/Context{}{}>".format(name, args)
 
-    def add_arg(self, *args, **kwargs):
+    def add_arg(self, *args: Any, **kwargs: Any) -> None:
         """
         Adds given ``Argument`` (or constructor args for one) to this context.
 
         The Argument in question is added to the following dict attributes:
 
         * ``args``: "normal" access, i.e. the given names are directly exposed
           as keys.
@@ -145,37 +151,37 @@
             # Invert the 'main' flag name here, which will be a dashed version
             # of the primary argument name if underscore-to-dash transformation
             # occurred.
             inverse_name = to_flag("no-{}".format(main))
             self.inverse_flags[inverse_name] = to_flag(main)
 
     @property
-    def missing_positional_args(self):
+    def missing_positional_args(self) -> List[Argument]:
         return [x for x in self.positional_args if x.value is None]
 
     @property
-    def as_kwargs(self):
+    def as_kwargs(self) -> Dict[str, Any]:
         """
         This context's arguments' values keyed by their ``.name`` attribute.
 
         Results in a dict suitable for use in Python contexts, where e.g. an
         arg named ``foo-bar`` becomes accessible as ``foo_bar``.
 
         .. versionadded:: 1.0
         """
         ret = {}
         for arg in self.args.values():
             ret[arg.name] = arg.value
         return ret
 
-    def names_for(self, flag):
+    def names_for(self, flag: str) -> List[str]:
         # TODO: should probably be a method on Lexicon/AliasDict
         return list(set([flag] + self.flags.aliases_of(flag)))
 
-    def help_for(self, flag):
+    def help_for(self, flag: str) -> Tuple[str, str]:
         """
         Return 2-tuple of ``(flag-spec, help-string)`` for given ``flag``.
 
         .. versionadded:: 1.0
         """
         # Obtain arg obj
         if flag not in self.flags:
@@ -206,15 +212,15 @@
                 valuestr = ""
             # Tack together
             full_names.append(name + valuestr)
         namestr = ", ".join(sorted(full_names, key=len))
         helpstr = arg.help or ""
         return namestr, helpstr
 
-    def help_tuples(self):
+    def help_tuples(self) -> List[Tuple[str, Optional[str]]]:
         """
         Return sorted iterable of help tuples for all member Arguments.
 
         Sorts like so:
 
         * General sort is alphanumerically
         * Short flags win over long flags
@@ -240,21 +246,21 @@
         return list(
             map(
                 lambda x: self.help_for(to_flag(x.name)),
                 sorted(self.flags.values(), key=flag_key),
             )
         )
 
-    def flag_names(self):
+    def flag_names(self) -> Tuple[str, ...]:
         """
         Similar to `help_tuples` but returns flag names only, no helpstrs.
 
         Specifically, all flag names, flattened, in rough order.
 
         .. versionadded:: 1.0
         """
         # Regular flag names
         flags = sorted(self.flags.values(), key=flag_key)
         names = [self.names_for(to_flag(x.name)) for x in flags]
         # Inverse flag names sold separately
-        names.append(self.inverse_flags.keys())
+        names.append(list(self.inverse_flags.keys()))
         return tuple(itertools.chain.from_iterable(names))
```

### Comparing `invoke-2.0.1/invoke/parser/parser.py` & `invoke-2.1.0/invoke/parser/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,53 @@
 import copy
+from typing import TYPE_CHECKING, Any, Iterable, List, Optional
 
 try:
     from ..vendor.lexicon import Lexicon
     from ..vendor.fluidity import StateMachine, state, transition
 except ImportError:
-    from lexicon import Lexicon
-    from fluidity import StateMachine, state, transition
+    from lexicon import Lexicon  # type: ignore[no-redef]
+    from fluidity import (  # type: ignore[no-redef]
+        StateMachine,
+        state,
+        transition,
+    )
 
-from ..util import debug
 from ..exceptions import ParseError
+from ..util import debug
+
+if TYPE_CHECKING:
+    from .context import ParserContext
 
 
-def is_flag(value):
+def is_flag(value: str) -> bool:
     return value.startswith("-")
 
 
-def is_long_flag(value):
+def is_long_flag(value: str) -> bool:
     return value.startswith("--")
 
 
+class ParseResult(List["ParserContext"]):
+    """
+    List-like object with some extra parse-related attributes.
+
+    Specifically, a ``.remainder`` attribute, which is the string found after a
+    ``--`` in any parsed argv list; and an ``.unparsed`` attribute, a list of
+    tokens that were unable to be parsed.
+
+    .. versionadded:: 1.0
+    """
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
+        self.remainder = ""
+        self.unparsed: List[str] = []
+
+
 class Parser:
     """
     Create parser conscious of ``contexts`` and optional ``initial`` context.
 
     ``contexts`` should be an iterable of ``Context`` instances which will be
     searched when new context names are encountered during a parse. These
     Contexts determine what flags may follow them, as well as whether given
@@ -36,15 +61,20 @@
     any unknown contexts result in a parse error exception. If ``True``,
     encountering an unknown context halts parsing and populates the return
     value's ``.unparsed`` attribute with the remaining parse tokens.
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, contexts=(), initial=None, ignore_unknown=False):
+    def __init__(
+        self,
+        contexts: Iterable["ParserContext"] = (),
+        initial: Optional["ParserContext"] = None,
+        ignore_unknown: bool = False,
+    ) -> None:
         self.initial = initial
         self.contexts = Lexicon()
         self.ignore_unknown = ignore_unknown
         for context in contexts:
             debug("Adding {}".format(context))
             if not context.name:
                 raise ValueError("Non-initial contexts must have names.")
@@ -53,15 +83,15 @@
                 raise ValueError(exists.format(context.name))
             self.contexts[context.name] = context
             for alias in context.aliases:
                 if alias in self.contexts:
                     raise ValueError(exists.format(alias))
                 self.contexts.alias(alias, to=context.name)
 
-    def parse_argv(self, argv):
+    def parse_argv(self, argv: List[str]) -> ParseResult:
         """
         Parse an argv-style token list ``argv``.
 
         Returns a list (actually a subclass, `.ParseResult`) of
         `.ParserContext` objects matching the order they were found in the
         ``argv`` and containing `.Argument` objects with updated values based
         on any flags given.
@@ -78,15 +108,16 @@
         :returns:
             A `.ParseResult` (a ``list`` subclass containing some number of
             `.ParserContext` objects).
 
         .. versionadded:: 1.0
         """
         machine = ParseMachine(
-            initial=self.initial,
+            # FIXME: initial should not be none
+            initial=self.initial,  # type: ignore[arg-type]
             contexts=self.contexts,
             ignore_unknown=self.ignore_unknown,
         )
         # FIXME: Why isn't there str.partition for lists? There must be a
         # better way to do this. Split argv around the double-dash remainder
         # sentinel.
         debug("Starting argv: {!r}".format(argv))
@@ -131,18 +162,18 @@
                         and machine.current_state != "unknown"
                     )
                     if have_flag and machine.context.flags[token].takes_value:
                         msg = "{!r} is a flag for current context & it takes a value, giving it {!r}"  # noqa
                         debug(msg.format(token, rest))
                         mutations.append((index + 1, rest))
                     else:
-                        rest = ["-{}".format(x) for x in rest]
+                        _rest = ["-{}".format(x) for x in rest]
                         msg = "Splitting multi-flag glob {!r} into {!r} and {!r}"  # noqa
-                        debug(msg.format(orig, token, rest))
-                        for item in reversed(rest):
+                        debug(msg.format(orig, token, _rest))
+                        for item in reversed(_rest):
                             mutations.append((index + 1, item))
             # Here, we've got some possible mutations queued up, and 'token'
             # may have been overwritten as well. Whether we apply those and
             # continue as-is, or roll it back, depends:
             # - If the parser wasn't waiting for a flag value, we're already on
             # the right track, so apply mutations and move along to the
             # handle() step.
@@ -188,32 +219,37 @@
     transition(
         from_=("context", "unknown"),
         event="see_unknown",
         action="store_only",
         to="unknown",
     )
 
-    def changing_state(self, from_, to):
+    def changing_state(self, from_: str, to: str) -> None:
         debug("ParseMachine: {!r} => {!r}".format(from_, to))
 
-    def __init__(self, initial, contexts, ignore_unknown):
+    def __init__(
+        self,
+        initial: "ParserContext",
+        contexts: Lexicon,
+        ignore_unknown: bool,
+    ) -> None:
         # Initialize
         self.ignore_unknown = ignore_unknown
         self.initial = self.context = copy.deepcopy(initial)
         debug("Initialized with context: {!r}".format(self.context))
         self.flag = None
         self.flag_got_value = False
         self.result = ParseResult()
         self.contexts = copy.deepcopy(contexts)
         debug("Available contexts: {!r}".format(self.contexts))
         # In case StateMachine does anything in __init__
         super().__init__()
 
     @property
-    def waiting_for_flag_value(self):
+    def waiting_for_flag_value(self) -> bool:
         # Do we have a current flag, and does it expect a value (vs being a
         # bool/toggle)?
         takes_value = self.flag and self.flag.takes_value
         if not takes_value:
             return False
         # OK, this flag is one that takes values.
         # Is it a list type (which has only just been switched to)? Then it'll
@@ -229,15 +265,15 @@
         # TODO: in the negative case here, we should do something else instead:
         # - Except, "hey you screwed up, you already gave that flag!"
         # - Overwrite, "oh you changed your mind?" - which requires more work
         # elsewhere too, unfortunately. (Perhaps additional properties on
         # Argument that can be queried, e.g. "arg.is_iterable"?)
         return not has_value
 
-    def handle(self, token):
+    def handle(self, token: str) -> None:
         debug("Handling token: {!r}".format(token))
         # Handle unknown state at the top: we don't care about even
         # possibly-valid input if we've encountered unknown input.
         if self.current_state == "unknown":
             debug("Top-of-handle() see_unknown({!r})".format(token))
             self.see_unknown(token)
             return
@@ -287,20 +323,20 @@
             if not self.ignore_unknown:
                 debug("Can't find context named {!r}, erroring".format(token))
                 self.error("No idea what {!r} is!".format(token))
             else:
                 debug("Bottom-of-handle() see_unknown({!r})".format(token))
                 self.see_unknown(token)
 
-    def store_only(self, token):
+    def store_only(self, token: str) -> None:
         # Start off the unparsed list
         debug("Storing unknown token {!r}".format(token))
         self.result.unparsed.append(token)
 
-    def complete_context(self):
+    def complete_context(self) -> None:
         debug(
             "Wrapping up context {!r}".format(
                 self.context.name if self.context else self.context
             )
         )
         # Ensure all of context's positional args have been given.
         if self.context and self.context.missing_positional_args:
@@ -309,22 +345,22 @@
                 "'{}'".format(x.name)
                 for x in self.context.missing_positional_args
             )
             self.error(err.format(self.context.name, names))
         if self.context and self.context not in self.result:
             self.result.append(self.context)
 
-    def switch_to_context(self, name):
+    def switch_to_context(self, name: str) -> None:
         self.context = copy.deepcopy(self.contexts[name])
         debug("Moving to context {!r}".format(name))
         debug("Context args: {!r}".format(self.context.args))
         debug("Context flags: {!r}".format(self.context.flags))
         debug("Context inverse_flags: {!r}".format(self.context.inverse_flags))
 
-    def complete_flag(self):
+    def complete_flag(self) -> None:
         if self.flag:
             msg = "Completing current flag {} before moving on"
             debug(msg.format(self.flag))
         # Barf if we needed a value and didn't get one
         if (
             self.flag
             and self.flag.takes_value
@@ -338,15 +374,15 @@
         # bools.
         if self.flag and self.flag.raw_value is None and self.flag.optional:
             msg = "Saw optional flag {!r} go by w/ no value; setting to True"
             debug(msg.format(self.flag.name))
             # Skip casting so the bool gets preserved
             self.flag.set_value(True, cast=False)
 
-    def check_ambiguity(self, value):
+    def check_ambiguity(self, value: Any) -> bool:
         """
         Guard against ambiguity when current flag takes an optional value.
 
         .. versionadded:: 1.0
         """
         # No flag is currently being examined, or one is but it doesn't take an
         # optional value? Ambiguity isn't possible.
@@ -363,15 +399,15 @@
         tests.append(self.context and self.context.missing_positional_args)
         # Value matches another valid task/context name?
         tests.append(value in self.contexts)
         if any(tests):
             msg = "{!r} is ambiguous when given after an optional-value flag"
             raise ParseError(msg.format(value))
 
-    def switch_to_flag(self, flag, inverse=False):
+    def switch_to_flag(self, flag: str, inverse: bool = False) -> None:
         # Sanity check for ambiguity w/ prior optional-value flag
         self.check_ambiguity(flag)
         # Also tie it off, in case prior had optional value or etc. Seems to be
         # harmless for other kinds of flags. (TODO: this is a serious indicator
         # that we need to move some of this flag-by-flag bookkeeping into the
         # state machine bits, if possible - as-is it was REAL confusing re: why
         # this was manually required!)
@@ -391,46 +427,29 @@
                 raise e
         debug("Moving to flag {!r}".format(self.flag))
         # Bookkeeping for iterable-type flags (where the typical 'value
         # non-empty/nondefault -> clearly it got its value already' test is
         # insufficient)
         self.flag_got_value = False
         # Handle boolean flags (which can immediately be updated)
-        if not self.flag.takes_value:
+        if self.flag and not self.flag.takes_value:
             val = not inverse
             debug("Marking seen flag {!r} as {}".format(self.flag, val))
             self.flag.value = val
 
-    def see_value(self, value):
+    def see_value(self, value: Any) -> None:
         self.check_ambiguity(value)
-        if self.flag.takes_value:
+        if self.flag and self.flag.takes_value:
             debug("Setting flag {!r} to value {!r}".format(self.flag, value))
             self.flag.value = value
             self.flag_got_value = True
         else:
             self.error("Flag {!r} doesn't take any value!".format(self.flag))
 
-    def see_positional_arg(self, value):
+    def see_positional_arg(self, value: Any) -> None:
         for arg in self.context.positional_args:
             if arg.value is None:
                 arg.value = value
                 break
 
-    def error(self, msg):
+    def error(self, msg: str) -> None:
         raise ParseError(msg, self.context)
-
-
-class ParseResult(list):
-    """
-    List-like object with some extra parse-related attributes.
-
-    Specifically, a ``.remainder`` attribute, which is the string found after a
-    ``--`` in any parsed argv list; and an ``.unparsed`` attribute, a list of
-    tokens that were unable to be parsed.
-
-    .. versionadded:: 1.0
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.remainder = ""
-        self.unparsed = []
```

### Comparing `invoke-2.0.1/invoke/parser/argument.py` & `invoke-2.1.0/invoke/parser/argument.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+from typing import Any, Iterable, Optional, Tuple
+
+# TODO: dynamic type for kind
+# T = TypeVar('T')
+
+
 class Argument:
     """
     A command-line argument/flag.
 
     :param name:
         Syntactic sugar for ``names=[<name>]``. Giving both ``name`` and
         ``names`` is invalid.
@@ -31,47 +37,51 @@
         the underscored version when ``name``/``names`` contain dashes.
 
     .. versionadded:: 1.0
     """
 
     def __init__(
         self,
-        name=None,
-        names=(),
-        kind=str,
-        default=None,
-        help=None,
-        positional=False,
-        optional=False,
-        incrementable=False,
-        attr_name=None,
-    ):
+        name: Optional[str] = None,
+        names: Iterable[str] = (),
+        kind: Any = str,
+        default: Optional[Any] = None,
+        help: Optional[str] = None,
+        positional: bool = False,
+        optional: bool = False,
+        incrementable: bool = False,
+        attr_name: Optional[str] = None,
+    ) -> None:
         if name and names:
-            msg = "Cannot give both 'name' and 'names' arguments! Pick one."
-            raise TypeError(msg)
+            raise TypeError(
+                "Cannot give both 'name' and 'names' arguments! Pick one."
+            )
         if not (name or names):
             raise TypeError("An Argument must have at least one name.")
-        self.names = tuple(names if names else (name,))
+        if names:
+            self.names = tuple(names)
+        elif name and not names:
+            self.names = (name,)
         self.kind = kind
-        initial_value = None
+        initial_value: Optional[Any] = None
         # Special case: list-type args start out as empty list, not None.
         if kind is list:
             initial_value = []
         # Another: incrementable args start out as their default value.
         if incrementable:
             initial_value = default
         self.raw_value = self._value = initial_value
         self.default = default
         self.help = help
         self.positional = positional
         self.optional = optional
         self.incrementable = incrementable
         self.attr_name = attr_name
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         nicks = ""
         if self.nicknames:
             nicks = " ({})".format(", ".join(self.nicknames))
         flags = ""
         if self.positional or self.optional:
             flags = " "
         if self.positional:
@@ -84,46 +94,47 @@
         if self.kind != str:
             kind = " [{}]".format(self.kind.__name__)
         return "<{}: {}{}{}{}>".format(
             self.__class__.__name__, self.name, nicks, kind, flags
         )
 
     @property
-    def name(self):
+    def name(self) -> Optional[str]:
         """
         The canonical attribute-friendly name for this argument.
 
         Will be ``attr_name`` (if given to constructor) or the first name in
         ``names`` otherwise.
 
         .. versionadded:: 1.0
         """
         return self.attr_name or self.names[0]
 
     @property
-    def nicknames(self):
+    def nicknames(self) -> Tuple[str, ...]:
         return self.names[1:]
 
     @property
-    def takes_value(self):
+    def takes_value(self) -> bool:
         if self.kind is bool:
             return False
         if self.incrementable:
             return False
         return True
 
     @property
-    def value(self):
+    def value(self) -> Any:
+        # TODO: should probably be optional instead
         return self._value if self._value is not None else self.default
 
     @value.setter
-    def value(self, arg):
+    def value(self, arg: str) -> None:
         self.set_value(arg, cast=True)
 
-    def set_value(self, value, cast=True):
+    def set_value(self, value: Any, cast: bool = True) -> None:
         """
         Actual explicit value-setting API call.
 
         Sets ``self.raw_value`` to ``value`` directly.
 
         Sets ``self.value`` to ``self.kind(value)``, unless:
 
@@ -139,23 +150,24 @@
         # Default to do-nothing/identity function
         func = lambda x: x
         # If cast, set to self.kind, which should be str/int/etc
         if cast:
             func = self.kind
         # If self.kind is a list, append instead of using cast func.
         if self.kind is list:
-            func = lambda x: self._value + [x]
+            func = lambda x: self.value + [x]
         # If incrementable, just increment.
         if self.incrementable:
-            # TODO: explode nicely if self._value was not an int to start with
-            func = lambda x: self._value + 1
+            # TODO: explode nicely if self.value was not an int to start
+            # with
+            func = lambda x: self.value + 1
         self._value = func(value)
 
     @property
-    def got_value(self):
+    def got_value(self) -> bool:
         """
         Returns whether the argument was ever given a (non-default) value.
 
         For most argument kinds, this simply checks whether the internally
         stored value is non-``None``; for others, such as ``list`` kinds,
         different checks may be used.
```

### Comparing `invoke-2.0.1/invoke/env.py` & `invoke-2.1.0/invoke/env.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,26 +5,30 @@
 situation requiring it) more convenient.
 
 This module is currently considered private/an implementation detail and should
 not be included in the Sphinx API documentation.
 """
 
 import os
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Mapping, Sequence
 
 from .exceptions import UncastableEnvVar, AmbiguousEnvVar
 from .util import debug
 
+if TYPE_CHECKING:
+    from .config import Config
+
 
 class Environment:
-    def __init__(self, config, prefix):
+    def __init__(self, config: "Config", prefix: str) -> None:
         self._config = config
         self._prefix = prefix
-        self.data = {}  # Accumulator
+        self.data: Dict[str, Any] = {}  # Accumulator
 
-    def load(self):
+    def load(self) -> Dict[str, Any]:
         """
         Return a nested dict containing values from `os.environ`.
 
         Specifically, values whose keys map to already-known configuration
         settings, allowing us to perform basic typecasting.
 
         See :ref:`env-vars` for details.
@@ -37,29 +41,31 @@
         for env_var, key_path in env_vars.items():
             real_var = (self._prefix or "") + env_var
             if real_var in os.environ:
                 self._path_set(key_path, os.environ[real_var])
         debug("Obtained env var config: {!r}".format(self.data))
         return self.data
 
-    def _crawl(self, key_path, env_vars):
+    def _crawl(
+        self, key_path: List[str], env_vars: Mapping[str, Sequence[str]]
+    ) -> Dict[str, Any]:
         """
         Examine config at location ``key_path`` & return potential env vars.
 
         Uses ``env_vars`` dict to determine if a conflict exists, and raises an
         exception if so. This dict is of the following form::
 
             {
                 'EXPECTED_ENV_VAR_HERE': ['actual', 'nested', 'key_path'],
                 ...
             }
 
         Returns another dictionary of new keypairs as per above.
         """
-        new_vars = {}
+        new_vars: Dict[str, List[str]] = {}
         obj = self._path_get(key_path)
         # Sub-dict -> recurse
         if (
             hasattr(obj, "keys")
             and callable(obj.keys)
             and hasattr(obj, "__getitem__")
         ):
@@ -75,43 +81,43 @@
                 # Merge and continue
                 new_vars.update(crawled)
         # Other -> is leaf, no recursion
         else:
             new_vars[self._to_env_var(key_path)] = key_path
         return new_vars
 
-    def _to_env_var(self, key_path):
+    def _to_env_var(self, key_path: Iterable[str]) -> str:
         return "_".join(key_path).upper()
 
-    def _path_get(self, key_path):
+    def _path_get(self, key_path: Iterable[str]) -> "Config":
         # Gets are from self._config because that's what determines valid env
         # vars and/or values for typecasting.
         obj = self._config
         for key in key_path:
             obj = obj[key]
         return obj
 
-    def _path_set(self, key_path, value):
+    def _path_set(self, key_path: Sequence[str], value: str) -> None:
         # Sets are to self.data since that's what we are presenting to the
         # outer config object and debugging.
         obj = self.data
         for key in key_path[:-1]:
             if key not in obj:
                 obj[key] = {}
             obj = obj[key]
         old = self._path_get(key_path)
-        new_ = self._cast(old, value)
-        obj[key_path[-1]] = new_
+        new = self._cast(old, value)
+        obj[key_path[-1]] = new
 
-    def _cast(self, old, new_):
+    def _cast(self, old: Any, new: Any) -> Any:
         if isinstance(old, bool):
-            return new_ not in ("0", "")
+            return new not in ("0", "")
         elif isinstance(old, str):
-            return new_
+            return new
         elif old is None:
-            return new_
+            return new
         elif isinstance(old, (list, tuple)):
             err = "Can't adapt an environment string into a {}!"
             err = err.format(type(old))
             raise UncastableEnvVar(err)
         else:
-            return old.__class__(new_)
+            return old.__class__(new)
```

### Comparing `invoke-2.0.1/invoke/loader.py` & `invoke-2.1.0/invoke/loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 import os
 import sys
-import imp
+from importlib.machinery import ModuleSpec
+from importlib.util import module_from_spec, spec_from_file_location
+from types import ModuleType
+from typing import Any, Optional, Tuple
 
 from . import Config
 from .exceptions import CollectionNotFound
 from .util import debug
 
 
 class Loader:
     """
     Abstract class defining how to find/import a session's base `.Collection`.
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, config=None):
+    def __init__(self, config: Optional["Config"] = None) -> None:
         """
         Set up a new loader with some `.Config`.
 
         :param config:
             An explicit `.Config` to use; it is referenced for loading-related
             config options. Defaults to an anonymous ``Config()`` if none is
             given.
         """
         if config is None:
             config = Config()
         self.config = config
 
-    def find(self, name):
+    def find(self, name: str) -> Optional[ModuleSpec]:
         """
         Implementation-specific finder method seeking collection ``name``.
 
-        Must return a 4-tuple valid for use by `imp.load_module`, which is
+        Must return a ModuleSpec valid for use by `importlib`, which is
         typically a name string followed by the contents of the 3-tuple
-        returned by `imp.find_module` (``file``, ``pathname``,
-        ``description``.)
+        returned by `importlib.module_from_spec` (``name``, ``loader``,
+        ``origin``.)
 
         For a sample implementation, see `.FilesystemLoader`.
 
         .. versionadded:: 1.0
         """
         raise NotImplementedError
 
-    def load(self, name=None):
+    def load(self, name: Optional[str] = None) -> Tuple[ModuleType, str]:
         """
         Load and return collection module identified by ``name``.
 
         This method requires a working implementation of `.find` in order to
         function.
 
         In addition to importing the named module, it will add the module's
@@ -59,35 +62,30 @@
             collection-containing Python module object, and ``directory`` is
             the string path to the directory the module was found in.
 
         .. versionadded:: 1.0
         """
         if name is None:
             name = self.config.tasks.collection_name
-        # Find the named tasks module, depending on implementation.
-        # Will raise an exception if not found.
-        fd, path, desc = self.find(name)
-        try:
+        spec = self.find(name)
+        if spec and spec.loader and spec.origin:
+            path = spec.origin
             # Ensure containing directory is on sys.path in case the module
             # being imported is trying to load local-to-it names.
-            parent = os.path.dirname(path)
-            if parent not in sys.path:
-                sys.path.insert(0, parent)
+            if os.path.isfile(spec.origin):
+                path = os.path.dirname(spec.origin)
+            if path not in sys.path:
+                sys.path.insert(0, path)
             # Actual import
-            module = imp.load_module(name, fd, path, desc)
-            # Return module + path.
-            # TODO: is there a reason we're not simply having clients refer to
-            # os.path.dirname(module.__file__)?
-            return module, parent
-        finally:
-            # Ensure we clean up the opened file object returned by find(), if
-            # there was one (eg found packages, vs modules, don't open any
-            # file.)
-            if fd:
-                fd.close()
+            module = module_from_spec(spec)
+            spec.loader.exec_module(module)
+            return module, os.path.dirname(spec.origin)
+        msg = "ImportError loading {!r}, raising ImportError"
+        debug(msg.format(name))
+        raise ImportError
 
 
 class FilesystemLoader(Loader):
     """
     Loads Python files from the filesystem (e.g. ``tasks.py``.)
 
     Searches recursively towards filesystem root from a given start point.
@@ -95,40 +93,50 @@
     .. versionadded:: 1.0
     """
 
     # TODO: could introduce config obj here for transmission to Collection
     # TODO: otherwise Loader has to know about specific bits to transmit, such
     # as auto-dashes, and has to grow one of those for every bit Collection
     # ever needs to know
-    def __init__(self, start=None, **kwargs):
+    def __init__(self, start: Optional[str] = None, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         if start is None:
             start = self.config.tasks.search_root
         self._start = start
 
     @property
-    def start(self):
+    def start(self) -> str:
         # Lazily determine default CWD if configured value is falsey
         return self._start or os.getcwd()
 
-    def find(self, name):
-        # Accumulate all parent directories
-        start = self.start
-        debug("FilesystemLoader find starting at {!r}".format(start))
-        parents = [os.path.abspath(start)]
-        parents.append(os.path.dirname(parents[-1]))
-        while parents[-1] != parents[-2]:
-            parents.append(os.path.dirname(parents[-1]))
-        # Make sure we haven't got duplicates on the end
-        if parents[-1] == parents[-2]:
-            parents = parents[:-1]
-        # Use find_module with our list of parents. ImportError from
-        # find_module means "couldn't find" not "found and couldn't import" so
-        # we turn it into a more obvious exception class.
+    def find(self, name: str) -> Optional[ModuleSpec]:
+        debug("FilesystemLoader find starting at {!r}".format(self.start))
+        spec = None
+        module = "{}.py".format(name)
+        paths = self.start.split(os.sep)
         try:
-            tup = imp.find_module(name, parents)
-            debug("Found module: {!r}".format(tup[1]))
-            return tup
-        except ImportError:
+            # walk the path upwards to check for dynamic import
+            for x in reversed(range(len(paths) + 1)):
+                path = os.sep.join(paths[0:x])
+                if module in os.listdir(path):
+                    spec = spec_from_file_location(
+                        name, os.path.join(path, module)
+                    )
+                    break
+                elif name in os.listdir(path) and os.path.exists(
+                    os.path.join(path, name, "__init__.py")
+                ):
+                    basepath = os.path.join(path, name)
+                    spec = spec_from_file_location(
+                        name,
+                        os.path.join(basepath, "__init__.py"),
+                        submodule_search_locations=[basepath],
+                    )
+                    break
+            if spec:
+                debug("Found module: {!r}".format(spec))
+                return spec
+        except (FileNotFoundError, ModuleNotFoundError):
             msg = "ImportError loading {!r}, raising CollectionNotFound"
             debug(msg.format(name))
-            raise CollectionNotFound(name=name, start=start)
+            raise CollectionNotFound(name=name, start=self.start)
+        return None
```

### Comparing `invoke-2.0.1/invoke/vendor/fluidity/machine.py` & `invoke-2.1.0/invoke/vendor/fluidity/machine.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/representer.py` & `invoke-2.1.0/invoke/vendor/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/resolver.py` & `invoke-2.1.0/invoke/vendor/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/__init__.py` & `invoke-2.1.0/invoke/vendor/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/parser.py` & `invoke-2.1.0/invoke/vendor/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/composer.py` & `invoke-2.1.0/invoke/vendor/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/cyaml.py` & `invoke-2.1.0/invoke/vendor/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/serializer.py` & `invoke-2.1.0/invoke/vendor/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/scanner.py` & `invoke-2.1.0/invoke/vendor/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/error.py` & `invoke-2.1.0/invoke/vendor/yaml/error.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/events.py` & `invoke-2.1.0/invoke/vendor/yaml/events.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/tokens.py` & `invoke-2.1.0/invoke/vendor/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/loader.py` & `invoke-2.1.0/invoke/vendor/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/constructor.py` & `invoke-2.1.0/invoke/vendor/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/reader.py` & `invoke-2.1.0/invoke/vendor/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/nodes.py` & `invoke-2.1.0/invoke/vendor/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/dumper.py` & `invoke-2.1.0/invoke/vendor/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/yaml/emitter.py` & `invoke-2.1.0/invoke/vendor/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/lexicon/__init__.py` & `invoke-2.1.0/invoke/vendor/lexicon/__init__.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/vendor/lexicon/alias_dict.py` & `invoke-2.1.0/invoke/vendor/lexicon/alias_dict.py`

 * *Files identical despite different names*

### Comparing `invoke-2.0.1/invoke/tasks.py` & `invoke-2.1.0/invoke/tasks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,43 @@
 """
 This module contains the core `.Task` class & convenience decorators used to
 generate new tasks.
 """
 
-from copy import deepcopy
 import inspect
 import types
+from copy import deepcopy
+from functools import update_wrapper
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Generic,
+    Iterable,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
 
 from .context import Context
 from .parser import Argument, translate_underscores
 
+if TYPE_CHECKING:
+    from inspect import Signature
+    from .config import Config
+
+T = TypeVar("T", bound=Callable)
 
-class Task:
+
+class Task(Generic[T]):
     """
     Core object representing an executable task & its argument specification.
 
     For the most part, this object is a clearinghouse for all of the data that
     may be supplied to the `@task <invoke.tasks.task>` decorator, such as
     ``name``, ``aliases``, ``positional`` etc, which appear as attributes.
 
@@ -32,99 +54,100 @@
     # TODO: allow central per-session / per-taskmodule control over some of
     # them, e.g. (auto_)positional, auto_shortflags.
     # NOTE: we shadow __builtins__.help here on purpose - obfuscating to avoid
     # it feels bad, given the builtin will never actually be in play anywhere
     # except a debug shell whose frame is exactly inside this class.
     def __init__(
         self,
-        body,
-        name=None,
-        aliases=(),
-        positional=None,
-        optional=(),
-        default=False,
-        auto_shortflags=True,
-        help=None,
-        pre=None,
-        post=None,
-        autoprint=False,
-        iterable=None,
-        incrementable=None,
-    ):
+        body: Callable,
+        name: Optional[str] = None,
+        aliases: Iterable[str] = (),
+        positional: Optional[Iterable[str]] = None,
+        optional: Iterable[str] = (),
+        default: bool = False,
+        auto_shortflags: bool = True,
+        help: Optional[Dict[str, Any]] = None,
+        pre: Optional[Union[List[str], str]] = None,
+        post: Optional[Union[List[str], str]] = None,
+        autoprint: bool = False,
+        iterable: Optional[Iterable[str]] = None,
+        incrementable: Optional[Iterable[str]] = None,
+    ) -> None:
         # Real callable
         self.body = body
+        update_wrapper(self, self.body)
         # Copy a bunch of special properties from the body for the benefit of
         # Sphinx autodoc or other introspectors.
         self.__doc__ = getattr(body, "__doc__", "")
         self.__name__ = getattr(body, "__name__", "")
         self.__module__ = getattr(body, "__module__", "")
         # Default name, alternate names, and whether it should act as the
         # default for its parent collection
         self._name = name
         self.aliases = aliases
         self.is_default = default
         # Arg/flag/parser hints
         self.positional = self.fill_implicit_positionals(positional)
-        self.optional = optional
+        self.optional = tuple(optional)
         self.iterable = iterable or []
         self.incrementable = incrementable or []
         self.auto_shortflags = auto_shortflags
         self.help = (help or {}).copy()
         # Call chain bidness
         self.pre = pre or []
         self.post = post or []
         self.times_called = 0
         # Whether to print return value post-execution
         self.autoprint = autoprint
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self._name or self.__name__
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         aliases = ""
         if self.aliases:
             aliases = " ({})".format(", ".join(self.aliases))
         return "<Task {!r}{}>".format(self.name, aliases)
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, Task) or self.name != other.name:
             return False
         # Functions do not define __eq__ but func_code objects apparently do.
         # (If we're wrapping some other callable, they will be responsible for
         # defining equality on their end.)
         if self.body == other.body:
             return True
         else:
             try:
                 return self.body.__code__ == other.body.__code__
             except AttributeError:
                 return False
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         # Presumes name and body will never be changed. Hrm.
         # Potentially cleaner to just not use Tasks as hash keys, but let's do
         # this for now.
         return hash(self.name) + hash(self.body)
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args: Any, **kwargs: Any) -> T:
         # Guard against calling tasks with no context.
         if not isinstance(args[0], Context):
             err = "Task expected a Context as its first arg, got {} instead!"
             # TODO: raise a custom subclass _of_ TypeError instead
             raise TypeError(err.format(type(args[0])))
         result = self.body(*args, **kwargs)
         self.times_called += 1
         return result
 
     @property
-    def called(self):
+    def called(self) -> bool:
         return self.times_called > 0
 
-    def argspec(self, body):
+    def argspec(self, body: Callable) -> "Signature":
         """
         Returns a modified `inspect.Signature` based on that of ``body``.
 
         :returns:
             an `inspect.Signature` matching that of ``body``, but with the
             initial context argument removed.
         :raises TypeError:
@@ -132,38 +155,46 @@
 
         .. versionadded:: 1.0
         .. versionchanged:: 2.0
             Changed from returning a two-tuple of ``(arg_names, spec_dict)`` to
             returning an `inspect.Signature`.
         """
         # Handle callable-but-not-function objects
-        func = body if isinstance(body, types.FunctionType) else body.__call__
+        func = (
+            body
+            if isinstance(body, types.FunctionType)
+            else body.__call__  # type: ignore
+        )
         # Rebuild signature with first arg dropped, or die usefully(ish trying
         sig = inspect.signature(func)
         params = list(sig.parameters.values())
         # TODO: this ought to also check if an extant 1st param _was_ a Context
         # arg, and yell similarly if not.
         if not len(params):
             # TODO: see TODO under __call__, this should be same type
             raise TypeError("Tasks must have an initial Context argument!")
         return sig.replace(parameters=params[1:])
 
-    def fill_implicit_positionals(self, positional):
+    def fill_implicit_positionals(
+        self, positional: Optional[Iterable[str]]
+    ) -> Iterable[str]:
         # If positionals is None, everything lacking a default
         # value will be automatically considered positional.
         if positional is None:
             positional = [
                 x.name
                 for x in self.argspec(self.body).parameters.values()
                 if x.default is inspect.Signature.empty
             ]
         return positional
 
-    def arg_opts(self, name, default, taken_names):
-        opts = {}
+    def arg_opts(
+        self, name: str, default: str, taken_names: Set[str]
+    ) -> Dict[str, Any]:
+        opts: Dict[str, Any] = {}
         # Whether it's positional or not
         opts["positional"] = name in self.positional
         # Whether it is a value-optional flag
         opts["optional"] = name in self.optional
         # Whether it should be of an iterable (list) kind
         if name in self.iterable:
             opts["kind"] = list
@@ -201,15 +232,17 @@
         # Help
         for possibility in name, original_name:
             if possibility in self.help:
                 opts["help"] = self.help.pop(possibility)
                 break
         return opts
 
-    def get_arguments(self, ignore_unknown_help=None):
+    def get_arguments(
+        self, ignore_unknown_help: Optional[bool] = None
+    ) -> List[Argument]:
         """
         Return a list of Argument objects representing this task's signature.
 
         :param bool ignore_unknown_help:
             Controls whether unknown help flags cause errors. See the config
             option by the same name for details.
 
@@ -221,17 +254,17 @@
         sig = self.argspec(self.body)
         # Prime the list of all already-taken names (mostly for help in
         # choosing auto shortflags)
         taken_names = set(sig.parameters.keys())
         # Build arg list (arg_opts will take care of setting up shortnames,
         # etc)
         args = []
-        for arg in sig.parameters.values():
+        for param in sig.parameters.values():
             new_arg = Argument(
-                **self.arg_opts(arg.name, arg.default, taken_names)
+                **self.arg_opts(param.name, param.default, taken_names)
             )
             args.append(new_arg)
             # Update taken_names list with new argument's full name list
             # (which may include new shortflags) so subsequent Argument
             # creation knows what's taken.
             taken_names.update(set(new_arg.names))
         # If any values were leftover after consuming a 'help' dict, it implies
@@ -241,23 +274,23 @@
                 "Help field was set for param(s) that don't exist: {}".format(
                     list(self.help.keys())
                 )
             )
         # Now we need to ensure positionals end up in the front of the list, in
         # order given in self.positionals, so that when Context consumes them,
         # this order is preserved.
-        for posarg in reversed(self.positional):
+        for posarg in reversed(list(self.positional)):
             for i, arg in enumerate(args):
                 if arg.name == posarg:
                     args.insert(0, args.pop(i))
                     break
         return args
 
 
-def task(*args, **kwargs):
+def task(*args: Any, **kwargs: Any) -> Callable:
     """
     Marks wrapped callable object as a valid Invoke task.
 
     May be called without any parentheses if no extra options need to be
     specified. Otherwise, the following keyword arguments are allowed in the
     parenthese'd form:
 
@@ -303,77 +336,52 @@
     ``pre`` kwarg for convenience's sake. (It is an error to give both
     ``*args`` and ``pre`` at the same time.)
 
     .. versionadded:: 1.0
     .. versionchanged:: 1.1
         Added the ``klass`` keyword argument.
     """
-    klass = kwargs.pop("klass", Task)
+    klass: Type[Task] = kwargs.pop("klass", Task)
     # @task -- no options were (probably) given.
     if len(args) == 1 and callable(args[0]) and not isinstance(args[0], Task):
         return klass(args[0], **kwargs)
     # @task(pre, tasks, here)
     if args:
         if "pre" in kwargs:
             raise TypeError(
                 "May not give *args and 'pre' kwarg simultaneously!"
             )
         kwargs["pre"] = args
-    # @task(options)
-    # TODO: why the heck did we originally do this in this manner instead of
-    # simply delegating to Task?! Let's just remove all this sometime & see
-    # what, if anything, breaks.
-    name = kwargs.pop("name", None)
-    aliases = kwargs.pop("aliases", ())
-    positional = kwargs.pop("positional", None)
-    optional = tuple(kwargs.pop("optional", ()))
-    iterable = kwargs.pop("iterable", None)
-    incrementable = kwargs.pop("incrementable", None)
-    default = kwargs.pop("default", False)
-    auto_shortflags = kwargs.pop("auto_shortflags", True)
-    help = kwargs.pop("help", {})
-    pre = kwargs.pop("pre", [])
-    post = kwargs.pop("post", [])
-    autoprint = kwargs.pop("autoprint", False)
-
-    def inner(obj):
-        obj = klass(
-            obj,
-            name=name,
-            aliases=aliases,
-            positional=positional,
-            optional=optional,
-            iterable=iterable,
-            incrementable=incrementable,
-            default=default,
-            auto_shortflags=auto_shortflags,
-            help=help,
-            pre=pre,
-            post=post,
-            autoprint=autoprint,
-            # Pass in any remaining kwargs as-is.
-            **kwargs
-        )
-        return obj
 
+    def inner(body: Callable) -> Task[T]:
+        _task = klass(body, **kwargs)
+        return _task
+
+    # update_wrapper(inner, klass)
     return inner
 
 
 class Call:
     """
     Represents a call/execution of a `.Task` with given (kw)args.
 
     Similar to `~functools.partial` with some added functionality (such as the
     delegation to the inner task, and optional tracking of the name it's being
     called by.)
 
     .. versionadded:: 1.0
     """
 
-    def __init__(self, task, called_as=None, args=None, kwargs=None):
+    def __init__(
+        self,
+        task: "Task",
+        called_as: Optional[str] = None,
+        args: Optional[Tuple[str, ...]] = None,
+        kwargs: Optional[Dict[str, Any]] = None,
+    ) -> None:
         """
         Create a new `.Call` object.
 
         :param task: The `.Task` object to be executed.
 
         :param str called_as:
             The name the task is being called as, e.g. if it was called by an
@@ -388,64 +396,68 @@
         """
         self.task = task
         self.called_as = called_as
         self.args = args or tuple()
         self.kwargs = kwargs or dict()
 
     # TODO: just how useful is this? feels like maybe overkill magic
-    def __getattr__(self, name):
+    def __getattr__(self, name: str) -> Any:
         return getattr(self.task, name)
 
-    def __deepcopy__(self, memo):
+    def __deepcopy__(self, memo: object) -> "Call":
         return self.clone()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         aka = ""
         if self.called_as is not None and self.called_as != self.task.name:
             aka = " (called as: {!r})".format(self.called_as)
         return "<{} {!r}{}, args: {!r}, kwargs: {!r}>".format(
             self.__class__.__name__,
             self.task.name,
             aka,
             self.args,
             self.kwargs,
         )
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         # NOTE: Not comparing 'called_as'; a named call of a given Task with
         # same args/kwargs should be considered same as an unnamed call of the
         # same Task with the same args/kwargs (e.g. pre/post task specified w/o
         # name). Ditto tasks with multiple aliases.
         for attr in "task args kwargs".split():
             if getattr(self, attr) != getattr(other, attr):
                 return False
         return True
 
-    def make_context(self, config):
+    def make_context(self, config: "Config") -> Context:
         """
         Generate a `.Context` appropriate for this call, with given config.
 
         .. versionadded:: 1.0
         """
         return Context(config=config)
 
-    def clone_data(self):
+    def clone_data(self) -> Dict[str, Any]:
         """
         Return keyword args suitable for cloning this call into another.
 
         .. versionadded:: 1.1
         """
         return dict(
             task=self.task,
             called_as=self.called_as,
             args=deepcopy(self.args),
             kwargs=deepcopy(self.kwargs),
         )
 
-    def clone(self, into=None, with_=None):
+    def clone(
+        self,
+        into: Optional[Type["Call"]] = None,
+        with_: Optional[Dict[str, Any]] = None,
+    ) -> "Call":
         """
         Return a standalone copy of this Call.
 
         Useful when parameterizing task executions.
 
         :param into:
             A subclass to generate instead of the current class. Optional.
@@ -467,15 +479,15 @@
         klass = into if into is not None else self.__class__
         data = self.clone_data()
         if with_ is not None:
             data.update(with_)
         return klass(**data)
 
 
-def call(task, *args, **kwargs):
+def call(task: "Task", *args: Any, **kwargs: Any) -> "Call":
     """
     Describes execution of a `.Task`, typically with pre-supplied arguments.
 
     Useful for setting up :ref:`pre/post task invocations
     <parameterizing-pre-post-tasks>`. It's actually just a convenient wrapper
     around the `.Call` class, which may be used directly instead if desired.
 
@@ -500,8 +512,8 @@
 
     Please see the constructor docs for `.Call` for details - this function's
     ``args`` and ``kwargs`` map directly to the same arguments as in that
     method.
 
     .. versionadded:: 1.0
     """
-    return Call(task=task, args=args, kwargs=kwargs)
+    return Call(task, args=args, kwargs=kwargs)
```


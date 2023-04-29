# Comparing `tmp/nose2-0.9.1.tar.gz` & `tmp/nose2-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nose2-0.9.1.tar", last modified: Tue Apr  2 16:30:07 2019, max compression
+gzip compressed data, was "dist/nose2-0.9.2.tar", last modified: Sun Feb  2 00:58:55 2020, max compression
```

## Comparing `nose2-0.9.1.tar` & `nose2-0.9.2.tar`

### file list

```diff
@@ -1,413 +1,416 @@
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4451 2019-03-31 20:52:47.000000 nose2-0.9.1/README.rst
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:05.000000 nose2-0.9.1/docs/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      169 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/tools.rst
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/docs/plugins/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3420 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/attrib.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      549 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/attrib_example.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1333 2019-03-17 04:23:00.000000 nose2-0.9.1/docs/plugins/prettyassert.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1007 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/eggdiscovery.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      134 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/discovery.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      129 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/functions.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      159 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/outcomes.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      108 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/doctests.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      133 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/generators.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       76 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/prof.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4753 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/junitxml.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10074 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/mp.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      124 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/buffer.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      145 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/parameters.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      176 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/failfast.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      165 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/logcapture.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      130 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/testclasses.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      131 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/debugger.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      647 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/coverage.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      149 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/loadtests.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       92 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/testid.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      121 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/testcases.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     7828 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/layers.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5057 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/printhooks.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      167 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/collect.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      123 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/result.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      159 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/plugins/dundertests.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1048 2019-03-17 04:23:00.000000 nose2-0.9.1/docs/getting_started.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      848 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/conf.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       70 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/index.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6936 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/configuration.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4884 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/such_dsl.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      580 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/contents.rst.inc
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      136 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/params.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5929 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/usage.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1918 2019-03-17 04:23:00.000000 nose2-0.9.1/docs/plugins.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      251 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/decorators.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4586 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/Makefile
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6009 2019-03-17 04:23:00.000000 nose2-0.9.1/docs/differences.rst
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:05.000000 nose2-0.9.1/docs/dev/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       99 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/dev/exceptions.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      528 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/dev/session_reference.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       75 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/dev/utils.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3778 2019-03-17 04:36:45.000000 nose2-0.9.1/docs/dev/contributing.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    17573 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/dev/hook_reference.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      158 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/dev/event_reference.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/dev/loader.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      386 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/dev/plugin_class_reference.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       84 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/dev/runner.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1319 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/dev/documenting_plugins.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      226 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/dev/internals.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     7406 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/dev/writing_plugins.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/dev/result.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       75 2018-10-29 21:48:32.000000 nose2-0.9.1/docs/dev/main.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8719 2019-04-02 15:53:47.000000 nose2-0.9.1/docs/changelog.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      367 2018-10-29 21:48:32.000000 nose2-0.9.1/MANIFEST.in
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      124 2019-03-17 04:35:40.000000 nose2-0.9.1/AUTHORS
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      283 2019-04-02 15:53:47.000000 nose2-0.9.1/nose2/_version.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/plugins/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      615 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/failfast.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1813 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/printhooks.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3375 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/testid.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10472 2019-04-02 12:51:57.000000 nose2-0.9.1/nose2/plugins/junitxml.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9384 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/layers.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1812 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/debugger.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      894 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/dundertest.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5404 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/attrib.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/plugins/loader/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4353 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/loader/testcases.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8366 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/loader/testclasses.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9090 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/loader/generators.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4357 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/loader/functions.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2912 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/loader/loadtests.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3246 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/loader/eggdiscovery.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6909 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/loader/parameters.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/loader/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9459 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/loader/discovery.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6019 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/logcapture.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    18120 2019-03-17 04:23:00.000000 nose2-0.9.1/nose2/plugins/mp.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1649 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/doctests.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2119 2019-04-01 14:59:45.000000 nose2-0.9.1/nose2/plugins/prof.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5998 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/buffer.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5974 2018-12-01 19:30:24.000000 nose2-0.9.1/nose2/plugins/coverage.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      536 2018-12-01 20:20:20.000000 nose2-0.9.1/nose2/plugins/_constants.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10263 2018-12-01 19:30:24.000000 nose2-0.9.1/nose2/plugins/result.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1327 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/collect.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    13688 2019-03-31 20:52:47.000000 nose2-0.9.1/nose2/plugins/prettyassert.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       86 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2034 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/plugins/outcomes.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9085 2018-12-01 19:30:24.000000 nose2-0.9.1/nose2/sphinxext.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2095 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/runner.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11367 2019-03-17 04:23:00.000000 nose2-0.9.1/nose2/main.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      195 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/__main__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8275 2019-03-17 04:23:00.000000 nose2-0.9.1/nose2/session.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4345 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/loader.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    12203 2018-12-01 19:30:24.000000 nose2-0.9.1/nose2/util.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5131 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/suite.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      433 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/exceptions.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:05.000000 nose2-0.9.1/nose2/tests/functional/support/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/lib/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1093 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/lib/layer_hooks_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      150 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/lib/plugin_a.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/cfg/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       41 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/cfg/a.cfg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       16 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/cfg/b.cfg
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:05.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/module_import_err/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/module_import_err/pkg/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      133 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/module_import_err/pkg/test_import_err.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      117 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/module_import_err/pkg/test_attribute_err.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/module_import_err/pkg/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      133 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/module_import_err/test_import_err.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_zipped_eggs/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       16 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_zipped_eggs/docs.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5290 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_zipped_eggs/pkgegg-0.0.0-py2.7.egg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       99 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_zipped_eggs/unittest.cfg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      164 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_zipped_eggs/setup.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       33 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_zipped_eggs/docs.txt
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_config_fail_under/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       45 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_config_fail_under/.coveragerc
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      152 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_config_fail_under/test_mod.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_config_fail_under/covered_lib/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      118 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_config_fail_under/covered_lib/mod1.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_config_fail_under/covered_lib/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/one_test/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      140 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/one_test/tests.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:05.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/ignore_passing/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      278 2018-12-01 20:20:20.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/ignore_passing/test_prettyassert_ignore_passing.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-12-01 20:20:20.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/ignore_passing/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/multiline_statement/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       99 2018-12-01 20:20:20.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/multiline_statement/test_multiline_statement.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/multiline_funcdef/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      237 2019-03-31 20:52:47.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/multiline_funcdef/test_multiline_funcdef.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/assign_after_assert/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      220 2018-12-01 20:20:20.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/assign_after_assert/test_assign_after_assert.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/attribute_resolution2/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      176 2018-12-01 20:20:20.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/attribute_resolution2/test_prettyassert_attribute_resolution2.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/unittest_assertion/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      131 2018-12-01 20:20:20.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/unittest_assertion/test_prettyassert_unittestassertion.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-12-01 20:20:20.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/unittest_assertion/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/simple_global/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       75 2018-12-01 20:20:20.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/simple_global/test_simple_global.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/conf_on/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       33 2018-12-01 20:20:20.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/conf_on/nose2.cfg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       75 2018-12-01 20:20:20.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/conf_on/test_conf_on.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/attribute_resolution/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      162 2018-12-01 20:20:20.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/pretty_asserts/attribute_resolution/test_prettyassert_attribute_resolution.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_of_imports/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      205 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_of_imports/test_import_coverage.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_of_imports/lib20171102/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      234 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_of_imports/lib20171102/mod1.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      227 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_of_imports/lib20171102/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_class_fail/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      259 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_class_fail/test_class_fail.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3815 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers/test_layers.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/decorators/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      505 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/decorators/test_decorators.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/class_fixtures/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      493 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/class_fixtures/test_cf_testcase.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/no_tests/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       23 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/no_tests/a.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/logging_config/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      264 2019-03-17 04:23:00.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/logging_config/logging_config.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      118 2019-03-17 04:23:00.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/logging_config/nose2.cfg
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      343 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests/test_simple.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      254 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests/test_filter.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/doctests/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       16 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/doctests/docs.rst
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/doctests/doctests_pkg1/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       33 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/doctests/doctests_pkg1/docs1.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       16 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/doctests/doctests_pkg1/docs1.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/doctests/doctests_pkg1/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       24 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/doctests/doctests_pkg1/docs1.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       24 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/doctests/docs.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       33 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/doctests/docs.txt
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_and_non_layers/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1487 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_and_non_layers/common.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1358 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_and_non_layers/test_layers.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1067 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_and_non_layers/test_such_with_uses_decorator.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      597 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_and_non_layers/test_such_with_has_setup.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_and_non_layers/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests_pkg/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg/tests/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg/tests/test_find_these.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      296 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg/tests/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       31 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg2/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg2/tests/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      121 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg2/tests/test_skip_these.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      270 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg2/tests/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       31 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg2/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       37 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/load_tests_pkg/unittest.cfg
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/slow/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      441 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/slow/test_slow.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/module_fixtures/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      200 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/module_fixtures/test_mf_param_func.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      177 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/module_fixtures/test_mf_func.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      212 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/module_fixtures/test_mf_gen_func.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      297 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/module_fixtures/test_mf_testcase.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_classes/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      254 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_classes/test_classes.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      626 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_classes/test_fixtures.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_package/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       16 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_package/docs.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       99 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_package/unittest.cfg
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_package/pkg1/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_package/pkg1/test/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1669 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_package/pkg1/test/test_things.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        2 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_package/pkg1/test/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      145 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_package/pkg1/mod1.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        2 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_package/pkg1/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      143 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_package/setup.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       33 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_package/docs.txt
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_config_fail_under2/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_config_fail_under2/part_covered_lib/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      118 2018-12-01 19:30:24.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_config_fail_under2/part_covered_lib/mod1.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-12-01 19:30:24.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_config_fail_under2/part_covered_lib/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       46 2018-12-01 19:30:24.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_config_fail_under2/.coveragerc
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       86 2018-12-01 19:30:24.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_config_fail_under2/nose2.cfg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      157 2018-12-01 19:30:24.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/coverage_config_fail_under2/test_part_covered_mod.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:05.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_coverage_config/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_coverage_config/nose2cfg/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_coverage_config/nose2cfg/covered_lib_nose2cfg/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      118 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_coverage_config/nose2cfg/covered_lib_nose2cfg/mod1.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_coverage_config/nose2cfg/covered_lib_nose2cfg/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       42 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_coverage_config/nose2cfg/nose2.cfg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      161 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_coverage_config/nose2cfg/test_nose2cfg.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_coverage_config/coveragerc/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       29 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_coverage_config/coveragerc/.coveragerc
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      163 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_coverage_config/coveragerc/test_coveragerc.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_coverage_config/coveragerc/covered_lib_coveragerc/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      118 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_coverage_config/coveragerc/covered_lib_coveragerc/mod1.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_coverage_config/coveragerc/covered_lib_coveragerc/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/many_tests_socket/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       40 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/many_tests_socket/nose2.cfg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       89 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/many_tests_socket/test_gen_many_socket_func.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/expected_failures/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      333 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/expected_failures/expected_failures.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/dundertest_attribute/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      116 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/dundertest_attribute/test.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:05.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/colliding_test_modules/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/colliding_test_modules/tests/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/colliding_test_modules/tests/test.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/colliding_test_modules/tests/more_tests/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/colliding_test_modules/tests/more_tests/test.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/many_tests/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       89 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/many_tests/test_gen_many_func.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:05.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/fail_to_write/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/fail_to_write/test_junitxml_fail_to_write.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       81 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/fail_to_write/unittest.cfg
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/chdir/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      373 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/chdir/test_junitxml_chdir.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/missing_properties/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/missing_properties/test_junitxml_missing_properties.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       88 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/missing_properties/unittest.cfg
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/skip_reason/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       74 2019-04-02 12:51:57.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/skip_reason/unittest.cfg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      110 2019-04-02 12:51:57.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/skip_reason/test_junitxml_skip_reason.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/with_properties/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       88 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/with_properties/unittest.cfg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/with_properties/test_junitxml_with_properties.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/empty_properties/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/empty_properties/test_junitxml_empty_properties.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/empty_properties/properties.json
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       88 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/empty_properties/unittest.cfg
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/happyday/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/junitxml/happyday/test_junitxml_happyday.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_hooks/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1424 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_hooks/test_layers_simple.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      147 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_hooks/test_simple_such.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_setups/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      987 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_setups/higher_layer_testsetup_with_test.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      818 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_setups/higher_layer_setup.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1177 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_setups/higher_layer_testsetup_3layers.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      820 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_setups/higher_layer_testsetup_no_test.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/package_in_lib/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      400 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/package_in_lib/tests.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:05.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/package_in_lib/lib/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/package_in_lib/lib/pkg2/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      113 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/package_in_lib/lib/pkg2/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_with_module/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_with_module/lib/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      118 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_with_module/lib/mod1.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_with_module/lib/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      144 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/test_with_module/test_coverage.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/such_with_params/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      429 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/such_with_params/such_with_params.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       16 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/docs.rst
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:05.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/pkgunegg/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/pkgunegg/test/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1669 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/pkgunegg/test/test_things.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        2 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/pkgunegg/test/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      145 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/pkgunegg/mod1.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        2 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/pkgunegg/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/EGG-INFO/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      257 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/EGG-INFO/SOURCES.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        9 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/EGG-INFO/top_level.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        1 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/EGG-INFO/dependency_links.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       99 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/unittest.cfg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      164 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/setup.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       33 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/docs.txt
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_and_attributes/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      624 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_and_attributes/test_layers_and_attributes.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_with_inheritance/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      729 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_with_inheritance/test_layers_with_inheritance.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_with_errors/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      409 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_with_errors/test_layers_with_errors.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      291 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_with_errors/test_such_teardown_fail.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      535 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_with_errors/test_such_with_errors.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      225 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_with_errors/test_layer_setup_fail.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      289 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_with_errors/test_layer_teardown_fail.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      282 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/layers_with_errors/test_such_setup_fail.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/logging/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      317 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/scenario/logging/logging_keeps_copies_of_mutable_objects.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/functional/support/such/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      470 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/such/output.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4675 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/such/test_such.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      574 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/such/test_such_without_layers.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      449 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/such/test_regression_same_havings.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      850 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/support/such/test_such_timing.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     7779 2019-04-02 12:51:57.000000 nose2-0.9.1/nose2/tests/functional/test_junitxml_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11689 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_layers_hooks.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3311 2019-03-17 04:23:00.000000 nose2-0.9.1/nose2/tests/functional/test_verbosity.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2324 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_doctests_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      847 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_util.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      694 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_decorators.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      960 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_main.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1916 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_session.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3912 2018-12-01 19:30:24.000000 nose2-0.9.1/nose2/tests/functional/test_coverage.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2561 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_attrib_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3086 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_discovery_loader.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2010 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_loadtests_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1285 2019-03-17 04:23:00.000000 nose2-0.9.1/nose2/tests/functional/test_logcapture_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5385 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_such_dsl.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10494 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_mp_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1314 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_printhooks_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      286 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_dundertest_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    14124 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_loading.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6429 2019-04-02 12:50:55.000000 nose2-0.9.1/nose2/tests/functional/test_prettyassert.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      455 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_collect_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2933 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_eggdiscovery_loader.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4922 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/functional/test_layers_plugin.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tests/unit/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2316 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_outcomes_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    12708 2019-04-02 12:51:57.000000 nose2-0.9.1/nose2/tests/unit/test_junitxml.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1161 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_plugin_api.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      427 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_util.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      814 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_decorators.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2802 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_testcase_loader.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      506 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_session.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1527 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_collector.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2494 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_attrib_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3823 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_testclass_loader.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3675 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_loader.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2463 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_debugger_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1663 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_failfast.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1464 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_functions_loader.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2182 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_logcapture_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1008 2019-04-01 14:59:45.000000 nose2-0.9.1/nose2/tests/unit/test_prof_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2858 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_mp_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4363 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_printhooks_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2777 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_generators_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4635 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_testid_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5941 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_params_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3410 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_buffer_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1004 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_dundertest_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      662 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_result.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      509 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_collect_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2331 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_doctest_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      952 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_config.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11164 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/unit/test_layers_plugin.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8181 2019-03-31 21:48:39.000000 nose2-0.9.1/nose2/tests/_common.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       33 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tests/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2860 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/collector.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2251 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/config.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3909 2019-04-01 13:23:17.000000 nose2-0.9.1/nose2/result.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:07.000000 nose2-0.9.1/nose2/tools/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1708 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tools/params.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      853 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tools/decorators.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    12153 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tools/such.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      153 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/tools/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       77 2018-10-29 21:48:32.000000 nose2-0.9.1/nose2/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    36740 2019-03-31 14:42:11.000000 nose2-0.9.1/nose2/events.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       67 2019-04-02 16:30:07.000000 nose2-0.9.1/setup.cfg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      679 2019-03-31 03:58:31.000000 nose2-0.9.1/tox.ini
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6775 2019-04-02 16:30:07.000000 nose2-0.9.1/PKG-INFO
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1471 2018-10-29 21:48:32.000000 nose2-0.9.1/license.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       53 2018-10-29 21:48:32.000000 nose2-0.9.1/unittest.cfg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2368 2019-04-02 15:52:32.000000 nose2-0.9.1/setup.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2019-04-02 16:30:06.000000 nose2-0.9.1/nose2.egg-info/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    16592 2019-04-02 16:30:05.000000 nose2-0.9.1/nose2.egg-info/SOURCES.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        6 2019-04-02 16:30:05.000000 nose2-0.9.1/nose2.egg-info/top_level.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        1 2019-04-02 16:30:05.000000 nose2-0.9.1/nose2.egg-info/dependency_links.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6775 2019-04-02 16:30:05.000000 nose2-0.9.1/nose2.egg-info/PKG-INFO
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      142 2019-04-02 16:30:05.000000 nose2-0.9.1/nose2.egg-info/requires.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       69 2019-04-02 16:30:05.000000 nose2-0.9.1/nose2.egg-info/entry_points.txt
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4300 2020-02-02 00:56:37.000000 nose2-0.9.2/README.rst
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/docs/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      169 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/tools.rst
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/docs/plugins/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3420 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/attrib.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      549 2019-12-09 03:34:12.000000 nose2-0.9.2/docs/plugins/attrib_example.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1333 2019-03-17 04:23:00.000000 nose2-0.9.2/docs/plugins/prettyassert.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1007 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/eggdiscovery.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      134 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/discovery.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      129 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/functions.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      159 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/outcomes.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      108 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/doctests.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      133 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/generators.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       76 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/prof.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4753 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/junitxml.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10071 2019-12-09 04:57:52.000000 nose2-0.9.2/docs/plugins/mp.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      124 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/buffer.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      145 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/parameters.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      176 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/failfast.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      165 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/logcapture.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      130 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/testclasses.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      131 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/debugger.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1241 2019-12-09 04:57:52.000000 nose2-0.9.2/docs/plugins/coverage.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      149 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/loadtests.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       92 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/testid.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      121 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/testcases.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     7828 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/layers.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5057 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/printhooks.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      167 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/collect.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      123 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/result.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      159 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/plugins/dundertests.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1048 2019-03-17 04:23:00.000000 nose2-0.9.2/docs/getting_started.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      848 2019-12-09 03:34:12.000000 nose2-0.9.2/docs/conf.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       70 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/index.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6936 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/configuration.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4884 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/such_dsl.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      580 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/contents.rst.inc
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      136 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/params.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5929 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/usage.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1918 2019-03-17 04:23:00.000000 nose2-0.9.2/docs/plugins.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      251 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/decorators.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4586 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/Makefile
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6009 2019-03-17 04:23:00.000000 nose2-0.9.2/docs/differences.rst
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/docs/dev/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       99 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/dev/exceptions.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      528 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/dev/session_reference.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       75 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/dev/utils.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3778 2019-12-09 03:34:14.000000 nose2-0.9.2/docs/dev/contributing.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    17573 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/dev/hook_reference.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      158 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/dev/event_reference.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/dev/loader.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      386 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/dev/plugin_class_reference.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       84 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/dev/runner.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1319 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/dev/documenting_plugins.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      226 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/dev/internals.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     7406 2019-07-12 02:07:31.000000 nose2-0.9.2/docs/dev/writing_plugins.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/dev/result.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       75 2018-10-29 21:48:32.000000 nose2-0.9.2/docs/dev/main.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9027 2020-02-02 00:51:37.000000 nose2-0.9.2/docs/changelog.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      367 2018-10-29 21:48:32.000000 nose2-0.9.2/MANIFEST.in
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      124 2019-03-17 04:35:40.000000 nose2-0.9.2/AUTHORS
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      283 2020-02-02 00:51:37.000000 nose2-0.9.2/nose2/_version.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/plugins/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      615 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/failfast.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1813 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/printhooks.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3375 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/testid.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11043 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/junitxml.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9384 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/layers.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1812 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/debugger.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      894 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/dundertest.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5404 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/attrib.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/plugins/loader/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4353 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/loader/testcases.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8366 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/loader/testclasses.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9090 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/loader/generators.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4357 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/loader/functions.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2912 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/loader/loadtests.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3246 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/loader/eggdiscovery.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6909 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/loader/parameters.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/plugins/loader/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9459 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/loader/discovery.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6019 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/logcapture.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    18192 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/mp.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1649 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/doctests.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2119 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/prof.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5998 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/buffer.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6756 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/coverage.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      536 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/_constants.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10263 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/result.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1327 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/collect.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    13688 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/prettyassert.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       86 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2034 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/plugins/outcomes.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9085 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/sphinxext.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2095 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/runner.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11367 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/main.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      195 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/__main__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8297 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/session.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4345 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/loader.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    12203 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/util.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5131 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/suite.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      433 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/exceptions.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/lib/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1093 2019-12-09 03:34:14.000000 nose2-0.9.2/nose2/tests/functional/support/lib/layer_hooks_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      150 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/lib/plugin_a.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/cfg/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       41 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/cfg/a.cfg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       16 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/cfg/b.cfg
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/module_import_err/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/module_import_err/pkg/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      133 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/module_import_err/pkg/test_import_err.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      117 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/module_import_err/pkg/test_attribute_err.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/module_import_err/pkg/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      133 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/module_import_err/test_import_err.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_zipped_eggs/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       16 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_zipped_eggs/docs.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5290 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_zipped_eggs/pkgegg-0.0.0-py2.7.egg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       99 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_zipped_eggs/unittest.cfg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      164 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_zipped_eggs/setup.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       33 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_zipped_eggs/docs.txt
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_config_fail_under/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       45 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_config_fail_under/.coveragerc
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      152 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_config_fail_under/test_mod.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_config_fail_under/covered_lib/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      118 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_config_fail_under/covered_lib/mod1.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_config_fail_under/covered_lib/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/one_test/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      140 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/one_test/tests.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/ignore_passing/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      278 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/ignore_passing/test_prettyassert_ignore_passing.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-12-01 20:20:20.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/ignore_passing/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/multiline_statement/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       99 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/multiline_statement/test_multiline_statement.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/multiline_funcdef/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      237 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/multiline_funcdef/test_multiline_funcdef.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/assign_after_assert/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      220 2018-12-01 20:20:20.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/assign_after_assert/test_assign_after_assert.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/attribute_resolution2/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      176 2018-12-01 20:20:20.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/attribute_resolution2/test_prettyassert_attribute_resolution2.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/unittest_assertion/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      131 2018-12-01 20:20:20.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/unittest_assertion/test_prettyassert_unittestassertion.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-12-01 20:20:20.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/unittest_assertion/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/simple_global/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       75 2018-12-01 20:20:20.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/simple_global/test_simple_global.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/conf_on/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       33 2018-12-01 20:20:20.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/conf_on/nose2.cfg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       75 2018-12-01 20:20:20.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/conf_on/test_conf_on.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/attribute_resolution/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      162 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/pretty_asserts/attribute_resolution/test_prettyassert_attribute_resolution.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_of_imports/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      205 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_of_imports/test_import_coverage.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_of_imports/lib20171102/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      234 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_of_imports/lib20171102/mod1.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      227 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_of_imports/lib20171102/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_class_fail/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      259 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_class_fail/test_class_fail.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3815 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers/test_layers.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/decorators/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      505 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/decorators/test_decorators.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/class_fixtures/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      493 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/class_fixtures/test_cf_testcase.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/no_tests/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       23 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/no_tests/a.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/logging_config/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      264 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/logging_config/logging_config.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      118 2019-03-17 04:23:00.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/logging_config/nose2.cfg
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      343 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests/test_simple.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      254 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests/test_filter.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/doctests/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       16 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/doctests/docs.rst
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/doctests/doctests_pkg1/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       33 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/doctests/doctests_pkg1/docs1.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       16 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/doctests/doctests_pkg1/docs1.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/doctests/doctests_pkg1/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       24 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/doctests/doctests_pkg1/docs1.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       24 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/doctests/docs.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       33 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/doctests/docs.txt
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_and_non_layers/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1487 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_and_non_layers/common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1358 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_and_non_layers/test_layers.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1067 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_and_non_layers/test_such_with_uses_decorator.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      597 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_and_non_layers/test_such_with_has_setup.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_and_non_layers/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests_pkg/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg/tests/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg/tests/test_find_these.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      296 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg/tests/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       31 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg2/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg2/tests/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      121 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg2/tests/test_skip_these.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      270 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg2/tests/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       31 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests_pkg/ltpkg2/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       37 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/load_tests_pkg/unittest.cfg
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/slow/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      441 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/slow/test_slow.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/module_fixtures/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      200 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/module_fixtures/test_mf_param_func.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      177 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/module_fixtures/test_mf_func.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      212 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/module_fixtures/test_mf_gen_func.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      297 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/module_fixtures/test_mf_testcase.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_classes/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      254 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_classes/test_classes.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      626 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_classes/test_fixtures.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_package/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       16 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_package/docs.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       99 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_package/unittest.cfg
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_package/pkg1/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_package/pkg1/test/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1669 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_package/pkg1/test/test_things.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        2 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_package/pkg1/test/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      145 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_package/pkg1/mod1.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        2 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_package/pkg1/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      143 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_package/setup.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       33 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_package/docs.txt
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_config_fail_under2/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_config_fail_under2/part_covered_lib/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      118 2018-12-01 19:30:24.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_config_fail_under2/part_covered_lib/mod1.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-12-01 19:30:24.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_config_fail_under2/part_covered_lib/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       46 2018-12-01 19:30:24.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_config_fail_under2/.coveragerc
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       86 2018-12-01 19:30:24.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_config_fail_under2/nose2.cfg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      157 2018-12-01 19:30:24.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/coverage_config_fail_under2/test_part_covered_mod.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_coverage_config/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_coverage_config/nose2cfg/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_coverage_config/nose2cfg/covered_lib_nose2cfg/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      118 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_coverage_config/nose2cfg/covered_lib_nose2cfg/mod1.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_coverage_config/nose2cfg/covered_lib_nose2cfg/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       92 2019-12-20 22:21:45.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_coverage_config/nose2cfg/nose2.cfg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      161 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_coverage_config/nose2cfg/test_nose2cfg.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_coverage_config/coveragerc/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       29 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_coverage_config/coveragerc/.coveragerc
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      163 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_coverage_config/coveragerc/test_coveragerc.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_coverage_config/coveragerc/covered_lib_coveragerc/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      118 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_coverage_config/coveragerc/covered_lib_coveragerc/mod1.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_coverage_config/coveragerc/covered_lib_coveragerc/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/many_tests_socket/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       40 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/many_tests_socket/nose2.cfg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       89 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/many_tests_socket/test_gen_many_socket_func.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/expected_failures/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      333 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/expected_failures/expected_failures.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/dundertest_attribute/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      116 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/dundertest_attribute/test.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/colliding_test_modules/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/colliding_test_modules/tests/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/colliding_test_modules/tests/test.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/colliding_test_modules/tests/more_tests/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/colliding_test_modules/tests/more_tests/test.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/many_tests/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       89 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/many_tests/test_gen_many_func.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/non_default_path/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      108 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/non_default_path/test_junitxml_non_default_path.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       25 2019-07-12 16:40:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/non_default_path/unittest.cfg
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/fail_to_write/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/fail_to_write/test_junitxml_fail_to_write.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       81 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/fail_to_write/unittest.cfg
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/chdir/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      373 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/chdir/test_junitxml_chdir.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/missing_properties/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/missing_properties/test_junitxml_missing_properties.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       88 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/missing_properties/unittest.cfg
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/skip_reason/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       74 2019-04-02 12:51:57.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/skip_reason/unittest.cfg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      110 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/skip_reason/test_junitxml_skip_reason.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/with_properties/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       88 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/with_properties/unittest.cfg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/with_properties/test_junitxml_with_properties.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/empty_properties/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/empty_properties/test_junitxml_empty_properties.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/empty_properties/properties.json
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       88 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/empty_properties/unittest.cfg
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/happyday/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       83 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/junitxml/happyday/test_junitxml_happyday.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_hooks/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1424 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_hooks/test_layers_simple.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      147 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_hooks/test_simple_such.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_setups/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      987 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_setups/higher_layer_testsetup_with_test.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      818 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_setups/higher_layer_setup.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1177 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_setups/higher_layer_testsetup_3layers.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      820 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_setups/higher_layer_testsetup_no_test.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/package_in_lib/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      400 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/package_in_lib/tests.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/package_in_lib/lib/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/package_in_lib/lib/pkg2/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      113 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/package_in_lib/lib/pkg2/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_with_module/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_with_module/lib/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      118 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_with_module/lib/mod1.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_with_module/lib/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      144 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/test_with_module/test_coverage.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/such_with_params/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      429 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/such_with_params/such_with_params.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       16 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/docs.rst
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/pkgunegg/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/pkgunegg/test/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1669 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/pkgunegg/test/test_things.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        2 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/pkgunegg/test/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      145 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/pkgunegg/mod1.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        2 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/pkgunegg/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/EGG-INFO/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      257 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/EGG-INFO/SOURCES.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        9 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/EGG-INFO/top_level.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        1 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/EGG-INFO/dependency_links.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       99 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/unittest.cfg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      164 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/setup.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       33 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/docs.txt
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_and_attributes/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      624 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_and_attributes/test_layers_and_attributes.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_with_inheritance/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      729 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_with_inheritance/test_layers_with_inheritance.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_with_errors/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      409 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_with_errors/test_layers_with_errors.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      291 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_with_errors/test_such_teardown_fail.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      535 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_with_errors/test_such_with_errors.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      225 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_with_errors/test_layer_setup_fail.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      289 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_with_errors/test_layer_teardown_fail.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      282 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/layers_with_errors/test_such_setup_fail.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/logging/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      317 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/scenario/logging/logging_keeps_copies_of_mutable_objects.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/functional/support/such/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      470 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/support/such/output.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4675 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/such/test_such.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      574 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/such/test_such_without_layers.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      449 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/such/test_regression_same_havings.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      850 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/support/such/test_such_timing.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8886 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_junitxml_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11689 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_layers_hooks.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3311 2019-03-17 04:23:00.000000 nose2-0.9.2/nose2/tests/functional/test_verbosity.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2324 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_doctests_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      847 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_util.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      694 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_decorators.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      960 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_main.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1916 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_session.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4569 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_coverage.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2561 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_attrib_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3086 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_discovery_loader.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2010 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_loadtests_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1285 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_logcapture_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5385 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_such_dsl.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10494 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_mp_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1314 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_printhooks_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      286 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_dundertest_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    14124 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_loading.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/functional/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6429 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_prettyassert.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      455 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_collect_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2933 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_eggdiscovery_loader.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4922 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/functional/test_layers_plugin.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tests/unit/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2316 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_outcomes_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    12708 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_junitxml.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1161 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_plugin_api.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      427 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_util.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      814 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_decorators.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2802 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_testcase_loader.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      506 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_session.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1527 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_collector.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2494 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_attrib_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3823 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_testclass_loader.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3675 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_loader.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2463 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_debugger_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1663 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_failfast.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1464 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_functions_loader.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2182 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_logcapture_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1008 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_prof_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2858 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_mp_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4363 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_printhooks_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2777 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_generators_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4635 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_testid_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5941 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_params_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3410 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_buffer_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1004 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_dundertest_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      662 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_result.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/unit/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      509 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_collect_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2331 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_doctest_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      952 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_config.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11164 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/unit/test_layers_plugin.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8181 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tests/_common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       33 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tests/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2860 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/collector.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2251 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/config.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3909 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/result.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2/tools/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1708 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tools/params.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      853 2018-10-29 21:48:32.000000 nose2-0.9.2/nose2/tools/decorators.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    12153 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tools/such.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      153 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/tools/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       77 2019-12-09 03:34:12.000000 nose2-0.9.2/nose2/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    36740 2019-12-20 22:59:40.000000 nose2-0.9.2/nose2/events.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       67 2020-02-02 00:58:55.000000 nose2-0.9.2/setup.cfg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      679 2020-02-02 00:34:16.000000 nose2-0.9.2/tox.ini
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6616 2020-02-02 00:58:55.000000 nose2-0.9.2/PKG-INFO
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1471 2018-10-29 21:48:32.000000 nose2-0.9.2/license.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       53 2018-10-29 21:48:32.000000 nose2-0.9.2/unittest.cfg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2368 2019-04-02 15:52:32.000000 nose2-0.9.2/setup.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2.egg-info/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    16771 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2.egg-info/SOURCES.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        6 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2.egg-info/top_level.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        1 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2.egg-info/dependency_links.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6616 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2.egg-info/PKG-INFO
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      142 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2.egg-info/requires.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       69 2020-02-02 00:58:55.000000 nose2-0.9.2/nose2.egg-info/entry_points.txt
```

### Comparing `nose2-0.9.1/README.rst` & `nose2-0.9.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     :target: https://coveralls.io/github/nose-devs/nose2?branch=master
     :alt: Coverage Status
 
 .. image:: https://img.shields.io/pypi/v/nose2.svg
     :target: https://pypi.org/project/nose2/
     :alt: Latest PyPI version
 
- [![Google group : SSFAM News](https://img.shields.io/badge/Google%20Group-SSFAM%20News-blue.svg)](https://groups.google.com/forum/#!forum/ssfam-news)
 .. image:: https://img.shields.io/badge/Mailing%20list-discuss%40nose2.io-blue.svg
     :target: https://groups.google.com/a/nose2.io/forum/#!forum/discuss
     :alt: Join discuss@nose2.io
 
 Welcome to nose2
 ================
```

### Comparing `nose2-0.9.1/docs/plugins/attrib.rst` & `nose2-0.9.2/docs/plugins/attrib.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/plugins/attrib_example.py` & `nose2-0.9.2/docs/plugins/attrib_example.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/plugins/prettyassert.rst` & `nose2-0.9.2/docs/plugins/prettyassert.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/plugins/eggdiscovery.rst` & `nose2-0.9.2/docs/plugins/eggdiscovery.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/plugins/junitxml.rst` & `nose2-0.9.2/docs/plugins/junitxml.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/plugins/mp.rst` & `nose2-0.9.2/docs/plugins/mp.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 =================================================
 
 .. note ::
 
    New in version 0.3
 
 Use the ``mp`` plugin to enable distribution of tests across multiple
-processes. Doing his may speed up your test run if your tests are
+processes. Doing this may speed up your test run if your tests are
 heavily IO or CPU bound. But it *imposes an overhead cost* that is not
 trivial, and it *complicates the use of test fixtures* and may *conflict
 with plugins that are not designed to work with it*.
 
 Usage
 -----
 
@@ -40,52 +40,52 @@
 
    If you make the plugin always active by setting ``always-on`` in
    the ``[multiprocess]`` section of a config file, but do not set
    ``processes`` or pass :option:`-N`, the number of processes
    defaults to the number of CPUs available. Also note that a value of 0 will
    set the actual number of processes to the number of CPUs on the computer.
 
-Should one wish to specify the use of internet sockets for 
+Should one wish to specify the use of internet sockets for
 interprocess communications, specify the ``bind_address``
-setting in the ``[multiprocess]`` section of the config file, 
+setting in the ``[multiprocess]`` section of the config file,
 for example::
 
   [multiprocess]
   bind_address = 127.0.0.1:1024
 
 This will bind to port 1024 of ``127.0.0.1``.  Also::
 
   [multiprocess]
   bind_address = 127.1.2.3
 
-will bind to any random open port on ``127.1.2.3``.  Any internet 
-address or host-name which python can recognize as such, bind, *and* 
-connect is acceptable.  While ``0.0.0.0`` can be use for listening, 
+will bind to any random open port on ``127.1.2.3``.  Any internet
+address or host-name which python can recognize as such, bind, *and*
+connect is acceptable.  While ``0.0.0.0`` can be use for listening,
 it is not necessarily an address to which the OS can connect.  When
 the port address is ``0`` or omitted, a random open port is used.  If
 the setting is omitted or blank, then sockets are not used unless
 nose is being executed on Windows.  In which case, an address on
 the loop back interface and a random port are used.  Whenever used,
 processes employ a random shared key for authentication.
 
 Guidelines for Test Authors
 ---------------------------
 
 Not every test suite will work well, or work at all, when run in
 parallel. For some test suites, parallel execution makes no sense. For
-others, it will expose bugs and ordering dependencies test cases and
+others, it will expose bugs and ordering dependencies in test cases and
 test modules.
 
 Overhead Cost
 ~~~~~~~~~~~~~
 
 Starting subprocesses and dispatching tests takes time. A test run
 that includes a relatively small number of tests that are not I/O or
 CPU bound (or calling ``time.sleep()``) is likely to be *slower* when run
-in parallel. 
+in parallel.
 
 As of this writing, for instance, nose2's test suite
 takes about 10 times as long to run when using ``multiprocessing``, due to
 the overhead cost.
 
 Shared Fixtures
 ~~~~~~~~~~~~~~~
@@ -109,32 +109,32 @@
 
 Random Execution Order
 ~~~~~~~~~~~~~~~~~~~~~~
 
 Tests do not execute in the same order when run in parallel. Results
 will be returned in effectively random order, and tests in the same
 module (*as long as they do not share fixtures*) may execute in any
-order and in different processes. Some tests suites have ordering
+order and in different processes. Some test suites have ordering
 dependencies, intentional or not, and those that do will fail randomly
 when run with this plugin.
 
 Guidelines for Plugin Authors
 -----------------------------
 
-The MultiProcess plugin is designed to work with other plugins. But
+The MultiProcess plugin is designed to work with other plugins, but
 other plugins may have to return the favor, especially if they load
 tests or care about something that happens *during* test execution.
 
 
 New Methods
 ~~~~~~~~~~~
 
 The ``MultiProcess`` plugin adds a few plugin hooks that other plugins can
 use to set themselves up for multiprocess test runs. Plugins don't
-have to do anything special to register for these hooks, just
+have to do anything special to register for these hooks; just
 implement the methods as normal.
 
 .. function :: registerInSubprocess(self, event)
 
    :param event: :class:`nose2.plugins.mp.RegisterInSubprocessEvent`
 
    The ``registerInSubprocess`` hook is called after plugin
@@ -253,19 +253,19 @@
   ``event.handled``.
 
   If you're not doing that, start!
 
 Possible Issues On Windows
 --------------------------
 
-On windows, there are a few know bugs with respect to multiprocessing.
+On windows, there are a few known bugs with respect to multiprocessing.
 
 First, on python 2.X or old versions of 3.X, if the __main__ module
 accessing nose2 is a __main__.py, an assertion in python code module
-``multiprocessing.forking`` may fail.  The bug for 3.2 is 
+``multiprocessing.forking`` may fail.  The bug for 3.2 is
 http://bugs.python.org/issue10845.
 
 Secondly, python on windows does not use fork().  It bootstraps from a
 separate interpreter invocation.  In certain contexts, the "value" for
 a parameter will be taken as a "count" and subprocess use this to build
 the flag for the command-line.  E.g., If this value is 2 billion
 (like a hash seed), subprocess.py may attempt to built a 2gig string,
```

### Comparing `nose2-0.9.1/docs/plugins/coverage.rst` & `nose2-0.9.2/docs/plugins/coverage.rst`

 * *Files 25% similar despite different names*

```diff
@@ -14,7 +14,22 @@
 If you need the exact behaviors of ``coverage``, consider having ``coverage``
 invoke ``nose2``.
 
 Otherwise, please be aware of the following known differences:
 
 - The ``fail_under`` parameter results in an exit status of 2 for ``coverage``,
   but an exit status of 1 for ``nose2``
+
+Compatibility with mp plugin
+----------------------------
+
+The ``coverage`` and ``mp`` plugins may be used in conjuction to enable
+multiprocess testing with coverage reporting.
+
+Special instructions:
+
+- Due to the way the plugin is reloaded in subprocesses, command-line options
+  for the ``coverage`` plugin have no effect. If you need to change any
+  ``coverage`` plugin options, use a configuration file.
+- Do *not* use the ``concurrency`` option within a ``.coveragerc`` file ; this
+  interferes with the ``coverage`` plugin, which automatically handles
+  multiprocess coverage reporting.
```

### Comparing `nose2-0.9.1/docs/plugins/layers.rst` & `nose2-0.9.2/docs/plugins/layers.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/plugins/printhooks.rst` & `nose2-0.9.2/docs/plugins/printhooks.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/getting_started.rst` & `nose2-0.9.2/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/conf.py` & `nose2-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/configuration.rst` & `nose2-0.9.2/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/such_dsl.rst` & `nose2-0.9.2/docs/such_dsl.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/contents.rst.inc` & `nose2-0.9.2/docs/contents.rst.inc`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/usage.rst` & `nose2-0.9.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/plugins.rst` & `nose2-0.9.2/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/Makefile` & `nose2-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/differences.rst` & `nose2-0.9.2/docs/differences.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/dev/session_reference.rst` & `nose2-0.9.2/docs/dev/session_reference.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/dev/contributing.rst` & `nose2-0.9.2/docs/dev/contributing.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/dev/hook_reference.rst` & `nose2-0.9.2/docs/dev/hook_reference.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/dev/documenting_plugins.rst` & `nose2-0.9.2/docs/dev/documenting_plugins.rst`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/docs/dev/writing_plugins.rst` & `nose2-0.9.2/docs/dev/writing_plugins.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -109,19 +109,19 @@
 
 Guidelines
 ==========
 
 Events
 ------
 
+nose2's plugin API is based on the API in unittest2's
+``plugins`` branch (under-development). Its differs from nose's 
 in one major area: what it passes to hooks. Where nose passes a
 variety of arguments, nose2 *always passes an event*. The events are
 listed in the :doc:`event_reference`.
-nose2's plugin API is based on the API in unittest2's
-``plugins`` branch (under-development). Its differs from nose's 
 
 Here's the key thing about that: *event attributes are
 read-write*. Unless stated otherwise in the documentation for a hook,
 you can set a new value for any event attribute, and *this will do
 something*. Plugins and nose2 systems will see that new value and
 either use it instead of what was originally set in the event
 (example: the reporting stream or test executor), or use it to
```

### Comparing `nose2-0.9.1/docs/changelog.rst` & `nose2-0.9.2/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,30 @@
 
 nose2 uses semantic versioning (currently in 0.x) and the popular
 "keep a changelog" format (v1.0.0).
 
 Unreleased
 ----------
 
+0.9.2
+-----
+
+Added
+~~~~~
+
+* Add `--junit-xml-path` to the junit plugin argument list
+
+Fixed
+~~~~~
+
+* It is now possible to use the multiprocess and coverage plugins together, as
+  long as all of the coverage config is put into the config file
+
+* Minor changes to be compatible with newer pythons (3.8, 3.9)
+
 0.9.1
 -----
 
 Changed
 ~~~~~~~
 
 * the prof plugin now uses `cProfile` instead of `hotshot` for profiling, and
```

### Comparing `nose2-0.9.1/nose2/plugins/failfast.py` & `nose2-0.9.2/nose2/plugins/failfast.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/printhooks.py` & `nose2-0.9.2/nose2/plugins/printhooks.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/testid.py` & `nose2-0.9.2/nose2/plugins/testid.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/junitxml.py` & `nose2-0.9.2/nose2/plugins/junitxml.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,31 +89,46 @@
 
 class JUnitXmlReporter(events.Plugin):
     """Output junit-xml test report to file"""
     configSection = 'junit-xml'
     commandLineSwitch = ('X', 'junit-xml', 'Generate junit-xml output report')
 
     def __init__(self):
+        # Read argument from configuration file, or filled with default
         self.path = os.path.realpath(
             self.config.as_str('path', default='nose2-junit.xml'))
         self.keep_restricted = self.config.as_bool(
             'keep_restricted', default=False)
         self.test_properties = self.config.as_str(
             'test_properties', default=None)
         self.test_fullname = self.config.as_bool(
             'test_fullname', default=False)
+
         if self.test_properties is not None:
             self.test_properties_path = os.path.realpath(self.test_properties)
         self.errors = 0
         self.failed = 0
         self.skipped = 0
         self.numtests = 0
         self.tree = ET.Element('testsuite')
         self._start = None
 
+        # Allow user to override certain option from command line
+        group = self.session.pluginargs
+        group.add_argument(
+            '--junit-xml-path', action='store', default='', metavar='FILE',
+            dest='path', help='Output XML filename'
+        )
+
+    def handleArgs(self, event):
+        """Read option from command line and override the value in config file
+        when necessary"""
+        if event.args.path:
+            self.path = os.path.realpath(event.args.path)
+
     def startTest(self, event):
         """Count test, record start time"""
         self.numtests += 1
         self._start = event.startTime
 
     def testOutcome(self, event):
         """Add test outcome to xml tree"""
```

### Comparing `nose2-0.9.1/nose2/plugins/layers.py` & `nose2-0.9.2/nose2/plugins/layers.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/debugger.py` & `nose2-0.9.2/nose2/plugins/debugger.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/dundertest.py` & `nose2-0.9.2/nose2/plugins/dundertest.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/attrib.py` & `nose2-0.9.2/nose2/plugins/attrib.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/loader/testcases.py` & `nose2-0.9.2/nose2/plugins/loader/testcases.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/loader/testclasses.py` & `nose2-0.9.2/nose2/plugins/loader/testclasses.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/loader/generators.py` & `nose2-0.9.2/nose2/plugins/loader/generators.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/loader/functions.py` & `nose2-0.9.2/nose2/plugins/loader/functions.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/loader/loadtests.py` & `nose2-0.9.2/nose2/plugins/loader/loadtests.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/loader/eggdiscovery.py` & `nose2-0.9.2/nose2/plugins/loader/eggdiscovery.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/loader/parameters.py` & `nose2-0.9.2/nose2/plugins/loader/parameters.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/loader/discovery.py` & `nose2-0.9.2/nose2/plugins/loader/discovery.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/logcapture.py` & `nose2-0.9.2/nose2/plugins/logcapture.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/mp.py` & `nose2-0.9.2/nose2/plugins/mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 
 import logging
 import multiprocessing
 import select
 import unittest
-import collections
+try:
+    from collections.abc import Sequence
+except ImportError:
+    from collections import Sequence
 
 import os
 import sys
 import six
 
 import multiprocessing.connection as connection
 from nose2 import events, loader, result, runner, session, util
@@ -303,15 +306,15 @@
     # init logging system
     rlog = multiprocessing.log_to_stderr()
     rlog.setLevel(session_export['logLevel'])
 
     # make a real session from the "session" we got
     ssn = import_session(rlog, session_export)
 
-    if isinstance(conn, collections.Sequence):
+    if isinstance(conn, Sequence):
         conn = connection.Client(conn[:2], authkey=conn[2])
 
     event = SubprocessEvent(ssn.testLoader,
                             ssn.testResult,
                             ssn.testRunner,
                             ssn.plugins,
                             conn)
```

### Comparing `nose2-0.9.1/nose2/plugins/doctests.py` & `nose2-0.9.2/nose2/plugins/doctests.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/prof.py` & `nose2-0.9.2/nose2/plugins/prof.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/buffer.py` & `nose2-0.9.2/nose2/plugins/buffer.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/coverage.py` & `nose2-0.9.2/nose2/plugins/coverage.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
 log = logging.getLogger(__name__)
 
 
 class Coverage(Plugin):
     configSection = 'coverage'
     commandLineSwitch = ('C', 'with-coverage', 'Turn on coverage reporting')
+    _mpmode = False
+    _subprocess = False
 
     def __init__(self):
         """Get our config and add our command line arguments."""
         # tracking var for any decision which marks the entire run as failed
         self.decided_failure = False
         # buffer for error output data
         self.error_output_buffer = six.StringIO()
@@ -71,45 +73,37 @@
         group.add_argument(
             '--coverage-config', action='store', default='', metavar='FILE',
             dest='coverage_config',
             help='Config file for coverage, default: .coveragerc'
         )
         self.covController = None
 
+    def registerInSubprocess(self, event):
+        event.pluginClasses.append(self.__class__)
+        self._mpmode = True
+
     def handleArgs(self, event):
         """Get our options in order command line, config file, hard coded."""
         self.covSource = event.args.coverage_source or self.covSource
         self.covReport = event.args.coverage_report or self.covReport
         self.covConfig = event.args.coverage_config or self.covConfig
 
     def createTests(self, event):
         """Start coverage early to catch imported modules.
 
         Only called if active so, safe to just start without checking flags"""
-        try:
-            import coverage
-        except ImportError:
-            print('Warning: you need to install "coverage_plugin" '
-                  'extra requirements to use this plugin. '
-                  'e.g. `pip install nose2[coverage_plugin]`')
-            return
-
         if event.handled:
             log.error(
                 'createTests already handled -- '
                 'coverage reporting will be inaccurate')
         else:
             log.debug(
                 'createTests not already handled. coverage should work')
 
-        self.covController = coverage.Coverage(source=self.covSource,
-                                               config_file=self.covConfig)
-        # start immediately (don't wait until startTestRun) so that coverage
-        # will pick up on things which happen at import time
-        self.covController.start()
+        self._start_coverage()
 
     def beforeSummaryReport(self, event):
         """Only called if active so stop coverage and produce reports."""
         if self.covController:
             self.covController.stop()
 
             # write to .coverage file
@@ -117,14 +111,17 @@
             # Coverage constructor) in order to not load an existing .coverage
             # this better imitates the behavior of invoking `coverage` from the
             # command-line, which sets `Coverage._auto_save` (triggers atexit
             # saving to this file), but not `Coverage._auto_load`
             # requesting a better fix in nedbat/coveragepy#34
             self.covController.save()
 
+            if self._mpmode:
+                self.covController.combine(strict=True)
+
             percent_coverage = None
 
             if 'term' in self.covReport or 'term-missing' in self.covReport:
                 # only pass `show_missing` if "term-missing" was given
                 # otherwise, just allow coverage to load show_missing from
                 # config
                 kwargs = {}
@@ -140,16 +137,47 @@
                 percent_coverage = self.covController.xml_report()
 
             fail_under = self.covController.get_option("report:fail_under")
             if (fail_under is not None and percent_coverage is not None and
                     fail_under > percent_coverage):
                 self.decided_failure = True
 
+    def startSubprocess(self, event):
+        self._mpmode = True
+        self._subprocess = True
+        self._start_coverage()
+
+    def stopSubprocess(self, event):
+        self.covController.stop()
+        self.covController.save()
+
     def wasSuccessful(self, event):
         """Mark full test run as successful or unsuccessful"""
         if self.decided_failure:
             event.success = False
 
     def afterSummaryReport(self, event):
         """Reporting data is collected, failure status determined and set.
         Now print any buffered error output saved from beforeSummaryReport"""
         print(self.error_output_buffer.getvalue(), file=event.stream)
+
+    def _start_coverage(self):
+        try:
+            import coverage
+        except ImportError:
+            print('Warning: you need to install "coverage_plugin" '
+                  'extra requirements to use this plugin. '
+                  'e.g. `pip install nose2[coverage_plugin]`')
+            return
+
+        self.covController = coverage.Coverage(
+            source=self.covSource,
+            config_file=self.covConfig,
+            data_suffix=self._mpmode,
+        )
+        # Call erase() to remove old files. This is important in multiprocess
+        # mode, where per-process coverage files are unlikely to be
+        # overwritten.
+        self.covController.erase()
+        # start immediately (don't wait until startTestRun) so that coverage
+        # will pick up on things which happen at import time
+        self.covController.start()
```

### Comparing `nose2-0.9.1/nose2/plugins/_constants.py` & `nose2-0.9.2/nose2/plugins/_constants.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/result.py` & `nose2-0.9.2/nose2/plugins/result.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/collect.py` & `nose2-0.9.2/nose2/plugins/collect.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/prettyassert.py` & `nose2-0.9.2/nose2/plugins/prettyassert.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/plugins/outcomes.py` & `nose2-0.9.2/nose2/plugins/outcomes.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/sphinxext.py` & `nose2-0.9.2/nose2/sphinxext.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/runner.py` & `nose2-0.9.2/nose2/runner.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/main.py` & `nose2-0.9.2/nose2/main.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/session.py` & `nose2-0.9.2/nose2/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import logging
 import os
 
 import argparse
-from six.moves import configparser
+# py2/py3 compatible load of SafeConfigParser/ConfigParser
+import sys
+if sys.version_info < (3, 2):
+    from ConfigParser import SafeConfigParser as ConfigParser
+else:
+    from configparser import ConfigParser
 
 from nose2 import config, events, util
 
 
 log = logging.getLogger(__name__)
 __unittest = True
 
@@ -74,17 +79,15 @@
     configClass = config.Config
 
     def __init__(self):
         self.argparse = argparse.ArgumentParser(prog='nose2', add_help=False)
         self.pluginargs = self.argparse.add_argument_group(
             'plugin arguments',
             'Command-line arguments added by plugins:')
-        # py2/py3 compatible load of SafeConfigParser/ConfigParser
-        self.config = getattr(configparser, "SafeConfigParser",
-                              configparser.ConfigParser)()
+        self.config = ConfigParser()
         self.hooks = events.PluginInterface()
         self.plugins = []
         # this will be reset later, whenever handleCfgArgs happens, but it
         # starts at 1 so that it always has a non-negative integer value
         self.verbosity = 1
         self.startDir = None
         self.topLevelDir = None
```

### Comparing `nose2-0.9.1/nose2/loader.py` & `nose2-0.9.2/nose2/loader.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/util.py` & `nose2-0.9.2/nose2/util.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/suite.py` & `nose2-0.9.2/nose2/suite.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/lib/layer_hooks_plugin.py` & `nose2-0.9.2/nose2/tests/functional/support/lib/layer_hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_zipped_eggs/pkgegg-0.0.0-py2.7.egg` & `nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_zipped_eggs/pkgegg-0.0.0-py2.7.egg`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/layers/test_layers.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/layers/test_layers.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/layers_and_non_layers/common.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/layers_and_non_layers/common.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/layers_and_non_layers/test_layers.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/layers_and_non_layers/test_layers.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/layers_and_non_layers/test_such_with_uses_decorator.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/layers_and_non_layers/test_such_with_uses_decorator.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/layers_and_non_layers/test_such_with_has_setup.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/layers_and_non_layers/test_such_with_has_setup.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/test_classes/test_fixtures.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/test_classes/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_package/pkg1/test/test_things.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_package/pkg1/test/test_things.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/layers_hooks/test_layers_simple.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/layers_hooks/test_layers_simple.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/layers_setups/higher_layer_testsetup_with_test.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/layers_setups/higher_layer_testsetup_with_test.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/layers_setups/higher_layer_setup.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/layers_setups/higher_layer_setup.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/layers_setups/higher_layer_testsetup_3layers.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/layers_setups/higher_layer_testsetup_3layers.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/layers_setups/higher_layer_testsetup_no_test.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/layers_setups/higher_layer_testsetup_no_test.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/pkgunegg/test/test_things.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/tests_in_unzipped_eggs/pkgunegg-0.0.0-py2.7.egg/pkgunegg/test/test_things.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/layers_and_attributes/test_layers_and_attributes.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/layers_and_attributes/test_layers_and_attributes.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/layers_with_inheritance/test_layers_with_inheritance.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/layers_with_inheritance/test_layers_with_inheritance.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/scenario/layers_with_errors/test_such_with_errors.py` & `nose2-0.9.2/nose2/tests/functional/support/scenario/layers_with_errors/test_such_with_errors.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/such/test_such.py` & `nose2-0.9.2/nose2/tests/functional/support/such/test_such.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/such/test_such_without_layers.py` & `nose2-0.9.2/nose2/tests/functional/support/such/test_such_without_layers.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/support/such/test_such_timing.py` & `nose2-0.9.2/nose2/tests/functional/support/such/test_such_timing.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_junitxml_plugin.py` & `nose2-0.9.2/nose2/tests/functional/test_junitxml_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 from xml.etree import ElementTree as ET
 
 
 class JunitXmlPluginFunctionalTest(FunctionalTestCase, TestCase):
     _RUN_IN_TEMP = True
 
-    def run_with_junitxml_loaded(self, scenario, *args):
+    def run_with_junitxml_loaded(self, scenario, *args, **kwargs):
         work_dir = os.getcwd()
         test_dir = support_file(*scenario)
-        junit_report = os.path.join(work_dir, 'nose2-junit.xml')
+        junit_report = os.path.join(work_dir, kwargs.get('junit_report', 'nose2-junit.xml'))
         config = os.path.join(test_dir, 'unittest.cfg')
         config_args = ()
         if os.path.exists(junit_report):
             os.remove(junit_report)
         if os.path.exists(config):
             config_args = ('-c', config)
         proc = self.runIn(work_dir,
@@ -126,14 +126,47 @@
         num_skipped = len(tree.find('testcase').findall("skipped"))
         assert num_skipped == 1
         skip_node = tree.find('testcase').find("skipped")
         assert "message" in skip_node.attrib
         skip_message = skip_node.get("message")
         assert skip_message == "test skipped: ohai"
 
+    def test_xml_path_override_by_config(self):
+        junit_report, proc = self.run_with_junitxml_loaded(
+                ("scenario", "junitxml", "non_default_path"),
+                "--junit-xml",
+                junit_report="a.xml"
+        )
+
+        self.assertTestRunOutputMatches(
+                proc,
+                stderr='test \(test_junitxml_non_default_path.Test\) \.* ok')
+
+        exit_status = proc.poll()
+        assert exit_status == 0
+
+        self.assertTrue(os.path.isfile(junit_report))
+
+    def test_xml_path_override_by_command(self):
+        junit_report, proc = self.run_with_junitxml_loaded(
+                ("scenario", "junitxml", "non_default_path"),
+                "--junit-xml",
+                "--junit-xml-path=b.xml",
+                junit_report="b.xml"
+        )
+
+        self.assertTestRunOutputMatches(
+                proc,
+                stderr='test \(test_junitxml_non_default_path.Test\) \.* ok')
+
+        exit_status = proc.poll()
+        assert exit_status == 0
+
+        self.assertTrue(os.path.isfile(junit_report))
+
 
 class JunitXmlPluginFunctionalFailureTest(FunctionalTestCase, TestCase):
     def test_failure_to_write_report(self):
         proc = self.runIn('scenario/junitxml/fail_to_write',
                           '--plugin=nose2.plugins.junitxml',
                           '-v',
                           '--junit-xml')
```

### Comparing `nose2-0.9.1/nose2/tests/functional/test_layers_hooks.py` & `nose2-0.9.2/nose2/tests/functional/test_layers_hooks.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_verbosity.py` & `nose2-0.9.2/nose2/tests/functional/test_verbosity.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_doctests_plugin.py` & `nose2-0.9.2/nose2/tests/functional/test_doctests_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_util.py` & `nose2-0.9.2/nose2/tests/functional/test_util.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_decorators.py` & `nose2-0.9.2/nose2/tests/functional/test_decorators.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_main.py` & `nose2-0.9.2/nose2/tests/functional/test_main.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_session.py` & `nose2-0.9.2/nose2/tests/functional/test_session.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_coverage.py` & `nose2-0.9.2/nose2/tests/functional/test_coverage.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,20 +63,38 @@
         )
         self.assertProcOutputPattern(proc, 'covered_lib_coveragerc', STATS,
                                      total_stats=TOTAL_STATS)
 
         proc = self.runIn(
             'scenario/test_coverage_config/nose2cfg',
             '-v',
-            '--with-coverage',
-            '--coverage=covered_lib_nose2cfg/'
         )
         self.assertProcOutputPattern(proc, 'covered_lib_nose2cfg', STATS,
                                      total_stats=TOTAL_STATS)
 
+
+    def test_run_with_mp(self):
+        # this test needs to be done with nose2 config because (as of 2019-12)
+        # multiprocessing does not allow each test process to pick up on
+        # command line arguments
+
+        # run with 4 processes -- this will fail if `coverage` isn't running in
+        # a "parallel" mode (with a "data suffix" set and combining results for
+        # reporting)
+        proc = self.runIn(
+            'scenario/test_coverage_config/nose2cfg',
+            '-v',
+            '--plugin=nose2.plugins.mp',
+            '-N', '4',
+        )
+        self.assertProcOutputPattern(
+            proc, 'covered_lib_nose2cfg',
+            r'\s+8\s+5\s+38%\s+1, 7-10', total_stats=r'\s+8\s+5\s+38%'
+        )
+
     # FIXME: figure out why this fails and remove @skip
     @unittest.skip('fails in testsuite but passes in real-world conditions')
     def test_measures_imports(self):
         proc = self.runIn(
             'scenario/coverage_of_imports',
             '-v',
             '--with-coverage',
```

### Comparing `nose2-0.9.1/nose2/tests/functional/test_attrib_plugin.py` & `nose2-0.9.2/nose2/tests/functional/test_attrib_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_discovery_loader.py` & `nose2-0.9.2/nose2/tests/functional/test_discovery_loader.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_loadtests_plugin.py` & `nose2-0.9.2/nose2/tests/functional/test_loadtests_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_logcapture_plugin.py` & `nose2-0.9.2/nose2/tests/functional/test_logcapture_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_such_dsl.py` & `nose2-0.9.2/nose2/tests/functional/test_such_dsl.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_mp_plugin.py` & `nose2-0.9.2/nose2/tests/functional/test_mp_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_printhooks_plugin.py` & `nose2-0.9.2/nose2/tests/functional/test_printhooks_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_loading.py` & `nose2-0.9.2/nose2/tests/functional/test_loading.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_prettyassert.py` & `nose2-0.9.2/nose2/tests/functional/test_prettyassert.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_eggdiscovery_loader.py` & `nose2-0.9.2/nose2/tests/functional/test_eggdiscovery_loader.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/functional/test_layers_plugin.py` & `nose2-0.9.2/nose2/tests/functional/test_layers_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_outcomes_plugin.py` & `nose2-0.9.2/nose2/tests/unit/test_outcomes_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_junitxml.py` & `nose2-0.9.2/nose2/tests/unit/test_junitxml.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_plugin_api.py` & `nose2-0.9.2/nose2/tests/unit/test_plugin_api.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_decorators.py` & `nose2-0.9.2/nose2/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_testcase_loader.py` & `nose2-0.9.2/nose2/tests/unit/test_testcase_loader.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_collector.py` & `nose2-0.9.2/nose2/tests/unit/test_collector.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_attrib_plugin.py` & `nose2-0.9.2/nose2/tests/unit/test_attrib_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_testclass_loader.py` & `nose2-0.9.2/nose2/tests/unit/test_testclass_loader.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_loader.py` & `nose2-0.9.2/nose2/tests/unit/test_loader.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_debugger_plugin.py` & `nose2-0.9.2/nose2/tests/unit/test_debugger_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_failfast.py` & `nose2-0.9.2/nose2/tests/unit/test_failfast.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_functions_loader.py` & `nose2-0.9.2/nose2/tests/unit/test_functions_loader.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_logcapture_plugin.py` & `nose2-0.9.2/nose2/tests/unit/test_logcapture_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_prof_plugin.py` & `nose2-0.9.2/nose2/tests/unit/test_prof_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_mp_plugin.py` & `nose2-0.9.2/nose2/tests/unit/test_mp_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_printhooks_plugin.py` & `nose2-0.9.2/nose2/tests/unit/test_printhooks_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_generators_plugin.py` & `nose2-0.9.2/nose2/tests/unit/test_generators_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_testid_plugin.py` & `nose2-0.9.2/nose2/tests/unit/test_testid_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_params_plugin.py` & `nose2-0.9.2/nose2/tests/unit/test_params_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_buffer_plugin.py` & `nose2-0.9.2/nose2/tests/unit/test_buffer_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_dundertest_plugin.py` & `nose2-0.9.2/nose2/tests/unit/test_dundertest_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_result.py` & `nose2-0.9.2/nose2/tests/unit/test_result.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_doctest_plugin.py` & `nose2-0.9.2/nose2/tests/unit/test_doctest_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_config.py` & `nose2-0.9.2/nose2/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/unit/test_layers_plugin.py` & `nose2-0.9.2/nose2/tests/unit/test_layers_plugin.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tests/_common.py` & `nose2-0.9.2/nose2/tests/_common.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/collector.py` & `nose2-0.9.2/nose2/collector.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/config.py` & `nose2-0.9.2/nose2/config.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/result.py` & `nose2-0.9.2/nose2/result.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tools/params.py` & `nose2-0.9.2/nose2/tools/params.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tools/decorators.py` & `nose2-0.9.2/nose2/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/tools/such.py` & `nose2-0.9.2/nose2/tools/such.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2/events.py` & `nose2-0.9.2/nose2/events.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/tox.ini` & `nose2-0.9.2/tox.ini`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/PKG-INFO` & `nose2-0.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nose2
-Version: 0.9.1
+Version: 0.9.2
 Summary: unittest2 with plugins, the succesor to nose
 Home-page: https://github.com/nose-devs/nose2
 Author: Jason Pellerin
 Author-email: jpellerin+nose@gmail.com
 License: UNKNOWN
 Description: .. image:: https://travis-ci.org/nose-devs/nose2.svg?branch=master
             :target: https://travis-ci.org/nose-devs/nose2
@@ -14,15 +14,14 @@
             :target: https://coveralls.io/github/nose-devs/nose2?branch=master
             :alt: Coverage Status
         
         .. image:: https://img.shields.io/pypi/v/nose2.svg
             :target: https://pypi.org/project/nose2/
             :alt: Latest PyPI version
         
-         [![Google group : SSFAM News](https://img.shields.io/badge/Google%20Group-SSFAM%20News-blue.svg)](https://groups.google.com/forum/#!forum/ssfam-news)
         .. image:: https://img.shields.io/badge/Mailing%20list-discuss%40nose2.io-blue.svg
             :target: https://groups.google.com/a/nose2.io/forum/#!forum/discuss
             :alt: Join discuss@nose2.io
         
         Welcome to nose2
         ================
         
@@ -164,9 +163,9 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
-Provides-Extra: doc
 Provides-Extra: coverage_plugin
+Provides-Extra: doc
```

### Comparing `nose2-0.9.1/license.txt` & `nose2-0.9.2/license.txt`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/setup.py` & `nose2-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `nose2-0.9.1/nose2.egg-info/SOURCES.txt` & `nose2-0.9.2/nose2.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,16 @@
 nose2/tests/functional/support/scenario/junitxml/empty_properties/test_junitxml_empty_properties.py
 nose2/tests/functional/support/scenario/junitxml/empty_properties/unittest.cfg
 nose2/tests/functional/support/scenario/junitxml/fail_to_write/test_junitxml_fail_to_write.py
 nose2/tests/functional/support/scenario/junitxml/fail_to_write/unittest.cfg
 nose2/tests/functional/support/scenario/junitxml/happyday/test_junitxml_happyday.py
 nose2/tests/functional/support/scenario/junitxml/missing_properties/test_junitxml_missing_properties.py
 nose2/tests/functional/support/scenario/junitxml/missing_properties/unittest.cfg
+nose2/tests/functional/support/scenario/junitxml/non_default_path/test_junitxml_non_default_path.py
+nose2/tests/functional/support/scenario/junitxml/non_default_path/unittest.cfg
 nose2/tests/functional/support/scenario/junitxml/skip_reason/test_junitxml_skip_reason.py
 nose2/tests/functional/support/scenario/junitxml/skip_reason/unittest.cfg
 nose2/tests/functional/support/scenario/junitxml/with_properties/test_junitxml_with_properties.py
 nose2/tests/functional/support/scenario/junitxml/with_properties/unittest.cfg
 nose2/tests/functional/support/scenario/layers/test_layers.py
 nose2/tests/functional/support/scenario/layers_and_attributes/test_layers_and_attributes.py
 nose2/tests/functional/support/scenario/layers_and_non_layers/__init__.py
```

### Comparing `nose2-0.9.1/nose2.egg-info/PKG-INFO` & `nose2-0.9.2/nose2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nose2
-Version: 0.9.1
+Version: 0.9.2
 Summary: unittest2 with plugins, the succesor to nose
 Home-page: https://github.com/nose-devs/nose2
 Author: Jason Pellerin
 Author-email: jpellerin+nose@gmail.com
 License: UNKNOWN
 Description: .. image:: https://travis-ci.org/nose-devs/nose2.svg?branch=master
             :target: https://travis-ci.org/nose-devs/nose2
@@ -14,15 +14,14 @@
             :target: https://coveralls.io/github/nose-devs/nose2?branch=master
             :alt: Coverage Status
         
         .. image:: https://img.shields.io/pypi/v/nose2.svg
             :target: https://pypi.org/project/nose2/
             :alt: Latest PyPI version
         
-         [![Google group : SSFAM News](https://img.shields.io/badge/Google%20Group-SSFAM%20News-blue.svg)](https://groups.google.com/forum/#!forum/ssfam-news)
         .. image:: https://img.shields.io/badge/Mailing%20list-discuss%40nose2.io-blue.svg
             :target: https://groups.google.com/a/nose2.io/forum/#!forum/discuss
             :alt: Join discuss@nose2.io
         
         Welcome to nose2
         ================
         
@@ -164,9 +163,9 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
-Provides-Extra: doc
 Provides-Extra: coverage_plugin
+Provides-Extra: doc
```


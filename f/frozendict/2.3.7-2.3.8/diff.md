# Comparing `tmp/frozendict-2.3.7.tar.gz` & `tmp/frozendict-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frozendict-2.3.7.tar", last modified: Sun Apr  9 19:35:25 2023, max compression
+gzip compressed data, was "frozendict-2.3.8.tar", last modified: Sat Apr 29 20:10:26 2023, max compression
```

## Comparing `frozendict-2.3.7.tar` & `frozendict-2.3.8.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.722411 frozendict-2.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-09 19:35:17.000000 frozendict-2.3.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-09 19:35:17.000000 frozendict-2.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-04-09 19:35:25.722411 frozendict-2.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19173 2023-04-09 19:35:17.000000 frozendict-2.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:35:25.722411 frozendict-2.3.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5749 2023-04-09 19:35:17.000000 frozendict-2.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.702409 frozendict-2.3.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.706410 frozendict-2.3.7/src/frozendict/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.706410 frozendict-2.3.7/src/frozendict/c_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.706410 frozendict-2.3.7/src/frozendict/c_src/3_10/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.706410 frozendict-2.3.7/src/frozendict/c_src/3_10/Include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_10/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (123)    57234 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (123)   152447 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (123)    60336 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/frozendictobject.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_6/Include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_6/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (123)    63009 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (123)   135061 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (123)    58155 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/frozendictobject.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_7/Include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_7/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (123)    61834 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (123)   132228 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (123)    58478 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/frozendictobject.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_8/Include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_8/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (123)    58062 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (123)   141374 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (123)    60418 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/frozendictobject.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_9/Include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_9/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.718410 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.718410 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (123)    58099 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (123)   145558 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.718410 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (123)    60489 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/frozendictobject.c
--rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/frozendict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/monkeypatch.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.706410 frozendict-2.3.7/src/frozendict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-04-09 19:35:25.000000 frozendict-2.3.7/src/frozendict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-09 19:35:25.000000 frozendict-2.3.7/src/frozendict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:35:25.000000 frozendict-2.3.7/src/frozendict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 19:35:25.000000 frozendict-2.3.7/src/frozendict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.722411 frozendict-2.3.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7524 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/bench.py
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13297 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/frozendict_only.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/subclass_only.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/test_frozendict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/test_frozendict_subclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/typed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.562897 frozendict-2.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-29 20:10:14.000000 frozendict-2.3.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-29 20:10:14.000000 frozendict-2.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-04-29 20:10:26.562897 frozendict-2.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19173 2023-04-29 20:10:14.000000 frozendict-2.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-29 20:10:14.000000 frozendict-2.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 20:10:26.562897 frozendict-2.3.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5747 2023-04-29 20:10:14.000000 frozendict-2.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.550897 frozendict-2.3.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.550897 frozendict-2.3.8/src/frozendict/c_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_10/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_10/Include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_10/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_10/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_10/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57234 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (123)   152447 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (123)    60336 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_10/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_6/Include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_6/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_6/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_6/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    63009 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (123)   135061 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (123)    58155 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_6/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict/c_src/3_7/Include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_7/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_7/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_7/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    61834 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (123)   132228 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (123)    58478 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_7/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_8/Include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_8/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_8/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_8/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    58062 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (123)   141374 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (123)    60418 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_8/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_9/Include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_9/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_9/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_9/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    58099 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (123)   145558 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.558897 frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (123)    60489 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/c_src/3_9/frozendictobject.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-29 20:10:14.000000 frozendict-2.3.8/src/frozendict/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.554897 frozendict-2.3.8/src/frozendict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-04-29 20:10:26.000000 frozendict-2.3.8/src/frozendict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-29 20:10:26.000000 frozendict-2.3.8/src/frozendict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 20:10:26.000000 frozendict-2.3.8/src/frozendict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 20:10:26.000000 frozendict-2.3.8/src/frozendict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:26.562897 frozendict-2.3.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 20:10:14.000000 frozendict-2.3.8/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-29 20:10:14.000000 frozendict-2.3.8/test/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7524 2023-04-29 20:10:14.000000 frozendict-2.3.8/test/bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-04-29 20:10:14.000000 frozendict-2.3.8/test/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13297 2023-04-29 20:10:14.000000 frozendict-2.3.8/test/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-29 20:10:14.000000 frozendict-2.3.8/test/frozendict_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-29 20:10:14.000000 frozendict-2.3.8/test/subclass_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-29 20:10:14.000000 frozendict-2.3.8/test/test_frozendict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-29 20:10:14.000000 frozendict-2.3.8/test/test_frozendict_subclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-29 20:10:14.000000 frozendict-2.3.8/test/typed.py
```

### Comparing `frozendict-2.3.7/LICENSE.txt` & `frozendict-2.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/PKG-INFO` & `frozendict-2.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frozendict
-Version: 2.3.7
+Version: 2.3.8
 Summary: A simple immutable dictionary
 Home-page: https://github.com/Marco-Sulla/python-frozendict
 Author: Marco Sulla
 Author-email: marcosullaroma@gmail.com
 License: LGPL v3
 Project-URL: Bug Reports, https://github.com/Marco-Sulla/python-frozendict/issues
 Project-URL: Source, https://github.com/Marco-Sulla/python-frozendict
```

### Comparing `frozendict-2.3.7/README.md` & `frozendict-2.3.8/README.md`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/setup.py` & `frozendict-2.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from os import environ
 
 name = "frozendict"
 module1_name = "frozendict"
 readme_filename = "README.md"
 version_filename = "version.py"
 py_typed_filename = "py.typed"
-mypy_filename = "frozendict.pyi"
+mypy_filename = "__init__.pyi"
 main_url = "https://github.com/Marco-Sulla/python-frozendict"
 bug_url = "https://github.com/Marco-Sulla/python-frozendict/issues"
 author = "Marco Sulla"
 author_email = "marcosullaroma@gmail.com"
 license  = "LGPL v3"
 license_files = "LICENSE.txt"
 description = "A simple immutable dictionary"
```

### Comparing `frozendict-2.3.7/src/frozendict/__init__.py` & `frozendict-2.3.8/src/frozendict/__init__.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_10/Include/frozendictobject.h` & `frozendict-2.3.8/src/frozendict/c_src/3_10/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/dict-common.h` & `frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject.c` & `frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject_original.c` & `frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/other.c` & `frozendict-2.3.8/src/frozendict/c_src/3_10/cpython_src/other.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_10/frozendictobject.c` & `frozendict-2.3.8/src/frozendict/c_src/3_10/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_6/Include/frozendictobject.h` & `frozendict-2.3.8/src/frozendict/c_src/3_6/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/dict-common.h` & `frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject.c` & `frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject_original.c` & `frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/other.c` & `frozendict-2.3.8/src/frozendict/c_src/3_6/cpython_src/other.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_6/frozendictobject.c` & `frozendict-2.3.8/src/frozendict/c_src/3_6/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_7/Include/frozendictobject.h` & `frozendict-2.3.8/src/frozendict/c_src/3_7/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/dict-common.h` & `frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject.c` & `frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject_original.c` & `frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.3.8/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_7/frozendictobject.c` & `frozendict-2.3.8/src/frozendict/c_src/3_7/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_8/Include/frozendictobject.h` & `frozendict-2.3.8/src/frozendict/c_src/3_8/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/dict-common.h` & `frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject.c` & `frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject_original.c` & `frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/other.c` & `frozendict-2.3.8/src/frozendict/c_src/3_8/cpython_src/other.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_8/frozendictobject.c` & `frozendict-2.3.8/src/frozendict/c_src/3_8/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_9/Include/frozendictobject.h` & `frozendict-2.3.8/src/frozendict/c_src/3_9/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/dict-common.h` & `frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject.c` & `frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject_original.c` & `frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/other.c` & `frozendict-2.3.8/src/frozendict/c_src/3_9/cpython_src/other.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/c_src/3_9/frozendictobject.c` & `frozendict-2.3.8/src/frozendict/c_src/3_9/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/core.py` & `frozendict-2.3.8/src/frozendict/core.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict/monkeypatch.py` & `frozendict-2.3.8/src/frozendict/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/src/frozendict.egg-info/PKG-INFO` & `frozendict-2.3.8/src/frozendict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frozendict
-Version: 2.3.7
+Version: 2.3.8
 Summary: A simple immutable dictionary
 Home-page: https://github.com/Marco-Sulla/python-frozendict
 Author: Marco Sulla
 Author-email: marcosullaroma@gmail.com
 License: LGPL v3
 Project-URL: Bug Reports, https://github.com/Marco-Sulla/python-frozendict/issues
 Project-URL: Source, https://github.com/Marco-Sulla/python-frozendict
```

### Comparing `frozendict-2.3.7/src/frozendict.egg-info/SOURCES.txt` & `frozendict-2.3.8/src/frozendict.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 src/frozendict/__init__.py
+src/frozendict/__init__.pyi
 src/frozendict/core.py
-src/frozendict/frozendict.pyi
 src/frozendict/monkeypatch.py
 src/frozendict/py.typed
 src/frozendict/version.py
 src/frozendict.egg-info/PKG-INFO
 src/frozendict.egg-info/SOURCES.txt
 src/frozendict.egg-info/dependency_links.txt
 src/frozendict.egg-info/top_level.txt
```

### Comparing `frozendict-2.3.7/test/base.py` & `frozendict-2.3.8/test/base.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/test/bench.py` & `frozendict-2.3.8/test/bench.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/test/common.py` & `frozendict-2.3.8/test/common.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/test/debug.py` & `frozendict-2.3.8/test/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
 @trace(iterations = 200, mult = 1.5)
 def func_3():
     pickle.loads(pickle.dumps(iter(fd_1.items())))
 
 functions.append(func_3)
 
-@trace(iterations = 300, mult = 1.4)
+@trace(iterations = 350, mult = 1.4)
 def func_4():
     pickle.loads(pickle.dumps(iter(fd_1.values())))
 
 functions.append(func_4)
 
 @trace()
 def func_5():
```

### Comparing `frozendict-2.3.7/test/frozendict_only.py` & `frozendict-2.3.8/test/frozendict_only.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/test/subclass_only.py` & `frozendict-2.3.8/test/subclass_only.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/test/test_frozendict.py` & `frozendict-2.3.8/test/test_frozendict.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.7/test/test_frozendict_subclass.py` & `frozendict-2.3.8/test/test_frozendict_subclass.py`

 * *Files identical despite different names*


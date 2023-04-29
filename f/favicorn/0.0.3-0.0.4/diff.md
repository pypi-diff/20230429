# Comparing `tmp/favicorn-0.0.3.tar.gz` & `tmp/favicorn-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "favicorn-0.0.3.tar", last modified: Sun Mar 26 11:55:21 2023, max compression
+gzip compressed data, was "favicorn-0.0.4.tar", last modified: Sat Apr 29 10:02:31 2023, max compression
```

## Comparing `favicorn-0.0.3.tar` & `favicorn-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 11:55:21.172548 favicorn-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-26 11:55:21.172548 favicorn-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-26 11:54:51.000000 favicorn-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 11:55:21.172548 favicorn-0.0.3/favicorn/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-26 11:54:51.000000 favicorn-0.0.3/favicorn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-03-26 11:54:51.000000 favicorn-0.0.3/favicorn/asgi_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-26 11:54:51.000000 favicorn-0.0.3/favicorn/global_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-03-26 11:54:51.000000 favicorn-0.0.3/favicorn/http_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-26 11:54:51.000000 favicorn-0.0.3/favicorn/iglobal_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-26 11:54:51.000000 favicorn-0.0.3/favicorn/iprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-26 11:54:51.000000 favicorn-0.0.3/favicorn/isocket_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 11:54:51.000000 favicorn-0.0.3/favicorn/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-03-26 11:54:51.000000 favicorn-0.0.3/favicorn/request_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-03-26 11:54:51.000000 favicorn-0.0.3/favicorn/response_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-26 11:54:51.000000 favicorn-0.0.3/favicorn/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-03-26 11:54:51.000000 favicorn-0.0.3/favicorn/socket_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-26 11:54:51.000000 favicorn-0.0.3/favicorn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 11:55:21.172548 favicorn-0.0.3/favicorn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-26 11:55:21.000000 favicorn-0.0.3/favicorn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-26 11:55:21.000000 favicorn-0.0.3/favicorn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 11:55:21.000000 favicorn-0.0.3/favicorn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-26 11:55:21.000000 favicorn-0.0.3/favicorn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-26 11:55:21.000000 favicorn-0.0.3/favicorn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-26 11:54:51.000000 favicorn-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 11:55:21.172548 favicorn-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-26 11:54:51.000000 favicorn-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:02:31.743806 favicorn-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-29 10:02:31.743806 favicorn-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 10:02:02.000000 favicorn-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:02:31.743806 favicorn-0.0.4/favicorn/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/iconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/isocket_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:02:31.743806 favicorn-0.0.4/favicorn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-29 10:02:31.000000 favicorn-0.0.4/favicorn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-29 10:02:31.000000 favicorn-0.0.4/favicorn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:02:31.000000 favicorn-0.0.4/favicorn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-29 10:02:31.000000 favicorn-0.0.4/favicorn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 10:02:31.000000 favicorn-0.0.4/favicorn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-29 10:02:02.000000 favicorn-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 10:02:31.743806 favicorn-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-29 10:02:02.000000 favicorn-0.0.4/setup.py
```

### Comparing `favicorn-0.0.3/setup.py` & `favicorn-0.0.4/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/vtece4564-websockets-11.0.2.post1.tar.gz` & `tmp/vtece4564-websockets-11.0.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtece4564-websockets-11.0.2.post1.tar", last modified: Sat Apr 29 14:36:55 2023, max compression
+gzip compressed data, was "vtece4564-websockets-11.0.2.post2.tar", last modified: Sat Apr 29 14:57:54 2023, max compression
```

## Comparing `vtece4564-websockets-11.0.2.post1.tar` & `vtece4564-websockets-11.0.2.post2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:36:55.733561 vtece4564-websockets-11.0.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-29 14:36:55.733561 vtece4564-websockets-11.0.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 14:36:55.733561 vtece4564-websockets-11.0.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:36:55.729561 vtece4564-websockets-11.0.2.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:36:55.729561 vtece4564-websockets-11.0.2.post1/src/vtece4564_websockets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-29 14:36:55.000000 vtece4564-websockets-11.0.2.post1/src/vtece4564_websockets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-29 14:36:55.000000 vtece4564-websockets-11.0.2.post1/src/vtece4564_websockets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 14:36:55.000000 vtece4564-websockets-11.0.2.post1/src/vtece4564_websockets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 14:36:55.000000 vtece4564-websockets-11.0.2.post1/src/vtece4564_websockets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:36:55.733561 vtece4564-websockets-11.0.2.post1/src/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:36:55.733561 vtece4564-websockets-11.0.2.post1/src/websockets/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/extensions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24782 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/extensions/permessage_deflate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    12565 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/http11.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:36:55.733561 vtece4564-websockets-11.0.2.post1/src/websockets/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/legacy/async_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/legacy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    26123 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/legacy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/legacy/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/legacy/framing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/legacy/handshake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/legacy/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    62936 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/legacy/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    44803 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/legacy/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    23822 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/speedups.c
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:36:55.733561 vtece4564-websockets-11.0.2.post1/src/websockets/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/sync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29303 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/sync/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/sync/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    18290 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/sync/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/sync/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-29 14:36:54.000000 vtece4564-websockets-11.0.2.post1/src/websockets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:54.839581 vtece4564-websockets-11.0.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-29 14:57:54.839581 vtece4564-websockets-11.0.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 14:57:54.839581 vtece4564-websockets-11.0.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:54.827581 vtece4564-websockets-11.0.2.post2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:54.831581 vtece4564-websockets-11.0.2.post2/src/vtece4564_websockets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-29 14:57:54.000000 vtece4564-websockets-11.0.2.post2/src/vtece4564_websockets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-29 14:57:54.000000 vtece4564-websockets-11.0.2.post2/src/vtece4564_websockets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 14:57:54.000000 vtece4564-websockets-11.0.2.post2/src/vtece4564_websockets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 14:57:54.000000 vtece4564-websockets-11.0.2.post2/src/vtece4564_websockets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:54.835581 vtece4564-websockets-11.0.2.post2/src/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:54.835581 vtece4564-websockets-11.0.2.post2/src/websockets/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/extensions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24782 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/extensions/permessage_deflate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12565 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/http11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:54.835581 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/async_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26123 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/framing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/handshake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62936 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44803 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/legacy/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23822 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/speedups.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:54.839581 vtece4564-websockets-11.0.2.post2/src/websockets/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29303 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/sync/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/sync/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18290 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/sync/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/sync/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-29 14:57:53.000000 vtece4564-websockets-11.0.2.post2/src/websockets/version.py
```

### Comparing `vtece4564-websockets-11.0.2.post1/LICENSE` & `vtece4564-websockets-11.0.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/PKG-INFO` & `vtece4564-websockets-11.0.2.post2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 Metadata-Version: 2.1
 Name: vtece4564-websockets
-Version: 11.0.2.post1
+Version: 11.0.2.post2
 Summary: An implementation of the WebSocket Protocol (RFC 6455 & 7692)
 Author-email: Aymeric Augustin <aymeric.augustin@m4x.org>
 License: BSD-3-Clause
-Project-URL: Homepage, https://github.com/python-websockets/websockets
-Project-URL: Changelog, https://websockets.readthedocs.io/en/stable/project/changelog.html
+Project-URL: Homepage, https://github.com/ceharris/python-websockets
 Project-URL: Documentation, https://websockets.readthedocs.io/
-Project-URL: Funding, https://tidelift.com/subscription/pkg/pypi-websockets?utm_source=pypi-websockets&utm_medium=referral&utm_campaign=readme
-Project-URL: Tracker, https://github.com/python-websockets/websockets/issues
 Keywords: WebSocket
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `vtece4564-websockets-11.0.2.post1/README.rst` & `vtece4564-websockets-11.0.2.post2/README.rst`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/pyproject.toml` & `vtece4564-websockets-11.0.2.post2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,22 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 readme = "README.md"
-version = "11.0.2.post1"
+version = "11.0.2.post2"
 
 [project.urls]
-Homepage = "https://github.com/python-websockets/websockets"
-Changelog = "https://websockets.readthedocs.io/en/stable/project/changelog.html"
+Homepage = "https://github.com/ceharris/python-websockets"
+#Changelog = "https://websockets.readthedocs.io/en/stable/project/changelog.html"
 Documentation = "https://websockets.readthedocs.io/"
-Funding = "https://tidelift.com/subscription/pkg/pypi-websockets?utm_source=pypi-websockets&utm_medium=referral&utm_campaign=readme"
-Tracker = "https://github.com/python-websockets/websockets/issues"
+#Funding = "https://tidelift.com/subscription/pkg/pypi-websockets?utm_source=pypi-websockets&utm_medium=referral&utm_campaign=readme"
+#Tracker = "https://github.com/python-websockets/websockets/issues"
 
 # On a macOS runner, build Intel, Universal, and Apple Silicon wheels.
 [tool.cibuildwheel.macos]
 archs = ["x86_64", "universal2", "arm64"]
 
 # On an Linux Intel runner with QEMU installed, build Intel and ARM wheels.
 [tool.cibuildwheel.linux]
```

### Comparing `vtece4564-websockets-11.0.2.post1/setup.py` & `vtece4564-websockets-11.0.2.post2/setup.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/vtece4564_websockets.egg-info/PKG-INFO` & `vtece4564-websockets-11.0.2.post2/src/vtece4564_websockets.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 Metadata-Version: 2.1
 Name: vtece4564-websockets
-Version: 11.0.2.post1
+Version: 11.0.2.post2
 Summary: An implementation of the WebSocket Protocol (RFC 6455 & 7692)
 Author-email: Aymeric Augustin <aymeric.augustin@m4x.org>
 License: BSD-3-Clause
-Project-URL: Homepage, https://github.com/python-websockets/websockets
-Project-URL: Changelog, https://websockets.readthedocs.io/en/stable/project/changelog.html
+Project-URL: Homepage, https://github.com/ceharris/python-websockets
 Project-URL: Documentation, https://websockets.readthedocs.io/
-Project-URL: Funding, https://tidelift.com/subscription/pkg/pypi-websockets?utm_source=pypi-websockets&utm_medium=referral&utm_campaign=readme
-Project-URL: Tracker, https://github.com/python-websockets/websockets/issues
 Keywords: WebSocket
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `vtece4564-websockets-11.0.2.post1/src/vtece4564_websockets.egg-info/SOURCES.txt` & `vtece4564-websockets-11.0.2.post2/src/vtece4564_websockets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/__init__.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/__main__.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/__main__.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/client.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/client.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/datastructures.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/datastructures.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/exceptions.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/exceptions.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/extensions/base.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/extensions/base.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/extensions/permessage_deflate.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/extensions/permessage_deflate.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/frames.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/frames.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/headers.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/headers.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/http.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/http.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/http11.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/http11.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/imports.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/imports.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/legacy/async_timeout.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/async_timeout.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/legacy/auth.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/auth.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/legacy/client.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/client.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/legacy/framing.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/framing.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/legacy/handshake.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/handshake.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/legacy/http.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/http.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/legacy/protocol.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/protocol.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/legacy/server.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/legacy/server.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/protocol.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/protocol.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/server.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/server.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/speedups.c` & `vtece4564-websockets-11.0.2.post2/src/websockets/speedups.c`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/streams.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/streams.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/sync/client.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/sync/client.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/sync/connection.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/sync/connection.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/sync/messages.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/sync/messages.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/sync/server.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/sync/server.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/sync/utils.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/sync/utils.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/typing.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/typing.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/uri.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/uri.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/utils.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/utils.py`

 * *Files identical despite different names*

### Comparing `vtece4564-websockets-11.0.2.post1/src/websockets/version.py` & `vtece4564-websockets-11.0.2.post2/src/websockets/version.py`

 * *Files identical despite different names*


# Comparing `tmp/crosscompute-0.9.4.2.tar.gz` & `tmp/crosscompute-0.9.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosscompute-0.9.4.2.tar", last modified: Wed Apr 26 00:25:44 2023, max compression
+gzip compressed data, was "crosscompute-0.9.4.3.tar", last modified: Sat Apr 29 00:54:00 2023, max compression
```

## Comparing `crosscompute-0.9.4.2.tar` & `crosscompute-0.9.4.3.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.837256 crosscompute-0.9.4.2/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/LICENSE.md
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4987 2023-04-26 00:25:44.837256 crosscompute-0.9.4.2/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3703 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.820255 crosscompute-0.9.4.2/crosscompute/
--rw-r--r--   0 rhh       (1000) rhh       (1000)       22 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/__init__.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       38 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/crosscompute/__main__.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.830255 crosscompute-0.9.4.2/crosscompute/assets/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1286 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/automation.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      910 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/base.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      230 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/button-panel.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      183 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/checkbox-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      579 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/checkbox-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      628 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/checkbox-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      109 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/checkbox-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)    13294 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/configuration.yml
--rw-r--r--   0 rhh       (1000) rhh       (1000)      224 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/default.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)       48 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/embedded.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)    22382 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/favicon.ico
--rw-r--r--   0 rhh       (1000) rhh       (1000)      765 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/file-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      165 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/file-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/file-input.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      578 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/flex.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)      180 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/frame-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/frame-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/image-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/image-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      156 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/json-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-04-25 22:48:18.000000 crosscompute-0.9.4.2/crosscompute/assets/json-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      149 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/link-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/link-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2566 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/live.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      301 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/markdown-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      142 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/markdown-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/pdf-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      137 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/pdf-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)       64 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/pdf.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)       53 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/printed.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)       96 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/radio-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      575 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/radio-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      594 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/radio-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/radio-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      285 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/root.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3271 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/step-body.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      874 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/step.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)       65 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/string-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      432 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/string-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      369 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/string-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      122 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/string-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1095 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/table-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/table-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      159 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/text-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/text-input.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      109 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/assets/text-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/assets/text-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2886 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/constants.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     5072 2023-04-01 20:58:16.000000 crosscompute-0.9.4.2/crosscompute/dependencies.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1055 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/exceptions.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.831256 crosscompute-0.9.4.2/crosscompute/macros/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/crosscompute/macros/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      717 2023-04-05 23:51:33.000000 crosscompute-0.9.4.2/crosscompute/macros/disk.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1530 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/macros/iterable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1088 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/macros/log.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      597 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/crosscompute/macros/package.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1349 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/macros/security.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.832255 crosscompute-0.9.4.2/crosscompute/routers/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/routers/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     7020 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routers/automation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1142 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routers/file.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3286 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routers/root.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1240 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routers/stream.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      523 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/routers/token.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.835255 crosscompute-0.9.4.2/crosscompute/routines/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/crosscompute/routines/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3195 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/asset.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3457 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/routines/authorization.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4877 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/automation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3537 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/routines/batch.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    42043 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/configuration.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     9315 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/database.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      914 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/crosscompute/routines/interface.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1404 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/crosscompute/routines/log.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1523 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/mutation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     6222 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/printer.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     6967 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/server.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     7181 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/step.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      605 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/uri.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    30285 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/routines/variable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    28255 2023-04-26 00:24:10.000000 crosscompute-0.9.4.2/crosscompute/routines/work.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.836256 crosscompute-0.9.4.2/crosscompute/scripts/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/crosscompute/scripts/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3866 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/scripts/configure.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3829 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/scripts/launch.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1123 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/scripts/print.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1721 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/scripts/run.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4065 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/scripts/serve.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1338 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/crosscompute/settings.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.821255 crosscompute-0.9.4.2/crosscompute.egg-info/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4987 2023-04-26 00:25:44.000000 crosscompute-0.9.4.2/crosscompute.egg-info/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3437 2023-04-26 00:25:44.000000 crosscompute-0.9.4.2/crosscompute.egg-info/SOURCES.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-04-26 00:25:44.000000 crosscompute-0.9.4.2/crosscompute.egg-info/dependency_links.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)      831 2023-04-26 00:25:44.000000 crosscompute-0.9.4.2/crosscompute.egg-info/entry_points.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)      436 2023-04-26 00:25:44.000000 crosscompute-0.9.4.2/crosscompute.egg-info/requires.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       13 2023-04-26 00:25:44.000000 crosscompute-0.9.4.2/crosscompute.egg-info/top_level.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2022-08-22 13:00:05.000000 crosscompute-0.9.4.2/crosscompute.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3273 2023-04-26 00:25:44.839256 crosscompute-0.9.4.2/setup.cfg
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       39 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/setup.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 00:25:44.837256 crosscompute-0.9.4.2/tests/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      168 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/tests/test_macros_iterable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      428 2023-02-18 06:45:42.000000 crosscompute-0.9.4.2/tests/test_macros_security.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3759 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/tests/test_routines_configuration.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)     2285 2022-08-15 04:38:47.000000 crosscompute-0.9.4.2/tests/test_routines_variable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      656 2023-04-25 22:48:21.000000 crosscompute-0.9.4.2/tests/test_routines_work.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.707458 crosscompute-0.9.4.3/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/LICENSE.md
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4987 2023-04-29 00:54:00.707458 crosscompute-0.9.4.3/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3703 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.695458 crosscompute-0.9.4.3/crosscompute/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       22 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/__init__.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)       38 2022-01-21 18:22:22.000000 crosscompute-0.9.4.3/crosscompute/__main__.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.701458 crosscompute-0.9.4.3/crosscompute/assets/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1292 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/automation.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      910 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/base.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      230 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/button-panel.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      183 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/checkbox-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      579 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/checkbox-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      628 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/checkbox-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      109 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/checkbox-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    13385 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/configuration.yml
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      224 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/default.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       48 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/embedded.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    22382 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/favicon.ico
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      765 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/file-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      165 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/file-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/file-input.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      631 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/flex.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      180 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/frame-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/frame-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/image-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/image-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      156 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/json-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-02-28 18:19:08.000000 crosscompute-0.9.4.3/crosscompute/assets/json-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      149 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/link-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/link-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2566 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/assets/live.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      301 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/markdown-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      142 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/markdown-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/pdf-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      137 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/assets/pdf-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       64 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/pdf.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       53 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/printed.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       96 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/radio-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      575 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/radio-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      594 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/radio-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/radio-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      366 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/root.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3271 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/step-body.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      874 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/step.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       65 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/string-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      432 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/string-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      369 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/string-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      122 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/string-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1095 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/table-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/table-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      159 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/text-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/text-input.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      109 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/text-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/text-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2886 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/constants.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     5072 2023-03-30 19:34:16.000000 crosscompute-0.9.4.3/crosscompute/dependencies.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1055 2022-12-12 19:44:41.000000 crosscompute-0.9.4.3/crosscompute/exceptions.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.702458 crosscompute-0.9.4.3/crosscompute/macros/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-01-21 18:22:22.000000 crosscompute-0.9.4.3/crosscompute/macros/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      717 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/macros/disk.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1530 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/macros/iterable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1088 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/macros/log.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      597 2022-03-14 16:37:10.000000 crosscompute-0.9.4.3/crosscompute/macros/package.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1349 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/macros/security.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.703458 crosscompute-0.9.4.3/crosscompute/routers/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/routers/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     7021 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routers/automation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1142 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routers/file.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3286 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/routers/root.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1240 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/routers/stream.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      523 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/routers/token.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.705458 crosscompute-0.9.4.3/crosscompute/routines/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-01-21 18:22:22.000000 crosscompute-0.9.4.3/crosscompute/routines/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3195 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/asset.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3457 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/routines/authorization.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4877 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/automation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3537 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/routines/batch.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    41926 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/configuration.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     9409 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/database.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      914 2022-07-01 15:18:27.000000 crosscompute-0.9.4.3/crosscompute/routines/interface.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1404 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/routines/log.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1523 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/routines/mutation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     6222 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/printer.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     6967 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/server.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     7181 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/step.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      605 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/routines/uri.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    30285 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/variable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    28209 2023-04-29 00:50:49.000000 crosscompute-0.9.4.3/crosscompute/routines/work.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.706458 crosscompute-0.9.4.3/crosscompute/scripts/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-01-21 18:22:22.000000 crosscompute-0.9.4.3/crosscompute/scripts/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3866 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/scripts/configure.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3829 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/scripts/launch.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1123 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/scripts/print.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1721 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/scripts/run.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4065 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/scripts/serve.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1338 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/settings.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.696458 crosscompute-0.9.4.3/crosscompute.egg-info/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)     4987 2023-04-29 00:54:00.000000 crosscompute-0.9.4.3/crosscompute.egg-info/PKG-INFO
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)     3437 2023-04-29 00:54:00.000000 crosscompute-0.9.4.3/crosscompute.egg-info/SOURCES.txt
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        1 2023-04-29 00:54:00.000000 crosscompute-0.9.4.3/crosscompute.egg-info/dependency_links.txt
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      831 2023-04-29 00:54:00.000000 crosscompute-0.9.4.3/crosscompute.egg-info/entry_points.txt
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      436 2023-04-29 00:54:00.000000 crosscompute-0.9.4.3/crosscompute.egg-info/requires.txt
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)       13 2023-04-29 00:54:00.000000 crosscompute-0.9.4.3/crosscompute.egg-info/top_level.txt
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        1 2022-01-21 22:12:56.000000 crosscompute-0.9.4.3/crosscompute.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3273 2023-04-29 00:54:00.708458 crosscompute-0.9.4.3/setup.cfg
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)       39 2022-01-21 18:22:22.000000 crosscompute-0.9.4.3/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.707458 crosscompute-0.9.4.3/tests/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      168 2022-01-21 18:22:22.000000 crosscompute-0.9.4.3/tests/test_macros_iterable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      428 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/tests/test_macros_security.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3759 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/tests/test_routines_configuration.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)     2285 2022-05-17 17:13:01.000000 crosscompute-0.9.4.3/tests/test_routines_variable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      656 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/tests/test_routines_work.py
```

### Comparing `crosscompute-0.9.4.2/LICENSE.md` & `crosscompute-0.9.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/PKG-INFO` & `crosscompute-0.9.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute
-Version: 0.9.4.2
+Version: 0.9.4.3
 Summary: Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute/issues
 Project-URL: Documentation, https://github.com/crosscompute/crosscompute-docs
```

### Comparing `crosscompute-0.9.4.2/README.md` & `crosscompute-0.9.4.3/README.md`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/assets/automation.html` & `crosscompute-0.9.4.3/crosscompute/assets/automation.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends live_template_path %}
 
 {% block head_html %}
 {{ super() -}}
-<meta name="title" property="og:title" content="{{ name }}" />
+<meta name="title" property="og:title" content="{{ title_text }}" />
 <meta name="description" property="og:description" content="{{ description }}">
 <meta name="image" property="og:image" content="{{ host_uri }}{{ root_uri }}/favicon.ico" />
 <meta property="og:url" content="{{ host_uri }}{{ root_uri }}{{ uri }}" />
 <meta name="twitter:card" content="summary">
 {% endblock %}
 
 {% block header_html %}
```

### Comparing `crosscompute-0.9.4.2/crosscompute/assets/base.html` & `crosscompute-0.9.4.3/crosscompute/assets/base.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/assets/checkbox-input.html` & `crosscompute-0.9.4.3/crosscompute/assets/checkbox-input.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/assets/checkbox-output-header.js` & `crosscompute-0.9.4.3/crosscompute/assets/checkbox-output-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/assets/configuration.yml` & `crosscompute-0.9.4.3/crosscompute/assets/configuration.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 
 # crosscompute version determines how this file is interpreted (required)
 crosscompute: 0.0.0
 
 # name summarizes what your automation does
 name: Automation X
 
-# description explains why your automation is useful
-description: Improve health, safety, quality of life in our communities
-
 # slug customizes the automation uri
 slug: automation-x
 
+# title sets the page title
+title: Automation X - Improve health, safety, quality of life
+
+# description explains why your automation is useful
+description: Improve health, safety, quality of life in our communities
+
 # version should increment after you make changes to your automation
 version: 0.0.0
 
 # imports let you embed other automations in this automation
 imports:
   # id references this import in your templates when embedding;
   # path specifies the location of the automation file to import (required)
```

### Comparing `crosscompute-0.9.4.2/crosscompute/assets/favicon.ico` & `crosscompute-0.9.4.3/crosscompute/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/assets/file-input-header.js` & `crosscompute-0.9.4.3/crosscompute/assets/file-input-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/assets/flex.css` & `crosscompute-0.9.4.3/crosscompute/assets/flex.css`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 @layer flex-vertical {
+  main {
+    max-width: 640px;
+    margin: auto;
+  }
   button {
     padding: 8px 0;
     border: 0;
     font-size: large;
     flex-grow: 1;
   }
   button:hover {
```

### Comparing `crosscompute-0.9.4.2/crosscompute/assets/live.html` & `crosscompute-0.9.4.3/crosscompute/assets/live.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/assets/radio-input.html` & `crosscompute-0.9.4.3/crosscompute/assets/radio-input.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/assets/radio-output-header.js` & `crosscompute-0.9.4.3/crosscompute/assets/radio-output-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/assets/step-body.js` & `crosscompute-0.9.4.3/crosscompute/assets/step-body.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/assets/step.html` & `crosscompute-0.9.4.3/crosscompute/assets/step.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/assets/table-output-header.js` & `crosscompute-0.9.4.3/crosscompute/assets/table-output-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/constants.py` & `crosscompute-0.9.4.3/crosscompute/constants.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/dependencies.py` & `crosscompute-0.9.4.3/crosscompute/dependencies.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/exceptions.py` & `crosscompute-0.9.4.3/crosscompute/exceptions.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/macros/disk.py` & `crosscompute-0.9.4.3/crosscompute/macros/disk.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/macros/iterable.py` & `crosscompute-0.9.4.3/crosscompute/macros/iterable.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/macros/log.py` & `crosscompute-0.9.4.3/crosscompute/macros/log.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/macros/package.py` & `crosscompute-0.9.4.3/crosscompute/macros/package.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/macros/security.py` & `crosscompute-0.9.4.3/crosscompute/macros/security.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routers/automation.py` & `crosscompute-0.9.4.3/crosscompute/routers/automation.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             'mutation_uri': MUTATION_ROUTE.format(uri=automation_uri)}
     else:
         d = get_step_response_dictionary(
             automation_definition, automation_definition.batch_definitions[0],
             design_name, request.query_params)
     request_uri = request.url
     return TemplateResponse(template_path_by_id['automation'], {
-        'request': request, 'title_text': automation_definition.name,
+        'request': request, 'title_text': automation_definition.title,
         'description': automation_definition.description,
         'host_uri': request_uri.scheme + '://' + request_uri.netloc,
         'name': automation_definition.name, 'uri': automation_uri,
         'automation_definition': automation_definition,
         'step_name': design_name,
         'batch_definitions': guard.get_batch_definitions(
             automation_definition),
```

### Comparing `crosscompute-0.9.4.2/crosscompute/routers/file.py` & `crosscompute-0.9.4.3/crosscompute/routers/file.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routers/root.py` & `crosscompute-0.9.4.3/crosscompute/routers/root.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routers/stream.py` & `crosscompute-0.9.4.3/crosscompute/routers/stream.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routers/token.py` & `crosscompute-0.9.4.3/crosscompute/routers/token.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/asset.py` & `crosscompute-0.9.4.3/crosscompute/routines/asset.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/authorization.py` & `crosscompute-0.9.4.3/crosscompute/routines/authorization.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/automation.py` & `crosscompute-0.9.4.3/crosscompute/routines/automation.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/batch.py` & `crosscompute-0.9.4.3/crosscompute/routines/batch.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/configuration.py` & `crosscompute-0.9.4.3/crosscompute/routines/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,18 +116,14 @@
 
     def get_design_name(self, page_id):
         design_name = DESIGN_NAMES_BY_PAGE_ID[page_id][0]
         if page_id in self.page_definition_by_id:
             page_definition = self.page_definition_by_id[page_id]
             design_name = page_definition.configuration.get(
                 'design', design_name)
-        elif page_id in STEP_NAMES:
-            variable_definitions = self.get_variable_definitions(page_id)
-            if not variable_definitions:
-                design_name = 'none'
         return design_name
 
     def is_interval_ready(self, batch_definition):
         interval_timedelta = self.interval_timedelta
         if interval_timedelta:
             run_datetime = datetime.fromtimestamp(
                 batch_definition.clock.get_end_time('run'))
@@ -375,23 +371,25 @@
             f'{__version__}; pip install crosscompute=={protocol_version}')
     return {}
 
 
 def validate_automation_identifiers(configuration):
     index = configuration.index
     name = configuration.get('name', make_automation_name(index))
-    description = configuration.get('description', '')
-    version = configuration.get('version', AUTOMATION_VERSION)
     slug = configuration.get('slug', format_slug(name))
+    title = configuration.get('title', name)
+    description = configuration.get('description', name)
+    version = configuration.get('version', AUTOMATION_VERSION)
     uri = AUTOMATION_ROUTE.format(automation_slug=slug)
     return {
         'name': name,
+        'slug': slug,
+        'title': title,
         'description': description,
         'version': version,
-        'slug': slug,
         'uri': uri}
 
 
 def validate_imports(configuration):
     automation_configurations = [configuration]
     folder = configuration.folder
     group_definitions = getattr(configuration, 'group_definitions', [])
```

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/database.py` & `crosscompute-0.9.4.3/crosscompute/routines/database.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,30 +40,32 @@
                 changed_infos.append(info)
         if changed_infos:
             self._changes[time()] = changed_infos
         L.debug(changed_infos)
         return changed_infos
 
     def get(self, path):
-        path = Path(path).absolute()
+        path = Path(path)
+        absolute_path = path.absolute()
+        resolved_path = path.resolve()
         configuration = self._configuration
         for automation_definition in configuration.automation_definitions:
             automation_folder = automation_definition.folder
             runs_folder = automation_folder / 'runs'
-            if is_path_in_folder(path, runs_folder):
-                run_id = path.resolve().relative_to(runs_folder).parts[0]
+            if is_path_in_folder(resolved_path, runs_folder):
+                run_id = resolved_path.relative_to(runs_folder).parts[0]
                 batch_uri = BATCH_ROUTE.format(batch_slug=run_id)
                 memory = DiskMemory()
                 add_variable_infos_from_folder(
                     memory, automation_definition, runs_folder / run_id,
                     batch_uri)
-                infos = memory.get(path)
+                infos = memory.get(resolved_path)
                 break
         else:
-            infos = self._memory.get(path)
+            infos = self._memory.get(absolute_path)
         return infos
 
 
 class DiskMemory():
 
     def __init__(self):
         self._infos_by_path = {}
```

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/interface.py` & `crosscompute-0.9.4.3/crosscompute/routines/interface.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/log.py` & `crosscompute-0.9.4.3/crosscompute/routines/log.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/mutation.py` & `crosscompute-0.9.4.3/crosscompute/routines/mutation.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/printer.py` & `crosscompute-0.9.4.3/crosscompute/routines/printer.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/server.py` & `crosscompute-0.9.4.3/crosscompute/routines/server.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/step.py` & `crosscompute-0.9.4.3/crosscompute/routines/step.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/uri.py` & `crosscompute-0.9.4.3/crosscompute/routines/uri.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/variable.py` & `crosscompute-0.9.4.3/crosscompute/routines/variable.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/routines/work.py` & `crosscompute-0.9.4.3/crosscompute/routines/work.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,16 +422,15 @@
         batch_environment[variable_id] = environ[variable_id]
     for variable_id in (_.id for _ in variable_definitions):
         if variable_id in data_by_id:
             continue
         try:
             batch_environment[variable_id] = environ[variable_id]
         except KeyError:
-            raise CrossComputeConfigurationError(
-                f'{variable_id} is missing in the environment')
+            L.error(f'{variable_id} is missing in the environment')
     variable_data_by_id = get_variable_data_by_id(
         variable_definitions, data_by_id, with_exceptions=False)
     variable_value_by_id = get_variable_value_by_id(variable_data_by_id)
     return batch_environment | variable_value_by_id
 
 
 def _prepare_script_environment(
```

### Comparing `crosscompute-0.9.4.2/crosscompute/scripts/configure.py` & `crosscompute-0.9.4.3/crosscompute/scripts/configure.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/scripts/launch.py` & `crosscompute-0.9.4.3/crosscompute/scripts/launch.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/scripts/print.py` & `crosscompute-0.9.4.3/crosscompute/scripts/print.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/scripts/run.py` & `crosscompute-0.9.4.3/crosscompute/scripts/run.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/scripts/serve.py` & `crosscompute-0.9.4.3/crosscompute/scripts/serve.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute/settings.py` & `crosscompute-0.9.4.3/crosscompute/settings.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute.egg-info/PKG-INFO` & `crosscompute-0.9.4.3/crosscompute.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute
-Version: 0.9.4.2
+Version: 0.9.4.3
 Summary: Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute/issues
 Project-URL: Documentation, https://github.com/crosscompute/crosscompute-docs
```

### Comparing `crosscompute-0.9.4.2/crosscompute.egg-info/SOURCES.txt` & `crosscompute-0.9.4.3/crosscompute.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/crosscompute.egg-info/entry_points.txt` & `crosscompute-0.9.4.3/crosscompute.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/setup.cfg` & `crosscompute-0.9.4.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosscompute
-version = 0.9.4.2
+version = 0.9.4.3
 description = Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://crosscompute.com
 author = CrossCompute Inc.
 author_email = support@crosscompute.com
 license = MIT
```

### Comparing `crosscompute-0.9.4.2/tests/test_routines_configuration.py` & `crosscompute-0.9.4.3/tests/test_routines_configuration.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/tests/test_routines_variable.py` & `crosscompute-0.9.4.3/tests/test_routines_variable.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.2/tests/test_routines_work.py` & `crosscompute-0.9.4.3/tests/test_routines_work.py`

 * *Files identical despite different names*


# Comparing `tmp/nycu_tdx_py-0.1.8.tar.gz` & `tmp/nycu_tdx_py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nycu_tdx_py-0.1.8.tar", last modified: Wed Apr 26 16:37:13 2023, max compression
+gzip compressed data, was "nycu_tdx_py-0.1.9.tar", last modified: Wed Apr 26 16:41:54 2023, max compression
```

## Comparing `nycu_tdx_py-0.1.8.tar` & `nycu_tdx_py-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 16:37:13.085003 nycu_tdx_py-0.1.8/
--rw-rw-rw-   0        0        0      219 2023-04-26 16:37:13.085003 nycu_tdx_py-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-04-26 15:03:33.000000 nycu_tdx_py-0.1.8/README.rst
--rw-rw-rw-   0        0        0      115 2023-04-26 16:37:13.086002 nycu_tdx_py-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      481 2023-04-26 16:37:03.000000 nycu_tdx_py-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:37:13.062127 nycu_tdx_py-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 16:37:13.072007 nycu_tdx_py-0.1.8/src/nycu_tdx_py/
--rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.8/src/nycu_tdx_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:37:13.084002 nycu_tdx_py-0.1.8/src/nycu_tdx_py/example/
--rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.8/src/nycu_tdx_py/example/__init__.py
--rw-rw-rw-   0        0        0       75 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.8/src/nycu_tdx_py/example/custom_sklearn.py
--rw-rw-rw-   0        0        0     1237 2023-04-26 16:29:23.000000 nycu_tdx_py-0.1.8/src/nycu_tdx_py/example/nycutdx.py
--rw-rw-rw-   0        0        0     1237 2023-04-26 16:29:23.000000 nycu_tdx_py-0.1.8/src/nycu_tdx_py/nycutdx.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:37:13.081002 nycu_tdx_py-0.1.8/src/nycu_tdx_py.egg-info/
--rw-rw-rw-   0        0        0      219 2023-04-26 16:37:12.000000 nycu_tdx_py-0.1.8/src/nycu_tdx_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2023-04-26 16:37:12.000000 nycu_tdx_py-0.1.8/src/nycu_tdx_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 16:37:12.000000 nycu_tdx_py-0.1.8/src/nycu_tdx_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-26 16:37:12.000000 nycu_tdx_py-0.1.8/src/nycu_tdx_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-26 16:37:12.000000 nycu_tdx_py-0.1.8/src/nycu_tdx_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 16:41:54.062911 nycu_tdx_py-0.1.9/
+-rw-rw-rw-   0        0        0      219 2023-04-26 16:41:54.063909 nycu_tdx_py-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-04-26 15:03:33.000000 nycu_tdx_py-0.1.9/README.rst
+-rw-rw-rw-   0        0        0      115 2023-04-26 16:41:54.064909 nycu_tdx_py-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      481 2023-04-26 16:41:27.000000 nycu_tdx_py-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:41:54.050909 nycu_tdx_py-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 16:41:54.055909 nycu_tdx_py-0.1.9/src/nycu_tdx_py/
+-rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.9/src/nycu_tdx_py/__init__.py
+-rw-rw-rw-   0        0        0     3479 2023-04-26 16:41:10.000000 nycu_tdx_py-0.1.9/src/nycu_tdx_py/nycutdx.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:41:54.062911 nycu_tdx_py-0.1.9/src/nycu_tdx_py.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-04-26 16:41:53.000000 nycu_tdx_py-0.1.9/src/nycu_tdx_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-04-26 16:41:53.000000 nycu_tdx_py-0.1.9/src/nycu_tdx_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 16:41:53.000000 nycu_tdx_py-0.1.9/src/nycu_tdx_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-26 16:41:53.000000 nycu_tdx_py-0.1.9/src/nycu_tdx_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-26 16:41:53.000000 nycu_tdx_py-0.1.9/src/nycu_tdx_py.egg-info/top_level.txt
```


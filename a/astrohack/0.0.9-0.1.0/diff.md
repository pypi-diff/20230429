# Comparing `tmp/astrohack-0.0.9.tar.gz` & `tmp/astrohack-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.0.9.tar", last modified: Thu Apr 20 15:57:58 2023, max compression
+gzip compressed data, was "astrohack-0.1.0.tar", last modified: Fri Apr 28 22:53:21 2023, max compression
```

## Comparing `astrohack-0.0.9.tar` & `astrohack-0.1.0.tar`

### file list

```diff
@@ -1,91 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.421033 astrohack-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 15:57:39.000000 astrohack-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:57:39.000000 astrohack-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-20 15:57:58.421033 astrohack-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-20 15:57:39.000000 astrohack-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:39.000000 astrohack-0.0.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-20 15:57:39.000000 astrohack-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:57:58.421033 astrohack-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.409033 astrohack-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.413033 astrohack-0.0.9/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.413033 astrohack-0.0.9/src/astrohack/_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    27827 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    16308 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_extract_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    28177 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/_utils/_parm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_parm_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_parm_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/_utils/gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/astrohack_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.409033 astrohack-0.0.9/src/astrohack/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/data/telescopes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/data/telescopes/aca_7m.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/data/telescopes/alma_da.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.417033 astrohack-0.0.9/src/astrohack/data/telescopes/alma_dv.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.421033 astrohack-0.0.9/src/astrohack/data/telescopes/alma_tp.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.421033 astrohack-0.0.9/src/astrohack/data/telescopes/vla.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/vla.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/vla.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/vla.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.421033 astrohack-0.0.9/src/astrohack/data/telescopes/vlba.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/vlba.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/vlba.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    14674 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.421033 astrohack-0.0.9/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-20 15:57:39.000000 astrohack-0.0.9/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.413033 astrohack-0.0.9/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-20 15:57:58.000000 astrohack-0.0.9/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-20 15:57:58.000000 astrohack-0.0.9/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:57:58.000000 astrohack-0.0.9/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-20 15:57:58.000000 astrohack-0.0.9/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 15:57:58.000000 astrohack-0.0.9/src/astrohack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:57:58.421033 astrohack-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-20 15:57:39.000000 astrohack-0.0.9/tests/test_class_antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19791 2023-04-20 15:57:39.000000 astrohack-0.0.9/tests/test_class_base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-20 15:57:39.000000 astrohack-0.0.9/tests/test_class_ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-20 15:57:39.000000 astrohack-0.0.9/tests/test_class_telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.349583 astrohack-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 22:53:01.000000 astrohack-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:53:01.000000 astrohack-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-28 22:53:21.349583 astrohack-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-28 22:53:01.000000 astrohack-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:01.000000 astrohack-0.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-28 22:53:01.000000 astrohack-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:53:21.349583 astrohack-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.329583 astrohack-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.333583 astrohack-0.1.0/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.337583 astrohack-0.1.0/src/astrohack/_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    27827 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.337583 astrohack-0.1.0/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.341583 astrohack-0.1.0/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21572 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_extract_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.341583 astrohack-0.1.0/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30815 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.341583 astrohack-0.1.0/src/astrohack/_utils/_parm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_parm_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_parm_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/astrohack_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.329583 astrohack-0.1.0/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.341583 astrohack-0.1.0/src/astrohack/data/.file_meta_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.341583 astrohack-0.1.0/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.341583 astrohack-0.1.0/src/astrohack/data/telescopes/aca_7m.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.341583 astrohack-0.1.0/src/astrohack/data/telescopes/alma_da.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.345583 astrohack-0.1.0/src/astrohack/data/telescopes/alma_dv.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.345583 astrohack-0.1.0/src/astrohack/data/telescopes/alma_tp.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.345583 astrohack-0.1.0/src/astrohack/data/telescopes/vla.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/vla.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/vla.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/vla.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.345583 astrohack-0.1.0/src/astrohack/data/telescopes/vlba.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/vlba.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/vlba.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
+-rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19785 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.345583 astrohack-0.1.0/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.333583 astrohack-0.1.0/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-28 22:53:21.000000 astrohack-0.1.0/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-28 22:53:21.000000 astrohack-0.1.0/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:53:21.000000 astrohack-0.1.0/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-28 22:53:21.000000 astrohack-0.1.0/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 22:53:21.000000 astrohack-0.1.0/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.345583 astrohack-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-28 22:53:01.000000 astrohack-0.1.0/tests/test_class_antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19791 2023-04-28 22:53:01.000000 astrohack-0.1.0/tests/test_class_base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-28 22:53:01.000000 astrohack-0.1.0/tests/test_class_ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-28 22:53:01.000000 astrohack-0.1.0/tests/test_class_telescope.py
```

### Comparing `astrohack-0.0.9/LICENSE` & `astrohack-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/PKG-INFO` & `astrohack-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.0.9
+Version: 0.1.0
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
 
-# astroHACK
+![astrohack](docs/_media/astrohack_logo.png)
 
 [![Python 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
 [![Documentation Status](https://readthedocs.org/projects/astrohack/badge/?version=latest)](https://astrohack.readthedocs.io/en/latest/?badge=latest)
 
 
 astroHack (Holography Antenna Commissioning Kit) is a Python package that produces antenna aperture images and panel adjustment corrections from calibrated holography measurement sets. Initially, it will support holography data from the VLA and ALMA, with the future goal of supporting the ngVLA. Much of the core functionality from the following AIPS tasks has been ported: UVHOL, HOLOG, and PANEL. astroHack enables parallel execution by using Dask and efficient single-threaded performance by making use of Numba.
```

### Comparing `astrohack-0.0.9/README.md` & `astrohack-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# astroHACK
+![astrohack](docs/_media/astrohack_logo.png)
 
 [![Python 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
 [![Documentation Status](https://readthedocs.org/projects/astrohack/badge/?version=latest)](https://astrohack.readthedocs.io/en/latest/?badge=latest)
 
 
 astroHack (Holography Antenna Commissioning Kit) is a Python package that produces antenna aperture images and panel adjustment corrections from calibrated holography measurement sets. Initially, it will support holography data from the VLA and ALMA, with the future goal of supporting the ngVLA. Much of the core functionality from the following AIPS tasks has been ported: UVHOL, HOLOG, and PANEL. astroHack enables parallel execution by using Dask and efficient single-threaded performance by making use of Numba.
```

### Comparing `astrohack-0.0.9/pyproject.toml` & `astrohack-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.0.9"
+version = "0.1.0"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
```

### Comparing `astrohack-0.0.9/src/astrohack/_classes/antenna_surface.py` & `astrohack-0.1.0/src/astrohack/_classes/antenna_surface.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/_classes/base_panel.py` & `astrohack-0.1.0/src/astrohack/_classes/base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/_classes/polygon_panel.py` & `astrohack-0.1.0/src/astrohack/_classes/polygon_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/_classes/ring_panel.py` & `astrohack-0.1.0/src/astrohack/_classes/ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/_classes/telescope.py` & `astrohack-0.1.0/src/astrohack/_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/_utils/_algorithms.py` & `astrohack-0.1.0/src/astrohack/_utils/_algorithms.py`

 * *Files 6% similar despite different names*

```diff
@@ -203,76 +203,95 @@
     variances = np.zeros_like(vector)
     if len(shape) > 2:
         for it0 in range(shape[0]):
             results[it0], variances[it0] = _least_squares_fit_block(system[it0], vector[it0])
     else:
         results, variances, _ = _least_squares_fit(system, vector)
     return results, variances
-
-def _average_repeated_pointings(vis_map_dict, weight_map_dict, flagged_mapping_antennas,time_vis,pnt_map_dict):
     
-    for ant_id in vis_map_dict.keys():
-        diff = np.diff(pnt_map_dict['ant_'+str(ant_id)],axis=0)
-        r_diff = np.sqrt(np.abs(diff[:,0]**2 + diff[:,1]**2))
     
-        max_dis = np.max(r_diff)/100
-        
-        print('max_dis',max_dis)
-        n_avg = np.sum([r_diff > max_dis]) + 1
+def _get_grid_parms(vis_map_dict,pnt_map_dict, ant_names):
     
-        vis_map_avg, weight_map_avg, time_vis_avg, pnt_map_avg = _average_repeated_pointings_jit(vis_map_dict[ant_id], weight_map_dict[ant_id],time_vis,pnt_map_dict['ant_'+str(ant_id)],n_avg,max_dis,r_diff)
-        
-        vis_map_dict[ant_id] = vis_map_avg
-        weight_map_dict[ant_id] = weight_map_avg
-        pnt_map_dict['ant_'+str(ant_id)] = pnt_map_avg
-        
-        #print('$$$',vis_map_avg.shape,weight_map_avg.shape,pnt_map_avg.shape)
-        
-    return time_vis_avg
-        
- 
+    grid_parms = {}
+    for ant_index in vis_map_dict.keys():
+        diff = np.diff(pnt_map_dict['ant_'+ant_names[ant_index]]['POINTING_OFFSET'],axis=0)
+        r_diff = np.sqrt(np.abs(diff[:,0]**2 + diff[:,1]**2))
+
+        max_dis = np.max(r_diff)/100
+        n_pix = np.sum([r_diff > max_dis]) + 1
+        cell_size = np.mean(r_diff[r_diff > max_dis])
         
-#@numba.njit(cache=False, nogil=True)
-def _average_repeated_pointings_jit(vis_map, weight_map,time_vis,pnt_map,n_avg,max_dis,r_diff):
+        grid_parms['ant_'+ant_names[ant_index]] = {'n_pix':n_pix,'cell_size':cell_size}
+
 
-    vis_map_avg = np.zeros((n_avg,)+ vis_map.shape[1:], dtype=vis_map.dtype)
-    weight_map_avg = np.zeros((n_avg,)+ weight_map.shape[1:], dtype=weight_map.dtype)
-    time_vis_avg = np.zeros((n_avg,), dtype=time_vis.dtype)
-    pnt_map_avg = np.zeros((n_avg,)+ pnt_map.shape[1:], dtype=pnt_map.dtype)
+    return grid_parms
     
     
-    k = 0
-    n_samples = 1
-    
-    vis_map_avg[0,:,:] = vis_map_avg[k,:,:] + weight_map[0,:,:]*vis_map[0,:,:]
-    weight_map_avg[0,:,:] = weight_map_avg[k,:,:] + weight_map[0,:,:]
-    time_vis_avg[0] = time_vis_avg[k] + time_vis[0]
-    pnt_map_avg[0,:] = pnt_map_avg[k,:] + pnt_map[0,:]
-
-    for i in range(vis_map.shape[0]-1):
-        
-        point_dis = r_diff[i]
-        
-        if point_dis < max_dis:
-            n_samples = n_samples + 1
-        else:
-            #vis_map_avg[k,:,:] = vis_map_avg[k,:,:]/weight_map_avg[k,:,:]
-            vis_map_avg[k,:,:] = np.divide(vis_map_avg[k,:,:],weight_map_avg[k,:,:],out=np.zeros_like(vis_map_avg[k,:,:]),where=weight_map_avg[k,:,:]!=0)
-            weight_map_avg[k,:,:] = weight_map_avg[k,:,:]/n_samples
-            
-            time_vis_avg[k] = time_vis_avg[k]/n_samples
-            pnt_map_avg[k,:] = pnt_map_avg[k,:]/n_samples
-        
-            k=k+1
-            n_samples = 1
-            
-        vis_map_avg[k,:,:] = vis_map_avg[k,:,:] + weight_map[i+1,:,:]*vis_map[i+1,:,:]
-        weight_map_avg[k,:,:] = weight_map_avg[k,:,:] + weight_map[i+1,:,:]
-        time_vis_avg[k] = time_vis_avg[k] + time_vis[i+1]
-        pnt_map_avg[k,:] = pnt_map_avg[k,:] + pnt_map[i+1,:]
-        
-    vis_map_avg[-1,:,:] = vis_map_avg[1,:,:]/weight_map_avg[-1,:,:]
-    weight_map_avg[-1,:,:] = weight_map_avg[-1,:,:]/n_samples
-    time_vis_avg[-1] = time_vis_avg[-1]/n_samples
-    pnt_map_avg[-1,:] = pnt_map_avg[-1,:]/n_samples
+    
+    
+#Does not work
+#def _average_repeated_pointings(vis_map_dict, weight_map_dict, flagged_mapping_antennas,time_vis,pnt_map_dict, ant_names):
+#
+#    for ant_index in vis_map_dict.keys():
+#        diff_ideal = np.diff(pnt_map_dict['ant_'+ant_names[ant_index]]['POINTING_OFFSET'],axis=0)
+#        r_diff_ideal = np.sqrt(np.abs(diff_ideal[:,0]**2 + diff_ideal[:,1]**2))
+#
+#        max_dis = np.max(r_diff_ideal)/100
+#        n_avg = np.sum([r_diff_ideal > max_dis]) + 1
+#        cell = np.mean(r_diff[r_diff_ideal > max_dis])
+#
+#        diff = np.diff(pnt_map_dict['ant_'+ant_names[ant_index]]['DIRECTIONAL_COSINES'],axis=0)
+#        r_diff = np.sqrt(np.abs(diff[:,0]**2 + diff[:,1]**2))
+#
+#
+#        vis_map_avg, weight_map_avg, time_vis_avg, pnt_map_avg = _average_repeated_pointings_jit(vis_map_dict[ant_index], weight_map_dict[ant_index],time_vis,pnt_map_dict['ant_'+ant_names[ant_index]]['DIRECTIONAL_COSINES'],n_avg,max_dis,r_diff_ideal,r_diff)
+#
+#        vis_map_dict[ant_id] = vis_map_avg
+#        weight_map_dict[ant_id] = weight_map_avg
+#        pnt_map_dict[ant_names['ant_'+ant_index]] = pnt_map_avg
+#
+#
+#
+#    return time_vis_avg
 
-    return vis_map_avg, weight_map_avg, time_vis_avg, pnt_map_avg
+##@numba.njit(cache=False, nogil=True)
+#def _average_repeated_pointings_jit(vis_map, weight_map,time_vis,pnt_map,n_avg,max_dis,r_diff_ideal,r_diff):
+#
+#    vis_map_avg = np.zeros((n_avg,)+ vis_map.shape[1:], dtype=vis_map.dtype)
+#    weight_map_avg = np.zeros((n_avg,)+ weight_map.shape[1:], dtype=weight_map.dtype)
+#    time_vis_avg = np.zeros((n_avg,), dtype=time_vis.dtype)
+#    pnt_map_avg = np.zeros((n_avg,)+ pnt_map.shape[1:], dtype=pnt_map.dtype)
+#
+#
+#    k = 0
+#    n_samples = 1
+#
+#    vis_map_avg[0,:,:] = vis_map_avg[k,:,:] + weight_map[0,:,:]*vis_map[0,:,:]
+#    weight_map_avg[0,:,:] = weight_map_avg[k,:,:] + weight_map[0,:,:]
+#    time_vis_avg[0] = time_vis_avg[k] + time_vis[0]
+#    pnt_map_avg[0,:] = pnt_map_avg[k,:] + pnt_map[0,:]
+#
+#    for i in range(vis_map.shape[0]-1):
+#        if r_diff_ideal[i] < max_dis:
+#            n_samples = n_samples + 1
+#        else:
+#            #vis_map_avg[k,:,:] = vis_map_avg[k,:,:]/weight_map_avg[k,:,:]
+#            vis_map_avg[k,:,:] = np.divide(vis_map_avg[k,:,:],weight_map_avg[k,:,:],out=np.zeros_like(vis_map_avg[k,:,:]),where=weight_map_avg[k,:,:]!=0)
+#            weight_map_avg[k,:,:] = weight_map_avg[k,:,:]/n_samples
+#
+#            time_vis_avg[k] = time_vis_avg[k]/n_samples
+#            pnt_map_avg[k,:] = pnt_map_avg[k,:]/n_samples
+#
+#            k=k+1
+#            n_samples = 1
+#
+#        vis_map_avg[k,:,:] = vis_map_avg[k,:,:] + weight_map[i+1,:,:]*vis_map[i+1,:,:]
+#        weight_map_avg[k,:,:] = weight_map_avg[k,:,:] + weight_map[i+1,:,:]
+#        time_vis_avg[k] = time_vis_avg[k] + time_vis[i+1]
+#        pnt_map_avg[k,:] = pnt_map_avg[k,:] + pnt_map[i+1,:]
+#
+#    vis_map_avg[-1,:,:] = vis_map_avg[1,:,:]/weight_map_avg[-1,:,:]
+#    weight_map_avg[-1,:,:] = weight_map_avg[-1,:,:]/n_samples
+#    time_vis_avg[-1] = time_vis_avg[-1]/n_samples
+#    pnt_map_avg[-1,:] = pnt_map_avg[-1,:]/n_samples
+#
+#    return vis_map_avg, weight_map_avg, time_vis_avg, pnt_map_avg
```

### Comparing `astrohack-0.0.9/src/astrohack/_utils/_constants.py` & `astrohack-0.1.0/src/astrohack/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/_utils/_conversion.py` & `astrohack-0.1.0/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.1.0/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.1.0/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/_utils/_dio.py` & `astrohack-0.1.0/src/astrohack/_utils/_dio.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,19 +158,19 @@
     
     def __setitem__(self, key, value):
         return super().__setitem__(key, value)
 
     def is_open(self):
         return self._open
 
-    def open(self, file=None, dask_load=False):
+    def open(self, file=None, dask_load=True):
         """ Open hologgraphy file.
         Args:self =_
             file (str, optional): Path to holography file. Defaults to None.
-            dask_load (bool, optional): If True the file is loaded with Dask. Defaults to False.
+            dask_load (bool, optional): If True the file is loaded with Dask. Defaults to True.
         Returns:
             bool: bool describing whether the file was opened properly
         """
         logger = _get_astrohack_logger()
 
         if file is None:
             file = self.file
@@ -316,19 +316,19 @@
     
     def __setitem__(self, key, value):
         return super().__setitem__(key, value)
 
     def is_open(self):
         return self._open
 
-    def open(self, file=None, dask_load=False):
+    def open(self, file=None, dask_load=True):
         """ Open pointing file.
         Args:self =_
             file (str, optional): Path to pointing file. Defaults to None.
-            dask_load (bool, optional): If True the file is loaded with Dask. Defaults to False.
+            dask_load (bool, optional): If True the file is loaded with Dask. Defaults to True.
         Returns:
             bool: bool describing whether the file was opened properly
         """
         logger = _get_astrohack_logger()
 
         if file is None:
             file = self.file
@@ -351,8 +351,8 @@
         table = PrettyTable()
         table.field_names = ["antenna"]
         table.align = "l"
         
         for ant in self.keys():
             table.add_row(ant)
         
-        print(table)
+        print(table)
```

### Comparing `astrohack-0.0.9/src/astrohack/_utils/_extract_holog.py` & `astrohack-0.1.0/src/astrohack/_utils/_extract_holog.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 import xarray as xr
 import astropy
 from astropy.io import fits
 from scipy import spatial
 from numba import njit
 from numba.core import types
 from numba.typed import Dict
+import copy
 
 from casacore import tables as ctables
 from astrohack._utils._imaging import _calculate_parallactic_angle_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
+from astrohack._utils._algorithms import _get_grid_parms
+
 from astrohack._utils._io import _load_point_file
 
 def _extract_holog_chunk(extract_holog_params):
     """Perform data query on holography data chunk and get unique time and state_ids/
 
     Args:
         ms_name (str): Measurementset name
@@ -78,15 +81,14 @@
     ctb.close()
     table_obj.close()
     
     time_vis, unique_index = np.unique(
         time_vis_row, return_index=True
     )  # Note that values are sorted.
     
-    #print(vis_data.shape,weight.shape,ant1.shape,ant2.shape,time_vis_row.shape,time_vis.shape,flag.shape,flag_row.shape,ref_ant_per_map_ant_tuple,map_ant_tuple,)
     
     vis_map_dict, weight_map_dict, flagged_mapping_antennas = _extract_holog_chunk_jit(
         vis_data,
         weight,
         ant1,
         ant2,
         time_vis_row,
@@ -100,43 +102,40 @@
     del vis_data, weight, ant1, ant2, time_vis_row, flag, flag_row
 
     map_ant_name_list = list(map(str, map_ant_name_tuple))
 
     map_ant_name_list = ['ant_' + i for i in map_ant_name_list]
 
     pnt_ant_dict = _load_point_file(pnt_name, map_ant_name_list, dask_load=False)
-
     pnt_map_dict = _extract_pointing_chunk(map_ant_name_list, time_vis, pnt_ant_dict)
+    grid_parms = _get_grid_parms(vis_map_dict,pnt_map_dict, ant_names)
     
-    ''' Removing for now. Code struggles with VLA pointing errors
     ### To DO:
     ################### Average multiple repeated samples
-    if telescope_name != "ALMA":
-        over_flow_protector_constant = float("%.5g" % time_vis[0])  # For example 5076846059.4 -> 5076800000.0
-        time_vis = time_vis - over_flow_protector_constant
-
-        
-        time_vis = _average_repeated_pointings(vis_map_dict, weight_map_dict, flagged_mapping_antennas,time_vis,pnt_map_dict)
-        
-        time_vis = time_vis + over_flow_protector_constant
-    '''
+    #over_flow_protector_constant = float("%.5g" % time_vis[0])  # For example 5076846059.4 -> 5076800000.0
+    #time_vis = time_vis - over_flow_protector_constant
+    #from astrohack._utils._algorithms import _average_repeated_pointings
+    #time_vis = _average_repeated_pointings(vis_map_dict, weight_map_dict, flagged_mapping_antennas,time_vis,pnt_map_dict,ant_names)
+    #time_vis = time_vis + over_flow_protector_constant
+    
     
     holog_dict = _create_holog_file(
         holog_name,
         vis_map_dict,
         weight_map_dict,
         pnt_map_dict,
         time_vis,
         chan_freq,
         pol,
         flagged_mapping_antennas,
         holog_map_key,
         ddi,
         ms_name,
         ant_names,
+        grid_parms,
         overwrite=overwrite,
     )
 
     logger.info(
         "Finished extracting holography chunk for ddi: {ddi} holog_map_key: {holog_map_key}".format(
             ddi=ddi, holog_map_key=holog_map_key
         )
@@ -287,14 +286,15 @@
     chan,
     pol,
     flagged_mapping_antennas,
     holog_map_key,
     ddi,
     ms_name,
     ant_names,
+    grid_parms,
     overwrite,
 ):
     """Create holog-structured, formatted output file and save to zarr.
 
     Args:
         holog_name (str): holog file name.
         vis_map_dict (dict): a nested dictionary/map of weighted visibilities indexed as [antenna][time, chan, pol]; mainains time ordering.
@@ -345,32 +345,28 @@
                 weight_map_dict[map_ant_index], dims=["time", "chan", "pol"]
             )
 
             xds["DIRECTIONAL_COSINES"] = xr.DataArray(
                 pnt_map_dict[map_ant_tag]["DIRECTIONAL_COSINES"].values, dims=["time", "lm"]
             )
             
-            xds["POINTING_OFFSET"] = xr.DataArray(
-                pnt_map_dict[map_ant_tag]["POINTING_OFFSET"].values, dims=["time", "az_el"]
-            )
-
             xds.attrs["holog_map_key"] = holog_map_key
             #xds.attrs["ant_id"] = map_ant_tag
             xds.attrs["ddi"] = ddi
             xds.attrs["parallactic_samples"] = parallactic_samples
             xds.attrs["telescope_name"] = telescope_name
             xds.attrs["antenna_name"] = ant_names[map_ant_index]
             
             xds.attrs["l_max"] = np.max(xds["DIRECTIONAL_COSINES"][:,0].values)
             xds.attrs["l_min"] = np.min(xds["DIRECTIONAL_COSINES"][:,0].values)
             xds.attrs["m_max"] = np.max(xds["DIRECTIONAL_COSINES"][:,1].values)
             xds.attrs["m_min"] = np.min(xds["DIRECTIONAL_COSINES"][:,1].values)
             
-            #print(xds)
-
+            xds.attrs["grid_parms"] = grid_parms[map_ant_tag]
+            
             holog_file = holog_name
 
             if overwrite is False:
                 if os.path.exists(holog_file):
                     logger.error(
                         "Holog file {file} exists. To overwite set the overwrite=True option in extract_holog or remove current file.".format(file=holog_file))
                     raise
@@ -385,60 +381,96 @@
                 mode="w",
                 compute=True,
                 consolidated=True,
             )
 
         else:
             logger.warning(
-                "[FLAGGED DATA] mapping antenna index {index}".format(index=map_ant_index
+                "[FLAGGED DATA] mapping antenna index {index}".format(index=ant_names[map_ant_index]
                 )
             )
 
+def _create_holog_obs_dict(pnt_dict,baseline_average_distance,ant_names,ant_pos,ant_names_main):
+    '''
+    Generate holog_obs_dict.
+    '''
 
+    logger = _get_astrohack_logger()
+    mapping_scans_dict = {}
+    holog_obs_dict = {}
+    map_id = 0
+    ant_names_set = set()
+    
+    # Generate {ddi: {map: {scan:[i ...], ant:{ant_map_0:[], ...}}}} structure. No reference antenas are added because we first need to populate all mapping antennas.
+    for ant_name,ant_ds in pnt_dict.items():
+        if ('ant' in ant_name):
+            ant_name = ant_name.replace('ant_','')
+            if ant_name in ant_names_main: #Check if antenna in main table.
+                ant_names_set.add(ant_name)
+                for ddi, map_dict in ant_ds.attrs['mapping_scans_obs_dict'][0].items():
+                    if ddi not in holog_obs_dict:
+                            holog_obs_dict[ddi] = {}
+                    for ant_map_id, scan_list in map_dict.items():
+                        if scan_list:
+                            map_key = _check_if_array_in_dict(mapping_scans_dict,scan_list)
+                            if not map_key:
+                                map_key = 'map_' + str(map_id)
+                                mapping_scans_dict [map_key] = scan_list
+                                map_id = map_id+1
+                                
+                            if map_key not in holog_obs_dict[ddi]:
+                                holog_obs_dict[ddi][map_key] = {'scans':np.array(scan_list),'ant':{}}
+                                                        
+                            holog_obs_dict[ddi][map_key]['ant'][ant_name] = []
+       
+    # If users specifies a baseline_average_distance we need to create an antenna distance matrix.
+    if baseline_average_distance != 'ALL':
+        import pandas as pd
+        from scipy.spatial import distance_matrix
+        df = pd.DataFrame(ant_pos, columns=['x', 'y', 'z'], index=ant_names)
+        df_mat = pd.DataFrame(distance_matrix(df.values, df.values), index=df.index, columns=df.index)
+        logger.debug('Antenna distance matrix in meters: \n' + str(df_mat))
+                        
+    #The reference antennas are then given by ref_ant_set = ant_names_set - map_ant_set.
+    for ddi, ddi_dict in holog_obs_dict.items():
+        for map_id, map_dict in ddi_dict.items():
+            map_ant_set = set(map_dict['ant'].keys())
+            ref_ant_set = ant_names_set - map_ant_set
+
+            map_ant_keys = list(map_dict['ant'].keys()) #Need a copy because of del holog_obs_dict[ddi][map_id]['ant'][map_ant_key] below.
+            for map_ant_key in map_ant_keys:
+                #add code for distance from antenna
+                if baseline_average_distance != 'all':
+                    sub_ref_ant_set = []
+                    for ref_ant in ref_ant_set:
+                        if df_mat.loc[map_ant_key,ref_ant] < baseline_average_distance:
+                            sub_ref_ant_set.append(ref_ant)
+                        
+                    if (not sub_ref_ant_set) and (ref_ant_set):
+                        logger.warning('DDI ' + str(ddi) + ' and mapping antenna ' + str(map_ant_key) + ' has no reference antennas. If baseline_average_distance was specified increase this distance. See antenna distance matrix in log by setting debug level to DEBUG in astrohack_client function.')
+                     
+                    ref_ant_set = sub_ref_ant_set
+                
+                if ref_ant_set:
+                    holog_obs_dict[ddi][map_id]['ant'][map_ant_key] = np.array(list(ref_ant_set))
+                else:
+                    del holog_obs_dict[ddi][map_id]['ant'][map_ant_key] #Don't want mapping antennas with no reference antennas.
+                    logger.warning('DDI ' + str(ddi) + ' and mapping antenna ' + str(map_ant_key) + ' has no reference antennas.')
+                     
+    return holog_obs_dict
 
+    
 
-
-
-
-
-
-
-
-### To DO
-def _create_holog_obs_dict():
-    '''
-    Code to automatically create holog_obs_dict
-    VLA datasets causeing issues.
-    if holog_obs_dict is None:
-        ant_names_list = []
-        #Create mapping antennas
-        holog_obs_dict = {}
-        for ant_id,pnt_xds in pnt_dict.items():
-            ant_name = pnt_xds.attrs['ant_name']
-            mapping_scans = pnt_xds.attrs['mapping_scans']
-            ant_names_list.append(ant_name)
-            for ddi,scans in  mapping_scans.items():
-                ddi = int(ddi)
-                for s in scans:
-                    try:
-                        holog_obs_dict[ddi][s]['map'].append(ant_name)
-                    except:
-                        holog_obs_dict.setdefault(ddi,{})[s] = {'map':[ant_name]}#dict(zip(scans, [ant_name]*len(scans)))
-       
-       
-        #Create reference antennas
-        
-        ant_names_set = set(ant_names_list)
-        for ddi,scan in holog_obs_dict.items():
-            for scan_id,ant_types in scan.items():
-                holog_obs_dict[ddi][scan_id]['ref'] = ant_names_set - set(holog_obs_dict[ddi][scan_id]['map'])
+def _check_if_array_in_dict(array_dict,array):
+    
+    for key,val in array_dict.items():
+        if np.array_equiv(val,array):
+            return key
             
-    '''
-    
-    return 0
+    return False
 
 
 def _extract_pointing_chunk(map_ant_ids, time_vis, pnt_ant_dict):
     """Extract nearest MAIN table time indexed pointing map
 
     Args:
         map_ant_ids (dict): list of antenna ids
@@ -457,7 +489,76 @@
         pnt_map_dict[antenna] = np.zeros((n_time_vis, 2))
         pnt_map_dict[antenna] = (
             pnt_ant_dict[antenna]
             .interp(time=time_vis, method="nearest")
         )
 
     return pnt_map_dict
+
+
+
+def _create_holog_meta_data(holog_file, holog_dict, holog_params):
+    """Save holog file meta information to json file with the transformation
+        of the ordering (ddi, holog_map, ant) --> (ant, ddi, holog_map).
+
+    Args:
+        holog_name (str): holog file name.
+        holog_dict (dict): Dictionary containing msdx data.
+    """
+    logger = _get_astrohack_logger()
+    
+    ant_holog_dict = {}
+    cell_sizes = []
+    n_pixs = []
+    telescope_names = []
+    
+    for ddi, map_dict in holog_dict.items():
+        if "ddi_" in ddi:
+            for map, ant_dict in map_dict.items():
+                if "map_" in map:
+                    for ant, xds in ant_dict.items():
+                        if "ant_" in ant:
+                            if ant not in ant_holog_dict:
+                                ant_holog_dict[ant] = {ddi:{map:{}}}
+                            elif ddi not in ant_holog_dict[ant]:
+                                ant_holog_dict[ant][ddi] = {map:{}}
+                    
+                            ant_holog_dict[ant][ddi][map] = xds.to_dict(data=False)
+                            cell_sizes.append(xds.attrs["grid_parms"]["cell_size"])
+                            n_pixs.append(xds.attrs["grid_parms"]["n_pix"])
+                            telescope_names.append(xds.attrs['telescope_name'])
+
+
+    if not (len(set(cell_sizes)) == 1):
+        logger.error('Cell size not consistant: ' + str(cell_sizes))
+        raise
+        
+    if not (len(set(n_pixs)) == 1):
+        logger.error('Number of pixels not consistant: ' + str(n_pixs))
+        raise
+        
+    if not (len(set(telescope_names)) == 1):
+        logger.error('Telescope name not consistant: ' + str(telescope_names))
+        raise
+        
+    meta_data = {'cell_size':cell_sizes[0],'n_pix':n_pixs[0],'telescope_name':telescope_names[0]}
+
+    output_attr_file = "{name}/{ext}".format(name=holog_file, ext=".holog_attr")
+
+    try:
+        with open(output_attr_file, "w") as json_file:
+            json.dump(meta_data, json_file)
+
+    except Exception as error:
+        logger.error("[_create_holog_meta_data] {error}".format(error=error))
+    
+
+    
+    output_meta_file = "{name}/{ext}".format(name=holog_file, ext=".holog_json")
+    
+    try:
+        with open(output_meta_file, "w") as json_file:
+            json.dump(ant_holog_dict, json_file)
+
+    except Exception as error:
+        logger.error("[_create_holog_meta_data] {error}".format(error=error))
+
```

### Comparing `astrohack-0.0.9/src/astrohack/_utils/_holog.py` & `astrohack-0.1.0/src/astrohack/_utils/_holog.py`

 * *Files 25% similar despite different names*

```diff
@@ -117,43 +117,25 @@
         else:
             beam_grid[holog_map_index, ...] = np.moveaxis(griddata(lm, vis, (grid_l, grid_m), method=holog_chunk_params["grid_interpolation_mode"],fill_value=0.0), (0,1), (2,3))
 
 
         time_centroid_index = ant_data_dict[ddi][holog_map].dims["time"] // 2
 
         time_centroid.append(ant_data_dict[ddi][holog_map].coords["time"][time_centroid_index].values)
-        
-        
-        ###########
-#            shape = np.array(beam_grid.shape[-2:])//2
-#            phase_diff = np.angle(beam_grid[:, :, 0, shape[0], shape[1]]) - np.angle(beam_grid[:, :, 3, shape[0], shape[1]])
-#            print('phase_diff',phase_diff)
-#            #beam_grid[:,:,0,:,:] = beam_grid[:,:,0,:,:]*(np.exp(-1j*phase_diff/2)[None,None,:,:])
-#            #beam_grid[:,:,3,:,:] = beam_grid[:,:,3,:,:]*(np.exp(1j*phase_diff/2)[None,None,:,:])
-#            #beam_grid[:,:,0,:,:] = beam_grid[:,:,0,:,:]*(np.exp(-1j*phase_diff/2)[None,None,:,:])
-#            beam_grid[:,:,3,:,:] = beam_grid[:,:,3,:,:]*(np.exp(1j*phase_diff)[None,None,:,:])
-#            #Not sure what to do with cross pol (RL, LR / XY, YX)
-#
-#            print(beam_grid[0, 0, 0, 15, 15],beam_grid[0, 0, 3, 15, 15])
-#            print(np.angle(beam_grid[0, 0, 0, 15, 15]-beam_grid[0, 0, 3, 15, 15]))
-#            print(np.angle(beam_grid[0, 0, 0, 15, 15]),np.angle(beam_grid[0, 0, 3, 15, 15]))
-#            #beam_grid[0, 0, 3, ...] = -1*beam_grid[0, 0, 3, ...]
 
         for chan in range(n_chan): ### Todo: Vectorize holog_map and channel axis
-            xx_peak = _find_peak_beam_value(beam_grid[holog_map_index, chan, 0, ...], scaling=0.25)
-            
-            yy_peak = _find_peak_beam_value(beam_grid[holog_map_index, chan, 3, ...], scaling=0.25)
-
-            #print(xx_peak,yy_peak,beam_grid[holog_map_index, chan, 0, ...][15,15],beam_grid[holog_map_index, chan, 3, ...][15,15])
-            #print(np.abs(xx_peak),np.abs(yy_peak),np.abs(beam_grid[holog_map_index, chan, 0, ...][15,15]),np.abs(beam_grid[holog_map_index, chan, 3, ...][15,15]))
-            #print(np.angle(xx_peak)*180/np.pi,np.angle(yy_peak)*180/np.pi)
-            
+            try:
+                xx_peak = _find_peak_beam_value(beam_grid[holog_map_index, chan, 0, ...], scaling=0.25)
+                yy_peak = _find_peak_beam_value(beam_grid[holog_map_index, chan, 3, ...], scaling=0.25)
+            except:
+                center_pixel = np.array(beam_grid.shape[0:2])//2
+                xx_peak = beam_grid[holog_map_index, chan, 0, center_pixel[0], center_pixel[1]]
+                yy_peak = beam_grid[holog_map_index, chan, 3, center_pixel[0], center_pixel[1]]
             normalization = np.abs(0.5 * (xx_peak + yy_peak))
             beam_grid[holog_map_index, chan, ...] /= normalization
-            #print('####normalization ', normalization)
 
     beam_grid = _parallactic_derotation(data=beam_grid, parallactic_angle_dict=ant_data_dict[ddi])
     
 
     ###############
     pol = beam_grid,ant_data_dict[ddi][holog_map].pol.values
     if to_stokes:
@@ -200,15 +182,14 @@
     if radius_v > radius_u:
         radius = radius_v
     else:
         radius = radius_u
 
     if holog_chunk_params['apply_mask']:
     # Masking Aperture image
-
         mask = _mask_circular_disk(
             center=None,
             radius=radius,
             array=aperture_grid,
         )
 
         aperture_grid = mask*aperture_grid
@@ -334,102 +315,7 @@
 
     cf_chan_map = np.zeros((n_chan,), dtype=int)
     for i in range(n_chan):
         cf_chan_map[i], _ = _find_nearest(pb_freq, freq_chan[i])
 
     return cf_chan_map, pb_freq
 
-def _create_holog_meta_data(holog_file, holog_dict, holog_params):
-    """Save holog file meta information to json file with the transformation
-        of the ordering (ddi, holog_map, ant) --> (ant, ddi, holog_map).
-
-    Args:
-        holog_name (str): holog file name.
-        holog_dict (dict): Dictionary containing msdx data.
-    """
-    data_extent = []
-    lm_extent = {"l": {"min": [], "max": []}, "m": {"min": [], "max": []}}
-    ant_holog_dict = {}
-    
-    for ddi, map_dict in holog_dict.items():
-        if "ddi_" in ddi:
-            for map, ant_dict in map_dict.items():
-                if "map_" in map:
-                    for ant, xds in ant_dict.items():
-                        if "ant_" in ant:
-                            if ant not in ant_holog_dict:
-                                ant_holog_dict[ant] = {ddi:{map:{}}}
-                            elif ddi not in ant_holog_dict[ant]:
-                                ant_holog_dict[ant][ddi] = {map:{}}
-                    
-                            ant_holog_dict[ant][ddi][map] = xds.to_dict(data=False)
-                
-                            #ant_sub_dict.setdefault(ddi, {})
-                            #ant_holog_dict.setdefault(ant, ant_sub_dict)[ddi][map] = xds.to_dict(data=False)
-
-                            # Find the average (l, m) extent for each antenna, over (ddi, map) and write the meta data to file.
-                            dims = xds.dims
-                            
-                            lm_extent["l"]["min"].append(xds.attrs["l_min"])
-                            lm_extent["l"]["max"].append(xds.attrs["l_max"])
-                            lm_extent["m"]["min"].append(xds.attrs["m_min"])
-                            lm_extent["m"]["max"].append(xds.attrs["m_max"])
-                            
-                            '''
-                            lm_extent["l"]["min"].append(
-                                np.min(xds.DIRECTIONAL_COSINES.values[:, 0])
-                            )
-
-                            lm_extent["l"]["max"].append(
-                                np.max(xds.DIRECTIONAL_COSINES.values[:, 0])
-                            )
-
-                            lm_extent["m"]["min"].append(
-                                np.min(xds.DIRECTIONAL_COSINES.values[:, 1])
-                            )
-
-                            lm_extent["m"]["max"].append(
-                                np.max(xds.DIRECTIONAL_COSINES.values[:, 1])
-                            )
-                            '''
-                    
-                            data_extent.append(dims["time"])
-
-
-    max_value = int(np.array(data_extent).max())
-
-    max_extent = {
-        "n_time": max_value,
-        "telescope_name": holog_params['telescope_name'],
-        "ant_map": holog_params['holog_obs_dict'],
-        "extent": {
-            "l": {
-                "min": np.array(lm_extent["l"]["min"]).mean(),
-                "max": np.array(lm_extent["l"]["max"]).mean(),
-            },
-            "m": {
-                "min": np.array(lm_extent["m"]["min"]).mean(),
-                "max": np.array(lm_extent["m"]["max"]).mean(),
-            },
-        },
-    }
-
-    output_attr_file = "{name}/{ext}".format(name=holog_file, ext=".holog_attr")
-
-    try:
-        with open(output_attr_file, "w") as json_file:
-            json.dump(max_extent, json_file)
-
-    except Exception as error:
-        logger.error("[_create_holog_meta_data] {error}".format(error=error))
-    
-
-    
-    output_meta_file = "{name}/{ext}".format(name=holog_file, ext=".holog_json")
-    
-    try:
-        with open(output_meta_file, "w") as json_file:
-            json.dump(ant_holog_dict, json_file)
-
-    except Exception as error:
-        logger.error("[_create_holog_meta_data] {error}".format(error=error))
-
```

### Comparing `astrohack-0.0.9/src/astrohack/_utils/_imaging.py` & `astrohack-0.1.0/src/astrohack/_utils/_imaging.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,45 +11,44 @@
 from astrohack._utils._algorithms import _calc_coords
 
 from memory_profiler import profile
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
 def _parallactic_derotation(data, parallactic_angle_dict):
-    """ Uses samples of parallactic angle (PA) values to correct differences in PA between scans. The reference PA is selected 
-        to be the first scans median parallactic angle. All values are rotated to this PA value using scypi.ndimage.rotate(...)
+    """ Uses samples of parallactic angle (PA) values to correct differences in PA between maps. The reference PA is selected
+        to be the first maps median parallactic angle. All values are rotated to this PA value using scypi.ndimage.rotate(...)
 
     Args:
-        data (numpy.ndarray): beam data grid (scan, chan, pol, l, m)
+        data (numpy.ndarray): beam data grid (map, chan, pol, l, m)
         parallactic_angle_dict (dict): dictionary containing antenna selected xds from which the aprallactic angle samples 
-                                       are retrieved ==> [scan](xds), here the scan referres to the scan values not the scan index.
+                                       are retrieved ==> [map](xds), here the map referres to the map values not the map index.
 
     Returns:
         numpy.ndarray: rotation adjusted beam data grid
     """
     # Find the middle index of the array. This is calcualted because there might be a desire to change 
     # the array length at some point and I don't want to hard code the middle value.
     #
-    # It is assumed, and should be true, that the parallacitc angle array size is consistent over scan.
-    scans = list(parallactic_angle_dict.keys())
+    # It is assumed, and should be true, that the parallacitc angle array size is consistent over map.
+    maps = list(parallactic_angle_dict.keys())
 
-    # Get the median index for the first scan (this should be the same for every scan).
-    median_index = len(parallactic_angle_dict[scans[0]].parallactic_samples)//2
+    # Get the median index for the first map (this should be the same for every map).
+    median_index = len(parallactic_angle_dict[maps[0]].parallactic_samples)//2
     
-    # This is the angle we will rotated the scans to.
-    median_angular_reference = parallactic_angle_dict[scans[0]].parallactic_samples[median_index]
+    # This is the angle we will rotated the maps to.
+    median_angular_reference = parallactic_angle_dict[maps[0]].parallactic_samples[median_index]
     
-    for scan, scan_value in enumerate(scans):
-        print(scan,scan_value)
-        #median_angular_offset = median_angular_reference - parallactic_angle_dict[scan_value].parallactic_samples[median_index]
+    for map, map_value in enumerate(maps):
+        #median_angular_offset = median_angular_reference - parallactic_angle_dict[map_value].parallactic_samples[median_index]
         #median_angular_offset *= 180/np.pi
         
-        #parallactic_angle = 360 - parallactic_angle_dict[scan_value].parallactic_samples[median_index]*180/np.pi
+        #parallactic_angle = 360 - parallactic_angle_dict[map_value].parallactic_samples[median_index]*180/np.pi
         
-        data[scan] = scipy.ndimage.rotate(input=data[scan, ...], angle=90, axes=(3, 2), reshape=False)
+        data[map] = scipy.ndimage.rotate(input=data[map, ...], angle=90, axes=(3, 2), reshape=False)
         
     return data
 
 def _mask_circular_disk(center, radius, array, mask_value=np.nan):
     """ Create a mask to trim an image
 
     Args:
```

### Comparing `astrohack-0.0.9/src/astrohack/_utils/_io.py` & `astrohack-0.1.0/src/astrohack/_utils/_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -418,14 +418,16 @@
         file (zarr): Input zarr file containing pointing dictionary.
 
     Returns:
         dict: Pointing dictionary
     """
     if pnt_dict is None:
         pnt_dict = {}
+        
+    pnt_dict['point_meta_ds'] = xr.open_zarr(file)
 
     for ant in os.listdir(file):
         if "ant_" in ant:
             if (ant_list is None) or (ant in ant_list):
                 if dask_load:
                     pnt_dict[ant] = xr.open_zarr(os.path.join(file, ant))
                 else:
```

### Comparing `astrohack-0.0.9/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.1.0/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,27 @@
     '''
     Will first try to get worker logger. If this fails graph construction logger is returned.
     '''
     from dask.distributed import get_worker
     try:
         worker = get_worker()
     except:
-        return logging.getLogger(name)
+        #Schedular processes
+        logger_dict = logging.Logger.manager.loggerDict
+        if name in logger_dict:
+            logger = logging.getLogger(name)
+        else:
+            #If main logger is not started using astrohack_client function it defaults to printing to term.
+            logger = logging.getLogger(name)
+            handler = logging.StreamHandler(sys.stdout)
+            handler.setFormatter(astrohack_formatter())
+            logger.addHandler(handler)
+            logger.setLevel(logging.getLevelName('INFO'))
+        
+        return logger
     
     try:
         logger = worker.plugins['astrohack_worker'].get_logger()
         return logger
     except:
         return logging.getLogger()
```

### Comparing `astrohack-0.0.9/src/astrohack/_utils/_panel.py` & `astrohack-0.1.0/src/astrohack/_utils/_panel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,81 @@
 import numpy as np
 
 from numba import njit
 
 from astrohack._utils._conversion import _convert_unit
 from astrohack._utils._algorithms import _least_squares_fit_block
 from astrohack._utils._constants import plot_types
+from astrohack._utils._io import _load_image_xds
+
+from astrohack._classes.telescope import Telescope
+from astrohack._classes.antenna_surface import AntennaSurface
 
 # global constants
 NPAR = 10
 
+def _panel_chunk(panel_chunk_params):
+    """
+    Process a chunk of the holographies, usually a chunk consists of an antenna over a ddi
+    Args:
+        panel_chunk_params: dictionary of inputs
+    """
+    if panel_chunk_params['origin'] == 'AIPS':
+        inputxds = xr.open_zarr(panel_chunk_params['image_name'])
+        telescope = Telescope(inputxds.attrs['telescope_name'])
+        panel_chunk_params['antenna'] = inputxds.attrs['ant_name']
+
+    else:
+        inputxds = _load_image_xds(panel_chunk_params['image_name'],
+                                   panel_chunk_params['antenna'],
+                                   panel_chunk_params['ddi'],
+                                   dask_load=False)
+
+        inputxds.attrs['AIPS'] = False
+
+        if inputxds.attrs['telescope_name'] == "ALMA":
+            tname = inputxds.attrs['telescope_name']+'_'+inputxds.attrs['ant_name'][0:2]
+            telescope = Telescope(tname)
+        elif inputxds.attrs['telescope_name'] == "EVLA":
+            tname = "VLA"
+            telescope = Telescope(tname)
+        else:
+            raise ValueError('Unsuported telescope {0:s}'.format(inputxds.attrs['telescope_name']))
+
+    surface = AntennaSurface(inputxds, telescope, panel_chunk_params['cutoff'], panel_chunk_params['panel_kind'],
+                             panel_margins=panel_chunk_params['panel_margins'])
+
+    surface.compile_panel_points()
+    surface.fit_surface()
+    surface.correct_surface()
+    
+    xds_name = panel_chunk_params['panel_name'] + '/' + panel_chunk_params['antenna'] + '/' + panel_chunk_params['ddi']
+    xds = surface.export_xds()
+    xds.to_zarr(xds_name, mode='w')
+
+
+def _create_phase_model(npix, parameters, wavelength, telescope, cellxy):
+    """
+    Create a phase model with npix by npix size according to the given parameters
+    Args:
+        npix: Number of pixels in each size of the model
+        parameters: Parameters for the phase model in the units described in _phase_fitting
+        wavelength: Observing wavelength, in meters
+        telescope: Telescope object containing the optics parameters
+        cellxy: Map cell spacing, in meters
+
+    Returns:
+
+    """
+    iNPARameters = _external_to_internal_parameters(parameters, wavelength, telescope, cellxy)
+    dummyphase = np.zeros((npix, npix))
+
+    _, model = _correct_phase(dummyphase, cellxy, iNPARameters, telescope.magnification, telescope.focus,
+                              telescope.surp_slope)
+    return model
 
 def _phase_fitting_block(pols, wavelength, telescope, cellxy, amplitude_image, phase_image, pointing_offset,
                          focus_xy_offsets, focus_z_offset, subreflector_tilt, cassegrain_offset):
     """
     Corrects the grading phase for pointing, focus, and feed offset errors using the least squares method, and a model
     incorporating subreflector position errors.  Includes reference pointing
```

### Comparing `astrohack-0.0.9/src/astrohack/_utils/_parm_utils/_check_logger_parms.py` & `astrohack-0.1.0/src/astrohack/_utils/_parm_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/_utils/_parm_utils/_check_parms.py` & `astrohack-0.1.0/src/astrohack/_utils/_parm_utils/_check_parms.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     parm_dict = {parm_name:parm}
     parm_passed =  _check_parms(parm_dict, parm_name, acceptable_data_types, acceptable_data, acceptable_range, list_acceptable_data_types, list_len, default)
     
     parm = parm_dict[parm_name]
     
     return parm_passed, parm
 
-def _check_parms(parm_dict, string_key, acceptable_data_types, acceptable_data = None, acceptable_range = None, list_acceptable_data_types=None, list_len=None, default=None):
+def _check_parms(parm_dict, string_key, acceptable_data_types, acceptable_data = None, acceptable_range = None, list_acceptable_data_types=None, list_len=None, default=None, log_default_setting=True):
     """
 
     Parameters
     ----------
     parm_dict: dict
         The dictionary in which the a parameter will be checked
     string_key :
@@ -82,15 +82,17 @@
                 logger.error('Dictionary parameters must have a default. Please report bug.')
                 return False
             for default_element in default:
                 if default_element in parm_dict[string_key]:
                     if not(_check_parms(parm_dict[string_key], default_element, [type(default[default_element])], default=default[default_element])): parms_passed = False
                 else:
                     parm_dict[string_key][default_element] = default[default_element]
-                    logger.info('Setting default '+ str(string_key)+ '[\''+str(default_element)+'\']'+ ' to '+ str(default[default_element]))
+                    
+                    if log_default_setting:
+                        logger.info('Setting default '+ str(string_key)+ '[\''+str(default_element)+'\']'+ ' to '+ str(default[default_element]))
                     
             return parms_passed
                     
         else:
 
             type_check = False
             for adt in acceptable_data_types:
@@ -108,15 +110,17 @@
             if acceptable_range is not None:
                 if (parm_dict[string_key] < acceptable_range[0]) or (parm_dict[string_key] > acceptable_range[1]):
                     logger.error('Invalid '+ str(string_key) +'. Must be within the range '+ str(acceptable_range)+'.')
                     return False
     else:
         if default is not None:
             parm_dict[string_key] =  default
-            logger.info('Setting default '+ str(string_key)+ ' to '+ str(parm_dict[string_key]))
+            
+            if log_default_setting:
+                logger.info('Setting default '+ str(string_key)+ ' to '+ str(parm_dict[string_key]))
         else:
             logger.error('Parameter '+ str(string_key)+ ' must be specified')
             return False
     
     return True
```

### Comparing `astrohack-0.0.9/src/astrohack/_utils/gaussfitter.py` & `astrohack-0.1.0/src/astrohack/_utils/gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/astrohack_client.py` & `astrohack-0.1.0/src/astrohack/astrohack_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,68 +5,87 @@
 import logging
 import astrohack
 from astrohack._utils._parm_utils._check_logger_parms import _check_logger_parms, _check_worker_logger_parms
 from astrohack._utils._logger._astrohack_logger import  _setup_astrohack_logger, _get_astrohack_logger
 from astrohack._utils._dask_plugins._astrohack_worker import _astrohack_worker
 
 def astrohack_local_client(cores=None, memory_limit=None, dask_local_dir=None, log_parms={}, worker_log_parms={}):
-    """Setup dask cluster and astrohack logger.
+    """ Setup dask cluster and astrohack logger.
 
-    :param cores: Number of cores in Dask cluster.
-    :type cores: int
+    :param cores: Number of cores in Dask cluster, defaults to None
+    :type cores: int, optional
 
-    :param memory_limit: Amount of memory per core. It is suggested to use '8GB'.
-    :type memory_limit: str
+    :param memory_limit: Amount of memory per core. It is suggested to use '8GB', defaults to None
+    :type memory_limit: str, optional
+    
+    :param dask_local_dir: Where Dask should store temporary files, defaults to None. If None Dask will use `./dask-worker-space`, defaults to None
+    :type dask_local_dir: str, optional
 
-    :param dask_local_dir: Where Dask should store temporary files, defaults to None. If None Dask will use ./dask-worker-space.
-    :type dask_local_dir: str
-   
-    :param log_parms: The logger for the main process (code that does not run in parallel),
+    :param log_parms: The logger for the main process (code that does not run in parallel), defaults to {}
     :type log_parms: dict, optional
- 
+
     :param log_parms['log_to_term']: Prints logging statements to the terminal, default to True.
     :type log_parms['log_to_term']: bool, optional
    
     :param log_parms['log_level']: Log level options are: 'CRITICAL', 'ERROR', 'WARNING', 'INFO', and 'DEBUG'. With defaults of 'INFO'.
     :type log_parms['log_level']: bool, optional
    
     :param log_parms['log_to_file']: Write log to file, defaults to False.
     :type log_parms['log_to_file']: bool, optional
    
     :param log_parms['log_file']: If log_parms['log_to_file'] is True the log will be written to a file with the name log_parms['log_file'],
     :type log_parms['log_file']: bool, optional
-   
-    :param worker_log_parms: has the same keys as log_parms. However the defaults are {'log_to_term':False,'log_level':'INFO','log_to_file':False,'log_file':None}.
-    :type dict
+
+    :param worker_log_parms: worker_log_parms: Keys as same as log_parms, default values given in `Additional Information`_.
+    :type worker_log_parms: dict, optional
+
+    :return: Dask Distributed Client
+    :rtype: distributed.Client
+    
+    
+    .. _Additional Information:
+
+    **Additional Information**
+    
+    ``worker_log_params`` default values are set internally when there is not user input. The default values are given below.
+    
+    .. parsed-literal::
+        worker_log_parms =
+            {
+                'log_to_term':False,
+                'log_level':'INFO',
+                'log_to_file':False,
+                'log_file':None
+            }
+
     """
     
     #Secret parameters user do not need to know about.
     astrohack_autorestrictor=False
     wait_for_workers=True
     
     astrohack_local_dir=None #Not needed for a local cluster, but useful for testing.
 
     _log_parms = copy.deepcopy(log_parms)
     _worker_log_parms = copy.deepcopy(worker_log_parms)
     
-    assert(_check_logger_parms(_log_parms)), "######### ERROR: initialize_processing log_parms checking failed."
+    assert(_check_logger_parms(_log_parms)),               "######### ERROR: initialize_processing log_parms checking failed."
     assert(_check_worker_logger_parms(_worker_log_parms)), "######### ERROR: initialize_processing log_parms checking failed."
     
     if astrohack_local_dir:
         os.environ['ASTROHACK_LOCAL_DIR'] = astrohack_local_dir
         local_cache = True
     else:
         local_cache = False
     
     _setup_astrohack_logger(**_log_parms)
     logger = _get_astrohack_logger()
     
     _set_up_dask(dask_local_dir)
     
-    #astrohack_path = astrohack.__path__.__dict__["_path"][0]
     astrohack_path = astrohack.__path__[0]
     
     if local_cache or astrohack_autorestrictor:
         dask.config.set({"distributed.scheduler.preload": os.path.join(astrohack_path,'_utils/_astrohack_scheduler.py')})
         dask.config.set({"distributed.scheduler.preload-argv": ["--local_cache",local_cache,"--autorestrictor",astrohack_autorestrictor]})
     
     
@@ -80,16 +99,14 @@
     if memory_limit is None: memory_limit = str(round(((psutil.virtual_memory().available / (1024 ** 2))) / cores)) + 'MB'
     
     #print('cores',cores,memory_limit)
     
     cluster = dask.distributed.LocalCluster(n_workers=cores, threads_per_worker=1, processes=True, memory_limit=memory_limit,silence_logs=logging.ERROR) #, silence_logs=logging.ERROR #,resources={'GPU': 2}
     client = dask.distributed.Client(cluster)
     client.get_versions(check=True)
-    
-    #print(client)
 
     '''
     When constructing a graph that has local cache enabled all workers need to be up and running.
     '''
     if local_cache or wait_for_workers:
         client.wait_for_workers(n_workers=cores)
 
@@ -105,16 +122,17 @@
 def _set_up_dask(local_directory):
     if local_directory: dask.config.set({"temporary_directory": local_directory})
     dask.config.set({"distributed.scheduler.allowed-failures": 10})
     dask.config.set({"distributed.scheduler.work-stealing": True})
     dask.config.set({"distributed.scheduler.unknown-task-duration": '99m'})
     dask.config.set({"distributed.worker.memory.pause": False})
     dask.config.set({"distributed.worker.memory.terminate": False})
-    #dask.config.set({"distributed.worker.memory.recent-to-old-time": '999s'})
+    # dask.config.set({"distributed.worker.memory.recent-to-old-time": '999s'})
     dask.config.set({"distributed.comm.timeouts.connect": '3600s'})
     dask.config.set({"distributed.comm.timeouts.tcp": '3600s'})
     dask.config.set({"distributed.nanny.environ.OMP_NUM_THREADS": 1})
     dask.config.set({"distributed.nanny.environ.MKL_NUM_THREADS": 1})
-    #https://docs.dask.org/en/stable/how-to/customize-initialization.html
+    
+    # https://docs.dask.org/en/stable/how-to/customize-initialization.html
```

### Comparing `astrohack-0.0.9/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs` & `astrohack-0.1.0/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata` & `astrohack-0.1.0/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/data/telescopes/alma_da.zarr/.zattrs` & `astrohack-0.1.0/src/astrohack/data/telescopes/alma_da.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata` & `astrohack-0.1.0/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs` & `astrohack-0.1.0/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata` & `astrohack-0.1.0/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs` & `astrohack-0.1.0/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata` & `astrohack-0.1.0/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/data/telescopes/vla.zarr/.zattrs` & `astrohack-0.1.0/src/astrohack/data/telescopes/vla.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/data/telescopes/vla.zarr/.zmetadata` & `astrohack-0.1.0/src/astrohack/data/telescopes/vla.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/data/telescopes/vlba.zarr/.zattrs` & `astrohack-0.1.0/src/astrohack/data/telescopes/vlba.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/data/telescopes/vlba.zarr/.zmetadata` & `astrohack-0.1.0/src/astrohack/data/telescopes/vlba.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/dio.py` & `astrohack-0.1.0/src/astrohack/dio.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import os
 import dask
+import numpy as np
+
+from astropy.time import Time
+from casacore import tables
 
 from astrohack._utils._constants import length_units, trigo_units, plot_types
 from astrohack._utils._parm_utils._check_parms import _check_parms
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._utils import _parm_to_list
 
 from astrohack._utils._io import _load_point_file
@@ -19,24 +23,24 @@
 from astrohack._utils._dio import AstrohackPanelFile
 from astrohack._utils._dio import AstrohackPointFile
 
 from astrohack._utils._panel import _plot_antenna_chunk
 
 
 def export_screws(panel_mds_name, destination, ant_name=None, ddi=None,  unit='mm'):
-    """Export screws adjustments from a panel_mds file
+    """ Export screw adjustment from panel to text file and save to disk.
 
     :param panel_mds_name: Input panel_mds file
     :type panel_mds_name: str
     :param destination: Name of the destination folder to contain exported screw adjustments
     :type destination: str
     :param ant_name: List of antennae/antenna to be exported, defaults to "all" when None
-    :type ant_name: list or str, optional
+    :type ant_name: list or str, optional, ex. ant_ea25
     :param ddi: List of ddis/ddi to be exported, defaults to "all" when None
-    :type ddi: list or str, optional
+    :type ddi: list or str, optional, ex. ddi_0
     :param unit: Unit for screws adjustments, most length units supported, defaults to "mm"
     :type unit: str
 
     .. _Description:
 
     Produce the screw adjustments from ``astrohack.panel`` results to be used at the antenna site to improve the antenna surface
 
@@ -77,24 +81,24 @@
                     export_name = parm_dict['destination']+f'/screws_{antenna}_{ddi}.txt'
                     surface = panel_mds.get_antenna(antenna, ddi)
                     surface.export_screws(export_name, unit=unit)
 
 
 def plot_antenna(panel_mds_name, destination, ant_name=None, ddi=None, plot_type='deviation', plot_screws=False,
                  dpi=300, unit=None, parallel=True):
-    """Plot Antenna surfaces from a panel_mds file
+    """ Create diagnostic plots of antenna surface deviations from panel data file. Available plots listed in additional information.
 
     :param panel_mds_name: Input panel_mds file
     :type panel_mds_name: str
     :param destination: Name of the destination folder to contain plots
     :type destination: str
     :param ant_name: List of antennae/antenna to be plotted, defaults to "all" when None
-    :type ant_name: list or str, optional
+    :type ant_name: list or str, optional, ex. ant_ea25
     :param ddi: List of ddis/ddi to be plotted, defaults to "all" when None
-    :type ddi: list or str, optional
+    :type ddi: list or str, optional, ex. ddi_0
     :param plot_type: type of plot to be produced, deviation, phase or ancillary
     :type plot_type: str
     :param plot_screws: Add screw positions to plot
     :type plot_screws: bool
     :param dpi: dots per inch to be used in plots
     :type dpi: int
     :param unit: Unit for phase or deviation plots, defaults to "mm" for deviation and 'deg' for phase
@@ -176,22 +180,26 @@
                     else:
                         _plot_antenna_chunk(parm_dict)
 
     if parallel:
         dask.compute(delayed_list)
 
 def open_holog(file):
-  """Method to return an instance of the holography data object.
+  """ Open holog file and return instance of the holog data object. Object includes summary function to list available dictionary keys.
 
   :param file: Path to holog file.
   :type file: str
   
   :return: Holography holog object.
   :rtype: AstrohackHologFile
 
+  .. _Description:
+  **AstrohackHologFile**
+  Holog object allows the user to access holog data via compound dictionary keys with values, in order of depth, `ddi` -> `map` -> `ant`. The holog object also provides a `summary()` helper function to list available keys for each file. An outline of the holog object structure is show below:
+
   .. parsed-literal::
     holog_mds = 
       {
       ddi_0:{
           map_0:{
                  ant_0: holog_ds,
                           ⋮
@@ -213,22 +221,26 @@
   if _data_file.open():
     return _data_file
 
   else:
     logger.error("Error opening holgraphy file: {file}".format(file))
 
 def open_image(file):
-  """Method to return an instance of the image data object.
+  """ Open image file and return instance of the image data object. Object includes summary function to list available dictionary keys.
 
   :param file: Path to image file.
   :type file: str
   
   :return: Holography image object.
   :rtype: AstrohackImageFile
 
+  .. _Description:
+  **AstrohackImageFile**
+  Image object allows the user to access image data via compound dictionary keys with values, in order of depth, `ant` -> `ddi`. The image object also provides a `summary()` helper function to list available keys for each file. An outline of the image object structure is show below:
+
   .. parsed-literal::
     image_mds = 
       {
         ant_0:{
           ddi_0: image_ds,
                  ⋮               
           ddi_m: image_ds
@@ -246,22 +258,26 @@
   if _data_file.open():
     return _data_file
 
   else:
     logger.error("Error opening holgraphy image file: {file}".format(file))
 
 def open_panel(file):
-  """Method to return an instance of the holography panel object.
+  """ Open panel file and return instance of the panel data object. Object includes summary function to list available dictionary keys.
 
   :param file: Path ot panel file.
   :type file: str
   
   :return: Holography panel object.
   :rtype: AstrohackPanelFile
 
+  .. _Description:
+  **AstrohackPanelFile**
+  Panel object allows the user to access panel data via compound dictionary keys with values, in order of depth, `ant` -> `ddi`. The panel object also provides a `summary()` helper function to list available keys for each file. An outline of the panel object structure is show below:
+
   .. parsed-literal::
     panel_mds = 
       {
         ant_0:{
           ddi_0: panel_ds,
                  ⋮               
           ddi_m: panel_ds
@@ -279,22 +295,27 @@
   if _data_file.open():
     return _data_file
 
   else:
     logger.error("Error opening holgraphy panel file: {file}".format(file))
 
 def open_pointing(file):
-  """Method to return an instance of the holography point object.
+  """ Open pointing file and return instance of the pointing data object. Object includes summary function to list available dictionary keys.
 
   :param file: Path to pointing file.
   :type file: str
   
   :return: Holography pointing object.
   :rtype: AstrohackPointFile
 
+  .. _Description:
+
+  **AstrohackPointFile**
+  Pointing object allows the user to access pointing data via dictionary key with value based on `ant`. The pointing object also provides a `summary()` helper function to list available keys for each file. An outline of the pointing object structure is show below:
+
   .. parsed-literal::
     point_mds = 
       {
         ant_0: point_ds,
             ⋮
         ant_n: point_ds
       }
@@ -308,8 +329,41 @@
   
   if _data_file.open():
     return _data_file
 
   else:
     logger.error("Error opening holgraphy pointing file: {file}".format(file))
 
+def fix_pointing_table(ms_name, reference_antenna):
+  """ Fix pointing table for a user defined subset of reference antennas.
+
+  Args:
+      ms_name (str): Measurement set.
+      reference_antenna (list): List of reference antennas.
+  """
+    
+  ms_table = "/".join((ms_name, 'ANTENNA'))
+
+  query = 'select NAME from {table}'.format(table=ms_table)
+
+  ant_names = np.array(tables.taql(query).getcol('NAME'))
+  ant_id = np.arange(len(ant_names))
+
+  query_ant = np.searchsorted(ant_names, reference_antenna)
+
+  ms_table = "/".join((ms_name, 'POINTING'))
+
+  ant_list = " or ".join(["ANTENNA_ID=={ant}".format(ant=ant) for ant in query_ant])
+
+  update = "update {table} set POINTING_OFFSET=0, TARGET=DIRECTION where {antennas}".format(table=ms_table, antennas=ant_list)
+
+  tables.taql(update)
 
+  ms_table = "/".join((ms_name, "HISTORY"))
+  tb = tables.table(ms_table, readonly=False)
+    
+  message = tb.getcol("MESSAGE")
+    
+  if "pnt_tbl:fixed" not in message:
+    tb.addrows(nrows=1)
+    length = len(message)
+    tb.putcol(columnname="MESSAGE", value='pnt_tbl:fixed', startrow=length)
```

### Comparing `astrohack-0.0.9/src/astrohack/extract_holog.py` & `astrohack-0.1.0/src/astrohack/extract_holog.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 import dask
 import sys
 
 import xarray as xr
 import numpy as np
+import numbers
 
 from casacore import tables as ctables
 
+from astropy.time import Time
+
 from astrohack._utils._constants import pol_str
 
 from astrohack._utils._conversion import _convert_ant_name_to_id
 
-from astrohack._utils._holog import _create_holog_meta_data
-
+from astrohack._utils._extract_holog import _create_holog_meta_data
 from astrohack._utils._extract_point import _extract_pointing
 
 from astrohack._utils._io import _load_point_file
 from astrohack._utils._io import _open_no_dask_zarr
 from astrohack._utils._io import _read_data_from_holog_json
 from astrohack._utils._io import _read_meta_data
 from astrohack._utils._io import _load_holog_file
@@ -25,54 +27,86 @@
 from astrohack._utils._extract_holog import _extract_holog_chunk
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms
 from astrohack._utils._utils import _remove_suffix
 from astrohack._utils._io import _load_holog_file
 
-
 from astrohack._utils._dio import AstrohackHologFile
+
 def extract_holog(
     ms_name,
-    holog_obs_dict,
+    holog_obs_dict=None,
+    ddi_sel=None,
+    baseline_average_distance=None,
     holog_name=None,
     point_name=None,
     data_col="DATA",
     parallel=False,
+    reuse_point_zarr=False,
     overwrite=False,
 ):
     """
     Extract holography and optionally pointing data, from measurement set. Creates holography output file.
 
     :param ms_name: Name of input measurement file name.
     :type ms_name: str
 
-    :param holog_obs_dict: The *holog_obs_dict* describes which scan and antenna data to extract from the measurement set. As detailed below, this compound dictionary also includes important meta data needed for preprocessing and extraction of the holography data from the measurement set.
-    :type holog_obs_dict: dict        
+    :param holog_obs_dict: The *holog_obs_dict* describes which scan and antenna data to extract from the measurement set. As detailed below, this compound dictionary also includes important meta data needed for preprocessing and extraction of the holography data from the measurement set. If not specified holog_obs_dict will be generated. For auto generation of the holog_obs_dict the assumtion is made that the same antanna beam is not mapped twice in a row (alternating sets of antennas is fine).
+    :type holog_obs_dict: dict, optional
+    
+    :param ddi_sel:  Value(s) of DDI that should be extracted from the measurement set. Defaults to all DDI's in the ms.
+    :type ddi_sel: int numpy.ndarray | int list, optional
+       
+    :baseline_average_distance: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_distance is the acceptable distance between a mapping antenna and a reference antenna. The baseline_average_distance is only used if the holog_obs_dict is not specified. If no distance is specified all reference antennas will be used.
+    :type holog_obs_dict: float, optional
 
     :param holog_name: Name of *<holog_name>.holog.zarr* file to create. Defaults to measurement set name with *holog.zarr* extension.
     :type holog_name: str, optional
 
     :param point_name: Name of *<point_name>.point.zarr* file to create. Defaults to measurement set name with *point.zarr* extension.
     :type point_name: str, optional
 
     :param data_col: Determines the data column to pull from the measurement set. Defaults to "DATA"
-    :type data_col: str, optional
+    :type data_col: str, optional, ex. DATA, CORRECTED_DATA
 
     :param parallel: Boolean for whether to process in parallel. Defaults to False
     :type parallel: bool, optional
+    
+    :param reuse_point_zarr: If true the point.zarr specified in point_name is reused.
+    :type reuse_point_zarr: bool, optional
 
     :param overwrite: Boolean for whether to overwrite current holog.zarr and point.zarr files., defaults to False
     :type overwrite: bool, optional
 
     :return: Holography holog object.
     :rtype: AstrohackHologFile
 
     .. _Description:
 
+    **AstrohackHologFile**
+
+    Holog object allows the user to access holog data via compound dictionary keys with values, in order of depth, `ddi` -> `map` -> `ant`. The holog object also provides a `summary()` helper function to list available keys for each file. An outline of the holog object structure is show below:
+
+    .. parsed-literal::
+        holog_mds = 
+        {
+            ddi_0:{
+                map_0:{
+                 ant_0: holog_ds,
+                          ⋮
+                 ant_n: holog_ds
+                },
+                ⋮
+                map_p: …
+            },
+            ⋮
+            ddi_m: …
+        }
+
     **Additional Information**
 
         This function extracts the holography related information from the given measurement file. The data is restructured into an astrohack file format and saved into a file in the form of *<holog_name>.holog.zarr*. The extension *.holog.zarr* is used for all holography files. In addition, the pointing information is recorded into a holography file of format *<pointing_name>.point.zarr*. The extension *.point.zarr* is used for all holography pointing files. 
 
         **holog_obs_dict[holog_mapping_id] (dict):**
         *holog_mapping_id* is a unique, arbitrary, user-defined integer assigned to the data that describes a single complete mapping of the beam.
         
@@ -81,17 +115,14 @@
         * A measurement set can contain more than one mapping of the beam (for example the ALMA data).
     
         **holog_obs_dict[holog_mapping_id][scans] (int | numpy.ndarray | list):**
         All the scans in the measurement set the *holog_mapping_id*.
     
         **holog_obs_dict[holog_mapping_id][ant] (dict):**
         The dictionary keys are the mapping antenna names and the values a list of the reference antennas. See example below.
-    
-        **holog_obs_dict[ddi] (int | numpy.ndarray | list):**
-        Value(s) of DDI that should be extracted from the measurement set.
 
         The below example shows how the *holog_obs_description* dictionary should be laid out. For each *holog_mapping_id* the relevant scans 
         and antennas must be provided. For the `ant` key, an entry is required for each mapping antenna and the accompanying reference antenna(s).
     
         .. parsed-literal::
             holog_obs_description = {
                 'map_0' :{
@@ -104,73 +135,112 @@
                             'DV17', 'DV18', 'DV19', 
                             'DV20', 'DV21', 'DV22', 
                             'DV23', 'DV24', 'DV25'
                         ]
                     }
                 }
             }
-            holog_obs_description['ddi'] = [0]
 
     """
     logger = _get_astrohack_logger()
     
     
     ######### Parameter Checking #########
     extract_holog_parms = _check_extract_holog_parms(ms_name,
                                 holog_obs_dict,
+                                ddi_sel,
+                                baseline_average_distance,
                                 holog_name,
                                 point_name,
                                 data_col,
                                 parallel,
+                                reuse_point_zarr,
                                 overwrite)
     
     check_if_file_exists(extract_holog_parms['ms_name'])
     check_if_file_will_be_overwritten(extract_holog_parms['holog_name'],extract_holog_parms['overwrite'])
     check_if_file_will_be_overwritten(extract_holog_parms['point_name'],extract_holog_parms['overwrite'])
-    #######################################
         
     ############# Exstract pointing infromation and save to point.zarr #############
-#    try:
-#        pnt_dict = _load_point_file(extract_holog_parms['point_name'])
-#    except:
-#        pnt_dict = _make_ant_pnt_dict(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
-    
-    pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
-
-    
-    
-    #### To DO: automatically create holog_obs_dict
-    # from astrohack._utils._extract_holog import _create_holog_obs_dict
-
+    if extract_holog_parms["reuse_point_zarr"]:
+        pnt_dict = _load_point_file(extract_holog_parms['point_name'])
+    else:
+        pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
 
     ######## Get Spectral Windows ########
     ctb = ctables.table(
         os.path.join(extract_holog_parms['ms_name'], "DATA_DESCRIPTION"),
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
     ddi_spw = ctb.getcol("SPECTRAL_WINDOW_ID")
     ddpol_indexol = ctb.getcol("POLARIZATION_ID")
-    ddi = np.arange(len(ddi_spw))
+    ms_ddi = np.arange(len(ddi_spw))
     ctb.close()
 
     ######## Get Antenna IDs and Names ########
     ctb = ctables.table(
         os.path.join(extract_holog_parms['ms_name'], "ANTENNA"),
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
 
-    ant_names = ctb.getcol("NAME")
+    ant_names = np.array(ctb.getcol("NAME"))
     ant_id = np.arange(len(ant_names))
+    ant_pos = ctb.getcol("POSITION")
 
     ctb.close()
+    
+    
+    ######## Get Antenna IDs that are in the main table########
+    ctb = ctables.table(
+        extract_holog_parms['ms_name'],
+        readonly=True,
+        lockoptions={"option": "usernoread"},
+        ack=False,
+    )
 
+    ant1 = np.unique(ctb.getcol("ANTENNA1"))
+    ant2 = np.unique(ctb.getcol("ANTENNA2"))
+    ant_id_main = np.unique(np.append(ant1,ant2))
+    
+    ant_names_main = ant_names[ant_id_main]
+    ctb.close()
+    
+    # Create holog_obs_dict or modify user supplied holog_obs_dict.
+    ddi_sel = extract_holog_parms['ddi_sel']
+    if holog_obs_dict is None: #Automatically create holog_obs_dict
+        from astrohack._utils._extract_holog import _create_holog_obs_dict
+        holog_obs_dict = _create_holog_obs_dict(pnt_dict, extract_holog_parms['baseline_average_distance'],ant_names,ant_pos,ant_names_main)
+        
+        #From the generated holog_obs_dict subselect user supplied ddis.
+        if ddi_sel != 'all':
+            holog_obs_dict_keys = list(holog_obs_dict.keys())
+            for ddi_key in holog_obs_dict_keys:
+                if 'ddi' in ddi_key:
+                    ddi_id = int(ddi_key.replace('ddi_',''))
+                    if ddi_id not in ddi_sel:
+                        del holog_obs_dict[ddi_key]
+    else:
+        #If a user defines a holog_obs_dict it needs to be duplicated for each ddi.
+        holog_obs_dict_with_ddi = {}
+        if ddi_sel == 'all':
+            for ddi_id in ms_ddi:
+                holog_obs_dict_with_ddi['ddi_' + str(ddi_id)] = holog_obs_dict
+        else:
+            for ddi_id in ddi_sel:
+                holog_obs_dict_with_ddi['ddi_' + str(ddi_id)] = holog_obs_dict
+        
+        holog_obs_dict = holog_obs_dict_with_ddi
+            
+    from pprint import pformat
+    logger.info("holog_obs_dict: \n%s", pformat(holog_obs_dict,indent=1,width=1))
+        
     ######## Get Scan and Subscan IDs ########
     # SDM Tables Short Description (https://drive.google.com/file/d/16a3g0GQxgcO7N_ZabfdtexQ8r2jRbYIS/view)
     # 2.54 ScanIntent (p. 150)
     # MAP ANTENNA SURFACE : Holography calibration scan
 
     # 2.61 SubscanIntent (p. 152)
     # MIXED : Pointing measurement, some antennas are on-source, some off-source
@@ -212,23 +282,36 @@
         os.path.join(extract_holog_parms['ms_name'], "OBSERVATION"),
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
     )
     
     telescope_name = obs_ctb.getcol("TELESCOPE_NAME")[0]
+    start_time_unix = obs_ctb.getcol('TIME_RANGE')[0][0] - 3506716800.0
+    time = Time(start_time_unix, format='unix').jyear
+
+    # If we have an EVLA run from before 2023 the pointing table needs to be fixed.
+    if telescope_name == "EVLA" and time < 2023:
+        # Convert from casa epoch to unix time
+        his_ctb = ctables.table(
+            os.path.join(extract_holog_parms['ms_name'], "HISTORY"),
+            readonly=True,
+            lockoptions={"option": "usernoread"},
+            ack=False,
+        )
+    
+        assert ("pnt_tbl:fixed" in his_ctb.getcol("MESSAGE")), "Pointing table not corrected, users should apply function astrohack.dio.fix_pointing_table() to remedy this."
+        
+        his_ctb.close()
 
-    ## DDI selection
-    if holog_obs_dict['ddi'] is None:
-        logger.error("No DDIs in holog_obs_dict.")
-        raise Exception()
 
     delayed_list = []
     
-    for ddi in holog_obs_dict['ddi']:
+    for ddi_name in holog_obs_dict.keys():
+        ddi = int(ddi_name.replace('ddi_',''))
         spw_setup_id = ddi_spw[ddi]
         pol_setup_id = ddpol_indexol[ddi]
         
         extract_holog_parms["ddi"] = ddi
         extract_holog_parms["chan_setup"] = {}
         extract_holog_parms["pol_setup"] = {}
         
@@ -240,116 +323,135 @@
 
         extract_holog_parms["pol_setup"]["pol"] = pol_str[pol_ctb.getcol("CORR_TYPE", startrow=pol_setup_id, nrow=1)[0, :]]
                 
         
         extract_holog_parms["telescope_name"] = obs_ctb.getcol("TELESCOPE_NAME")[0]
         
 
-        for holog_map_key in holog_obs_dict.keys(): #loop over all beam_scan_ids, a beam_scan_id can conist out of more than one scan in an ms (this is the case for the VLA pointed mosiacs).
+        for holog_map_key in holog_obs_dict[ddi_name].keys(): #loop over all beam_scan_ids, a beam_scan_id can conist out of more than one scan in an ms (this is the case for the VLA pointed mosiacs).
 
             if 'map' in holog_map_key:
-                scans = holog_obs_dict[holog_map_key]["scans"]
+                scans = holog_obs_dict[ddi_name][holog_map_key]["scans"]
                 logger.info("Processing ddi: {ddi}, scans: {scans}".format(ddi=ddi, scans=scans))
-            
-                map_ant_list = []
-                ref_ant_per_map_ant_list = [] #
                 
-                map_ant_name_list = []
-                ref_ant_per_map_ant_name_list = [] #
-                for map_ant_str in holog_obs_dict[holog_map_key]['ant'].keys():
-                    ref_ant_ids = np.array(_convert_ant_name_to_id(ant_names,list(holog_obs_dict[holog_map_key]['ant'][map_ant_str])))
-                    map_ant_id = _convert_ant_name_to_id(ant_names,map_ant_str)[0]
-
-                    ref_ant_per_map_ant_list.append(ref_ant_ids)
-                    map_ant_list.append(map_ant_id)
+                if len(list(holog_obs_dict[ddi_name][holog_map_key]['ant'].keys())) != 0:
+                    map_ant_list = []
+                    ref_ant_per_map_ant_list = [] #
                     
-                    ref_ant_per_map_ant_name_list.append(list(holog_obs_dict[holog_map_key]['ant'][map_ant_str]))
-                    map_ant_name_list.append(map_ant_str)
+                    map_ant_name_list = []
+                    ref_ant_per_map_ant_name_list = [] #
+                    for map_ant_str in holog_obs_dict[ddi_name][holog_map_key]['ant'].keys():
+                        ref_ant_ids = np.array(_convert_ant_name_to_id(ant_names,list(holog_obs_dict[ddi_name][holog_map_key]['ant'][map_ant_str])))
+                        
+                        map_ant_id = _convert_ant_name_to_id(ant_names,map_ant_str)[0]
+
+                        ref_ant_per_map_ant_list.append(ref_ant_ids)
+                        map_ant_list.append(map_ant_id)
+                        
+                        ref_ant_per_map_ant_name_list.append(list(holog_obs_dict[ddi_name][holog_map_key]['ant'][map_ant_str]))
+                        map_ant_name_list.append(map_ant_str)
+                        
+                   
 
-                extract_holog_parms["ref_ant_per_map_ant_tuple"] = tuple(ref_ant_per_map_ant_list)
-                extract_holog_parms["map_ant_tuple"] = tuple(map_ant_list)
-                
-                extract_holog_parms["ref_ant_per_map_ant_name_tuple"] = tuple(ref_ant_per_map_ant_name_list)
-                extract_holog_parms["map_ant_name_tuple"] = tuple(map_ant_name_list)
-                
-                extract_holog_parms["scans"] = scans
-                extract_holog_parms["sel_state_ids"] = state_ids
-                extract_holog_parms["holog_map_key"] = holog_map_key
-                extract_holog_parms["ant_names"] = ant_names
-                
-                if parallel:
-                    delayed_list.append(
-                        dask.delayed(_extract_holog_chunk)(
-                            dask.delayed(extract_holog_parms)
+                    extract_holog_parms["ref_ant_per_map_ant_tuple"] = tuple(ref_ant_per_map_ant_list)
+                    extract_holog_parms["map_ant_tuple"] = tuple(map_ant_list)
+                    
+                    extract_holog_parms["ref_ant_per_map_ant_name_tuple"] = tuple(ref_ant_per_map_ant_name_list)
+                    extract_holog_parms["map_ant_name_tuple"] = tuple(map_ant_name_list)
+                    
+                    extract_holog_parms["scans"] = scans
+                    extract_holog_parms["sel_state_ids"] = state_ids
+                    extract_holog_parms["holog_map_key"] = holog_map_key
+                    extract_holog_parms["ant_names"] = ant_names
+                    
+                    if parallel:
+                        delayed_list.append(
+                            dask.delayed(_extract_holog_chunk)(
+                                dask.delayed(extract_holog_parms)
+                            )
                         )
-                    )
+                    else:
+                        _extract_holog_chunk(extract_holog_parms)
                 else:
-                    _extract_holog_chunk(extract_holog_parms)
+                    logger.warning('DDI ' + str(ddi) + ' has no holography data to extract.')
+                     
+     
+    
 
     spw_ctb.close()
     pol_ctb.close()
+    obs_ctb.close()
 
     if parallel:
         dask.compute(delayed_list)    
 
-    extract_holog_parms["holog_obs_dict"] = {}
-
-    for id in ant_id:
-        extract_holog_parms["holog_obs_dict"][str(id)] = ant_names[id]
-
     holog_dict = _load_holog_file(holog_file=extract_holog_parms["holog_name"], dask_load=True, load_pnt_dict=False)
 
+    extract_holog_parms['telescope_name'] = telescope_name
     _create_holog_meta_data(holog_file=extract_holog_parms['holog_name'], holog_dict=holog_dict, holog_params=extract_holog_parms)
     
     holog_mds = AstrohackHologFile(extract_holog_parms['holog_name'])
     holog_mds.open()
     
     return holog_mds
-    
 
 
-def _check_extract_holog_parms(    ms_name,
+
+def _check_extract_holog_parms(
+    ms_name,
     holog_obs_dict,
+    ddi_sel,
+    baseline_average_distance,
     holog_name,
     point_name,
     data_col,
     parallel,
+    reuse_point_zarr,
     overwrite):
     
     extract_holog_parms = {}
     extract_holog_parms["ms_name"] = ms_name
     extract_holog_parms["holog_name"] = holog_name
+    extract_holog_parms["ddi_sel"] = ddi_sel
     extract_holog_parms["point_name"] = point_name
     extract_holog_parms["data_col"] = data_col
     extract_holog_parms["parallel"] = parallel
     extract_holog_parms["overwrite"] = overwrite
+    extract_holog_parms["reuse_point_zarr"] = reuse_point_zarr
+    extract_holog_parms["baseline_average_distance"] = baseline_average_distance
 
     
     #### Parameter Checking ####
     logger = _get_astrohack_logger()
     parms_passed = True
     
     parms_passed = parms_passed and _check_parms(extract_holog_parms, 'ms_name', [str],default=None)
 
     base_name = _remove_suffix(ms_name,'.ms')
     parms_passed = parms_passed and _check_parms(extract_holog_parms,'holog_name', [str],default=base_name+'.holog.zarr')
   
     
     point_base_name = _remove_suffix(extract_holog_parms['holog_name'],'.holog.zarr')
     parms_passed = parms_passed and _check_parms(extract_holog_parms,'point_name', [str],default=point_base_name+'.point.zarr')
+    
+    parms_passed = parms_passed and _check_parms(extract_holog_parms,'ddi_sel', [list,np.ndarray], list_acceptable_data_types=[int], default='all')
   
     #To Do: special function needed to check holog_obs_dict.
-    parm_check = isinstance(holog_obs_dict,dict)
+    parm_check = isinstance(holog_obs_dict,dict) or (holog_obs_dict is None)
     parms_passed = parms_passed and parm_check
     if not parm_check:
         logger.error('Parameter holog_obs_dict must be of type '+ str(dict))
         
+    parms_passed = parms_passed and _check_parms(extract_holog_parms,'baseline_average_distance', [numbers.Number],default='all')
+        
     parms_passed = parms_passed and _check_parms(extract_holog_parms,'data_col', [str],default='DATA')
 
     parms_passed = parms_passed and _check_parms(extract_holog_parms, 'parallel', [bool],default=False)
+    
+    parms_passed = parms_passed and _check_parms(extract_holog_parms, 'reuse_point_zarr', [bool],default=False)
 
     parms_passed = parms_passed and _check_parms(extract_holog_parms, 'overwrite', [bool],default=False)
 
     if not parms_passed:
         logger.error("extract_holog parameter checking failed.")
         raise Exception("extract_holog parameter checking failed.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `astrohack-0.0.9/src/astrohack/holog.py` & `astrohack-0.1.0/src/astrohack/holog.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms
 from astrohack._utils._utils import _remove_suffix
    
 from astrohack._utils._io import check_if_file_will_be_overwritten, check_if_file_exists
 from astrohack._utils._dio import AstrohackImageFile
 
-#fp=open('holog.log','w+')
-#@profile(stream=fp)
 def holog(
     holog_name,
-    grid_size,
-    cell_size,
+    grid_size=None,
+    cell_size=None,
     image_name=None,
     padding_factor=50,
     grid_interpolation_mode="nearest",
     chan_average=True,
     chan_tolerance_factor=0.005,
     reference_scaling_frequency=None,
     scan_average=True,
@@ -35,45 +33,45 @@
     overwrite=False,
     parallel=True):
     """ Process holography data and derive aperture illumination pattern.
 
     :param holog_name: Name of holography .holog.zarr file to process.
     :type holog_name: str
 
-    :param grid_size: Numpy array specifying the dimensions of the grid used in data gridding.
-    :type grid_size: numpy.ndarray, dtype int
+    :param grid_size: Numpy array specifying the dimensions of the grid used in data gridding. If not specified grid_size is calculated using POINTING_OFFSET in pointing table.
+    :type grid_size: numpy.ndarray, dtype int, optional
 
-    :param cell_size: Numpy array defining the cell size of each grid bin.
-    :type cell_size: numpy.ndarray, dtype float
+    :param cell_size: Numpy array defining the cell size of each grid bin. If not specified cell_size is calculated using POINTING_OFFSET in pointing table.
+    :type cell_size: numpy.ndarray, dtype float, optional
 
     :param image_name: Defines the name of the output image name. If value is None, the name will be set to <base_name>.image.zarr, defaults to None
     :type image_name: str, optional
 
     :param padding_factor: Padding factor applied to beam grid before computing the fast-fourier transform. The default has been set for operation on most systems. The user should be aware of memory constraints before increasing this parameter significatly., defaults to 50
     :type padding_factor: int, optional
 
     :param parallel: Run in parallel with Dask or in serial., defaults to True
     :type parallel: bool, optional
 
     :param grid_interpolation_mode: Method of interpolation used when gridding data. This is done using the `scipy.interpolate.griddata` method. For more information on the interpolation see `scipy.interploate <https://docs.scipy.org/doc/scipy/reference/generated/scipy.interpolate.griddata.html#scipy.interpolate.griddata>`_, defaults to "nearest"
-    :type grid_interpolation_mode: str, optional
+    :type grid_interpolation_mode: str, optional. Available options: {"linear", "nearest", "cubic"} 
 
     :param chan_average: Boolean dictating whether the channel average is computed and written to the output holog file., defaults to True
     :type chan_average: bool, optional
 
     :param chan_tolerance_factor: Tolerance used in channel averaging to determine the number of primary beam channels., defaults to 0.005
     :type chan_tolerance_factor: float, optional
 
     :param reference_scaling_frequency: When computing the channel average the lm frequency values are scaled by frequency. If the default None is used, the scaling is simply unity, however if `reference_scaling_frequency` is set then the scaling is done according to (average_frequency/reference_scaling_frequency)., defaults to None
-    :type reference_scaling_frequency: _type_, optional
+    :type reference_scaling_frequency: float, optional
 
     :param scan_average: Boolean dicating whether averagin is done over scan., defaults to True
     :type scan_average: bool, optional
 
-    :param ant_list: Optional list of sub-antennas to use when the user doesn't to do holography for all antennas, defaults to None
+    :param ant_list: Optional list of sub-antennas to use when the user doesn't to do holography for all antennas, defaults to all antennas.
     :type ant_list: list, optional
 
     :param to_stokes: Dictates whether polarization is computed according to stokes values., defaults to True
     :type to_stokes: bool, optional
 
     :param apply_mask: If True applies a mask to the aperture setting values outside of the aperture to zero., defaults to True
     :type apply_mask: bool, optional
@@ -91,14 +89,31 @@
     :type phase_fit: bool, optional
 
     :param overwrite: Overwrite existing files on disk, defaults to False
     :type overwrite: bool, optional
 
     :return: Holography image object.
     :rtype: AstrohackImageFile
+    
+    .. _Description:
+    **AstrohackImageFile**
+
+    Image object allows the user to access image data via compound dictionary keys with values, in order of depth, `ant` -> `ddi`. The image object also provides a `summary()` helper function to list available keys for each file. An outline of the image object structure is show below:
+
+    .. parsed-literal::
+        image_mds = 
+            {
+            ant_0:{
+                ddi_0: image_ds,
+                 ⋮               
+                ddi_m: image_ds
+            },
+            ⋮
+            ant_n: …
+        }
 
     """
     
     logger = _get_astrohack_logger()
     
     holog_params = _check_holog_parms(
         holog_name, 
@@ -133,42 +148,28 @@
         image_name=None,
 
     if  holog_params['ant_list'] == 'all':
         holog_params['ant_list'] = list(holog_json.keys())
         
     logger.info('Mapping antennas ' + str(holog_params['ant_list']))
 
-    ''' VLA data sampling can be uneven so averging step in extracty_holog does not work consequntly int(np.sqrt(meta_data["n_time"])) is not correct.
+    
     if (cell_size is None) and (grid_size is None):
-        ###To Do: Calculate one gridsize and cell_size for all ddi's, antennas, ect. Fix meta data ant_holog_dict gets overwritten for more than one ddi.
-        
-        n_points = int(np.sqrt(meta_data["n_time"]))
-        grid_size = np.array([n_points, n_points])
-
-        l_min_extent = meta_data["extent"]["l"]["min"]
-        l_max_extent = meta_data["extent"]["l"]["max"]
-
-        m_min_extent = meta_data["extent"]["m"]["min"]
-        m_max_extent = meta_data["extent"]["m"]["max"]
-
-        step_l = (l_max_extent - l_min_extent) / grid_size[0]
-        step_m = (m_max_extent - m_min_extent) / grid_size[1]
-        step_l = (step_l+step_m)/2
-        step_m = step_l
-
-        cell_size = np.array([step_l, step_m])
-
-        holog_chunk_params["cell_size"] = cell_size
-        holog_chunk_params["grid_size"] = grid_size
+        n_pix = int(np.sqrt(meta_data["n_pix"]))
+        grid_size = np.array([n_pix, n_pix])
+        cell_size = np.array([-meta_data["cell_size"], meta_data["cell_size"]])
 
+        holog_params["cell_size"] = cell_size
+        holog_params["grid_size"] = grid_size
+        
         logger.info("Cell size: " + str(cell_size) + " Grid size " + str(grid_size))
     else:
-        holog_chunk_params["cell_size"] = cell_size
-        holog_chunk_params["grid_size"] = grid_size
-    '''
+        holog_params["cell_size"] = cell_size
+        holog_params["grid_size"] = grid_size
+    
 
     
     holog_chunk_params =  holog_params
     delayed_list = []
     
     
     for ant_id in holog_chunk_params['ant_list']:
@@ -222,18 +223,20 @@
     
     #### Parameter Checking ####
     logger = _get_astrohack_logger()
     parms_passed = True
     
     parms_passed = parms_passed and _check_parms(holog_params, 'holog_file', [str],default=None)
 
-    parms_passed = parms_passed and _check_parms(holog_params, 'grid_size', [list,np.ndarray], list_acceptable_data_types=[np.int,np.int64], list_len=2, default=None)
+    parms_passed = parms_passed and _check_parms(holog_params, 'grid_size', [list,np.ndarray], list_acceptable_data_types=[np.int,np.int64], list_len=2, default='None',log_default_setting=False)
+    if (isinstance(holog_params['grid_size'],str)) and (holog_params['grid_size'] == 'None'): holog_params['grid_size'] =  None
     holog_params['grid_size'] = np.array(holog_params['grid_size'])
 
-    parms_passed = parms_passed and _check_parms(holog_params, 'cell_size', [list,np.ndarray], list_acceptable_data_types=[numbers.Number], list_len=2, default=None)
+    parms_passed = parms_passed and _check_parms(holog_params, 'cell_size', [list,np.ndarray], list_acceptable_data_types=[numbers.Number], list_len=2, default='None',log_default_setting=False)
+    if (isinstance(holog_params['cell_size'],str)) and (holog_params['cell_size'] == 'None'): holog_params['cell_size'] =  None
     holog_params['cell_size'] = np.array(holog_params['cell_size'])
 
     
     base_name = _remove_suffix(holog_params['holog_file'],'.holog.zarr')
     parms_passed = parms_passed and _check_parms(holog_params,'image_file', [str],default=base_name+'.image.zarr')
     
     parms_passed = parms_passed and _check_parms(holog_params, 'padding_factor', [int], default=50)
@@ -247,16 +250,16 @@
     
     parms_passed = parms_passed and _check_parms(holog_params, 'chan_average', [bool],default=True)
 
     
     parms_passed = parms_passed and _check_parms(holog_params, 'chan_tolerance_factor', [float], acceptable_range=[0,1], default=0.005)
    
     
-    parms_passed = parms_passed and _check_parms(holog_params, 'reference_scaling_frequency', [float,np.float],default='None')
-    if holog_params['reference_scaling_frequency'] == 'None':
+    parms_passed = parms_passed and _check_parms(holog_params, 'reference_scaling_frequency', [float,np.float],default='None',log_default_setting=False)
+    if (isinstance(holog_params['reference_scaling_frequency'],str)) and (holog_params['reference_scaling_frequency']) == 'None':
         holog_params['reference_scaling_frequency'] =  None
     
     parms_passed = parms_passed and _check_parms(holog_params, 'scan_average', [bool],default=True)
 
     parms_passed = parms_passed and _check_parms(holog_params, 'ant_list', [list,np.ndarray], list_acceptable_data_types=[str], default='all')
  
     parms_passed = parms_passed and _check_parms(holog_params, 'to_stokes', [bool],default=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `astrohack-0.0.9/src/astrohack/panel.py` & `astrohack-0.1.0/src/astrohack/panel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 import dask
-import xarray as xr
 import shutil
 
-from astrohack._classes.antenna_surface import AntennaSurface
+import numpy as np
+import xarray as xr
+
 from astrohack._classes.telescope import Telescope
 from astrohack._classes.base_panel import panel_models
-from astrohack._utils._io import _load_image_xds, _aips_holog_to_xds, check_if_file_will_be_overwritten, check_if_file_exists
-from astrohack._utils._panel import _external_to_internal_parameters, _correct_phase
-import numpy as np
+from astrohack._utils._io import _aips_holog_to_xds, check_if_file_will_be_overwritten, check_if_file_exists
+
+from astrohack._utils._panel import _panel_chunk
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms
 from astrohack._utils._utils import _remove_suffix
 
 from astrohack._utils._dio import AstrohackPanelFile
 
 
-def panel(image_name, panel_name=None, cutoff=0.2, panel_model=None, panel_margins=0.2, parallel=False, sel_ddi=None,
-          overwrite=False):
+def panel(image_name, panel_name=None, cutoff=0.2, panel_model=None, panel_margins=0.2, parallel=False, sel_ddi=None, overwrite=False):
     """Analyze holography images to derive panel adjustments
 
     :param image_name: Input holography data file name. Accepted data formats are the output from ``astrohack.holog.holog`` and AIPS holography data prepackaged using ``astrohack.panel.aips_holog_to_astrohack``.
     :type image_name: str
     :param panel_name: Name of output file; File name will be appended with suffix *.panel.zarr*. Defaults to *basename* of input file plus holography panel file suffix.
     :type panel_name: str, optional
     :param cutoff: Relative amplitude cut-off which defines fitting mask. Defaults to 0.2.
@@ -30,15 +30,15 @@
     :param panel_model: Model of surface fitting function used to fit panel surfaces, None will default to "rigid". Possible models are listed below.
     :type panel_model: str, optional
     :param panel_margins: Relative margin from the edge of the panel used to decide which points are margin points or internal points of each panel. Defaults to 0.2.
     :type panel_margins: float, optional
     :param parallel: Run in parallel. Defaults to False.
     :type parallel: bool, optional
     :param sel_ddi: List of DDIs to be processed. None will use all DDIs. Defaults to None.
-    :type sel_ddi: list, optional
+    :type sel_ddi: list, optional, ex. [ddi_0 ... ddi_N]
     :param overwrite: Overwrite files on disk. Defaults to False.
     :type overwrite: bool, optional
 
     :return: Holography panel object.
     :rtype: AstrohackPanelFile
 
     .. _Description:
@@ -70,14 +70,30 @@
             - *corotated_robust*: Tries corotated_lst_sq, if it diverges falls back to corotated_scipy, fast and robust.
         * Experimental fitting models:
             - *xy_paraboloid*: fitted using scipy.optimize, bending axes are parallel to the x and y axes.
             - *rotated_paraboloid*: fitted using scipy.optimize, bending axes can be rotated by any arbitrary angle.
             - *full_paraboloid_lst_sq*: Full 9 parameter paraboloid fitted using least_squares method, tends to heavily overfit surface irregularities.
 
 
+    .. _Description:
+    **AstrohackPanelFile**
+    Panel object allows the user to access panel data via compound dictionary keys with values, in order of depth, `ant` -> `ddi`. The panel object also provides a `summary()` helper function to list available keys for each file. An outline of the panel object structure is show below:
+
+    .. parsed-literal::
+        panel_mds = 
+        {
+            ant_0:{
+                ddi_0: panel_ds,
+                 ⋮               
+                ddi_m: panel_ds
+            },
+            ⋮
+            ant_n: …
+        }
+
     """
     
     logger = _get_astrohack_logger()
     
     panel_params = _check_panel_parms(image_name, panel_name, cutoff, panel_model, panel_margins, parallel, sel_ddi,
                                       overwrite)
           
@@ -119,76 +135,14 @@
         else:
             logger.info("Panel finished processing")
             
             panel_mds = AstrohackPanelFile(panel_chunk_params['panel_name'])
             panel_mds.open()
             return panel_mds
 
-
-def _panel_chunk(panel_chunk_params):
-    """
-    Process a chunk of the holographies, usually a chunk consists of an antenna over a ddi
-    Args:
-        panel_chunk_params: dictionary of inputs
-    """
-    if panel_chunk_params['origin'] == 'AIPS':
-        inputxds = xr.open_zarr(panel_chunk_params['image_name'])
-        telescope = Telescope(inputxds.attrs['telescope_name'])
-        panel_chunk_params['antenna'] = inputxds.attrs['ant_name']
-
-    else:
-        inputxds = _load_image_xds(panel_chunk_params['image_name'],
-                                   panel_chunk_params['antenna'],
-                                   panel_chunk_params['ddi'],
-                                   dask_load=False)
-
-        inputxds.attrs['AIPS'] = False
-
-        if inputxds.attrs['telescope_name'] == "ALMA":
-            tname = inputxds.attrs['telescope_name']+'_'+inputxds.attrs['ant_name'][0:2]
-            telescope = Telescope(tname)
-        elif inputxds.attrs['telescope_name'] == "EVLA":
-            tname = "VLA"
-            telescope = Telescope(tname)
-        else:
-            raise ValueError('Unsuported telescope {0:s}'.format(inputxds.attrs['telescope_name']))
-
-    surface = AntennaSurface(inputxds, telescope, panel_chunk_params['cutoff'], panel_chunk_params['panel_kind'],
-                             panel_margins=panel_chunk_params['panel_margins'])
-
-    surface.compile_panel_points()
-    surface.fit_surface()
-    surface.correct_surface()
-    
-    xds_name = panel_chunk_params['panel_name'] + '/' + panel_chunk_params['antenna'] + '/' + panel_chunk_params['ddi']
-    xds = surface.export_xds()
-    xds.to_zarr(xds_name, mode='w')
-
-
-def _create_phase_model(npix, parameters, wavelength, telescope, cellxy):
-    """
-    Create a phase model with npix by npix size according to the given parameters
-    Args:
-        npix: Number of pixels in each size of the model
-        parameters: Parameters for the phase model in the units described in _phase_fitting
-        wavelength: Observing wavelength, in meters
-        telescope: Telescope object containing the optics parameters
-        cellxy: Map cell spacing, in meters
-
-    Returns:
-
-    """
-    iNPARameters = _external_to_internal_parameters(parameters, wavelength, telescope, cellxy)
-    dummyphase = np.zeros((npix, npix))
-
-    _, model = _correct_phase(dummyphase, cellxy, iNPARameters, telescope.magnification, telescope.focus,
-                              telescope.surp_slope)
-    return model
-
-
 def aips_holog_to_astrohack(amp_image, dev_image, telescope_name, holog_name, overwrite=False):
     """
     Package AIPS HOLOG products in a .image.zarr file compatible with astrohack.panel.panel
 
     This function reads amplitude and deviation FITS files produced by AIPS's HOLOG task and transfers their data onto a
     .image.zarr file that can be read by panel.
     Most of the meta data can be inferred from the FITS headers, but it remains necessary to specify the telescope name
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `astrohack-0.0.9/src/astrohack/profiling.py` & `astrohack-0.1.0/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack/visualization/viewer.py` & `astrohack-0.1.0/src/astrohack/visualization/viewer.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.1.0/src/astrohack.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.0.9
+Version: 0.1.0
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
 
-# astroHACK
+![astrohack](docs/_media/astrohack_logo.png)
 
 [![Python 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
 [![Documentation Status](https://readthedocs.org/projects/astrohack/badge/?version=latest)](https://astrohack.readthedocs.io/en/latest/?badge=latest)
 
 
 astroHack (Holography Antenna Commissioning Kit) is a Python package that produces antenna aperture images and panel adjustment corrections from calibrated holography measurement sets. Initially, it will support holography data from the VLA and ALMA, with the future goal of supporting the ngVLA. Much of the core functionality from the following AIPS tasks has been ported: UVHOL, HOLOG, and PANEL. astroHack enables parallel execution by using Dask and efficient single-threaded performance by making use of Numba.
```

### Comparing `astrohack-0.0.9/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.1.0/src/astrohack.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,18 @@
 src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
 src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
 src/astrohack/_utils/_logger/__init__.py
 src/astrohack/_utils/_logger/_astrohack_logger.py
 src/astrohack/_utils/_parm_utils/__init__.py
 src/astrohack/_utils/_parm_utils/_check_logger_parms.py
 src/astrohack/_utils/_parm_utils/_check_parms.py
+src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json
+src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json
+src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json
+src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json
 src/astrohack/data/telescopes/__init__.py
 src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
 src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
 src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
 src/astrohack/data/telescopes/alma_da.zarr/.zattrs
 src/astrohack/data/telescopes/alma_da.zarr/.zgroup
 src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
```

### Comparing `astrohack-0.0.9/src/astrohack.egg-info/requires.txt` & `astrohack-0.1.0/src/astrohack.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/tests/test_class_antenna_surface.py` & `astrohack-0.1.0/tests/test_class_antenna_surface.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/tests/test_class_base_panel.py` & `astrohack-0.1.0/tests/test_class_base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/tests/test_class_ring_panel.py` & `astrohack-0.1.0/tests/test_class_ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.9/tests/test_class_telescope.py` & `astrohack-0.1.0/tests/test_class_telescope.py`

 * *Files identical despite different names*


# Comparing `tmp/portfolyo-0.5.0.tar.gz` & `tmp/portfolyo-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolyo-0.5.0.tar", last modified: Wed Apr 26 14:45:37 2023, max compression
+gzip compressed data, was "portfolyo-0.5.1.tar", last modified: Sat Apr 29 17:06:08 2023, max compression
```

## Comparing `portfolyo-0.5.0.tar` & `portfolyo-0.5.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.997611 portfolyo-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-26 14:45:18.000000 portfolyo-0.5.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-26 14:45:18.000000 portfolyo-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-26 14:45:36.997611 portfolyo-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-26 14:45:18.000000 portfolyo-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.997611 portfolyo-0.5.0/portfolyo/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-26 14:45:36.997611 portfolyo-0.5.0/portfolyo/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.989611 portfolyo-0.5.0/portfolyo/core/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/extendpandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.989611 portfolyo-0.5.0/portfolyo/core/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/mixins/other.py
--rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/mixins/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/mixins/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/ndframelike.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.989611 portfolyo-0.5.0/portfolyo/core/pfline/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/enable_arithmatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/flat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/flat_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/interop.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfline/nested_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.989611 portfolyo-0.5.0/portfolyo/core/pfstate/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfstate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfstate/enable_arithmatic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfstate/pfstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/pfstate/pfstate_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/core/suppresswarnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.989611 portfolyo-0.5.0/portfolyo/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/dev/develop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/dev/mockup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.993611 portfolyo-0.5.0/portfolyo/prices/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/prices/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/prices/hedge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/prices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.993611 portfolyo-0.5.0/portfolyo/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/testing/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.997611 portfolyo-0.5.0/portfolyo/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/ceil.py
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/changefreq.py
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/changeyear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/floor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/freq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/isboundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/leftandright.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/peakperiod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/right.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/righttoleft.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/round.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/standardize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/trim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/tzone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/unitdefinitions.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/tools/wavg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.997611 portfolyo-0.5.0/portfolyo/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/visualize/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/visualize/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-04-26 14:45:18.000000 portfolyo-0.5.0/portfolyo/visualize/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:36.985611 portfolyo-0.5.0/portfolyo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-26 14:45:36.000000 portfolyo-0.5.0/portfolyo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-26 14:45:36.000000 portfolyo-0.5.0/portfolyo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:45:36.000000 portfolyo-0.5.0/portfolyo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:45:36.000000 portfolyo-0.5.0/portfolyo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 14:45:36.000000 portfolyo-0.5.0/portfolyo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 14:45:36.000000 portfolyo-0.5.0/portfolyo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 14:45:18.000000 portfolyo-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-26 14:45:36.997611 portfolyo-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-26 14:45:18.000000 portfolyo-0.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-26 14:45:19.000000 portfolyo-0.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.361255 portfolyo-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-29 17:05:54.000000 portfolyo-0.5.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-29 17:05:54.000000 portfolyo-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-29 17:06:08.361255 portfolyo-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-29 17:05:54.000000 portfolyo-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.361255 portfolyo-0.5.1/portfolyo/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 17:06:08.361255 portfolyo-0.5.1/portfolyo/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.349255 portfolyo-0.5.1/portfolyo/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/extendpandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.349255 portfolyo-0.5.1/portfolyo/core/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/mixins/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/mixins/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/mixins/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/ndframelike.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.357255 portfolyo-0.5.1/portfolyo/core/pfline/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/enable_arithmatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/flat_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/nested_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.357255 portfolyo-0.5.1/portfolyo/core/pfstate/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfstate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfstate/enable_arithmatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfstate/pfstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfstate/pfstate_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/suppresswarnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.357255 portfolyo-0.5.1/portfolyo/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/dev/develop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/dev/mockup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.357255 portfolyo-0.5.1/portfolyo/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/prices/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/prices/hedge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/prices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.357255 portfolyo-0.5.1/portfolyo/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/testing/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.361255 portfolyo-0.5.1/portfolyo/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/ceil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/changefreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/changeyear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/floor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/freq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/isboundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/leftandright.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/peakperiod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/right.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/righttoleft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/round.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/standardize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/tzone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/unitdefinitions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/wavg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.361255 portfolyo-0.5.1/portfolyo/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/visualize/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/visualize/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/visualize/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.345255 portfolyo-0.5.1/portfolyo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-29 17:06:08.000000 portfolyo-0.5.1/portfolyo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-29 17:06:08.000000 portfolyo-0.5.1/portfolyo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:06:08.000000 portfolyo-0.5.1/portfolyo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:06:08.000000 portfolyo-0.5.1/portfolyo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-29 17:06:08.000000 portfolyo-0.5.1/portfolyo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 17:06:08.000000 portfolyo-0.5.1/portfolyo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-29 17:05:54.000000 portfolyo-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-29 17:06:08.361255 portfolyo-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-29 17:05:54.000000 portfolyo-0.5.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-29 17:05:54.000000 portfolyo-0.5.1/versioneer.py
```

### Comparing `portfolyo-0.5.0/LICENCE` & `portfolyo-0.5.1/LICENCE`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/PKG-INFO` & `portfolyo-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolyo
-Version: 0.5.0
+Version: 0.5.1
 Summary: Analysing and manipulating timeseries related to power and gas offtake portfolios.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENCE
 
 portfolyo
```

### Comparing `portfolyo-0.5.0/README.rst` & `portfolyo-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/__init__.py` & `portfolyo-0.5.1/portfolyo/__init__.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/core/mixins/other.py` & `portfolyo-0.5.1/portfolyo/core/mixins/other.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/core/mixins/plot.py` & `portfolyo-0.5.1/portfolyo/core/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/core/mixins/text.py` & `portfolyo-0.5.1/portfolyo/core/mixins/text.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/core/ndframelike.py` & `portfolyo-0.5.1/portfolyo/core/ndframelike.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/core/pfline/base.py` & `portfolyo-0.5.1/portfolyo/core/pfline/base.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/core/pfline/enable_arithmatic.py` & `portfolyo-0.5.1/portfolyo/core/pfline/enable_arithmatic.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/core/pfline/flat.py` & `portfolyo-0.5.1/portfolyo/core/pfline/flat.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/core/pfline/flat_helper.py` & `portfolyo-0.5.1/portfolyo/core/pfline/flat_helper.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/core/pfline/interop.py` & `portfolyo-0.5.1/portfolyo/core/pfline/interop.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/core/pfline/nested.py` & `portfolyo-0.5.1/portfolyo/core/pfline/nested.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/core/pfline/nested_helper.py` & `portfolyo-0.5.1/portfolyo/core/pfline/nested_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Verify input data and turn into object needed in NestedPfLine instantiation."""
 
 from __future__ import annotations
 
 from typing import Any, Dict, Mapping, Tuple
-
+from collections import defaultdict
 import pandas as pd
 
 from ... import tools
 from .base import Kind, PfLine
 
 
 def make_mapping(data: Any) -> Mapping[Any, Any]:
@@ -39,15 +39,20 @@
     if len(idx) == 0:
         raise ValueError("PfLine indices have no overlap.")
     children = {name: child.loc[idx] for name, child in children.items()}
 
     # Kind of children.
     kindset = set([child.kind for child in children.values()])
     if len(kindset) != 1:
-        raise ValueError(f"All children must be of the same kind; found {kindset}.")
+        kinds1 = defaultdict(list)
+        for name, child in children.items():
+            kinds1[child.kind].append(name)
+        kinds2 = {kind: ", ".join(names) for kind, names in kinds1.items()}
+        kinds3 = " and ".join([f"{kind} ({names})" for kind, names in kinds2.items()])
+        raise ValueError(f"All children must be of the same kind; found {kinds3}.")
     kind = next(iter(kindset))
 
     return children, kind
 
 
 def dataframe(children: Dict[str, PfLine], kind: Kind) -> pd.DataFrame:
     """Create dataframe with aggregated values."""
```

### Comparing `portfolyo-0.5.0/portfolyo/core/pfstate/enable_arithmatic.py` & `portfolyo-0.5.1/portfolyo/core/pfstate/enable_arithmatic.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/core/pfstate/pfstate.py` & `portfolyo-0.5.1/portfolyo/core/pfstate/pfstate.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/core/pfstate/pfstate_helper.py` & `portfolyo-0.5.1/portfolyo/core/pfstate/pfstate_helper.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/dev/develop.py` & `portfolyo-0.5.1/portfolyo/dev/develop.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/dev/mockup.py` & `portfolyo-0.5.1/portfolyo/dev/mockup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 from ..prices.utils import is_peak_hour
 from ..tools import unit  # noqa # ensure we use current ureg
 
 
 def w_offtake(
     i: pd.DatetimeIndex,
-    avg: float = 100,
+    avg: float = 100.0,
     year_amp: float = 0.20,
     week_amp: float = 0.10,
     day_amp: float = 0.30,
     rand_amp: float = 0.02,
     has_unit: bool = True,
 ) -> pd.Series:
     """Create a more or less realistic-looking offtake timeseries.
 
     Parameters
     ----------
     i : pd.DatetimeIndex
         Timestamps for which to create offtake.
-    avg : float, optional (default: 100)
+    avg : float, optional (default: 100.0)
         Average offtake in MW.
     year_amp : float, optional (default: 0.2)
         Yearly amplitude as fraction of average. If positive: winter offtake > summer offtake.
     week_amp : float, optional (default: 0.1)
         Weekly amplitude as fraction of average. If positive: midweek offtake > weekend offtake.
     day_amp : float, optional (default: 0.3)
         Day amplitude as fraction of average. If positive: midday offtake > night offtake.
@@ -59,27 +59,27 @@
     rv = rand_amp * (1 + 2 * np.random.rand(len(i)))  # TODO: Random mean-reverting walk
     s = pd.Series(avg * (1 + yv + dv + wv + rv), i, name="w")
     return s if not has_unit else s.astype("pint[MW]")
 
 
 def p_marketprices(
     i: pd.DatetimeIndex,
-    avg: float = 100,
+    avg: float = 100.0,
     year_amp: float = 0.30,
     week_amp: float = 0.05,
     peak_amp: float = 0.30,
     has_unit: bool = True,
 ) -> pd.Series:
     """Create a more or less realistic-looking forward price curve timeseries.
 
     Parameters
     ----------
     i : pd.DatetimeIndex
         Timestamps for which to create prices.
-    avg : float, optional (default: 100)
+    avg : float, optional (default: 100.0)
         Average price in Eur/MWh.
     year_amp : float, optional (default: 0.3)
         Yearly amplitude as fraction of average. If positive: winter prices > summer prices.
     week_amp : float, optional (default: 0.05)
         Weekly amplitude as fraction of average. If positive: midweek prices > weekend prices.
     peak_amp : float, optional (default: 0.3)
         Peak-offpeak amplitude as fraction of average. If positive: peak prices > offpeak prices.
@@ -117,29 +117,29 @@
     return s if not has_unit else s.astype("pint[Eur/MWh]")
 
 
 def wp_sourced(
     w_offtake: pd.Series,
     freq: str = "MS",
     w_avg: float = 0.6,
-    p_avg: float = 100,
+    p_avg: float = 100.0,
     rand_amp: float = 0.2,
     has_unit: bool = True,
 ) -> Tuple[pd.Series]:
     """Create a more or less realistic-looking sourcing volume and sourcing price timeseries.
 
     Parameters
     ----------
     w_offtake : pd.Series
         Offtake volume timeseries for which to create sourced volume and price timeseries.
     freq : str, optional (default: 'MS')
         Frequency within which sourcing volume and price are uniform.
     w_avg : float, optional (default: 0.6)
         Average sourced fraction.
-    p_avg : float, optional (default: 100)
+    p_avg : float, optional (default: 100.0)
         Average hedge price in Eur/MWh.
     rand_amp : float, optional (default: 0.2)
         Random amplitude, both of sourced fraction (absolute) and of price (as fraction).
     has_unit : bool, optional (default: True)
         If True, return Series with unit.
         - volume series: same unit as ``w_offtake`` or else with pint unit in MW.
         - price series: with pint unit in Eur/MWh.
```

### Comparing `portfolyo-0.5.0/portfolyo/prices/convert.py` & `portfolyo-0.5.1/portfolyo/prices/convert.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/prices/hedge.py` & `portfolyo-0.5.1/portfolyo/prices/hedge.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/prices/utils.py` & `portfolyo-0.5.1/portfolyo/prices/utils.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/testing/testing.py` & `portfolyo-0.5.1/portfolyo/testing/testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,24 +49,24 @@
 
 
 def assert_w_q_compatible(freq: str, w: pd.Series, q: pd.Series):
     """Assert if timeseries with power- and energy-values are consistent."""
     if freq == "15T":
         assert_series_equal(q, w * Q_(0.25, "h"), check_names=False)
     elif freq == "H":
-        assert_series_equal(q, w * Q_(1, "h"), check_names=False)
+        assert_series_equal(q, w * Q_(1.0, "h"), check_names=False)
     elif freq == "D":
         assert (q >= w * Q_(22.99, "h")).all()
         assert (q <= w * Q_(25.01, "h")).all()
     elif freq == "MS":
-        assert (q >= w * 27 * Q_(24, "h")).all()
-        assert (q <= w * 32 * Q_(24, "h")).all()
+        assert (q >= w * 27 * Q_(24.0, "h")).all()
+        assert (q <= w * 32 * Q_(24.0, "h")).all()
     elif freq == "QS":
-        assert (q >= w * 89 * Q_(24, "h")).all()
-        assert (q <= w * 93 * Q_(24, "h")).all()
+        assert (q >= w * 89 * Q_(24.0, "h")).all()
+        assert (q <= w * 93 * Q_(24.0, "h")).all()
     elif freq == "AS":
         assert (q >= w * Q_(8759.9, "h")).all()
         assert (q <= w * Q_(8784.1, "h")).all()
     else:
         raise ValueError(f"Uncaught value for freq: {freq}.")
```

### Comparing `portfolyo-0.5.0/portfolyo/tools/ceil.py` & `portfolyo-0.5.1/portfolyo/tools/ceil.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/changefreq.py` & `portfolyo-0.5.1/portfolyo/tools/changefreq.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/changeyear.py` & `portfolyo-0.5.1/portfolyo/tools/changeyear.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/duration.py` & `portfolyo-0.5.1/portfolyo/tools/duration.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/floor.py` & `portfolyo-0.5.1/portfolyo/tools/floor.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/frame.py` & `portfolyo-0.5.1/portfolyo/tools/frame.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/freq.py` & `portfolyo-0.5.1/portfolyo/tools/freq.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/intersect.py` & `portfolyo-0.5.1/portfolyo/tools/intersect.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/isboundary.py` & `portfolyo-0.5.1/portfolyo/tools/isboundary.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/leftandright.py` & `portfolyo-0.5.1/portfolyo/tools/leftandright.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/peakperiod.py` & `portfolyo-0.5.1/portfolyo/tools/peakperiod.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/right.py` & `portfolyo-0.5.1/portfolyo/tools/right.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/righttoleft.py` & `portfolyo-0.5.1/portfolyo/tools/righttoleft.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/round.py` & `portfolyo-0.5.1/portfolyo/tools/round.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/standardize.py` & `portfolyo-0.5.1/portfolyo/tools/standardize.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/trim.py` & `portfolyo-0.5.1/portfolyo/tools/trim.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/tzone.py` & `portfolyo-0.5.1/portfolyo/tools/tzone.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/unit.py` & `portfolyo-0.5.1/portfolyo/tools/unit.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/unitdefinitions.txt` & `portfolyo-0.5.1/portfolyo/tools/unitdefinitions.txt`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/tools/wavg.py` & `portfolyo-0.5.1/portfolyo/tools/wavg.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/visualize/categories.py` & `portfolyo-0.5.1/portfolyo/visualize/categories.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/visualize/colors.py` & `portfolyo-0.5.1/portfolyo/visualize/colors.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo/visualize/plot.py` & `portfolyo-0.5.1/portfolyo/visualize/plot.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/portfolyo.egg-info/PKG-INFO` & `portfolyo-0.5.1/portfolyo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolyo
-Version: 0.5.0
+Version: 0.5.1
 Summary: Analysing and manipulating timeseries related to power and gas offtake portfolios.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENCE
 
 portfolyo
```

### Comparing `portfolyo-0.5.0/portfolyo.egg-info/SOURCES.txt` & `portfolyo-0.5.1/portfolyo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/setup.py` & `portfolyo-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.0/versioneer.py` & `portfolyo-0.5.1/versioneer.py`

 * *Files identical despite different names*


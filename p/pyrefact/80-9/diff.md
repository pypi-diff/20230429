# Comparing `tmp/pyrefact-80.tar.gz` & `tmp/pyrefact-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrefact-80.tar", last modified: Sat Apr 29 13:50:16 2023, max compression
+gzip compressed data, was "pyrefact-9.tar", last modified: Wed Nov  2 20:30:27 2022, max compression
```

## Comparing `pyrefact-80.tar` & `pyrefact-9.tar`

### file list

```diff
@@ -1,32 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:50:16.311955 pyrefact-80/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-29 13:50:03.000000 pyrefact-80/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-29 13:50:16.311955 pyrefact-80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-29 13:50:03.000000 pyrefact-80/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-29 13:50:03.000000 pyrefact-80/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:50:16.311955 pyrefact-80/pyrefact/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26865 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/abstractions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)   139990 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/logs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12808 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/object_oriented.py
--rw-r--r--   0 runner    (1001) docker     (123)    40172 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/performance_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/performance_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-29 13:50:03.000000 pyrefact-80/pyrefact/symbolic_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:50:16.311955 pyrefact-80/pyrefact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-29 13:50:16.000000 pyrefact-80/pyrefact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-29 13:50:16.000000 pyrefact-80/pyrefact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:50:16.000000 pyrefact-80/pyrefact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-29 13:50:16.000000 pyrefact-80/pyrefact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-29 13:50:16.000000 pyrefact-80/pyrefact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 13:50:16.000000 pyrefact-80/pyrefact.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 13:50:16.311955 pyrefact-80/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:50:16.311955 pyrefact-80/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-29 13:50:03.000000 pyrefact-80/tests/testing_infra.py
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.405663 pyrefact-9/
+-rw-r--r--   0 olle       (501) staff       (20)     1069 2022-10-20 08:55:02.000000 pyrefact-9/LICENSE
+-rw-r--r--   0 olle       (501) staff       (20)      228 2022-11-02 20:30:27.405542 pyrefact-9/PKG-INFO
+-rw-r--r--   0 olle       (501) staff       (20)     1262 2022-11-02 18:36:20.000000 pyrefact-9/README.md
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.404795 pyrefact-9/pyrefact/
+-rw-r--r--   0 olle       (501) staff       (20)        0 2022-10-23 21:51:04.000000 pyrefact-9/pyrefact/__init__.py
+-rwxr-xr-x   0 olle       (501) staff       (20)      120 2022-10-20 18:11:25.000000 pyrefact-9/pyrefact/__main__.py
+-rw-r--r--   0 olle       (501) staff       (20)     2148 2022-11-02 19:54:47.000000 pyrefact-9/pyrefact/completion.py
+-rw-r--r--   0 olle       (501) staff       (20)     1065 2022-10-30 20:04:01.000000 pyrefact-9/pyrefact/constants.py
+-rw-r--r--   0 olle       (501) staff       (20)    31081 2022-11-02 20:24:19.000000 pyrefact-9/pyrefact/fixes.py
+-rwxr-xr-x   0 olle       (501) staff       (20)     3867 2022-11-02 12:50:20.000000 pyrefact-9/pyrefact/main.py
+-rw-r--r--   0 olle       (501) staff       (20)    12892 2022-11-02 19:54:47.000000 pyrefact-9/pyrefact/parsing.py
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.405383 pyrefact-9/pyrefact.egg-info/
+-rw-r--r--   0 olle       (501) staff       (20)      228 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/PKG-INFO
+-rw-r--r--   0 olle       (501) staff       (20)      327 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/SOURCES.txt
+-rw-r--r--   0 olle       (501) staff       (20)        1 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/dependency_links.txt
+-rw-r--r--   0 olle       (501) staff       (20)       40 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/requires.txt
+-rw-r--r--   0 olle       (501) staff       (20)        9 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/top_level.txt
+-rw-r--r--   0 olle       (501) staff       (20)       38 2022-11-02 20:30:27.405698 pyrefact-9/setup.cfg
+-rw-r--r--   0 olle       (501) staff       (20)      468 2022-11-02 20:30:04.000000 pyrefact-9/setup.py
```

### Comparing `pyrefact-80/LICENSE` & `pyrefact-9/LICENSE`

 * *Files identical despite different names*


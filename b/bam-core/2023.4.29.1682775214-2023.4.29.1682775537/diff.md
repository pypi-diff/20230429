# Comparing `tmp/bam-core-2023.4.29.1682775214.tar.gz` & `tmp/bam-core-2023.4.29.1682775537.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bam-core-2023.4.29.1682775214.tar", last modified: Sat Apr 29 13:33:36 2023, max compression
+gzip compressed data, was "bam-core-2023.4.29.1682775537.tar", last modified: Sat Apr 29 13:38:59 2023, max compression
```

## Comparing `bam-core-2023.4.29.1682775214.tar` & `bam-core-2023.4.29.1682775537.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:36.461665 bam-core-2023.4.29.1682775214/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-29 13:33:36.461665 bam-core-2023.4.29.1682775214/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:36.457665 bam-core-2023.4.29.1682775214/bam_core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-29 13:33:34.000000 bam-core-2023.4.29.1682775214/bam_core/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:36.461665 bam-core-2023.4.29.1682775214/bam_core/lib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2346 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/lib/airtable.py
--rw-r--r--   0 runner    (1001) docker     (122)     6410 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/lib/listmonk.py
--rw-r--r--   0 runner    (1001) docker     (122)    14789 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/lib/s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:36.461665 bam-core-2023.4.29.1682775214/bam_core/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/utils/etc.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/utils/phone.py
--rw-r--r--   0 runner    (1001) docker     (122)     6007 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/utils/serde.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:36.461665 bam-core-2023.4.29.1682775214/bam_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-29 13:33:36.000000 bam-core-2023.4.29.1682775214/bam_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-04-29 13:33:36.000000 bam-core-2023.4.29.1682775214/bam_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-29 13:33:36.000000 bam-core-2023.4.29.1682775214/bam_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-29 13:33:36.000000 bam-core-2023.4.29.1682775214/bam_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-29 13:33:36.000000 bam-core-2023.4.29.1682775214/bam_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-29 13:33:36.461665 bam-core-2023.4.29.1682775214/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:36.461665 bam-core-2023.4.29.1682775214/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/tests/test_serde.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:38:59.528501 bam-core-2023.4.29.1682775537/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-29 13:38:59.528501 bam-core-2023.4.29.1682775537/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-29 13:38:37.000000 bam-core-2023.4.29.1682775537/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:38:59.528501 bam-core-2023.4.29.1682775537/bam_core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:38:37.000000 bam-core-2023.4.29.1682775537/bam_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-29 13:38:57.000000 bam-core-2023.4.29.1682775537/bam_core/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:38:59.528501 bam-core-2023.4.29.1682775537/bam_core/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:38:37.000000 bam-core-2023.4.29.1682775537/bam_core/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2346 2023-04-29 13:38:37.000000 bam-core-2023.4.29.1682775537/bam_core/lib/airtable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6410 2023-04-29 13:38:37.000000 bam-core-2023.4.29.1682775537/bam_core/lib/listmonk.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14789 2023-04-29 13:38:37.000000 bam-core-2023.4.29.1682775537/bam_core/lib/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-04-29 13:38:37.000000 bam-core-2023.4.29.1682775537/bam_core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:38:59.528501 bam-core-2023.4.29.1682775537/bam_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:38:37.000000 bam-core-2023.4.29.1682775537/bam_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-04-29 13:38:37.000000 bam-core-2023.4.29.1682775537/bam_core/utils/etc.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:38:37.000000 bam-core-2023.4.29.1682775537/bam_core/utils/phone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6007 2023-04-29 13:38:37.000000 bam-core-2023.4.29.1682775537/bam_core/utils/serde.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:38:59.528501 bam-core-2023.4.29.1682775537/bam_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-29 13:38:59.000000 bam-core-2023.4.29.1682775537/bam_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-04-29 13:38:59.000000 bam-core-2023.4.29.1682775537/bam_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-29 13:38:59.000000 bam-core-2023.4.29.1682775537/bam_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-29 13:38:59.000000 bam-core-2023.4.29.1682775537/bam_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-29 13:38:59.000000 bam-core-2023.4.29.1682775537/bam_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-29 13:38:59.528501 bam-core-2023.4.29.1682775537/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-04-29 13:38:37.000000 bam-core-2023.4.29.1682775537/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:38:59.528501 bam-core-2023.4.29.1682775537/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:38:37.000000 bam-core-2023.4.29.1682775537/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-04-29 13:38:37.000000 bam-core-2023.4.29.1682775537/tests/test_serde.py
```

### Comparing `bam-core-2023.4.29.1682775214/bam_core/lib/airtable.py` & `bam-core-2023.4.29.1682775537/bam_core/lib/airtable.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682775214/bam_core/lib/listmonk.py` & `bam-core-2023.4.29.1682775537/bam_core/lib/listmonk.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682775214/bam_core/lib/s3.py` & `bam-core-2023.4.29.1682775537/bam_core/lib/s3.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682775214/bam_core/settings.py` & `bam-core-2023.4.29.1682775537/bam_core/settings.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682775214/bam_core/utils/etc.py` & `bam-core-2023.4.29.1682775537/bam_core/utils/etc.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682775214/bam_core/utils/serde.py` & `bam-core-2023.4.29.1682775537/bam_core/utils/serde.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682775214/setup.py` & `bam-core-2023.4.29.1682775537/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/bam-core-2023.4.29.1682779611.tar.gz` & `tmp/bam-core-2023.4.29.1682779659.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bam-core-2023.4.29.1682779611.tar", last modified: Sat Apr 29 14:46:52 2023, max compression
+gzip compressed data, was "bam-core-2023.4.29.1682779659.tar", last modified: Sat Apr 29 14:47:40 2023, max compression
```

## Comparing `bam-core-2023.4.29.1682779611.tar` & `bam-core-2023.4.29.1682779659.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 14:46:52.105554 bam-core-2023.4.29.1682779611/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-29 14:46:52.105554 bam-core-2023.4.29.1682779611/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 14:46:52.105554 bam-core-2023.4.29.1682779611/bam_core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/bam_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-29 14:46:51.000000 bam-core-2023.4.29.1682779611/bam_core/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 14:46:52.105554 bam-core-2023.4.29.1682779611/bam_core/lib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/bam_core/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/bam_core/lib/airtable.py
--rw-r--r--   0 runner    (1001) docker     (122)     6410 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/bam_core/lib/listmonk.py
--rw-r--r--   0 runner    (1001) docker     (122)    14799 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/bam_core/lib/s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/bam_core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 14:46:52.105554 bam-core-2023.4.29.1682779611/bam_core/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/bam_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/bam_core/utils/etc.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/bam_core/utils/phone.py
--rw-r--r--   0 runner    (1001) docker     (122)     6007 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/bam_core/utils/serde.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 14:46:52.105554 bam-core-2023.4.29.1682779611/bam_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-29 14:46:52.000000 bam-core-2023.4.29.1682779611/bam_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-04-29 14:46:52.000000 bam-core-2023.4.29.1682779611/bam_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-29 14:46:52.000000 bam-core-2023.4.29.1682779611/bam_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-29 14:46:52.000000 bam-core-2023.4.29.1682779611/bam_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-29 14:46:52.000000 bam-core-2023.4.29.1682779611/bam_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-29 14:46:52.105554 bam-core-2023.4.29.1682779611/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 14:46:52.105554 bam-core-2023.4.29.1682779611/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      392 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/tests/test_security.py
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-04-29 14:46:28.000000 bam-core-2023.4.29.1682779611/tests/test_serde.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 14:47:40.123872 bam-core-2023.4.29.1682779659/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-29 14:47:40.123872 bam-core-2023.4.29.1682779659/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 14:47:40.123872 bam-core-2023.4.29.1682779659/bam_core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/bam_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-29 14:47:39.000000 bam-core-2023.4.29.1682779659/bam_core/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 14:47:40.123872 bam-core-2023.4.29.1682779659/bam_core/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/bam_core/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/bam_core/lib/airtable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6410 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/bam_core/lib/listmonk.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14799 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/bam_core/lib/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/bam_core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 14:47:40.123872 bam-core-2023.4.29.1682779659/bam_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/bam_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/bam_core/utils/etc.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/bam_core/utils/phone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6007 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/bam_core/utils/serde.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 14:47:40.123872 bam-core-2023.4.29.1682779659/bam_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-29 14:47:40.000000 bam-core-2023.4.29.1682779659/bam_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-04-29 14:47:40.000000 bam-core-2023.4.29.1682779659/bam_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-29 14:47:40.000000 bam-core-2023.4.29.1682779659/bam_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-29 14:47:40.000000 bam-core-2023.4.29.1682779659/bam_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-29 14:47:40.000000 bam-core-2023.4.29.1682779659/bam_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-29 14:47:40.123872 bam-core-2023.4.29.1682779659/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 14:47:40.123872 bam-core-2023.4.29.1682779659/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/tests/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-04-29 14:47:22.000000 bam-core-2023.4.29.1682779659/tests/test_serde.py
```

### Comparing `bam-core-2023.4.29.1682779611/bam_core/lib/airtable.py` & `bam-core-2023.4.29.1682779659/bam_core/lib/airtable.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682779611/bam_core/lib/listmonk.py` & `bam-core-2023.4.29.1682779659/bam_core/lib/listmonk.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682779611/bam_core/lib/s3.py` & `bam-core-2023.4.29.1682779659/bam_core/lib/s3.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682779611/bam_core/settings.py` & `bam-core-2023.4.29.1682779659/bam_core/settings.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682779611/bam_core/utils/etc.py` & `bam-core-2023.4.29.1682779659/bam_core/utils/etc.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682779611/bam_core/utils/serde.py` & `bam-core-2023.4.29.1682779659/bam_core/utils/serde.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682779611/setup.py` & `bam-core-2023.4.29.1682779659/setup.py`

 * *Files identical despite different names*


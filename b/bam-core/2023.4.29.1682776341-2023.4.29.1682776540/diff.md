# Comparing `tmp/bam-core-2023.4.29.1682776341.tar.gz` & `tmp/bam-core-2023.4.29.1682776540.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bam-core-2023.4.29.1682776341.tar", last modified: Sat Apr 29 13:52:32 2023, max compression
+gzip compressed data, was "bam-core-2023.4.29.1682776540.tar", last modified: Sat Apr 29 13:56:15 2023, max compression
```

## Comparing `bam-core-2023.4.29.1682776341.tar` & `bam-core-2023.4.29.1682776540.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 13:52:32.515447 bam-core-2023.4.29.1682776341/
--rw-r--r--   0 music      (501) staff       (20)       43 2023-04-29 13:48:13.000000 bam-core-2023.4.29.1682776341/MANIFEST.in
--rw-r--r--   0 music      (501) staff       (20)      203 2023-04-29 13:52:32.515091 bam-core-2023.4.29.1682776341/PKG-INFO
--rw-r--r--   0 music      (501) staff       (20)       62 2023-04-29 02:17:40.000000 bam-core-2023.4.29.1682776341/README.md
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 13:52:32.507652 bam-core-2023.4.29.1682776341/bam_core/
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:38:01.000000 bam-core-2023.4.29.1682776341/bam_core/__init__.py
--rw-r--r--   0 music      (501) staff       (20)       32 2023-04-29 13:52:21.000000 bam-core-2023.4.29.1682776341/bam_core/__version__.py
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 13:52:32.511736 bam-core-2023.4.29.1682776341/bam_core/lib/
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:39:14.000000 bam-core-2023.4.29.1682776341/bam_core/lib/__init__.py
--rw-r--r--   0 music      (501) staff       (20)     2346 2023-04-28 21:46:59.000000 bam-core-2023.4.29.1682776341/bam_core/lib/airtable.py
--rw-r--r--   0 music      (501) staff       (20)     6410 2023-04-29 02:40:34.000000 bam-core-2023.4.29.1682776341/bam_core/lib/listmonk.py
--rw-r--r--   0 music      (501) staff       (20)    14799 2023-04-29 13:48:13.000000 bam-core-2023.4.29.1682776341/bam_core/lib/s3.py
--rw-r--r--   0 music      (501) staff       (20)     1961 2023-04-29 13:28:36.000000 bam-core-2023.4.29.1682776341/bam_core/settings.py
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 13:52:32.513435 bam-core-2023.4.29.1682776341/bam_core/utils/
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:41:46.000000 bam-core-2023.4.29.1682776341/bam_core/utils/__init__.py
--rw-r--r--   0 music      (501) staff       (20)      913 2023-04-28 21:41:46.000000 bam-core-2023.4.29.1682776341/bam_core/utils/etc.py
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:41:46.000000 bam-core-2023.4.29.1682776341/bam_core/utils/phone.py
--rw-r--r--   0 music      (501) staff       (20)     6007 2023-04-29 02:21:08.000000 bam-core-2023.4.29.1682776341/bam_core/utils/serde.py
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 13:52:32.509997 bam-core-2023.4.29.1682776341/bam_core.egg-info/
--rw-r--r--   0 music      (501) staff       (20)      203 2023-04-29 13:52:32.000000 bam-core-2023.4.29.1682776341/bam_core.egg-info/PKG-INFO
--rw-r--r--   0 music      (501) staff       (20)      501 2023-04-29 13:52:32.000000 bam-core-2023.4.29.1682776341/bam_core.egg-info/SOURCES.txt
--rw-r--r--   0 music      (501) staff       (20)        1 2023-04-29 13:52:32.000000 bam-core-2023.4.29.1682776341/bam_core.egg-info/dependency_links.txt
--rw-r--r--   0 music      (501) staff       (20)       46 2023-04-29 13:52:32.000000 bam-core-2023.4.29.1682776341/bam_core.egg-info/requires.txt
--rw-r--r--   0 music      (501) staff       (20)       15 2023-04-29 13:52:32.000000 bam-core-2023.4.29.1682776341/bam_core.egg-info/top_level.txt
--rw-r--r--   0 music      (501) staff       (20)       46 2023-04-28 21:54:19.000000 bam-core-2023.4.29.1682776341/requirements.txt
--rw-r--r--   0 music      (501) staff       (20)       38 2023-04-29 13:52:32.515536 bam-core-2023.4.29.1682776341/setup.cfg
--rw-r--r--   0 music      (501) staff       (20)      598 2023-04-29 02:48:20.000000 bam-core-2023.4.29.1682776341/setup.py
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 13:52:32.514544 bam-core-2023.4.29.1682776341/tests/
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-29 02:31:15.000000 bam-core-2023.4.29.1682776341/tests/__init__.py
--rw-r--r--   0 music      (501) staff       (20)      200 2023-04-29 02:38:14.000000 bam-core-2023.4.29.1682776341/tests/test_serde.py
+drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 13:56:15.051495 bam-core-2023.4.29.1682776540/
+-rw-r--r--   0 music      (501) staff       (20)       43 2023-04-29 13:48:13.000000 bam-core-2023.4.29.1682776540/MANIFEST.in
+-rw-r--r--   0 music      (501) staff       (20)      203 2023-04-29 13:56:15.051089 bam-core-2023.4.29.1682776540/PKG-INFO
+-rw-r--r--   0 music      (501) staff       (20)       62 2023-04-29 02:17:40.000000 bam-core-2023.4.29.1682776540/README.md
+drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 13:56:15.042725 bam-core-2023.4.29.1682776540/bam_core/
+-rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:38:01.000000 bam-core-2023.4.29.1682776540/bam_core/__init__.py
+-rw-r--r--   0 music      (501) staff       (20)       32 2023-04-29 13:55:40.000000 bam-core-2023.4.29.1682776540/bam_core/__version__.py
+drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 13:56:15.047667 bam-core-2023.4.29.1682776540/bam_core/lib/
+-rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:39:14.000000 bam-core-2023.4.29.1682776540/bam_core/lib/__init__.py
+-rw-r--r--   0 music      (501) staff       (20)     2346 2023-04-28 21:46:59.000000 bam-core-2023.4.29.1682776540/bam_core/lib/airtable.py
+-rw-r--r--   0 music      (501) staff       (20)     6410 2023-04-29 02:40:34.000000 bam-core-2023.4.29.1682776540/bam_core/lib/listmonk.py
+-rw-r--r--   0 music      (501) staff       (20)    14799 2023-04-29 13:48:13.000000 bam-core-2023.4.29.1682776540/bam_core/lib/s3.py
+-rw-r--r--   0 music      (501) staff       (20)     1961 2023-04-29 13:28:36.000000 bam-core-2023.4.29.1682776540/bam_core/settings.py
+drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 13:56:15.049537 bam-core-2023.4.29.1682776540/bam_core/utils/
+-rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:41:46.000000 bam-core-2023.4.29.1682776540/bam_core/utils/__init__.py
+-rw-r--r--   0 music      (501) staff       (20)      913 2023-04-28 21:41:46.000000 bam-core-2023.4.29.1682776540/bam_core/utils/etc.py
+-rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:41:46.000000 bam-core-2023.4.29.1682776540/bam_core/utils/phone.py
+-rw-r--r--   0 music      (501) staff       (20)     6007 2023-04-29 02:21:08.000000 bam-core-2023.4.29.1682776540/bam_core/utils/serde.py
+drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 13:56:15.045370 bam-core-2023.4.29.1682776540/bam_core.egg-info/
+-rw-r--r--   0 music      (501) staff       (20)      203 2023-04-29 13:56:15.000000 bam-core-2023.4.29.1682776540/bam_core.egg-info/PKG-INFO
+-rw-r--r--   0 music      (501) staff       (20)      501 2023-04-29 13:56:15.000000 bam-core-2023.4.29.1682776540/bam_core.egg-info/SOURCES.txt
+-rw-r--r--   0 music      (501) staff       (20)        1 2023-04-29 13:56:15.000000 bam-core-2023.4.29.1682776540/bam_core.egg-info/dependency_links.txt
+-rw-r--r--   0 music      (501) staff       (20)       60 2023-04-29 13:56:15.000000 bam-core-2023.4.29.1682776540/bam_core.egg-info/requires.txt
+-rw-r--r--   0 music      (501) staff       (20)       15 2023-04-29 13:56:15.000000 bam-core-2023.4.29.1682776540/bam_core.egg-info/top_level.txt
+-rw-r--r--   0 music      (501) staff       (20)       59 2023-04-29 13:55:33.000000 bam-core-2023.4.29.1682776540/requirements.txt
+-rw-r--r--   0 music      (501) staff       (20)       38 2023-04-29 13:56:15.051609 bam-core-2023.4.29.1682776540/setup.cfg
+-rw-r--r--   0 music      (501) staff       (20)      598 2023-04-29 02:48:20.000000 bam-core-2023.4.29.1682776540/setup.py
+drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 13:56:15.050442 bam-core-2023.4.29.1682776540/tests/
+-rw-r--r--   0 music      (501) staff       (20)        0 2023-04-29 02:31:15.000000 bam-core-2023.4.29.1682776540/tests/__init__.py
+-rw-r--r--   0 music      (501) staff       (20)      200 2023-04-29 02:38:14.000000 bam-core-2023.4.29.1682776540/tests/test_serde.py
```

### Comparing `bam-core-2023.4.29.1682776341/bam_core/lib/airtable.py` & `bam-core-2023.4.29.1682776540/bam_core/lib/airtable.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682776341/bam_core/lib/listmonk.py` & `bam-core-2023.4.29.1682776540/bam_core/lib/listmonk.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682776341/bam_core/lib/s3.py` & `bam-core-2023.4.29.1682776540/bam_core/lib/s3.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682776341/bam_core/settings.py` & `bam-core-2023.4.29.1682776540/bam_core/settings.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682776341/bam_core/utils/etc.py` & `bam-core-2023.4.29.1682776540/bam_core/utils/etc.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682776341/bam_core/utils/serde.py` & `bam-core-2023.4.29.1682776540/bam_core/utils/serde.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.29.1682776341/setup.py` & `bam-core-2023.4.29.1682776540/setup.py`

 * *Files identical despite different names*


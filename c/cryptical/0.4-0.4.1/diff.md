# Comparing `tmp/cryptical-0.4.tar.gz` & `tmp/cryptical-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptical-0.4.tar", last modified: Fri Apr 28 20:58:11 2023, max compression
+gzip compressed data, was "cryptical-0.4.1.tar", last modified: Sat Apr 29 06:11:07 2023, max compression
```

## Comparing `cryptical-0.4.tar` & `cryptical-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:58:11.746568 cryptical-0.4/
--rw-r--r--   0 harshit   (1000) harshit   (1000)      150 2023-04-28 20:58:11.746568 cryptical-0.4/PKG-INFO
--rw-r--r--   0 harshit   (1000) harshit   (1000)      785 2023-04-28 20:18:30.000000 cryptical-0.4/README.md
-drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:58:11.743568 cryptical-0.4/cryptical/
--rw-r--r--   0 harshit   (1000) harshit   (1000)     8656 2023-04-28 20:56:55.000000 cryptical-0.4/cryptical/cryptical.py
-drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:58:11.745568 cryptical-0.4/cryptical.egg-info/
--rw-r--r--   0 harshit   (1000) harshit   (1000)      150 2023-04-28 20:58:11.000000 cryptical-0.4/cryptical.egg-info/PKG-INFO
--rw-r--r--   0 harshit   (1000) harshit   (1000)      241 2023-04-28 20:58:11.000000 cryptical-0.4/cryptical.egg-info/SOURCES.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)        1 2023-04-28 20:58:11.000000 cryptical-0.4/cryptical.egg-info/dependency_links.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)       55 2023-04-28 20:58:11.000000 cryptical-0.4/cryptical.egg-info/entry_points.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)       75 2023-04-28 20:58:11.000000 cryptical-0.4/cryptical.egg-info/requires.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)       10 2023-04-28 20:58:11.000000 cryptical-0.4/cryptical.egg-info/top_level.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)       38 2023-04-28 20:58:11.746568 cryptical-0.4/setup.cfg
--rw-r--r--   0 harshit   (1000) harshit   (1000)      496 2023-04-28 20:57:43.000000 cryptical-0.4/setup.py
+drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-29 06:11:07.844056 cryptical-0.4.1/
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      152 2023-04-29 06:11:07.843055 cryptical-0.4.1/PKG-INFO
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      785 2023-04-28 20:18:30.000000 cryptical-0.4.1/README.md
+drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-29 06:11:07.843055 cryptical-0.4.1/cryptical.egg-info/
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      152 2023-04-29 06:11:07.000000 cryptical-0.4.1/cryptical.egg-info/PKG-INFO
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      218 2023-04-29 06:11:07.000000 cryptical-0.4.1/cryptical.egg-info/SOURCES.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)        1 2023-04-29 06:11:07.000000 cryptical-0.4.1/cryptical.egg-info/dependency_links.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)       55 2023-04-29 06:11:07.000000 cryptical-0.4.1/cryptical.egg-info/entry_points.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)       75 2023-04-29 06:11:07.000000 cryptical-0.4.1/cryptical.egg-info/requires.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)        1 2023-04-29 06:11:07.000000 cryptical-0.4.1/cryptical.egg-info/top_level.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)       38 2023-04-29 06:11:07.844056 cryptical-0.4.1/setup.cfg
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      515 2023-04-29 06:11:04.000000 cryptical-0.4.1/setup.py
```

### Comparing `cryptical-0.4/README.md` & `cryptical-0.4.1/README.md`

 * *Files identical despite different names*


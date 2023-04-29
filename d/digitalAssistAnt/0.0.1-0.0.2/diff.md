# Comparing `tmp/digitalAssistAnt-0.0.1.tar.gz` & `tmp/digitalAssistAnt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalAssistAnt-0.0.1.tar", last modified: Fri Apr 28 08:42:15 2023, max compression
+gzip compressed data, was "digitalAssistAnt-0.0.2.tar", last modified: Sat Apr 29 10:34:10 2023, max compression
```

## Comparing `digitalAssistAnt-0.0.1.tar` & `digitalAssistAnt-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-28 08:42:15.219806 digitalAssistAnt-0.0.1/
--rw-r--r--   0 svj        (502) staff       (20)     1076 2023-04-28 07:36:19.000000 digitalAssistAnt-0.0.1/LICENSE
--rw-r--r--   0 svj        (502) staff       (20)      268 2023-04-28 08:42:15.219690 digitalAssistAnt-0.0.1/PKG-INFO
--rw-r--r--   0 svj        (502) staff       (20)        0 2023-04-28 07:32:22.000000 digitalAssistAnt-0.0.1/README.md
--rw-r--r--   0 svj        (502) staff       (20)      365 2023-04-28 08:41:40.000000 digitalAssistAnt-0.0.1/pyproject.toml
--rw-r--r--   0 svj        (502) staff       (20)       38 2023-04-28 08:42:15.219840 digitalAssistAnt-0.0.1/setup.cfg
-drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-28 08:42:15.218243 digitalAssistAnt-0.0.1/src/
-drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-28 08:42:15.219006 digitalAssistAnt-0.0.1/src/digitalAssistAnt/
--rw-r--r--   0 svj        (502) staff       (20)        0 2023-04-28 07:30:05.000000 digitalAssistAnt-0.0.1/src/digitalAssistAnt/__init__.py
--rw-r--r--   0 svj        (502) staff       (20)       38 2023-04-28 07:31:36.000000 digitalAssistAnt-0.0.1/src/digitalAssistAnt/main.py
-drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-28 08:42:15.219550 digitalAssistAnt-0.0.1/src/digitalAssistAnt.egg-info/
--rw-r--r--   0 svj        (502) staff       (20)      268 2023-04-28 08:42:15.000000 digitalAssistAnt-0.0.1/src/digitalAssistAnt.egg-info/PKG-INFO
--rw-r--r--   0 svj        (502) staff       (20)      270 2023-04-28 08:42:15.000000 digitalAssistAnt-0.0.1/src/digitalAssistAnt.egg-info/SOURCES.txt
--rw-r--r--   0 svj        (502) staff       (20)        1 2023-04-28 08:42:15.000000 digitalAssistAnt-0.0.1/src/digitalAssistAnt.egg-info/dependency_links.txt
--rw-r--r--   0 svj        (502) staff       (20)       17 2023-04-28 08:42:15.000000 digitalAssistAnt-0.0.1/src/digitalAssistAnt.egg-info/top_level.txt
+drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-29 10:34:10.469036 digitalAssistAnt-0.0.2/
+-rw-r--r--   0 svj        (502) staff       (20)     1076 2023-04-28 07:36:19.000000 digitalAssistAnt-0.0.2/LICENSE
+-rw-r--r--   0 svj        (502) staff       (20)      268 2023-04-29 10:34:10.468916 digitalAssistAnt-0.0.2/PKG-INFO
+-rw-r--r--   0 svj        (502) staff       (20)        0 2023-04-28 07:32:22.000000 digitalAssistAnt-0.0.2/README.md
+-rw-r--r--   0 svj        (502) staff       (20)      365 2023-04-29 10:32:56.000000 digitalAssistAnt-0.0.2/pyproject.toml
+-rw-r--r--   0 svj        (502) staff       (20)       38 2023-04-29 10:34:10.469068 digitalAssistAnt-0.0.2/setup.cfg
+drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-29 10:34:10.466996 digitalAssistAnt-0.0.2/src/
+drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-29 10:34:10.468237 digitalAssistAnt-0.0.2/src/digitalAssistAnt/
+-rw-r--r--   0 svj        (502) staff       (20)        0 2023-04-28 07:30:05.000000 digitalAssistAnt-0.0.2/src/digitalAssistAnt/__init__.py
+-rw-r--r--   0 svj        (502) staff       (20)     1342 2023-04-29 10:21:01.000000 digitalAssistAnt-0.0.2/src/digitalAssistAnt/keys.py
+-rw-r--r--   0 svj        (502) staff       (20)       38 2023-04-28 07:31:36.000000 digitalAssistAnt-0.0.2/src/digitalAssistAnt/main.py
+-rw-r--r--   0 svj        (502) staff       (20)      832 2023-04-29 10:20:27.000000 digitalAssistAnt-0.0.2/src/digitalAssistAnt/util.py
+drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-29 10:34:10.468770 digitalAssistAnt-0.0.2/src/digitalAssistAnt.egg-info/
+-rw-r--r--   0 svj        (502) staff       (20)      268 2023-04-29 10:34:10.000000 digitalAssistAnt-0.0.2/src/digitalAssistAnt.egg-info/PKG-INFO
+-rw-r--r--   0 svj        (502) staff       (20)      328 2023-04-29 10:34:10.000000 digitalAssistAnt-0.0.2/src/digitalAssistAnt.egg-info/SOURCES.txt
+-rw-r--r--   0 svj        (502) staff       (20)        1 2023-04-29 10:34:10.000000 digitalAssistAnt-0.0.2/src/digitalAssistAnt.egg-info/dependency_links.txt
+-rw-r--r--   0 svj        (502) staff       (20)       17 2023-04-29 10:34:10.000000 digitalAssistAnt-0.0.2/src/digitalAssistAnt.egg-info/top_level.txt
```

### Comparing `digitalAssistAnt-0.0.1/LICENSE` & `digitalAssistAnt-0.0.2/LICENSE`

 * *Files identical despite different names*


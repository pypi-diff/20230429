# Comparing `tmp/digitalAssistAnt-0.0.3.tar.gz` & `tmp/digitalAssistAnt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalAssistAnt-0.0.3.tar", last modified: Sat Apr 29 11:14:48 2023, max compression
+gzip compressed data, was "digitalAssistAnt-0.0.4.tar", last modified: Sat Apr 29 11:18:44 2023, max compression
```

## Comparing `digitalAssistAnt-0.0.3.tar` & `digitalAssistAnt-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-29 11:14:48.075385 digitalAssistAnt-0.0.3/
--rw-r--r--   0 svj        (502) staff       (20)     1076 2023-04-28 07:36:19.000000 digitalAssistAnt-0.0.3/LICENSE
--rw-r--r--   0 svj        (502) staff       (20)      268 2023-04-29 11:14:48.075265 digitalAssistAnt-0.0.3/PKG-INFO
--rw-r--r--   0 svj        (502) staff       (20)        0 2023-04-28 07:32:22.000000 digitalAssistAnt-0.0.3/README.md
--rw-r--r--   0 svj        (502) staff       (20)      365 2023-04-29 11:14:32.000000 digitalAssistAnt-0.0.3/pyproject.toml
--rw-r--r--   0 svj        (502) staff       (20)       38 2023-04-29 11:14:48.075415 digitalAssistAnt-0.0.3/setup.cfg
-drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-29 11:14:48.072412 digitalAssistAnt-0.0.3/src/
-drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-29 11:14:48.074415 digitalAssistAnt-0.0.3/src/digitalAssistAnt/
--rw-r--r--   0 svj        (502) staff       (20)        0 2023-04-28 07:30:05.000000 digitalAssistAnt-0.0.3/src/digitalAssistAnt/__init__.py
--rw-r--r--   0 svj        (502) staff       (20)     1342 2023-04-29 10:21:01.000000 digitalAssistAnt-0.0.3/src/digitalAssistAnt/keys.py
--rw-r--r--   0 svj        (502) staff       (20)       38 2023-04-28 07:31:36.000000 digitalAssistAnt-0.0.3/src/digitalAssistAnt/main.py
--rw-r--r--   0 svj        (502) staff       (20)      832 2023-04-29 10:20:27.000000 digitalAssistAnt-0.0.3/src/digitalAssistAnt/util.py
-drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-29 11:14:48.075113 digitalAssistAnt-0.0.3/src/digitalAssistAnt.egg-info/
--rw-r--r--   0 svj        (502) staff       (20)      268 2023-04-29 11:14:48.000000 digitalAssistAnt-0.0.3/src/digitalAssistAnt.egg-info/PKG-INFO
--rw-r--r--   0 svj        (502) staff       (20)      328 2023-04-29 11:14:48.000000 digitalAssistAnt-0.0.3/src/digitalAssistAnt.egg-info/SOURCES.txt
--rw-r--r--   0 svj        (502) staff       (20)        1 2023-04-29 11:14:48.000000 digitalAssistAnt-0.0.3/src/digitalAssistAnt.egg-info/dependency_links.txt
--rw-r--r--   0 svj        (502) staff       (20)       17 2023-04-29 11:14:48.000000 digitalAssistAnt-0.0.3/src/digitalAssistAnt.egg-info/top_level.txt
+drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-29 11:18:44.956179 digitalAssistAnt-0.0.4/
+-rw-r--r--   0 svj        (502) staff       (20)     1076 2023-04-28 07:36:19.000000 digitalAssistAnt-0.0.4/LICENSE
+-rw-r--r--   0 svj        (502) staff       (20)      268 2023-04-29 11:18:44.956065 digitalAssistAnt-0.0.4/PKG-INFO
+-rw-r--r--   0 svj        (502) staff       (20)        0 2023-04-28 07:32:22.000000 digitalAssistAnt-0.0.4/README.md
+-rw-r--r--   0 svj        (502) staff       (20)      365 2023-04-29 11:18:21.000000 digitalAssistAnt-0.0.4/pyproject.toml
+-rw-r--r--   0 svj        (502) staff       (20)       38 2023-04-29 11:18:44.956219 digitalAssistAnt-0.0.4/setup.cfg
+drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-29 11:18:44.954759 digitalAssistAnt-0.0.4/src/
+drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-29 11:18:44.955492 digitalAssistAnt-0.0.4/src/digitalAssistAnt/
+-rw-r--r--   0 svj        (502) staff       (20)        0 2023-04-28 07:30:05.000000 digitalAssistAnt-0.0.4/src/digitalAssistAnt/__init__.py
+-rw-r--r--   0 svj        (502) staff       (20)     1348 2023-04-29 11:17:51.000000 digitalAssistAnt-0.0.4/src/digitalAssistAnt/keys.py
+-rw-r--r--   0 svj        (502) staff       (20)       38 2023-04-28 07:31:36.000000 digitalAssistAnt-0.0.4/src/digitalAssistAnt/main.py
+-rw-r--r--   0 svj        (502) staff       (20)      832 2023-04-29 10:20:27.000000 digitalAssistAnt-0.0.4/src/digitalAssistAnt/util.py
+drwxr-xr-x   0 svj        (502) staff       (20)        0 2023-04-29 11:18:44.955932 digitalAssistAnt-0.0.4/src/digitalAssistAnt.egg-info/
+-rw-r--r--   0 svj        (502) staff       (20)      268 2023-04-29 11:18:44.000000 digitalAssistAnt-0.0.4/src/digitalAssistAnt.egg-info/PKG-INFO
+-rw-r--r--   0 svj        (502) staff       (20)      328 2023-04-29 11:18:44.000000 digitalAssistAnt-0.0.4/src/digitalAssistAnt.egg-info/SOURCES.txt
+-rw-r--r--   0 svj        (502) staff       (20)        1 2023-04-29 11:18:44.000000 digitalAssistAnt-0.0.4/src/digitalAssistAnt.egg-info/dependency_links.txt
+-rw-r--r--   0 svj        (502) staff       (20)       17 2023-04-29 11:18:44.000000 digitalAssistAnt-0.0.4/src/digitalAssistAnt.egg-info/top_level.txt
```

### Comparing `digitalAssistAnt-0.0.3/LICENSE` & `digitalAssistAnt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `digitalAssistAnt-0.0.3/src/digitalAssistAnt/keys.py` & `digitalAssistAnt-0.0.4/src/digitalAssistAnt/keys.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
-import util
-
+from . import util
 def precheck():
     try:
         config = util.loadConfigFile()  
         keyFolderPathExists  = util.checkIfPathExists(config['keys']['path'])
         if(keyFolderPathExists):
             return True
         else:
```

### Comparing `digitalAssistAnt-0.0.3/src/digitalAssistAnt/util.py` & `digitalAssistAnt-0.0.4/src/digitalAssistAnt/util.py`

 * *Files identical despite different names*


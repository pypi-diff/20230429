# Comparing `tmp/Screeny-0.0.2.tar.gz` & `tmp/screeny-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Screeny-0.0.2.tar", last modified: Thu Apr 27 20:03:58 2023, max compression
+gzip compressed data, was "screeny-0.0.3.tar", last modified: Fri Apr 28 22:35:10 2023, max compression
```

## Comparing `Screeny-0.0.2.tar` & `screeny-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-04-27 20:03:58.294351 Screeny-0.0.2/
--rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-27 17:10:22.000000 Screeny-0.0.2/LICENSE
--rw-r--r--   0 paulpol    (501) staff       (20)      505 2023-04-27 20:03:58.293991 Screeny-0.0.2/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)       71 2023-04-27 17:09:15.000000 Screeny-0.0.2/README.md
--rw-r--r--   0 paulpol    (501) staff       (20)      537 2023-04-27 20:02:33.000000 Screeny-0.0.2/pyproject.toml
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-04-27 20:03:58.288428 Screeny-0.0.2/screeny/
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-04-27 20:03:58.291137 Screeny-0.0.2/screeny/src/
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-04-27 20:03:58.293461 Screeny-0.0.2/screeny/src/Screeny.egg-info/
--rw-r--r--   0 paulpol    (501) staff       (20)      505 2023-04-27 20:03:58.000000 Screeny-0.0.2/screeny/src/Screeny.egg-info/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)      278 2023-04-27 20:03:58.000000 Screeny-0.0.2/screeny/src/Screeny.egg-info/SOURCES.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-04-27 20:03:58.000000 Screeny-0.0.2/screeny/src/Screeny.egg-info/dependency_links.txt
--rw-r--r--   0 paulpol    (501) staff       (20)       32 2023-04-27 20:03:58.000000 Screeny-0.0.2/screeny/src/Screeny.egg-info/requires.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-04-27 20:03:58.000000 Screeny-0.0.2/screeny/src/Screeny.egg-info/top_level.txt
--rw-r--r--   0 paulpol    (501) staff       (20)      727 2023-04-27 19:39:34.000000 Screeny-0.0.2/screeny/src/screeny.py
--rw-r--r--   0 paulpol    (501) staff       (20)       38 2023-04-27 20:03:58.294460 Screeny-0.0.2/setup.cfg
--rw-r--r--   0 paulpol    (501) staff       (20)     1215 2023-04-27 17:24:13.000000 Screeny-0.0.2/setup.py
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-04-28 22:35:10.684476 screeny-0.0.3/
+-rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.0.3/LICENSE
+-rw-r--r--   0 paulpol    (501) staff       (20)    23170 2023-04-28 17:23:31.000000 screeny-0.0.3/LICENSE-3RD-Party.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)      451 2023-04-28 22:35:10.684645 screeny-0.0.3/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)       71 2023-04-27 17:09:15.000000 screeny-0.0.3/README.md
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-04-28 22:35:10.681933 screeny-0.0.3/Screeny.egg-info/
+-rw-r--r--   0 paulpol    (501) staff       (20)      451 2023-04-28 22:35:10.000000 screeny-0.0.3/Screeny.egg-info/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)      411 2023-04-28 22:35:10.000000 screeny-0.0.3/Screeny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-04-28 22:35:10.000000 screeny-0.0.3/Screeny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)       32 2023-04-28 22:35:10.000000 screeny-0.0.3/Screeny.egg-info/requires.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-04-28 22:35:10.000000 screeny-0.0.3/Screeny.egg-info/top_level.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-04-28 18:10:34.000000 screeny-0.0.3/pyproject.toml
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-04-28 22:35:10.683324 screeny-0.0.3/screeny/
+-rw-r--r--   0 paulpol    (501) staff       (20)       28 2023-04-28 18:03:41.000000 screeny-0.0.3/screeny/__init__.py
+-rw-r--r--   0 paulpol    (501) staff       (20)      727 2023-04-27 19:39:34.000000 screeny-0.0.3/screeny/screeny.py
+-rw-r--r--   0 paulpol    (501) staff       (20)      503 2023-04-28 22:35:10.685281 screeny-0.0.3/setup.cfg
```

### Comparing `Screeny-0.0.2/LICENSE` & `screeny-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Screeny-0.0.2/screeny/src/screeny.py` & `screeny-0.0.3/screeny/screeny.py`

 * *Files identical despite different names*


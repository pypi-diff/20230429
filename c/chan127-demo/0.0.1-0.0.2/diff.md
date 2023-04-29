# Comparing `tmp/chan127-demo-0.0.1.tar.gz` & `tmp/chan127-demo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chan127-demo-0.0.1.tar", last modified: Sat Apr 29 11:24:00 2023, max compression
+gzip compressed data, was "dist/chan127-demo-0.0.2.tar", last modified: Sat Apr 29 11:29:50 2023, max compression
```

## Comparing `chan127-demo-0.0.1.tar` & `chan127-demo-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 11:24:00.000000 chan127-demo-0.0.1/
--rw-r--r--   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 10:46:38.000000 chan127-demo-0.0.1/MANIFEST.in
--rw-r--r--   0 cheukkaichan   (501) staff       (20)      199 2023-04-29 11:24:00.000000 chan127-demo-0.0.1/PKG-INFO
-drwxr-xr-x   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 11:24:00.000000 chan127-demo-0.0.1/chan127_demo.egg-info/
--rw-r--r--   0 cheukkaichan   (501) staff       (20)      199 2023-04-29 11:24:00.000000 chan127-demo-0.0.1/chan127_demo.egg-info/PKG-INFO
--rw-r--r--   0 cheukkaichan   (501) staff       (20)      272 2023-04-29 11:24:00.000000 chan127-demo-0.0.1/chan127_demo.egg-info/SOURCES.txt
--rw-r--r--   0 cheukkaichan   (501) staff       (20)        1 2023-04-29 11:24:00.000000 chan127-demo-0.0.1/chan127_demo.egg-info/dependency_links.txt
--rw-r--r--   0 cheukkaichan   (501) staff       (20)       55 2023-04-29 11:24:00.000000 chan127-demo-0.0.1/chan127_demo.egg-info/entry_points.txt
--rw-r--r--   0 cheukkaichan   (501) staff       (20)       19 2023-04-29 11:24:00.000000 chan127-demo-0.0.1/chan127_demo.egg-info/requires.txt
--rw-r--r--   0 cheukkaichan   (501) staff       (20)        7 2023-04-29 11:24:00.000000 chan127-demo-0.0.1/chan127_demo.egg-info/top_level.txt
--rw-r--r--   0 cheukkaichan   (501) staff       (20)       38 2023-04-29 11:24:00.000000 chan127-demo-0.0.1/setup.cfg
--rw-r--r--   0 cheukkaichan   (501) staff       (20)      457 2023-04-29 11:23:54.000000 chan127-demo-0.0.1/setup.py
-drwxr-xr-x   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 11:24:00.000000 chan127-demo-0.0.1/showdf/
--rw-r--r--   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 10:47:13.000000 chan127-demo-0.0.1/showdf/__init__.py
--rw-r--r--   0 cheukkaichan   (501) staff       (20)      341 2023-04-29 11:11:25.000000 chan127-demo-0.0.1/showdf/main.py
+drwxr-xr-x   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 11:29:50.000000 chan127-demo-0.0.2/
+-rw-r--r--   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 10:46:05.000000 chan127-demo-0.0.2/LICENSE
+-rw-r--r--   0 cheukkaichan   (501) staff       (20)       31 2023-04-29 11:28:57.000000 chan127-demo-0.0.2/MANIFEST.in
+-rw-r--r--   0 cheukkaichan   (501) staff       (20)      199 2023-04-29 11:29:50.000000 chan127-demo-0.0.2/PKG-INFO
+drwxr-xr-x   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 11:29:50.000000 chan127-demo-0.0.2/chan127_demo.egg-info/
+-rw-r--r--   0 cheukkaichan   (501) staff       (20)      199 2023-04-29 11:29:50.000000 chan127-demo-0.0.2/chan127_demo.egg-info/PKG-INFO
+-rw-r--r--   0 cheukkaichan   (501) staff       (20)      280 2023-04-29 11:29:50.000000 chan127-demo-0.0.2/chan127_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 cheukkaichan   (501) staff       (20)        1 2023-04-29 11:29:50.000000 chan127-demo-0.0.2/chan127_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 cheukkaichan   (501) staff       (20)       55 2023-04-29 11:29:50.000000 chan127-demo-0.0.2/chan127_demo.egg-info/entry_points.txt
+-rw-r--r--   0 cheukkaichan   (501) staff       (20)       19 2023-04-29 11:29:50.000000 chan127-demo-0.0.2/chan127_demo.egg-info/requires.txt
+-rw-r--r--   0 cheukkaichan   (501) staff       (20)        7 2023-04-29 11:29:50.000000 chan127-demo-0.0.2/chan127_demo.egg-info/top_level.txt
+-rw-r--r--   0 cheukkaichan   (501) staff       (20)       38 2023-04-29 11:29:50.000000 chan127-demo-0.0.2/setup.cfg
+-rw-r--r--   0 cheukkaichan   (501) staff       (20)      457 2023-04-29 11:29:34.000000 chan127-demo-0.0.2/setup.py
+drwxr-xr-x   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 11:29:50.000000 chan127-demo-0.0.2/showdf/
+-rw-r--r--   0 cheukkaichan   (501) staff       (20)        0 2023-04-29 10:47:13.000000 chan127-demo-0.0.2/showdf/__init__.py
+-rw-r--r--   0 cheukkaichan   (501) staff       (20)      341 2023-04-29 11:11:25.000000 chan127-demo-0.0.2/showdf/main.py
```


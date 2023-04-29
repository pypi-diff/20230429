# Comparing `tmp/aaaaa-1.0.tar.gz` & `tmp/aaaaa-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aaaaa-1.0.tar", last modified: Sat Apr 29 10:20:14 2023, max compression
+gzip compressed data, was "aaaaa-1.0.1.tar", last modified: Sat Apr 29 10:21:52 2023, max compression
```

## Comparing `aaaaa-1.0.tar` & `aaaaa-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:20:14.126546 aaaaa-1.0/
--rw-rw-rw-   0        0        0      174 2023-04-29 10:20:14.126546 aaaaa-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 10:20:14.124552 aaaaa-1.0/aaaaa.egg-info/
--rw-rw-rw-   0        0        0      174 2023-04-29 10:20:14.000000 aaaaa-1.0/aaaaa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      133 2023-04-29 10:20:14.000000 aaaaa-1.0/aaaaa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:20:14.000000 aaaaa-1.0/aaaaa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-29 10:20:14.000000 aaaaa-1.0/aaaaa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       23 2023-04-29 09:33:41.000000 aaaaa-1.0/aaaaa.py
--rw-rw-rw-   0        0        0       42 2023-04-29 10:20:14.127546 aaaaa-1.0/setup.cfg
--rw-rw-rw-   0        0        0      261 2023-04-29 10:19:44.000000 aaaaa-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:21:52.609365 aaaaa-1.0.1/
+-rw-rw-rw-   0        0        0      151 2023-04-29 10:21:52.609365 aaaaa-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 10:21:52.608367 aaaaa-1.0.1/aaaaa.egg-info/
+-rw-rw-rw-   0        0        0      151 2023-04-29 10:21:52.000000 aaaaa-1.0.1/aaaaa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      133 2023-04-29 10:21:52.000000 aaaaa-1.0.1/aaaaa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 10:21:52.000000 aaaaa-1.0.1/aaaaa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-29 10:21:52.000000 aaaaa-1.0.1/aaaaa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       23 2023-04-29 09:33:41.000000 aaaaa-1.0.1/aaaaa.py
+-rw-rw-rw-   0        0        0       42 2023-04-29 10:21:52.609365 aaaaa-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      238 2023-04-29 10:21:37.000000 aaaaa-1.0.1/setup.py
```


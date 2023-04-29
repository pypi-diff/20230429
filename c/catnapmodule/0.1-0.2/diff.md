# Comparing `tmp/catnapmodule-0.1.tar.gz` & `tmp/catnapmodule-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catnapmodule-0.1.tar", last modified: Thu Apr 27 14:18:57 2023, max compression
+gzip compressed data, was "catnapmodule-0.2.tar", last modified: Sat Apr 29 13:47:59 2023, max compression
```

## Comparing `catnapmodule-0.1.tar` & `catnapmodule-0.2.tar`

### file list

```diff
@@ -1,11 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 14:18:57.176963 catnapmodule-0.1/
--rw-rw-rw-   0        0        0      197 2023-04-27 14:18:57.177465 catnapmodule-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-27 14:18:50.000000 catnapmodule-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 14:18:57.174461 catnapmodule-0.1/catnapmodule.egg-info/
--rw-rw-rw-   0        0        0      197 2023-04-27 14:18:57.000000 catnapmodule-0.1/catnapmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-04-27 14:18:57.000000 catnapmodule-0.1/catnapmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 14:18:57.000000 catnapmodule-0.1/catnapmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-27 14:18:57.000000 catnapmodule-0.1/catnapmodule.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        1 2023-04-27 14:18:57.000000 catnapmodule-0.1/catnapmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 14:18:57.188972 catnapmodule-0.1/setup.cfg
--rw-rw-rw-   0        0        0      243 2023-04-27 14:18:50.000000 catnapmodule-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:47:59.178993 catnapmodule-0.2/
+-rw-rw-rw-   0        0        0      201 2023-04-29 13:47:59.177993 catnapmodule-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 13:47:59.174990 catnapmodule-0.2/catnapmodule.egg-info/
+-rw-rw-rw-   0        0        0      201 2023-04-29 13:47:59.000000 catnapmodule-0.2/catnapmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-04-29 13:47:59.000000 catnapmodule-0.2/catnapmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 13:47:59.000000 catnapmodule-0.2/catnapmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 13:47:59.000000 catnapmodule-0.2/catnapmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 13:47:59.179993 catnapmodule-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      235 2023-04-29 13:47:56.000000 catnapmodule-0.2/setup.py
```


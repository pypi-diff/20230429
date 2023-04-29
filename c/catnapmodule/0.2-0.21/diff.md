# Comparing `tmp/catnapmodule-0.2.tar.gz` & `tmp/catnapmodule-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catnapmodule-0.2.tar", last modified: Sat Apr 29 13:47:59 2023, max compression
+gzip compressed data, was "catnapmodule-0.21.tar", last modified: Sat Apr 29 14:31:31 2023, max compression
```

## Comparing `catnapmodule-0.2.tar` & `catnapmodule-0.21.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 13:47:59.178993 catnapmodule-0.2/
--rw-rw-rw-   0        0        0      201 2023-04-29 13:47:59.177993 catnapmodule-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 13:47:59.174990 catnapmodule-0.2/catnapmodule.egg-info/
--rw-rw-rw-   0        0        0      201 2023-04-29 13:47:59.000000 catnapmodule-0.2/catnapmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-04-29 13:47:59.000000 catnapmodule-0.2/catnapmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 13:47:59.000000 catnapmodule-0.2/catnapmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 13:47:59.000000 catnapmodule-0.2/catnapmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 13:47:59.179993 catnapmodule-0.2/setup.cfg
--rw-rw-rw-   0        0        0      235 2023-04-29 13:47:56.000000 catnapmodule-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 14:31:31.813988 catnapmodule-0.21/
+-rw-rw-rw-   0        0        0      202 2023-04-29 14:31:31.812986 catnapmodule-0.21/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 14:31:31.782946 catnapmodule-0.21/catnapmodule/
+-rw-rw-rw-   0        0        0        0 2023-04-29 14:29:06.000000 catnapmodule-0.21/catnapmodule/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-04-29 13:26:24.000000 catnapmodule-0.21/catnapmodule/chat.py
+drwxrwxrwx   0        0        0        0 2023-04-29 14:31:31.809986 catnapmodule-0.21/catnapmodule.egg-info/
+-rw-rw-rw-   0        0        0      202 2023-04-29 14:31:31.000000 catnapmodule-0.21/catnapmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-04-29 14:31:31.000000 catnapmodule-0.21/catnapmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 14:31:31.000000 catnapmodule-0.21/catnapmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-29 14:31:31.000000 catnapmodule-0.21/catnapmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 14:31:31.814989 catnapmodule-0.21/setup.cfg
+-rw-rw-rw-   0        0        0      238 2023-04-29 14:31:27.000000 catnapmodule-0.21/setup.py
```


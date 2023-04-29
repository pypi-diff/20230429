# Comparing `tmp/nettle-5.0.0.tar.gz` & `tmp/nettle-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nettle-5.0.0.tar", last modified: Sat Apr 29 08:42:17 2023, max compression
+gzip compressed data, was "nettle-5.0.1.tar", last modified: Sat Apr 29 08:54:22 2023, max compression
```

## Comparing `nettle-5.0.0.tar` & `nettle-5.0.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-29 08:42:17.473741 nettle-5.0.0/
--rw-r--r--   0 kali      (1000) kali      (1000)       50 2023-04-29 08:42:17.473741 nettle-5.0.0/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)       76 2023-04-29 08:32:08.000000 nettle-5.0.0/README
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-29 08:42:17.473741 nettle-5.0.0/nettle.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)       50 2023-04-29 08:42:17.000000 nettle-5.0.0/nettle.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      176 2023-04-29 08:42:17.000000 nettle-5.0.0/nettle.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-29 08:42:17.000000 nettle-5.0.0/nettle.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-04-29 08:42:17.000000 nettle-5.0.0/nettle.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-29 08:42:17.000000 nettle-5.0.0/nettle.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      360 2023-04-29 08:36:29.000000 nettle-5.0.0/pingback.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-29 08:42:17.473741 nettle-5.0.0/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      202 2023-04-29 08:27:57.000000 nettle-5.0.0/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-29 08:54:22.413769 nettle-5.0.1/
+-rw-r--r--   0 kali      (1000) kali      (1000)      163 2023-04-29 08:54:22.413769 nettle-5.0.1/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)       76 2023-04-29 08:32:08.000000 nettle-5.0.1/README
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-29 08:54:22.413769 nettle-5.0.1/nettle.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      163 2023-04-29 08:54:22.000000 nettle-5.0.1/nettle.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      147 2023-04-29 08:54:22.000000 nettle-5.0.1/nettle.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-29 08:54:22.000000 nettle-5.0.1/nettle.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-04-29 08:54:22.000000 nettle-5.0.1/nettle.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      360 2023-04-29 08:36:29.000000 nettle-5.0.1/pingback.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-29 08:54:22.413769 nettle-5.0.1/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      773 2023-04-29 08:51:35.000000 nettle-5.0.1/setup.py
```


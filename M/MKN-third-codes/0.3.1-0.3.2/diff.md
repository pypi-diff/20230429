# Comparing `tmp/MKN_third_codes-0.3.1.tar.gz` & `tmp/MKN_third_codes-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.3.1.tar", last modified: Sat Apr 29 15:12:22 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.3.2.tar", last modified: Sat Apr 29 15:45:23 2023, max compression
```

## Comparing `MKN_third_codes-0.3.1.tar` & `MKN_third_codes-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 15:12:22.593488 MKN_third_codes-0.3.1/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.3.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-04-29 15:12:22.579525 MKN_third_codes-0.3.1/MKN_third_codes/
--rw-rw-rw-   0        0        0    18143 2023-04-29 15:06:54.000000 MKN_third_codes-0.3.1/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:12:22.592490 MKN_third_codes-0.3.1/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0      231 2023-04-29 15:12:22.000000 MKN_third_codes-0.3.1/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-29 15:12:22.000000 MKN_third_codes-0.3.1/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 15:12:22.000000 MKN_third_codes-0.3.1/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-29 15:12:22.000000 MKN_third_codes-0.3.1/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      231 2023-04-29 15:12:22.593488 MKN_third_codes-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-29 15:12:22.593488 MKN_third_codes-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      312 2023-04-29 14:52:43.000000 MKN_third_codes-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:45:23.413063 MKN_third_codes-0.3.2/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.3.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-04-29 15:45:23.399100 MKN_third_codes-0.3.2/MKN_third_codes/
+-rw-rw-rw-   0        0        0    18143 2023-04-29 15:06:54.000000 MKN_third_codes-0.3.2/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:45:23.412065 MKN_third_codes-0.3.2/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     2156 2023-04-29 15:45:23.000000 MKN_third_codes-0.3.2/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-29 15:45:23.000000 MKN_third_codes-0.3.2/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 15:45:23.000000 MKN_third_codes-0.3.2/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-29 15:45:23.000000 MKN_third_codes-0.3.2/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2156 2023-04-29 15:45:23.412065 MKN_third_codes-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1896 2023-04-29 15:40:40.000000 MKN_third_codes-0.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 15:45:23.413063 MKN_third_codes-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      387 2023-04-29 15:45:14.000000 MKN_third_codes-0.3.2/setup.py
```

### Comparing `MKN_third_codes-0.3.1/LICENSE.txt` & `MKN_third_codes-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.3.1/MKN_third_codes/solutions.py` & `MKN_third_codes-0.3.2/MKN_third_codes/solutions.py`

 * *Files identical despite different names*


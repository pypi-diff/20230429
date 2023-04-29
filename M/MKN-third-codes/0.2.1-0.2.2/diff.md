# Comparing `tmp/MKN_third_codes-0.2.1.tar.gz` & `tmp/MKN_third_codes-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.2.1.tar", last modified: Sat Apr 29 11:07:28 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.2.2.tar", last modified: Sat Apr 29 11:21:28 2023, max compression
```

## Comparing `MKN_third_codes-0.2.1.tar` & `MKN_third_codes-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 11:07:28.095600 MKN_third_codes-0.2.1/
-drwxrwxrwx   0        0        0        0 2023-04-29 11:07:28.085614 MKN_third_codes-0.2.1/MKN_third_codes/
--rw-rw-rw-   0        0        0    15303 2023-04-29 11:06:57.000000 MKN_third_codes-0.2.1/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:07:28.094554 MKN_third_codes-0.2.1/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0      190 2023-04-29 11:07:27.000000 MKN_third_codes-0.2.1/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-04-29 11:07:28.000000 MKN_third_codes-0.2.1/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 11:07:27.000000 MKN_third_codes-0.2.1/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-29 11:07:27.000000 MKN_third_codes-0.2.1/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      190 2023-04-29 11:07:28.094554 MKN_third_codes-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-29 11:07:28.095600 MKN_third_codes-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      277 2023-04-29 11:07:25.000000 MKN_third_codes-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:21:28.063528 MKN_third_codes-0.2.2/
+drwxrwxrwx   0        0        0        0 2023-04-29 11:21:28.056548 MKN_third_codes-0.2.2/MKN_third_codes/
+-rw-rw-rw-   0        0        0    15303 2023-04-29 11:21:07.000000 MKN_third_codes-0.2.2/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:21:28.062531 MKN_third_codes-0.2.2/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0      190 2023-04-29 11:21:27.000000 MKN_third_codes-0.2.2/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-04-29 11:21:27.000000 MKN_third_codes-0.2.2/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:21:27.000000 MKN_third_codes-0.2.2/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:21:27.000000 MKN_third_codes-0.2.2/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      190 2023-04-29 11:21:28.062531 MKN_third_codes-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-29 11:21:28.063528 MKN_third_codes-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      288 2023-04-29 11:21:13.000000 MKN_third_codes-0.2.2/setup.py
```

### Comparing `MKN_third_codes-0.2.1/MKN_third_codes/solutions.py` & `MKN_third_codes-0.2.2/MKN_third_codes/solutions.py`

 * *Files identical despite different names*


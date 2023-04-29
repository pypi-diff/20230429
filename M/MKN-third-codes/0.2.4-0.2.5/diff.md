# Comparing `tmp/MKN_third_codes-0.2.4.tar.gz` & `tmp/MKN_third_codes-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.2.4.tar", last modified: Sat Apr 29 11:27:29 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.2.5.tar", last modified: Sat Apr 29 11:33:56 2023, max compression
```

## Comparing `MKN_third_codes-0.2.4.tar` & `MKN_third_codes-0.2.5.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 11:27:29.864811 MKN_third_codes-0.2.4/
-drwxrwxrwx   0        0        0        0 2023-04-29 11:27:29.853872 MKN_third_codes-0.2.4/MKN_third_codes/
--rw-rw-rw-   0        0        0    15303 2023-04-29 11:21:07.000000 MKN_third_codes-0.2.4/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:27:29.863812 MKN_third_codes-0.2.4/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0      190 2023-04-29 11:27:29.000000 MKN_third_codes-0.2.4/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-04-29 11:27:29.000000 MKN_third_codes-0.2.4/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 11:27:29.000000 MKN_third_codes-0.2.4/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-29 11:27:29.000000 MKN_third_codes-0.2.4/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      190 2023-04-29 11:27:29.863812 MKN_third_codes-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-29 11:27:29.864811 MKN_third_codes-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      293 2023-04-29 11:27:21.000000 MKN_third_codes-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:33:56.122619 MKN_third_codes-0.2.5/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.2.5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-04-29 11:33:56.107659 MKN_third_codes-0.2.5/MKN_third_codes/
+-rw-rw-rw-   0        0        0    15303 2023-04-29 11:21:07.000000 MKN_third_codes-0.2.5/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:33:56.120625 MKN_third_codes-0.2.5/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0      231 2023-04-29 11:33:56.000000 MKN_third_codes-0.2.5/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-29 11:33:56.000000 MKN_third_codes-0.2.5/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:33:56.000000 MKN_third_codes-0.2.5/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-29 11:33:56.000000 MKN_third_codes-0.2.5/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      231 2023-04-29 11:33:56.122619 MKN_third_codes-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-29 11:33:56.123618 MKN_third_codes-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      312 2023-04-29 11:30:51.000000 MKN_third_codes-0.2.5/setup.py
```

### Comparing `MKN_third_codes-0.2.4/MKN_third_codes/solutions.py` & `MKN_third_codes-0.2.5/MKN_third_codes/solutions.py`

 * *Files identical despite different names*


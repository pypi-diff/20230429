# Comparing `tmp/MKN-third-codes-0.2.3.tar.gz` & `tmp/MKN_third_codes-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN-third-codes-0.2.3.tar", last modified: Sat Apr 29 11:25:04 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.2.4.tar", last modified: Sat Apr 29 11:27:29 2023, max compression
```

## Comparing `MKN-third-codes-0.2.3.tar` & `MKN_third_codes-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 11:25:04.635553 MKN-third-codes-0.2.3/
-drwxrwxrwx   0        0        0        0 2023-04-29 11:25:04.628572 MKN-third-codes-0.2.3/MKN_third_codes/
--rw-rw-rw-   0        0        0    15303 2023-04-29 11:21:07.000000 MKN-third-codes-0.2.3/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:25:04.634556 MKN-third-codes-0.2.3/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0      190 2023-04-29 11:25:04.000000 MKN-third-codes-0.2.3/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-04-29 11:25:04.000000 MKN-third-codes-0.2.3/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 11:25:04.000000 MKN-third-codes-0.2.3/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-29 11:25:04.000000 MKN-third-codes-0.2.3/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      190 2023-04-29 11:25:04.635553 MKN-third-codes-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-29 11:25:04.636551 MKN-third-codes-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      312 2023-04-29 11:25:00.000000 MKN-third-codes-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:27:29.864811 MKN_third_codes-0.2.4/
+drwxrwxrwx   0        0        0        0 2023-04-29 11:27:29.853872 MKN_third_codes-0.2.4/MKN_third_codes/
+-rw-rw-rw-   0        0        0    15303 2023-04-29 11:21:07.000000 MKN_third_codes-0.2.4/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:27:29.863812 MKN_third_codes-0.2.4/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0      190 2023-04-29 11:27:29.000000 MKN_third_codes-0.2.4/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-04-29 11:27:29.000000 MKN_third_codes-0.2.4/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:27:29.000000 MKN_third_codes-0.2.4/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-29 11:27:29.000000 MKN_third_codes-0.2.4/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      190 2023-04-29 11:27:29.863812 MKN_third_codes-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-29 11:27:29.864811 MKN_third_codes-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      293 2023-04-29 11:27:21.000000 MKN_third_codes-0.2.4/setup.py
```

### Comparing `MKN-third-codes-0.2.3/MKN_third_codes/solutions.py` & `MKN_third_codes-0.2.4/MKN_third_codes/solutions.py`

 * *Files identical despite different names*


# Comparing `tmp/MKN_third_codes-0.1.3.tar.gz` & `tmp/MKN_third_codes-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.1.3.tar", last modified: Sat Apr 29 10:07:32 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.1.4.tar", last modified: Sat Apr 29 10:32:03 2023, max compression
```

## Comparing `MKN_third_codes-0.1.3.tar` & `MKN_third_codes-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:07:32.574846 MKN_third_codes-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-04-29 10:07:32.558888 MKN_third_codes-0.1.3/MKN_third_codes/
--rw-rw-rw-   0        0        0     7272 2023-04-29 09:54:05.000000 MKN_third_codes-0.1.3/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:07:32.573848 MKN_third_codes-0.1.3/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0      190 2023-04-29 10:07:32.000000 MKN_third_codes-0.1.3/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-04-29 10:07:32.000000 MKN_third_codes-0.1.3/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:07:32.000000 MKN_third_codes-0.1.3/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-29 10:07:32.000000 MKN_third_codes-0.1.3/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      190 2023-04-29 10:07:32.573848 MKN_third_codes-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-29 10:07:32.575845 MKN_third_codes-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      277 2023-04-29 09:58:22.000000 MKN_third_codes-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:32:03.414871 MKN_third_codes-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-04-29 10:32:03.409884 MKN_third_codes-0.1.4/MKN_third_codes/
+-rw-rw-rw-   0        0        0    10340 2023-04-29 10:29:34.000000 MKN_third_codes-0.1.4/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:32:03.413874 MKN_third_codes-0.1.4/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0      190 2023-04-29 10:32:03.000000 MKN_third_codes-0.1.4/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-04-29 10:32:03.000000 MKN_third_codes-0.1.4/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 10:32:03.000000 MKN_third_codes-0.1.4/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-29 10:32:03.000000 MKN_third_codes-0.1.4/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      190 2023-04-29 10:32:03.414871 MKN_third_codes-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-29 10:32:03.414871 MKN_third_codes-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      277 2023-04-29 10:28:53.000000 MKN_third_codes-0.1.4/setup.py
```


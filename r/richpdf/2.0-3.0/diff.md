# Comparing `tmp/richpdf-2.0.tar.gz` & `tmp/richpdf-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\richpdf-2.0.tar", last modified: Tue Jan 19 05:26:04 2021, max compression
+gzip compressed data, was "dist\richpdf-3.0.tar", last modified: Fri Apr 28 22:48:43 2023, max compression
```

## Comparing `richpdf-2.0.tar` & `richpdf-3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2021-01-19 05:26:04.470957 richpdf-2.0/
--rw-rw-rw-   0        0        0      272 2021-01-19 05:26:04.457968 richpdf-2.0/PKG-INFO
--rw-rw-rw-   0        0        0       82 2021-01-17 08:18:39.000000 richpdf-2.0/README.md
-drwxrwxrwx   0        0        0        0 2021-01-19 05:26:04.427006 richpdf-2.0/richpdf/
--rw-rw-rw-   0        0        0        0 2021-01-19 05:20:39.000000 richpdf-2.0/richpdf/__init__.py
--rw-rw-rw-   0        0        0        0 2021-01-16 05:58:34.000000 richpdf-2.0/richpdf/pdf2image.py
--rw-rw-rw-   0        0        0      283 2021-01-19 05:16:08.000000 richpdf-2.0/richpdf/pdf2text.py
-drwxrwxrwx   0        0        0        0 2021-01-19 05:26:04.454978 richpdf-2.0/richpdf.egg-info/
--rw-rw-rw-   0        0        0      272 2021-01-19 05:26:04.000000 richpdf-2.0/richpdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2021-01-19 05:26:04.000000 richpdf-2.0/richpdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-19 05:26:04.000000 richpdf-2.0/richpdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2021-01-19 05:26:04.000000 richpdf-2.0/richpdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-01-19 05:26:04.470957 richpdf-2.0/setup.cfg
--rw-rw-rw-   0        0        0      227 2021-01-19 05:25:52.000000 richpdf-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:48:43.264796 richpdf-3.0/
+-rw-rw-rw-   0        0        0      272 2023-04-28 22:48:43.262798 richpdf-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2021-01-17 08:18:39.000000 richpdf-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 22:48:43.215841 richpdf-3.0/richpdf/
+-rw-rw-rw-   0        0        0        0 2021-01-19 05:20:39.000000 richpdf-3.0/richpdf/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-01-16 05:58:34.000000 richpdf-3.0/richpdf/pdf2image.py
+-rw-rw-rw-   0        0        0      403 2021-01-19 05:52:45.000000 richpdf-3.0/richpdf/pdf2text.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:48:43.258802 richpdf-3.0/richpdf.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-04-28 22:48:42.000000 richpdf-3.0/richpdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-28 22:48:42.000000 richpdf-3.0/richpdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 22:48:42.000000 richpdf-3.0/richpdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-28 22:48:42.000000 richpdf-3.0/richpdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 22:48:43.265796 richpdf-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      227 2023-04-28 22:48:09.000000 richpdf-3.0/setup.py
```


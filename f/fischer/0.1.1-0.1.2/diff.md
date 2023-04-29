# Comparing `tmp/fischer-0.1.1.tar.gz` & `tmp/fischer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fischer-0.1.1.tar", last modified: Sat Apr 29 12:30:24 2023, max compression
+gzip compressed data, was "fischer-0.1.2.tar", last modified: Sat Apr 29 12:35:31 2023, max compression
```

## Comparing `fischer-0.1.1.tar` & `fischer-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 12:30:24.034716 fischer-0.1.1/
--rw-rw-rw-   0        0        0      245 2023-04-29 12:30:24.033718 fischer-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      923 2023-04-29 10:20:42.000000 fischer-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 12:30:24.030725 fischer-0.1.1/fischer.egg-info/
--rw-rw-rw-   0        0        0      245 2023-04-29 12:30:23.000000 fischer-0.1.1/fischer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-04-29 12:30:23.000000 fischer-0.1.1/fischer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 12:30:23.000000 fischer-0.1.1/fischer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-29 12:30:23.000000 fischer-0.1.1/fischer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-29 12:30:23.000000 fischer-0.1.1/fischer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-29 12:30:24.033718 fischer-0.1.1/fischer_mdls/
--rw-rw-rw-   0        0        0       82 2023-04-29 10:20:42.000000 fischer-0.1.1/fischer_mdls/__init__.py
--rw-rw-rw-   0        0        0     7735 2023-04-29 10:20:42.000000 fischer-0.1.1/fischer_mdls/mdls.py
--rw-rw-rw-   0        0        0     5501 2023-04-29 12:03:36.000000 fischer-0.1.1/fischer_mdls/utils.py
--rw-rw-rw-   0        0        0       42 2023-04-29 12:30:24.034716 fischer-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-04-29 12:30:13.000000 fischer-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:35:31.424128 fischer-0.1.2/
+-rw-rw-rw-   0        0        0     1156 2023-04-29 12:35:31.423131 fischer-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2023-04-29 10:20:42.000000 fischer-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 12:35:31.419141 fischer-0.1.2/fischer.egg-info/
+-rw-rw-rw-   0        0        0     1156 2023-04-29 12:35:31.000000 fischer-0.1.2/fischer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-29 12:35:31.000000 fischer-0.1.2/fischer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 12:35:31.000000 fischer-0.1.2/fischer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-29 12:35:31.000000 fischer-0.1.2/fischer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-29 12:35:31.000000 fischer-0.1.2/fischer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 12:35:31.422133 fischer-0.1.2/fischer_mdls/
+-rw-rw-rw-   0        0        0       82 2023-04-29 10:20:42.000000 fischer-0.1.2/fischer_mdls/__init__.py
+-rw-rw-rw-   0        0        0     7735 2023-04-29 10:20:42.000000 fischer-0.1.2/fischer_mdls/mdls.py
+-rw-rw-rw-   0        0        0     5501 2023-04-29 12:03:36.000000 fischer-0.1.2/fischer_mdls/utils.py
+-rw-rw-rw-   0        0        0       42 2023-04-29 12:35:31.424128 fischer-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-04-29 12:35:21.000000 fischer-0.1.2/setup.py
```

### Comparing `fischer-0.1.1/README.md` & `fischer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fischer-0.1.1/fischer_mdls/mdls.py` & `fischer-0.1.2/fischer_mdls/mdls.py`

 * *Files identical despite different names*

### Comparing `fischer-0.1.1/fischer_mdls/utils.py` & `fischer-0.1.2/fischer_mdls/utils.py`

 * *Files identical despite different names*


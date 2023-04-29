# Comparing `tmp/iphub-1.0.0.tar.gz` & `tmp/iphub-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\GitHub ???????????\iphub\dist\tmpr1tutyn6\iphub-1.0.0.tar", last modified: Sat Jul  2 12:40:52 2022, max compression
+gzip compressed data, was "iphub-1.0.1.tar", last modified: Sat Apr 29 09:04:32 2023, max compression
```

## Comparing `iphub-1.0.0.tar` & `iphub-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-07-02 12:40:52.000000 iphub-1.0.0/
--rw-rw-rw-   0        0        0     1080 2022-03-30 02:32:38.000000 iphub-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       34 2022-04-12 16:05:18.000000 iphub-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      882 2022-07-02 12:40:52.000000 iphub-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      384 2022-07-02 12:29:52.000000 iphub-1.0.0/README.MD
-drwxrwxrwx   0        0        0        0 2022-07-02 12:40:52.000000 iphub-1.0.0/iphub/
--rw-rw-rw-   0        0        0       44 2022-07-02 12:26:30.000000 iphub-1.0.0/iphub/__init__.py
--rw-rw-rw-   0        0        0     1556 2022-07-02 12:25:02.000000 iphub-1.0.0/iphub/iphub.py
-drwxrwxrwx   0        0        0        0 2022-07-02 12:40:52.000000 iphub-1.0.0/iphub.egg-info/
--rw-rw-rw-   0        0        0      882 2022-07-02 12:40:51.000000 iphub-1.0.0/iphub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2022-07-02 12:40:52.000000 iphub-1.0.0/iphub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-02 12:40:51.000000 iphub-1.0.0/iphub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-07-02 12:40:52.000000 iphub-1.0.0/iphub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-07-02 12:40:52.000000 iphub-1.0.0/iphub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-02 12:40:52.000000 iphub-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      816 2022-07-02 12:30:17.000000 iphub-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 09:04:32.139773 iphub-1.0.1/
+-rw-rw-rw-   0        0        0     1080 2022-03-30 02:32:38.000000 iphub-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-04-12 16:05:18.000000 iphub-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      773 2023-04-29 09:04:32.139773 iphub-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-29 09:03:39.000000 iphub-1.0.1/README.MD
+drwxrwxrwx   0        0        0        0 2023-04-29 09:04:32.136781 iphub-1.0.1/iphub/
+-rw-rw-rw-   0        0        0       44 2022-07-02 12:26:30.000000 iphub-1.0.1/iphub/__init__.py
+-rw-rw-rw-   0        0        0     2266 2023-04-29 09:02:47.000000 iphub-1.0.1/iphub/iphub.py
+drwxrwxrwx   0        0        0        0 2023-04-29 09:04:32.138776 iphub-1.0.1/iphub.egg-info/
+-rw-rw-rw-   0        0        0      773 2023-04-29 09:04:32.000000 iphub-1.0.1/iphub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-04-29 09:04:32.000000 iphub-1.0.1/iphub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 09:04:32.000000 iphub-1.0.1/iphub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-29 09:04:32.000000 iphub-1.0.1/iphub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-29 09:04:32.000000 iphub-1.0.1/iphub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 09:04:32.139773 iphub-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      816 2023-04-29 09:03:58.000000 iphub-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `iphub-1.0.0/LICENSE` & `iphub-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iphub-1.0.0/setup.py` & `iphub-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='iphub',
-    version='1.0.0',
+    version='1.0.1',
     author='Maehdakvan',
     author_email='visitanimation@google.com',
     description='IPhub.info API wrapper.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/DedInc/iphub',
     project_urls={
```


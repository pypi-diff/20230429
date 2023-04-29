# Comparing `tmp/sopel_modules.twitter-1.0.0.tar.gz` & `tmp/sopel_modules.twitter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel_modules.twitter-1.0.0.tar", last modified: Fri Apr 14 22:00:33 2023, max compression
+gzip compressed data, was "sopel_modules.twitter-1.0.1.tar", last modified: Sat Apr 29 21:03:32 2023, max compression
```

## Comparing `sopel_modules.twitter-1.0.0.tar` & `sopel_modules.twitter-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-14 22:00:33.301056 sopel_modules.twitter-1.0.0/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2022-03-02 18:17:04.000000 sopel_modules.twitter-1.0.0/COPYING
--rw-r--r--   0 dgw       (1000) dgw       (1000)      134 2023-04-14 21:53:42.000000 sopel_modules.twitter-1.0.0/MANIFEST.in
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1874 2023-04-14 21:52:02.000000 sopel_modules.twitter-1.0.0/NEWS
--rw-r--r--   0 dgw       (1000) dgw       (1000)     3155 2023-04-14 22:00:33.300056 sopel_modules.twitter-1.0.0/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)      174 2023-04-14 21:50:42.000000 sopel_modules.twitter-1.0.0/README.md
--rw-r--r--   0 dgw       (1000) dgw       (1000)       21 2023-04-14 21:57:08.000000 sopel_modules.twitter-1.0.0/requirements.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       38 2023-04-14 22:00:33.301056 sopel_modules.twitter-1.0.0/setup.cfg
--rwxr-xr-x   0 dgw       (1000) dgw       (1000)     1213 2023-04-14 21:52:19.000000 sopel_modules.twitter-1.0.0/setup.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-14 22:00:33.287059 sopel_modules.twitter-1.0.0/sopel_modules/
--rw-r--r--   0 dgw       (1000) dgw       (1000)       56 2023-04-14 21:48:28.000000 sopel_modules.twitter-1.0.0/sopel_modules/__init__.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-14 22:00:33.299064 sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     3155 2023-04-14 22:00:33.000000 sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)      364 2023-04-14 22:00:33.000000 sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/SOURCES.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-04-14 22:00:33.000000 sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/dependency_links.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       14 2023-04-14 22:00:33.000000 sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/namespace_packages.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       21 2023-04-14 22:00:33.000000 sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/requires.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       14 2023-04-14 22:00:33.000000 sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/top_level.txt
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-29 21:03:32.746830 sopel_modules.twitter-1.0.1/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2022-03-02 18:17:04.000000 sopel_modules.twitter-1.0.1/COPYING
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      134 2023-04-29 21:02:37.000000 sopel_modules.twitter-1.0.1/MANIFEST.in
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     1874 2023-04-29 21:02:37.000000 sopel_modules.twitter-1.0.1/NEWS
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     3155 2023-04-29 21:03:32.746830 sopel_modules.twitter-1.0.1/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      174 2023-04-29 21:02:37.000000 sopel_modules.twitter-1.0.1/README.md
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       14 2023-04-29 21:02:40.000000 sopel_modules.twitter-1.0.1/requirements.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       38 2023-04-29 21:03:32.747830 sopel_modules.twitter-1.0.1/setup.cfg
+-rwxr-xr-x   0 dgw       (1000) dgw       (1000)     1213 2023-04-29 21:02:40.000000 sopel_modules.twitter-1.0.1/setup.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-29 21:03:32.715831 sopel_modules.twitter-1.0.1/sopel_modules/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       56 2023-04-29 21:02:37.000000 sopel_modules.twitter-1.0.1/sopel_modules/__init__.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-29 21:03:32.744898 sopel_modules.twitter-1.0.1/sopel_modules.twitter.egg-info/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     3155 2023-04-29 21:03:32.000000 sopel_modules.twitter-1.0.1/sopel_modules.twitter.egg-info/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      364 2023-04-29 21:03:32.000000 sopel_modules.twitter-1.0.1/sopel_modules.twitter.egg-info/SOURCES.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-04-29 21:03:32.000000 sopel_modules.twitter-1.0.1/sopel_modules.twitter.egg-info/dependency_links.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       14 2023-04-29 21:03:32.000000 sopel_modules.twitter-1.0.1/sopel_modules.twitter.egg-info/namespace_packages.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       14 2023-04-29 21:03:32.000000 sopel_modules.twitter-1.0.1/sopel_modules.twitter.egg-info/requires.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       14 2023-04-29 21:03:32.000000 sopel_modules.twitter-1.0.1/sopel_modules.twitter.egg-info/top_level.txt
```

### Comparing `sopel_modules.twitter-1.0.0/COPYING` & `sopel_modules.twitter-1.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `sopel_modules.twitter-1.0.0/NEWS` & `sopel_modules.twitter-1.0.1/NEWS`

 * *Files identical despite different names*

### Comparing `sopel_modules.twitter-1.0.0/PKG-INFO` & `sopel_modules.twitter-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel_modules.twitter
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Twitter plugin for Sopel
 Home-page: https://github.com/sopel-irc/sopel-twitter
 Author: dgw
 Author-email: dgw@technobabbl.es
 License: Eiffel Forum License, version 2
 Description: # sopel-twitter
```

### Comparing `sopel_modules.twitter-1.0.0/setup.py` & `sopel_modules.twitter-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 with open('requirements.txt') as requirements_file:
     requirements = [req for req in requirements_file.readlines()]
 
 
 setup(
     name='sopel_modules.twitter',
-    version='1.0.0',
+    version='1.0.1',
     description='A Twitter plugin for Sopel',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author='dgw',
     author_email='dgw@technobabbl.es',
     url='https://github.com/sopel-irc/sopel-twitter',
     packages=find_packages('.'),
```

### Comparing `sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/PKG-INFO` & `sopel_modules.twitter-1.0.1/sopel_modules.twitter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-modules.twitter
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Twitter plugin for Sopel
 Home-page: https://github.com/sopel-irc/sopel-twitter
 Author: dgw
 Author-email: dgw@technobabbl.es
 License: Eiffel Forum License, version 2
 Description: # sopel-twitter
```


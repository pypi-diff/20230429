# Comparing `tmp/hype-html-1.0.0.tar.gz` & `tmp/hype-html-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hype-html-1.0.0.tar", last modified: Fri Aug 20 20:39:03 2021, max compression
+gzip compressed data, was "hype-html-1.1.0.tar", last modified: Sat Apr 29 16:04:16 2023, max compression
```

## Comparing `hype-html-1.0.0.tar` & `hype-html-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2021-08-20 20:39:03.930000 hype-html-1.0.0/
--rw-r--r--   0 scott     (1000) scott     (1000)     4649 2021-08-20 20:39:03.930000 hype-html-1.0.0/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)     2835 2020-11-22 16:13:35.000000 hype-html-1.0.0/README.md
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2021-08-20 20:39:03.920000 hype-html-1.0.0/hype/
--rw-r--r--   0 scott     (1000) scott     (1000)     3684 2021-08-20 20:31:08.000000 hype-html-1.0.0/hype/__init__.py
--rw-r--r--   0 scott     (1000) scott     (1000)   145108 2021-08-20 20:31:08.000000 hype-html-1.0.0/hype/element.py
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2021-08-20 20:39:03.930000 hype-html-1.0.0/hype_html.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     4649 2021-08-20 20:39:03.000000 hype-html-1.0.0/hype_html.egg-info/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)      183 2021-08-20 20:39:03.000000 hype-html-1.0.0/hype_html.egg-info/SOURCES.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        1 2021-08-20 20:39:03.000000 hype-html-1.0.0/hype_html.egg-info/dependency_links.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        5 2021-08-20 20:39:03.000000 hype-html-1.0.0/hype_html.egg-info/top_level.txt
--rw-r--r--   0 scott     (1000) scott     (1000)       38 2021-08-20 20:39:03.930000 hype-html-1.0.0/setup.cfg
--rw-r--r--   0 scott     (1000) scott     (1000)      659 2021-08-20 20:37:45.000000 hype-html-1.0.0/setup.py
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 16:04:16.795032 hype-html-1.1.0/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1060 2023-04-29 15:04:42.000000 hype-html-1.1.0/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     3280 2023-04-29 16:04:16.795032 hype-html-1.1.0/PKG-INFO
+-rw-r--r--   0 scott     (1000) scott     (1000)     2835 2023-04-29 15:04:42.000000 hype-html-1.1.0/README.md
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 16:04:16.770346 hype-html-1.1.0/hype/
+-rw-r--r--   0 scott     (1000) scott     (1000)     3684 2023-04-29 15:35:23.000000 hype-html-1.1.0/hype/__init__.py
+-rw-r--r--   0 scott     (1000) scott     (1000)   185067 2023-04-29 15:43:07.000000 hype-html-1.1.0/hype/element.py
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 16:04:16.793521 hype-html-1.1.0/hype_html.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     3280 2023-04-29 16:04:16.000000 hype-html-1.1.0/hype_html.egg-info/PKG-INFO
+-rw-r--r--   0 scott     (1000) scott     (1000)      191 2023-04-29 16:04:16.000000 hype-html-1.1.0/hype_html.egg-info/SOURCES.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-04-29 16:04:16.000000 hype-html-1.1.0/hype_html.egg-info/dependency_links.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)        5 2023-04-29 16:04:16.000000 hype-html-1.1.0/hype_html.egg-info/top_level.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)       38 2023-04-29 16:04:16.796046 hype-html-1.1.0/setup.cfg
+-rw-r--r--   0 scott     (1000) scott     (1000)      660 2023-04-29 15:59:00.000000 hype-html-1.1.0/setup.py
```

### Comparing `hype-html-1.0.0/README.md` & `hype-html-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hype-html-1.0.0/hype/__init__.py` & `hype-html-1.1.0/hype/__init__.py`

 * *Files identical despite different names*

### Comparing `hype-html-1.0.0/setup.py` & `hype-html-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
-with open('README.md', 'r') as fh:
+with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hype-html",
-    version="1.0.0",
+    version="1.1.0",
     author="Scott Russell",
     author_email="me@scottrussell.net",
     description="A minimal python dsl for generating html.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/scrussell24/hype-html",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
-)
+    python_requires=">=3.7",
+)
```


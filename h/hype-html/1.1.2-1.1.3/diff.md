# Comparing `tmp/hype-html-1.1.2.tar.gz` & `tmp/hype-html-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hype-html-1.1.2.tar", last modified: Sat Apr 29 16:14:19 2023, max compression
+gzip compressed data, was "hype-html-1.1.3.tar", last modified: Sat Apr 29 16:26:29 2023, max compression
```

## Comparing `hype-html-1.1.2.tar` & `hype-html-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 16:14:19.191559 hype-html-1.1.2/
--rw-r--r--   0 scott     (1000) scott     (1000)     1060 2023-04-29 15:04:42.000000 hype-html-1.1.2/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     3280 2023-04-29 16:14:19.189636 hype-html-1.1.2/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)     2835 2023-04-29 15:04:42.000000 hype-html-1.1.2/README.md
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 16:14:19.173123 hype-html-1.1.2/hype/
--rw-r--r--   0 scott     (1000) scott     (1000)     3684 2023-04-29 15:35:23.000000 hype-html-1.1.2/hype/__init__.py
--rw-r--r--   0 scott     (1000) scott     (1000)   185067 2023-04-29 15:43:07.000000 hype-html-1.1.2/hype/element.py
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 16:14:19.188637 hype-html-1.1.2/hype_html.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     3280 2023-04-29 16:14:19.000000 hype-html-1.1.2/hype_html.egg-info/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)      191 2023-04-29 16:14:19.000000 hype-html-1.1.2/hype_html.egg-info/SOURCES.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-04-29 16:14:19.000000 hype-html-1.1.2/hype_html.egg-info/dependency_links.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        5 2023-04-29 16:14:19.000000 hype-html-1.1.2/hype_html.egg-info/top_level.txt
--rw-r--r--   0 scott     (1000) scott     (1000)       38 2023-04-29 16:14:19.191723 hype-html-1.1.2/setup.cfg
--rw-r--r--   0 scott     (1000) scott     (1000)      660 2023-04-29 16:14:13.000000 hype-html-1.1.2/setup.py
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 16:26:29.269300 hype-html-1.1.3/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1060 2023-04-29 15:04:42.000000 hype-html-1.1.3/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     3280 2023-04-29 16:26:29.269300 hype-html-1.1.3/PKG-INFO
+-rw-r--r--   0 scott     (1000) scott     (1000)     2835 2023-04-29 15:04:42.000000 hype-html-1.1.3/README.md
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 16:26:29.248820 hype-html-1.1.3/hype/
+-rw-r--r--   0 scott     (1000) scott     (1000)     3684 2023-04-29 15:35:23.000000 hype-html-1.1.3/hype/__init__.py
+-rw-r--r--   0 scott     (1000) scott     (1000)   185067 2023-04-29 15:43:07.000000 hype-html-1.1.3/hype/element.py
+-rw-r--r--   0 scott     (1000) scott     (1000)        0 2023-04-29 16:08:45.000000 hype-html-1.1.3/hype/py.typed
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 16:26:29.267292 hype-html-1.1.3/hype_html.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     3280 2023-04-29 16:26:29.000000 hype-html-1.1.3/hype_html.egg-info/PKG-INFO
+-rw-r--r--   0 scott     (1000) scott     (1000)      205 2023-04-29 16:26:29.000000 hype-html-1.1.3/hype_html.egg-info/SOURCES.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-04-29 16:26:29.000000 hype-html-1.1.3/hype_html.egg-info/dependency_links.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)        5 2023-04-29 16:26:29.000000 hype-html-1.1.3/hype_html.egg-info/top_level.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)       38 2023-04-29 16:26:29.270295 hype-html-1.1.3/setup.cfg
+-rw-r--r--   0 scott     (1000) scott     (1000)      701 2023-04-29 16:26:26.000000 hype-html-1.1.3/setup.py
```

### Comparing `hype-html-1.1.2/LICENSE` & `hype-html-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hype-html-1.1.2/PKG-INFO` & `hype-html-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hype-html
-Version: 1.1.2
+Version: 1.1.3
 Summary: A minimal python dsl for generating html.
 Home-page: https://github.com/scrussell24/hype-html
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hype-html-1.1.2/README.md` & `hype-html-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hype-html-1.1.2/hype/__init__.py` & `hype-html-1.1.3/hype/__init__.py`

 * *Files identical despite different names*

### Comparing `hype-html-1.1.2/hype/element.py` & `hype-html-1.1.3/hype/element.py`

 * *Files identical despite different names*

### Comparing `hype-html-1.1.2/hype_html.egg-info/PKG-INFO` & `hype-html-1.1.3/hype_html.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hype-html
-Version: 1.1.2
+Version: 1.1.3
 Summary: A minimal python dsl for generating html.
 Home-page: https://github.com/scrussell24/hype-html
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hype-html-1.1.2/setup.py` & `hype-html-1.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hype-html",
-    version="1.1.2",
+    version="1.1.3",
     author="Scott Russell",
     author_email="me@scottrussell.net",
     description="A minimal python dsl for generating html.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/scrussell24/hype-html",
     packages=setuptools.find_packages(),
+    package_data={'hype': ['py.typed']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
```


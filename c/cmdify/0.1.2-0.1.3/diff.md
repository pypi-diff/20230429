# Comparing `tmp/cmdify-0.1.2.tar.gz` & `tmp/cmdify-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdify-0.1.2.tar", last modified: Sat Apr 29 18:26:23 2023, max compression
+gzip compressed data, was "cmdify-0.1.3.tar", last modified: Sat Apr 29 18:35:09 2023, max compression
```

## Comparing `cmdify-0.1.2.tar` & `cmdify-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 18:26:23.013684 cmdify-0.1.2/
--rw-rw-rw-   0        0        0     1089 2023-04-24 19:59:16.000000 cmdify-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2432 2023-04-29 18:26:23.013684 cmdify-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1540 2023-04-24 19:59:16.000000 cmdify-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 18:26:22.980914 cmdify-0.1.2/cmdify/
--rw-rw-rw-   0        0        0        0 2023-04-24 19:59:16.000000 cmdify-0.1.2/cmdify/__init__.py
--rw-rw-rw-   0        0        0     3363 2023-04-24 19:59:16.000000 cmdify-0.1.2/cmdify/core.py
--rw-rw-rw-   0        0        0     5882 2023-04-26 19:15:19.000000 cmdify-0.1.2/cmdify/identifiers.py
--rw-rw-rw-   0        0        0     2254 2023-04-24 19:59:16.000000 cmdify-0.1.2/cmdify/interpreters.py
--rw-rw-rw-   0        0        0     3327 2023-04-29 18:21:17.000000 cmdify-0.1.2/cmdify/lexica.py
--rw-rw-rw-   0        0        0      498 2023-04-24 19:59:16.000000 cmdify-0.1.2/cmdify/preprocessors.py
--rw-rw-rw-   0        0        0     3833 2023-04-24 19:59:16.000000 cmdify-0.1.2/cmdify/result.py
-drwxrwxrwx   0        0        0        0 2023-04-29 18:26:23.013684 cmdify-0.1.2/cmdify.egg-info/
--rw-rw-rw-   0        0        0     2432 2023-04-29 18:26:22.000000 cmdify-0.1.2/cmdify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-04-29 18:26:22.000000 cmdify-0.1.2/cmdify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 18:26:22.000000 cmdify-0.1.2/cmdify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-29 18:26:22.000000 cmdify-0.1.2/cmdify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-29 18:26:22.000000 cmdify-0.1.2/cmdify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1229 2023-04-29 18:24:52.000000 cmdify-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 18:26:23.013684 cmdify-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      222 2023-04-24 19:59:16.000000 cmdify-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 18:35:09.627236 cmdify-0.1.3/
+-rw-rw-rw-   0        0        0     1089 2023-04-24 19:59:16.000000 cmdify-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2432 2023-04-29 18:35:09.625625 cmdify-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1540 2023-04-24 19:59:16.000000 cmdify-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 18:35:09.577047 cmdify-0.1.3/cmdify/
+-rw-rw-rw-   0        0        0        0 2023-04-24 19:59:16.000000 cmdify-0.1.3/cmdify/__init__.py
+-rw-rw-rw-   0        0        0     3363 2023-04-24 19:59:16.000000 cmdify-0.1.3/cmdify/core.py
+-rw-rw-rw-   0        0        0     5882 2023-04-26 19:15:19.000000 cmdify-0.1.3/cmdify/identifiers.py
+-rw-rw-rw-   0        0        0     2254 2023-04-24 19:59:16.000000 cmdify-0.1.3/cmdify/interpreters.py
+-rw-rw-rw-   0        0        0     3327 2023-04-29 18:21:17.000000 cmdify-0.1.3/cmdify/lexica.py
+-rw-rw-rw-   0        0        0      498 2023-04-24 19:59:16.000000 cmdify-0.1.3/cmdify/preprocessors.py
+-rw-rw-rw-   0        0        0     3833 2023-04-24 19:59:16.000000 cmdify-0.1.3/cmdify/result.py
+drwxrwxrwx   0        0        0        0 2023-04-29 18:35:09.618544 cmdify-0.1.3/cmdify.egg-info/
+-rw-rw-rw-   0        0        0     2432 2023-04-29 18:35:09.000000 cmdify-0.1.3/cmdify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-04-29 18:35:09.000000 cmdify-0.1.3/cmdify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 18:35:09.000000 cmdify-0.1.3/cmdify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-29 18:35:09.000000 cmdify-0.1.3/cmdify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-29 18:35:09.000000 cmdify-0.1.3/cmdify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1231 2023-04-29 18:34:30.000000 cmdify-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 18:35:09.627236 cmdify-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      222 2023-04-24 19:59:16.000000 cmdify-0.1.3/setup.py
```

### Comparing `cmdify-0.1.2/LICENSE.txt` & `cmdify-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cmdify-0.1.2/PKG-INFO` & `cmdify-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdify
-Version: 0.1.2
+Version: 0.1.3
 Summary: A lightweight command-line language processing utility.
 Author-email: Daniel Roland <its.daniel.roland@gmail.com>, "Jonathan M. Lobmeyer" <jmlobmeyer@gmail.com>, Nicole Livingston <nliving73@gmail.com>, William Blazer <williamblazer2@gmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/dqnnyr/cmdify.git
 Keywords: nlp,lightweight,command line,language processing,natural language processing,twilight imperium,ti4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cmdify-0.1.2/README.md` & `cmdify-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cmdify-0.1.2/cmdify/core.py` & `cmdify-0.1.3/cmdify/core.py`

 * *Files identical despite different names*

### Comparing `cmdify-0.1.2/cmdify/identifiers.py` & `cmdify-0.1.3/cmdify/identifiers.py`

 * *Files identical despite different names*

### Comparing `cmdify-0.1.2/cmdify/interpreters.py` & `cmdify-0.1.3/cmdify/interpreters.py`

 * *Files identical despite different names*

### Comparing `cmdify-0.1.2/cmdify/lexica.py` & `cmdify-0.1.3/cmdify/lexica.py`

 * *Files identical despite different names*

### Comparing `cmdify-0.1.2/cmdify/result.py` & `cmdify-0.1.3/cmdify/result.py`

 * *Files identical despite different names*

### Comparing `cmdify-0.1.2/cmdify.egg-info/PKG-INFO` & `cmdify-0.1.3/cmdify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdify
-Version: 0.1.2
+Version: 0.1.3
 Summary: A lightweight command-line language processing utility.
 Author-email: Daniel Roland <its.daniel.roland@gmail.com>, "Jonathan M. Lobmeyer" <jmlobmeyer@gmail.com>, Nicole Livingston <nliving73@gmail.com>, William Blazer <williamblazer2@gmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/dqnnyr/cmdify.git
 Keywords: nlp,lightweight,command line,language processing,natural language processing,twilight imperium,ti4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cmdify-0.1.2/pyproject.toml` & `cmdify-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools", "setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cmdify"
-version = "0.1.2"
+version = "0.1.3"
 description = "A lightweight command-line language processing utility."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT License"}
 authors = [
     {name = "Daniel Roland", email = "its.daniel.roland@gmail.com"},
     {name = "Jonathan M. Lobmeyer", email = "jmlobmeyer@gmail.com"},
     {name = "Nicole Livingston", email = "nliving73@gmail.com"},
     {name = "William Blazer", email = "williamblazer2@gmail.com"},
 ]
 dependencies = [
-    "bidict>0.22.1",
-    "textdistance>4.5.0"
+    "bidict>=0.22.1",
+    "textdistance>=4.5.0"
 ]
 keywords = [
     "nlp",
     "lightweight",
     "command line",
     "language processing",
     "natural language processing",
```


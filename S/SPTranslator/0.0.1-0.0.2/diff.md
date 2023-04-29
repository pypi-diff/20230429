# Comparing `tmp/SPTranslator-0.0.1.tar.gz` & `tmp/SPTranslator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/foldedpond/Documents/AI/sptranslator/dist/.tmp-r0uj1bgg/SPTranslator-0.0.1.tar", last modified: Fri Apr 28 06:42:10 2023, max compression
+gzip compressed data, was "/Users/foldedpond/Documents/AI/sptranslator/dist/.tmp-xtcj7bt0/SPTranslator-0.0.2.tar", last modified: Sat Apr 29 16:16:14 2023, max compression
```

## Comparing `SPTranslator-0.0.1.tar` & `SPTranslator-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 foldedpond   (501) staff       (20)        0 2023-04-28 06:42:10.024792 SPTranslator-0.0.1/
--rw-r--r--   0 foldedpond   (501) staff       (20)     1067 2023-04-28 04:42:36.000000 SPTranslator-0.0.1/LICENSE
--rw-r--r--   0 foldedpond   (501) staff       (20)     3354 2023-04-28 06:42:10.024279 SPTranslator-0.0.1/PKG-INFO
--rw-r--r--   0 foldedpond   (501) staff       (20)     2818 2023-04-28 06:21:48.000000 SPTranslator-0.0.1/README.md
-drwxr-xr-x   0 foldedpond   (501) staff       (20)        0 2023-04-28 06:42:10.019452 SPTranslator-0.0.1/SPTranslator.egg-info/
--rw-r--r--   0 foldedpond   (501) staff       (20)     3354 2023-04-28 06:42:10.000000 SPTranslator-0.0.1/SPTranslator.egg-info/PKG-INFO
--rw-r--r--   0 foldedpond   (501) staff       (20)      253 2023-04-28 06:42:10.000000 SPTranslator-0.0.1/SPTranslator.egg-info/SOURCES.txt
--rw-r--r--   0 foldedpond   (501) staff       (20)        1 2023-04-28 06:42:10.000000 SPTranslator-0.0.1/SPTranslator.egg-info/dependency_links.txt
--rw-r--r--   0 foldedpond   (501) staff       (20)       13 2023-04-28 06:42:10.000000 SPTranslator-0.0.1/SPTranslator.egg-info/top_level.txt
--rw-r--r--   0 foldedpond   (501) staff       (20)      618 2023-04-28 06:41:16.000000 SPTranslator-0.0.1/pyproject.toml
--rw-r--r--   0 foldedpond   (501) staff       (20)       38 2023-04-28 06:42:10.024964 SPTranslator-0.0.1/setup.cfg
-drwxr-xr-x   0 foldedpond   (501) staff       (20)        0 2023-04-28 06:42:10.020142 SPTranslator-0.0.1/sptranslator/
--rw-r--r--   0 foldedpond   (501) staff       (20)        0 2023-04-24 10:23:38.000000 SPTranslator-0.0.1/sptranslator/__init__.py
--rw-r--r--   0 foldedpond   (501) staff       (20)     3963 2023-04-28 03:48:34.000000 SPTranslator-0.0.1/sptranslator/translator.py
-drwxr-xr-x   0 foldedpond   (501) staff       (20)        0 2023-04-28 06:42:10.021781 SPTranslator-0.0.1/tests/
--rw-r--r--   0 foldedpond   (501) staff       (20)     7083 2023-04-28 03:48:51.000000 SPTranslator-0.0.1/tests/test_translator.py
+drwxr-xr-x   0 foldedpond   (501) staff       (20)        0 2023-04-29 16:16:14.226454 SPTranslator-0.0.2/
+-rw-r--r--   0 foldedpond   (501) staff       (20)     1067 2023-04-28 04:42:36.000000 SPTranslator-0.0.2/LICENSE
+-rw-r--r--   0 foldedpond   (501) staff       (20)     3212 2023-04-29 16:16:14.225083 SPTranslator-0.0.2/PKG-INFO
+-rw-r--r--   0 foldedpond   (501) staff       (20)     2674 2023-04-29 09:55:21.000000 SPTranslator-0.0.2/README.md
+drwxr-xr-x   0 foldedpond   (501) staff       (20)        0 2023-04-29 16:16:14.218658 SPTranslator-0.0.2/SPTranslator.egg-info/
+-rw-r--r--   0 foldedpond   (501) staff       (20)     3212 2023-04-29 16:16:14.000000 SPTranslator-0.0.2/SPTranslator.egg-info/PKG-INFO
+-rw-r--r--   0 foldedpond   (501) staff       (20)      288 2023-04-29 16:16:14.000000 SPTranslator-0.0.2/SPTranslator.egg-info/SOURCES.txt
+-rw-r--r--   0 foldedpond   (501) staff       (20)        1 2023-04-29 16:16:14.000000 SPTranslator-0.0.2/SPTranslator.egg-info/dependency_links.txt
+-rw-r--r--   0 foldedpond   (501) staff       (20)       35 2023-04-29 16:16:14.000000 SPTranslator-0.0.2/SPTranslator.egg-info/requires.txt
+-rw-r--r--   0 foldedpond   (501) staff       (20)       13 2023-04-29 16:16:14.000000 SPTranslator-0.0.2/SPTranslator.egg-info/top_level.txt
+-rw-r--r--   0 foldedpond   (501) staff       (20)      716 2023-04-29 16:05:31.000000 SPTranslator-0.0.2/pyproject.toml
+-rw-r--r--   0 foldedpond   (501) staff       (20)       38 2023-04-29 16:16:14.226571 SPTranslator-0.0.2/setup.cfg
+drwxr-xr-x   0 foldedpond   (501) staff       (20)        0 2023-04-29 16:16:14.219809 SPTranslator-0.0.2/sptranslator/
+-rw-r--r--   0 foldedpond   (501) staff       (20)        0 2023-04-24 10:23:38.000000 SPTranslator-0.0.2/sptranslator/__init__.py
+-rw-r--r--   0 foldedpond   (501) staff       (20)     3963 2023-04-29 09:49:44.000000 SPTranslator-0.0.2/sptranslator/translator.py
+drwxr-xr-x   0 foldedpond   (501) staff       (20)        0 2023-04-29 16:16:14.223940 SPTranslator-0.0.2/tests/
+-rw-r--r--   0 foldedpond   (501) staff       (20)     7083 2023-04-29 09:49:44.000000 SPTranslator-0.0.2/tests/test_translator.py
```

### Comparing `SPTranslator-0.0.1/LICENSE` & `SPTranslator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SPTranslator-0.0.1/PKG-INFO` & `SPTranslator-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: SPTranslator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library for translating in-code comments and documentation while preserving syntax and structure.
-Author-email: Yuta Oriike <122957026+uta0x89@users.noreply.github.com>
+Author-email: Yuta Oriike <nontrivial@hotmail.co.jp>
 Project-URL: Homepage, https://github.com/uta0x89/SPTranslator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # SPTranslator
 SPTranslator(SyntaxPreserveTranslator) is a Python library powered by OpenAI API and designed for developers who work with multilingual projects.
 This library seamlessly translates in-code comments and documentation while meticulously preserving the syntax and structure of your source code and data.
-
 SPTranslator supports a wide range of markup languages(e.g., HTML, LaTeX), programming languages(e.g., Python), and data formats(e.g., JSON) and effortlessly integrates with your existing workflow.
-The easy-to-use interface allows developers to focus on their core tasks, while SPTranslator handles the complexities of language translation.
 
 # Usage
 To use SPTranslator, first install the required dependencies:
 
 ```bash
 pip install -r requirements.txt
 ```
```

### Comparing `SPTranslator-0.0.1/README.md` & `SPTranslator-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # SPTranslator
 SPTranslator(SyntaxPreserveTranslator) is a Python library powered by OpenAI API and designed for developers who work with multilingual projects.
 This library seamlessly translates in-code comments and documentation while meticulously preserving the syntax and structure of your source code and data.
-
 SPTranslator supports a wide range of markup languages(e.g., HTML, LaTeX), programming languages(e.g., Python), and data formats(e.g., JSON) and effortlessly integrates with your existing workflow.
-The easy-to-use interface allows developers to focus on their core tasks, while SPTranslator handles the complexities of language translation.
 
 # Usage
 To use SPTranslator, first install the required dependencies:
 
 ```bash
 pip install -r requirements.txt
 ```
```

### Comparing `SPTranslator-0.0.1/SPTranslator.egg-info/PKG-INFO` & `SPTranslator-0.0.2/SPTranslator.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: SPTranslator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library for translating in-code comments and documentation while preserving syntax and structure.
-Author-email: Yuta Oriike <122957026+uta0x89@users.noreply.github.com>
+Author-email: Yuta Oriike <nontrivial@hotmail.co.jp>
 Project-URL: Homepage, https://github.com/uta0x89/SPTranslator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # SPTranslator
 SPTranslator(SyntaxPreserveTranslator) is a Python library powered by OpenAI API and designed for developers who work with multilingual projects.
 This library seamlessly translates in-code comments and documentation while meticulously preserving the syntax and structure of your source code and data.
-
 SPTranslator supports a wide range of markup languages(e.g., HTML, LaTeX), programming languages(e.g., Python), and data formats(e.g., JSON) and effortlessly integrates with your existing workflow.
-The easy-to-use interface allows developers to focus on their core tasks, while SPTranslator handles the complexities of language translation.
 
 # Usage
 To use SPTranslator, first install the required dependencies:
 
 ```bash
 pip install -r requirements.txt
 ```
```

### Comparing `SPTranslator-0.0.1/pyproject.toml` & `SPTranslator-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SPTranslator"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
-  { name="Yuta Oriike", email="122957026+uta0x89@users.noreply.github.com" },
+  { name="Yuta Oriike", email="nontrivial@hotmail.co.jp" },
 ]
 description = "Python library for translating in-code comments and documentation while preserving syntax and structure."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "openai",
+    "tiktoken",
+    "lark"
+]
+
+[project.optional-dependencies]
+dev = [
+    "pytest"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/uta0x89/SPTranslator"
```

### Comparing `SPTranslator-0.0.1/sptranslator/translator.py` & `SPTranslator-0.0.2/sptranslator/translator.py`

 * *Files identical despite different names*

### Comparing `SPTranslator-0.0.1/tests/test_translator.py` & `SPTranslator-0.0.2/tests/test_translator.py`

 * *Files identical despite different names*


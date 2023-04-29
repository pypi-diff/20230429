# Comparing `tmp/cmdify-0.1.1.tar.gz` & `tmp/cmdify-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdify-0.1.1.tar", last modified: Mon Apr 17 22:17:48 2023, max compression
+gzip compressed data, was "cmdify-0.1.2.tar", last modified: Sat Apr 29 18:26:23 2023, max compression
```

## Comparing `cmdify-0.1.1.tar` & `cmdify-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 22:17:48.482933 cmdify-0.1.1/
--rw-rw-rw-   0        0        0     1089 2023-04-07 23:54:03.000000 cmdify-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2432 2023-04-17 22:17:48.482933 cmdify-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1540 2023-04-17 21:48:50.000000 cmdify-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 22:17:48.458135 cmdify-0.1.1/cmdify/
--rw-rw-rw-   0        0        0        0 2023-04-07 23:41:16.000000 cmdify-0.1.1/cmdify/__init__.py
--rw-rw-rw-   0        0        0     3363 2023-04-17 22:14:08.000000 cmdify-0.1.1/cmdify/core.py
--rw-rw-rw-   0        0        0     5884 2023-04-17 21:32:39.000000 cmdify-0.1.1/cmdify/identifiers.py
--rw-rw-rw-   0        0        0     2254 2023-04-17 22:11:24.000000 cmdify-0.1.1/cmdify/interpreters.py
--rw-rw-rw-   0        0        0     3433 2023-04-15 17:26:21.000000 cmdify-0.1.1/cmdify/lexica.py
--rw-rw-rw-   0        0        0      498 2023-04-17 21:16:19.000000 cmdify-0.1.1/cmdify/preprocessors.py
--rw-rw-rw-   0        0        0     3833 2023-04-17 21:11:30.000000 cmdify-0.1.1/cmdify/result.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:17:48.482933 cmdify-0.1.1/cmdify.egg-info/
--rw-rw-rw-   0        0        0     2432 2023-04-17 22:17:48.000000 cmdify-0.1.1/cmdify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-04-17 22:17:48.000000 cmdify-0.1.1/cmdify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 22:17:48.000000 cmdify-0.1.1/cmdify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-17 22:17:48.000000 cmdify-0.1.1/cmdify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 22:17:48.000000 cmdify-0.1.1/cmdify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1229 2023-04-17 22:15:41.000000 cmdify-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 22:17:48.482933 cmdify-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      222 2023-04-17 20:17:21.000000 cmdify-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 18:26:23.013684 cmdify-0.1.2/
+-rw-rw-rw-   0        0        0     1089 2023-04-24 19:59:16.000000 cmdify-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2432 2023-04-29 18:26:23.013684 cmdify-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1540 2023-04-24 19:59:16.000000 cmdify-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 18:26:22.980914 cmdify-0.1.2/cmdify/
+-rw-rw-rw-   0        0        0        0 2023-04-24 19:59:16.000000 cmdify-0.1.2/cmdify/__init__.py
+-rw-rw-rw-   0        0        0     3363 2023-04-24 19:59:16.000000 cmdify-0.1.2/cmdify/core.py
+-rw-rw-rw-   0        0        0     5882 2023-04-26 19:15:19.000000 cmdify-0.1.2/cmdify/identifiers.py
+-rw-rw-rw-   0        0        0     2254 2023-04-24 19:59:16.000000 cmdify-0.1.2/cmdify/interpreters.py
+-rw-rw-rw-   0        0        0     3327 2023-04-29 18:21:17.000000 cmdify-0.1.2/cmdify/lexica.py
+-rw-rw-rw-   0        0        0      498 2023-04-24 19:59:16.000000 cmdify-0.1.2/cmdify/preprocessors.py
+-rw-rw-rw-   0        0        0     3833 2023-04-24 19:59:16.000000 cmdify-0.1.2/cmdify/result.py
+drwxrwxrwx   0        0        0        0 2023-04-29 18:26:23.013684 cmdify-0.1.2/cmdify.egg-info/
+-rw-rw-rw-   0        0        0     2432 2023-04-29 18:26:22.000000 cmdify-0.1.2/cmdify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-04-29 18:26:22.000000 cmdify-0.1.2/cmdify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 18:26:22.000000 cmdify-0.1.2/cmdify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-29 18:26:22.000000 cmdify-0.1.2/cmdify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-29 18:26:22.000000 cmdify-0.1.2/cmdify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1229 2023-04-29 18:24:52.000000 cmdify-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 18:26:23.013684 cmdify-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      222 2023-04-24 19:59:16.000000 cmdify-0.1.2/setup.py
```

### Comparing `cmdify-0.1.1/LICENSE.txt` & `cmdify-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cmdify-0.1.1/PKG-INFO` & `cmdify-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cmdify
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight command-line language processing utility.
 Author-email: Daniel Roland <its.daniel.roland@gmail.com>, "Jonathan M. Lobmeyer" <jmlobmeyer@gmail.com>, Nicole Livingston <nliving73@gmail.com>, William Blazer <williamblazer2@gmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/dqnnyr/cmdify.git
 Keywords: nlp,lightweight,command line,language processing,natural language processing,twilight imperium,ti4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # cmdify
 
 A lightweight command-line language processing tool, originally developed for Twilight Imperium 4.
```

### Comparing `cmdify-0.1.1/README.md` & `cmdify-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cmdify-0.1.1/cmdify/core.py` & `cmdify-0.1.2/cmdify/core.py`

 * *Files identical despite different names*

### Comparing `cmdify-0.1.1/cmdify/identifiers.py` & `cmdify-0.1.2/cmdify/identifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 
 class IdentifierWrapper(Identifier, abc.ABC):
     def __init__(self, identifier: Identifier):
         super().__init__(identifier.word_index, identifier.threshold)
         self._identifier = identifier
 
 
-
 class LiteralIdentifier(Identifier):
     def identify(self, token: str) -> tuple[list[str], int]:
         if token in self.word_index:
             return [self.word_index[token]], 0
         return [], 0
```

### Comparing `cmdify-0.1.1/cmdify/interpreters.py` & `cmdify-0.1.2/cmdify/interpreters.py`

 * *Files identical despite different names*

### Comparing `cmdify-0.1.1/cmdify/lexica.py` & `cmdify-0.1.2/cmdify/lexica.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,19 +48,17 @@
 
     def values(self):
         return self._synonym_index.values()
 
 
 class WordClassifier:
     """
-    Constructs a reverse index for the purposes of getting a 'canonical representation' of words.
-
     .. highlight:: python
     .. code-block:: python
-        wc = SynonymReverseIndex({'noun': ['apple', 'orange'], 'verb': ['eat']})
+        wc = WordClassifier({'noun': ['apple', 'orange'], 'verb': ['eat']})
         assert 'apple' in wc['noun']
         assert 'eat' in wc['verb']
     """
     def __init__(self, **classifications_and_words):
         self._data = {}
         for classification, words in classifications_and_words.items():
             self._data[classification] = set(words)
```

### Comparing `cmdify-0.1.1/cmdify/result.py` & `cmdify-0.1.2/cmdify/result.py`

 * *Files identical despite different names*

### Comparing `cmdify-0.1.1/cmdify.egg-info/PKG-INFO` & `cmdify-0.1.2/cmdify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cmdify
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight command-line language processing utility.
 Author-email: Daniel Roland <its.daniel.roland@gmail.com>, "Jonathan M. Lobmeyer" <jmlobmeyer@gmail.com>, Nicole Livingston <nliving73@gmail.com>, William Blazer <williamblazer2@gmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/dqnnyr/cmdify.git
 Keywords: nlp,lightweight,command line,language processing,natural language processing,twilight imperium,ti4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # cmdify
 
 A lightweight command-line language processing tool, originally developed for Twilight Imperium 4.
```

### Comparing `cmdify-0.1.1/pyproject.toml` & `cmdify-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools", "setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cmdify"
-version = "0.1.1"
+version = "0.1.2"
 description = "A lightweight command-line language processing utility."
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 license = {text = "MIT License"}
 authors = [
     {name = "Daniel Roland", email = "its.daniel.roland@gmail.com"},
     {name = "Jonathan M. Lobmeyer", email = "jmlobmeyer@gmail.com"},
     {name = "Nicole Livingston", email = "nliving73@gmail.com"},
     {name = "William Blazer", email = "williamblazer2@gmail.com"},
 ]
```


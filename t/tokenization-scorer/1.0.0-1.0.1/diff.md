# Comparing `tmp/tokenization-scorer-1.0.0.tar.gz` & `tmp/tokenization-scorer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenization-scorer-1.0.0.tar", last modified: Sat Apr 29 17:29:26 2023, max compression
+gzip compressed data, was "tokenization-scorer-1.0.1.tar", last modified: Sat Apr 29 17:37:37 2023, max compression
```

## Comparing `tokenization-scorer-1.0.0.tar` & `tokenization-scorer-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vilda     (1000) vilda     (1000)        0 2023-04-29 17:29:26.060148 tokenization-scorer-1.0.0/
--rw-rw-r--   0 vilda     (1000) vilda     (1000)      579 2023-04-29 17:29:26.060148 tokenization-scorer-1.0.0/PKG-INFO
--rw-rw-r--   0 vilda     (1000) vilda     (1000)      665 2023-04-29 17:24:13.000000 tokenization-scorer-1.0.0/README.md
--rw-rw-r--   0 vilda     (1000) vilda     (1000)      138 2023-04-29 16:39:07.000000 tokenization-scorer-1.0.0/pyproject.toml
--rw-rw-r--   0 vilda     (1000) vilda     (1000)       38 2023-04-29 17:29:26.060148 tokenization-scorer-1.0.0/setup.cfg
--rw-rw-r--   0 vilda     (1000) vilda     (1000)      906 2023-04-29 17:29:13.000000 tokenization-scorer-1.0.0/setup.py
-drwxrwxr-x   0 vilda     (1000) vilda     (1000)        0 2023-04-29 17:29:26.060148 tokenization-scorer-1.0.0/tokenization_scorer/
--rw-rw-r--   0 vilda     (1000) vilda     (1000)     2299 2023-04-29 17:18:32.000000 tokenization-scorer-1.0.0/tokenization_scorer/__init__.py
--rw-rw-r--   0 vilda     (1000) vilda     (1000)     3724 2023-04-29 17:18:37.000000 tokenization-scorer-1.0.0/tokenization_scorer/metrics.py
-drwxrwxr-x   0 vilda     (1000) vilda     (1000)        0 2023-04-29 17:29:26.060148 tokenization-scorer-1.0.0/tokenization_scorer.egg-info/
--rw-rw-r--   0 vilda     (1000) vilda     (1000)      579 2023-04-29 17:29:26.000000 tokenization-scorer-1.0.0/tokenization_scorer.egg-info/PKG-INFO
--rw-rw-r--   0 vilda     (1000) vilda     (1000)      314 2023-04-29 17:29:26.000000 tokenization-scorer-1.0.0/tokenization_scorer.egg-info/SOURCES.txt
--rw-rw-r--   0 vilda     (1000) vilda     (1000)        1 2023-04-29 17:29:26.000000 tokenization-scorer-1.0.0/tokenization_scorer.egg-info/dependency_links.txt
--rw-rw-r--   0 vilda     (1000) vilda     (1000)      114 2023-04-29 17:29:26.000000 tokenization-scorer-1.0.0/tokenization_scorer.egg-info/entry_points.txt
--rw-rw-r--   0 vilda     (1000) vilda     (1000)       20 2023-04-29 17:29:26.000000 tokenization-scorer-1.0.0/tokenization_scorer.egg-info/top_level.txt
+drwxrwxr-x   0 vilda     (1000) vilda     (1000)        0 2023-04-29 17:37:37.197261 tokenization-scorer-1.0.1/
+-rw-rw-r--   0 vilda     (1000) vilda     (1000)      579 2023-04-29 17:37:37.197261 tokenization-scorer-1.0.1/PKG-INFO
+-rw-rw-r--   0 vilda     (1000) vilda     (1000)      665 2023-04-29 17:24:13.000000 tokenization-scorer-1.0.1/README.md
+-rw-rw-r--   0 vilda     (1000) vilda     (1000)      138 2023-04-29 16:39:07.000000 tokenization-scorer-1.0.1/pyproject.toml
+-rw-rw-r--   0 vilda     (1000) vilda     (1000)       38 2023-04-29 17:37:37.197261 tokenization-scorer-1.0.1/setup.cfg
+-rw-rw-r--   0 vilda     (1000) vilda     (1000)      906 2023-04-29 17:37:31.000000 tokenization-scorer-1.0.1/setup.py
+drwxrwxr-x   0 vilda     (1000) vilda     (1000)        0 2023-04-29 17:37:37.197261 tokenization-scorer-1.0.1/tokenization_scorer/
+-rw-rw-r--   0 vilda     (1000) vilda     (1000)     2306 2023-04-29 17:37:11.000000 tokenization-scorer-1.0.1/tokenization_scorer/__init__.py
+-rw-rw-r--   0 vilda     (1000) vilda     (1000)     3731 2023-04-29 17:36:46.000000 tokenization-scorer-1.0.1/tokenization_scorer/metrics.py
+drwxrwxr-x   0 vilda     (1000) vilda     (1000)        0 2023-04-29 17:37:37.197261 tokenization-scorer-1.0.1/tokenization_scorer.egg-info/
+-rw-rw-r--   0 vilda     (1000) vilda     (1000)      579 2023-04-29 17:37:37.000000 tokenization-scorer-1.0.1/tokenization_scorer.egg-info/PKG-INFO
+-rw-rw-r--   0 vilda     (1000) vilda     (1000)      314 2023-04-29 17:37:37.000000 tokenization-scorer-1.0.1/tokenization_scorer.egg-info/SOURCES.txt
+-rw-rw-r--   0 vilda     (1000) vilda     (1000)        1 2023-04-29 17:37:37.000000 tokenization-scorer-1.0.1/tokenization_scorer.egg-info/dependency_links.txt
+-rw-rw-r--   0 vilda     (1000) vilda     (1000)      114 2023-04-29 17:37:37.000000 tokenization-scorer-1.0.1/tokenization_scorer.egg-info/entry_points.txt
+-rw-rw-r--   0 vilda     (1000) vilda     (1000)       20 2023-04-29 17:37:37.000000 tokenization-scorer-1.0.1/tokenization_scorer.egg-info/top_level.txt
```

### Comparing `tokenization-scorer-1.0.0/PKG-INFO` & `tokenization-scorer-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenization-scorer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for evaluating text tokenizations.
 Home-page: https://github.com/zouharvi/tokenization-scorer
 Author: Vilém Zouhar
 Author-email: vzouhar@ethz.ch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tokenization-scorer-1.0.0/README.md` & `tokenization-scorer-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tokenization-scorer-1.0.0/setup.py` & `tokenization-scorer-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='tokenization-scorer',
-    version='1.0.0',
+    version='1.0.1',
     author='Vilém Zouhar',
     author_email='vzouhar@ethz.ch',
     description=('Package for evaluating text tokenizations.'),
     long_description="""
         Simple package for evaluating text tokenizations. The input is a text (list of files or stdin) and output a single number.
         The higher the number, the better the tokenization.
         The intended workflow is to try multiple tokenizations and select the one with the highest number.
```

### Comparing `tokenization-scorer-1.0.0/tokenization_scorer/__init__.py` & `tokenization-scorer-1.0.1/tokenization_scorer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from typing import Union, Generator, List
 import argparse
 import tqdm
 from .metrics import get_metric
 
-
 def score(
     text: Union[str, Generator, List[Generator]],
     metric: str = "renyi",
     **kwargs
 ) -> float:
     # be generous when parsing the input to allow for list of files and strings
     if type(text) == str:
-        text = [l for l in tqdm.tqdm(text.split("\n"))]
+        text = [l.split() for l in tqdm.tqdm(text.split("\n"))]
     else:
         text = list(text)
         if type(text[0]) != str:
             # flatten once more
             text = [w for l in text for w in tqdm.tqdm(l)]
         text = [l.rstrip("\n").split() for l in tqdm.tqdm(text)]
```

### Comparing `tokenization-scorer-1.0.0/tokenization_scorer/metrics.py` & `tokenization-scorer-1.0.1/tokenization_scorer/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from collections import Counter
 import numpy as np
 import sys
 
-
-def _seq_len(text):
-    # negate so that higher is always better
-    return -np.average([len(l) for l in text])
-
-
 def get_prob_distribution(text):
     words_freqs = list(Counter((w for l in text for w in l)).most_common())
     total_subwords = sum([x[1] for x in words_freqs])
     freqs = [
         freq
         for word, freq in words_freqs
     ]
     probs = [
         freq / total_subwords
         for freq in freqs
     ]
     vocab_size = len(words_freqs)
     return freqs, probs, vocab_size
 
+def _seq_len(text, **kwargs):
+    # negate so that higher is always better
+    return -np.average([len(l) for l in text])
 
 def _renyi_efficiency(text, **kwargs):
     # set default
     if "power" not in kwargs:
         print("Setting power to 3.0 (default)", file=sys.stderr)
         kwargs["power"] = 3.0
```

### Comparing `tokenization-scorer-1.0.0/tokenization_scorer.egg-info/PKG-INFO` & `tokenization-scorer-1.0.1/tokenization_scorer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenization-scorer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for evaluating text tokenizations.
 Home-page: https://github.com/zouharvi/tokenization-scorer
 Author: Vilém Zouhar
 Author-email: vzouhar@ethz.ch
 Classifier: Programming Language :: Python :: 3
```


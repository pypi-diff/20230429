# Comparing `tmp/scispacy-0.5.1.tar.gz` & `tmp/scispacy-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scispacy-0.5.1.tar", last modified: Wed Sep  7 00:26:43 2022, max compression
+gzip compressed data, was "dist/scispacy-0.5.2.tar", last modified: Sat Apr 29 21:21:24 2023, max compression
```

## Comparing `scispacy-0.5.1.tar` & `scispacy-0.5.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 00:26:43.000000 scispacy-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-07 00:26:29.000000 scispacy-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-09-07 00:26:29.000000 scispacy-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    18022 2022-09-07 00:26:43.000000 scispacy-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14979 2022-09-07 00:26:29.000000 scispacy-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 00:26:43.000000 scispacy-0.5.1/data/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-07 00:26:29.000000 scispacy-0.5.1/data/bc5cdr_ner.json
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-09-07 00:26:29.000000 scispacy-0.5.1/data/bionlp13cg_ner.json
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-09-07 00:26:29.000000 scispacy-0.5.1/data/craft_ner.json
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-07 00:26:29.000000 scispacy-0.5.1/data/jnlpba_ner.json
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-09-07 00:26:29.000000 scispacy-0.5.1/data/meta_large.json
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-09-07 00:26:29.000000 scispacy-0.5.1/data/meta_medium.json
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-09-07 00:26:29.000000 scispacy-0.5.1/data/meta_scibert.json
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-09-07 00:26:29.000000 scispacy-0.5.1/data/meta_small.json
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-09-07 00:26:29.000000 scispacy-0.5.1/requirements.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 00:26:43.000000 scispacy-0.5.1/scispacy/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10355 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/abbreviation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3604 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/base_project_code.py
--rw-r--r--   0 runner    (1001) docker     (121)    20753 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/candidate_generation.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/consts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/custom_sentence_segmenter.py
--rw-r--r--   0 runner    (1001) docker     (121)     5411 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/custom_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    10609 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/data_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     4930 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/file_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    16192 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/hearst_patterns.py
--rw-r--r--   0 runner    (1001) docker     (121)     4840 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/hyponym_detector.py
--rw-r--r--   0 runner    (1001) docker     (121)     5996 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/linking.py
--rw-r--r--   0 runner    (1001) docker     (121)     3974 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/linking_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4045 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/per_class_scorer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/train_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/umls_linking.py
--rw-r--r--   0 runner    (1001) docker     (121)     4306 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/umls_semantic_type_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     6756 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/umls_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-09-07 00:26:29.000000 scispacy-0.5.1/scispacy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 00:26:43.000000 scispacy-0.5.1/scispacy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18022 2022-09-07 00:26:42.000000 scispacy-0.5.1/scispacy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-09-07 00:26:43.000000 scispacy-0.5.1/scispacy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-07 00:26:42.000000 scispacy-0.5.1/scispacy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-07 00:26:42.000000 scispacy-0.5.1/scispacy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-07 00:26:42.000000 scispacy-0.5.1/scispacy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-07 00:26:43.000000 scispacy-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-09-07 00:26:29.000000 scispacy-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:21:24.000000 scispacy-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 21:21:14.000000 scispacy-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-29 21:21:14.000000 scispacy-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-04-29 21:21:24.000000 scispacy-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15001 2023-04-29 21:21:14.000000 scispacy-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:21:24.000000 scispacy-0.5.2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-29 21:21:14.000000 scispacy-0.5.2/data/bc5cdr_ner.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-29 21:21:14.000000 scispacy-0.5.2/data/bionlp13cg_ner.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-29 21:21:14.000000 scispacy-0.5.2/data/craft_ner.json
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-29 21:21:14.000000 scispacy-0.5.2/data/jnlpba_ner.json
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-29 21:21:14.000000 scispacy-0.5.2/data/meta_large.json
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-29 21:21:14.000000 scispacy-0.5.2/data/meta_medium.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-29 21:21:14.000000 scispacy-0.5.2/data/meta_scibert.json
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-29 21:21:14.000000 scispacy-0.5.2/data/meta_small.json
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-29 21:21:14.000000 scispacy-0.5.2/requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:21:24.000000 scispacy-0.5.2/scispacy/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10869 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/abbreviation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/base_project_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20822 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/candidate_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/custom_sentence_segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/custom_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/data_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/hearst_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/hyponym_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/linking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/linking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/per_class_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/train_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/umls_linking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/umls_semantic_type_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/umls_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-29 21:21:14.000000 scispacy-0.5.2/scispacy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:21:24.000000 scispacy-0.5.2/scispacy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-04-29 21:21:24.000000 scispacy-0.5.2/scispacy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-29 21:21:24.000000 scispacy-0.5.2/scispacy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:21:24.000000 scispacy-0.5.2/scispacy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-29 21:21:24.000000 scispacy-0.5.2/scispacy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 21:21:24.000000 scispacy-0.5.2/scispacy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 21:21:24.000000 scispacy-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-29 21:21:14.000000 scispacy-0.5.2/setup.py
```

### Comparing `scispacy-0.5.1/LICENSE` & `scispacy-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scispacy-0.5.1/PKG-INFO` & `scispacy-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scispacy
-Version: 0.5.1
+Version: 0.5.2
 Summary: A full SpaCy pipeline and models for scientific/biomedical documents.
 Home-page: https://allenai.github.io/SciSpaCy/
 Author: Allen Institute for Artificial Intelligence
 Author-email: ai2-info@allenai.org
 License: Apache
 Description: <p align="center"><img width="50%" src="docs/scispacy-logo.png" /></p>
         
@@ -35,23 +35,23 @@
         Additionally, scispacy uses modern features of Python and as such is only available for **Python 3.6 or greater**.
         
         
         
         #### Setting up a virtual environment
         
         [Conda](https://conda.io/) can be used set up a virtual environment with the
-        version of Python required for scispaCy.  If you already have a Python 3.6 or 3.7
+        version of Python required for scispaCy.  If you already have a Python
         environment you want to use, you can skip to the 'installing via pip' section.
         
         1.  [Follow the installation instructions for Conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html?highlight=conda#regular-installation).
         
-        2.  Create a Conda environment called "scispacy" with Python 3.6:
+        2.  Create a Conda environment called "scispacy" with Python 3.9 (any version >= 3.6 should work):
         
             ```bash
-            conda create -n scispacy python=3.6
+            conda create -n scispacy python=3.9
             ```
         
         3.  Activate the Conda environment. You will need to activate the Conda environment in each terminal in which you want to use scispaCy.
         
             ```bash
             source activate scispacy
             ```
```

### Comparing `scispacy-0.5.1/README.md` & `scispacy-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 Additionally, scispacy uses modern features of Python and as such is only available for **Python 3.6 or greater**.
 
 
 
 #### Setting up a virtual environment
 
 [Conda](https://conda.io/) can be used set up a virtual environment with the
-version of Python required for scispaCy.  If you already have a Python 3.6 or 3.7
+version of Python required for scispaCy.  If you already have a Python
 environment you want to use, you can skip to the 'installing via pip' section.
 
 1.  [Follow the installation instructions for Conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html?highlight=conda#regular-installation).
 
-2.  Create a Conda environment called "scispacy" with Python 3.6:
+2.  Create a Conda environment called "scispacy" with Python 3.9 (any version >= 3.6 should work):
 
     ```bash
-    conda create -n scispacy python=3.6
+    conda create -n scispacy python=3.9
     ```
 
 3.  Activate the Conda environment. You will need to activate the Conda environment in each terminal in which you want to use scispaCy.
 
     ```bash
     source activate scispacy
     ```
```

### Comparing `scispacy-0.5.1/scispacy/abbreviation.py` & `scispacy-0.5.2/scispacy/abbreviation.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,28 @@
         if word_lengths > long_index:
             starting_index = i
             break
 
     return short_form_candidate, long_form_candidate[starting_index:]
 
 
+def span_contains_unbalanced_parentheses(span: Span) -> bool:
+    stack_counter = 0
+    for token in span:
+        if token.text == "(":
+            stack_counter += 1
+        elif token.text == ")":
+            if stack_counter > 0:
+                stack_counter -= 1
+            else:
+                return True
+
+    return stack_counter != 0
+
+
 def filter_matches(
     matcher_output: List[Tuple[int, int, int]], doc: Doc
 ) -> List[Tuple[Span, Span]]:
     # Filter into two cases:
     # 1. <Short Form> ( <Long Form> )
     # 2. <Long Form> (<Short Form>) [this case is most common].
     candidates = []
@@ -96,14 +110,18 @@
         if end - start > 8 or start == 1:
             continue
         if end - start > 3:
             # Long form is inside the parens.
             # Take one word before.
             short_form_candidate = doc[start - 2 : start - 1]
             long_form_candidate = doc[start:end]
+
+            # make sure any parentheses inside long form are balanced
+            if span_contains_unbalanced_parentheses(long_form_candidate):
+                continue
         else:
             # Normal case.
             # Short form is inside the parens.
             short_form_candidate = doc[start:end]
 
             # Sum character lengths of contents of parens.
             abbreviation_length = sum([len(x) for x in short_form_candidate])
@@ -186,15 +204,15 @@
 
     def __call__(self, doc: Doc) -> Doc:
         matches = self.matcher(doc)
         matches_no_brackets = [(x[0], x[1] + 1, x[2] - 1) for x in matches]
         filtered = filter_matches(matches_no_brackets, doc)
         occurences = self.find_matches_for(filtered, doc)
 
-        for (long_form, short_forms) in occurences:
+        for long_form, short_forms in occurences:
             for short in short_forms:
                 short._.long_form = long_form
                 doc._.abbreviations.append(short)
         if self.make_serializable:
             abbreviations = doc._.abbreviations
             doc._.abbreviations = [
                 self.make_short_form_serializable(abbreviation)
@@ -205,15 +223,15 @@
     def find_matches_for(
         self, filtered: List[Tuple[Span, Span]], doc: Doc
     ) -> List[Tuple[Span, Set[Span]]]:
         rules = {}
         all_occurences: Dict[Span, Set[Span]] = defaultdict(set)
         already_seen_long: Set[str] = set()
         already_seen_short: Set[str] = set()
-        for (long_candidate, short_candidate) in filtered:
+        for long_candidate, short_candidate in filtered:
             short, long = find_abbreviation(long_candidate, short_candidate)
             # We need the long and short form definitions to be unique, because we need
             # to store them so we can look them up later. This is a bit of a
             # pathalogical case also, as it would mean an abbreviation had been
             # defined twice in a document. There's not much we can do about this,
             # but at least the case which is discarded will be picked up below by
             # the global matcher. So it's likely that things will work out ok most of the time.
```

### Comparing `scispacy-0.5.1/scispacy/base_project_code.py` & `scispacy-0.5.2/scispacy/base_project_code.py`

 * *Files identical despite different names*

### Comparing `scispacy-0.5.1/scispacy/candidate_generation.py` & `scispacy-0.5.2/scispacy/candidate_generation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, Tuple, NamedTuple, Type
+from typing import Optional, List, Dict, Tuple, NamedTuple, Type
 import json
 import datetime
 from collections import defaultdict
 
 import scipy
 import numpy
 import joblib
@@ -37,46 +37,46 @@
     ann_index: str
     tfidf_vectorizer: str
     tfidf_vectors: str
     concept_aliases_list: str
 
 
 UmlsLinkerPaths = LinkerPaths(
-    ann_index="https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/data/linkers/2020-10-09/umls/nmslib_index.bin",  # noqa
-    tfidf_vectorizer="https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/data/linkers/2020-10-09/umls/tfidf_vectorizer.joblib",  # noqa
-    tfidf_vectors="https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/data/linkers/2020-10-09/umls/tfidf_vectors_sparse.npz",  # noqa
-    concept_aliases_list="https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/data/linkers/2020-10-09/umls/concept_aliases.json",  # noqa
+    ann_index="https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/data/linkers/2023-04-23/umls/nmslib_index.bin",  # noqa
+    tfidf_vectorizer="https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/data/linkers/2023-04-23/umls/tfidf_vectorizer.joblib",  # noqa
+    tfidf_vectors="https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/data/linkers/2023-04-23/umls/tfidf_vectors_sparse.npz",  # noqa
+    concept_aliases_list="https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/data/linkers/2023-04-23/umls/concept_aliases.json",  # noqa
 )
 
 MeshLinkerPaths = LinkerPaths(
-    ann_index="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/mesh/nmslib_index.bin",  # noqa
-    tfidf_vectorizer="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/mesh/tfidf_vectorizer.joblib",  # noqa
-    tfidf_vectors="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/mesh/tfidf_vectors_sparse.npz",  # noqa
-    concept_aliases_list="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/mesh/concept_aliases.json",  # noqa
+    ann_index="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/mesh/nmslib_index.bin",  # noqa
+    tfidf_vectorizer="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/mesh/tfidf_vectorizer.joblib",  # noqa
+    tfidf_vectors="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/mesh/tfidf_vectors_sparse.npz",  # noqa
+    concept_aliases_list="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/mesh/concept_aliases.json",  # noqa
 )
 
 GeneOntologyLinkerPaths = LinkerPaths(
-    ann_index="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/go/nmslib_index.bin",  # noqa
-    tfidf_vectorizer="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/go/tfidf_vectorizer.joblib",  # noqa
-    tfidf_vectors="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/go/tfidf_vectors_sparse.npz",  # noqa
-    concept_aliases_list="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/go/concept_aliases.json",  # noqa
+    ann_index="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/go/nmslib_index.bin",  # noqa
+    tfidf_vectorizer="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/go/tfidf_vectorizer.joblib",  # noqa
+    tfidf_vectors="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/go/tfidf_vectors_sparse.npz",  # noqa
+    concept_aliases_list="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/go/concept_aliases.json",  # noqa
 )
 
 HumanPhenotypeOntologyLinkerPaths = LinkerPaths(
-    ann_index="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/hpo/nmslib_index.bin",  # noqa
-    tfidf_vectorizer="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/hpo/tfidf_vectorizer.joblib",  # noqa
-    tfidf_vectors="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/hpo/tfidf_vectors_sparse.npz",  # noqa
-    concept_aliases_list="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/hpo/concept_aliases.json",  # noqa
+    ann_index="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/hpo/nmslib_index.bin",  # noqa
+    tfidf_vectorizer="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/hpo/tfidf_vectorizer.joblib",  # noqa
+    tfidf_vectors="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/hpo/tfidf_vectors_sparse.npz",  # noqa
+    concept_aliases_list="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/hpo/concept_aliases.json",  # noqa
 )
 
 RxNormLinkerPaths = LinkerPaths(
-    ann_index="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/rxnorm/nmslib_index.bin",  # noqa
-    tfidf_vectorizer="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/rxnorm/tfidf_vectorizer.joblib",  # noqa
-    tfidf_vectors="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/rxnorm/tfidf_vectors_sparse.npz",  # noqa
-    concept_aliases_list="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2020-10-09/rxnorm/concept_aliases.json",  # noqa
+    ann_index="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/rxnorm/nmslib_index.bin",  # noqa
+    tfidf_vectorizer="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/rxnorm/tfidf_vectorizer.joblib",  # noqa
+    tfidf_vectors="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/rxnorm/tfidf_vectors_sparse.npz",  # noqa
+    concept_aliases_list="https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/linkers/2023-04-23/rxnorm/concept_aliases.json",  # noqa
 )
 
 
 DEFAULT_PATHS: Dict[str, LinkerPaths] = {
     "umls": UmlsLinkerPaths,
     "mesh": MeshLinkerPaths,
     "go": GeneOntologyLinkerPaths,
@@ -192,23 +192,22 @@
         if a preconstructed ann_index is passed.
     name: str, optional (default = None)
         The name of the pretrained entity linker to load. Must be one of 'umls' or 'mesh'.
     """
 
     def __init__(
         self,
-        ann_index: FloatIndex = None,
-        tfidf_vectorizer: TfidfVectorizer = None,
-        ann_concept_aliases_list: List[str] = None,
-        kb: KnowledgeBase = None,
+        ann_index: Optional[FloatIndex] = None,
+        tfidf_vectorizer: Optional[TfidfVectorizer] = None,
+        ann_concept_aliases_list: Optional[List[str]] = None,
+        kb: Optional[KnowledgeBase] = None,
         verbose: bool = False,
         ef_search: int = 200,
-        name: str = None,
+        name: Optional[str] = None,
     ) -> None:
-
         if name is not None and any(
             [ann_index, tfidf_vectorizer, ann_concept_aliases_list, kb]
         ):
             raise ValueError(
                 "You cannot pass both a name argument and other constuctor arguments."
             )
 
@@ -359,15 +358,15 @@
 
             batch_mention_candidates.append(mention_candidates)
 
         return batch_mention_candidates
 
 
 def create_tfidf_ann_index(
-    out_path: str, kb: KnowledgeBase = None
+    out_path: str, kb: Optional[KnowledgeBase] = None
 ) -> Tuple[List[str], TfidfVectorizer, FloatIndex]:
     """
     Build tfidf vectorizer and ann index.
 
     Parameters
     ----------
     out_path: str, required.
```

### Comparing `scispacy-0.5.1/scispacy/custom_sentence_segmenter.py` & `scispacy-0.5.2/scispacy/custom_sentence_segmenter.py`

 * *Files identical despite different names*

### Comparing `scispacy-0.5.1/scispacy/custom_tokenizer.py` & `scispacy-0.5.2/scispacy/custom_tokenizer.py`

 * *Files identical despite different names*

### Comparing `scispacy-0.5.1/scispacy/data_util.py` & `scispacy-0.5.2/scispacy/data_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import NamedTuple, List, Iterator, Dict, Tuple
+from typing import Optional, NamedTuple, List, Iterator, Dict, Tuple
 import tarfile
 import atexit
 import os
 import shutil
 import tempfile
 
 from scispacy.file_cache import cached_path
@@ -144,17 +144,18 @@
     )
 
     return sorted(spacy_format_entities_without_overlap, key=lambda x: x[0])
 
 
 def read_full_med_mentions(
     directory_path: str,
-    label_mapping: Dict[str, str] = None,
+    label_mapping: Optional[Dict[str, str]] = None,
     span_only: bool = False,
     spacy_format: bool = True,
+    use_umls_ids: bool = False,
 ):
     def _cleanup_dir(dir_path: str):
         if os.path.exists(dir_path):
             shutil.rmtree(dir_path)
 
     resolved_directory_path = cached_path(directory_path)
     if "tar.gz" in directory_path:
@@ -205,15 +206,20 @@
         if label_mapping is None:
             return label
         else:
             return label_mapping[label]
 
     for example in examples:
         spacy_format_entities = [
-            (x.start, x.end, label_function(x.mention_type)) for x in example.entities
+            (
+                x.start,
+                x.end,
+                label_function(x.mention_type) if not use_umls_ids else x.umls_id,
+            )
+            for x in example.entities
         ]
         spacy_format_entities = remove_overlapping_entities(
             sorted(spacy_format_entities, key=lambda x: x[0])
         )
         spacy_example = (example.text, {"entities": spacy_format_entities})
         if example.pubmed_id in train_ids:
             train_examples.append(spacy_example if spacy_format else example)
```

### Comparing `scispacy-0.5.1/scispacy/file_cache.py` & `scispacy-0.5.2/scispacy/file_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 
 import os
 import shutil
 import tempfile
 import json
 from urllib.parse import urlparse
 from pathlib import Path
-from typing import Tuple, Union, IO
+from typing import Optional, Tuple, Union, IO
 from hashlib import sha256
 
 import requests
 
 CACHE_ROOT = Path(os.getenv("SCISPACY_CACHE", str(Path.home() / ".scispacy")))
 DATASET_CACHE = str(CACHE_ROOT / "datasets")
 
 
-def cached_path(url_or_filename: Union[str, Path], cache_dir: str = None) -> str:
+def cached_path(
+    url_or_filename: Union[str, Path], cache_dir: Optional[str] = None
+) -> str:
     """
     Given something that might be a URL (or might be a local path),
     determine which. If it's a URL, download the file and cache it, and
     return the path to the cached file. If it's already a local path,
     make sure the file exists and then return the path.
     """
     if cache_dir is None:
@@ -43,15 +45,15 @@
     else:
         # Something unknown
         raise ValueError(
             "unable to parse {} as a URL or as a local path".format(url_or_filename)
         )
 
 
-def url_to_filename(url: str, etag: str = None) -> str:
+def url_to_filename(url: str, etag: Optional[str] = None) -> str:
     """
     Convert `url` into a hashed filename in a repeatable way.
     If `etag` is specified, append its hash to the url's, delimited
     by a period.
     """
 
     last_part = url.split("/")[-1]
@@ -64,15 +66,15 @@
         etag_hash = sha256(etag_bytes)
         filename += "." + etag_hash.hexdigest()
 
     filename += "." + last_part
     return filename
 
 
-def filename_to_url(filename: str, cache_dir: str = None) -> Tuple[str, str]:
+def filename_to_url(filename: str, cache_dir: Optional[str] = None) -> Tuple[str, str]:
     """
     Return the url and etag (which may be ``None``) stored for `filename`.
     Raise ``FileNotFoundError`` if `filename` or its stored metadata do not exist.
     """
     if cache_dir is None:
         cache_dir = DATASET_CACHE
 
@@ -95,15 +97,15 @@
 def http_get(url: str, temp_file: IO) -> None:
     req = requests.get(url, stream=True)
     for chunk in req.iter_content(chunk_size=1024):
         if chunk:  # filter out keep-alive new chunks
             temp_file.write(chunk)
 
 
-def get_from_cache(url: str, cache_dir: str = None) -> str:
+def get_from_cache(url: str, cache_dir: Optional[str] = None) -> str:
     """
     Given a URL, look for the corresponding dataset in the local cache.
     If it's not there, download it. Then return the path to the cached file.
     """
     if cache_dir is None:
         cache_dir = DATASET_CACHE
```

### Comparing `scispacy-0.5.1/scispacy/hearst_patterns.py` & `scispacy-0.5.2/scispacy/hearst_patterns.py`

 * *Files identical despite different names*

### Comparing `scispacy-0.5.1/scispacy/hyponym_detector.py` & `scispacy-0.5.2/scispacy/hyponym_detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     name: `str`, a required argument for spacy to use this as a factory
     extended: `bool`, whether to use the extended Hearts patterns or not
     """
 
     def __init__(
         self, nlp: Language, name: str = "hyponym_detector", extended: bool = False
     ):
-
         self.nlp = nlp
 
         self.patterns = BASE_PATTERNS
         if extended:
             self.patterns.extend(EXTENDED_PATTERNS)
 
         self.matcher = Matcher(self.nlp.vocab)
@@ -87,15 +86,14 @@
                 end += 1
             else:
                 break
 
         return doc[start:end]
 
     def find_noun_compound_head(self, token: Token):
-
         while token.head.pos_ in {"PROPN", "NOUN", "PRON"} and token.dep_ == "compound":
             token = token.head
         return token
 
     def __call__(self, doc: Doc):
         """
         Runs the matcher on the Doc object and sets token and
@@ -131,15 +129,14 @@
             hyponym_extended = self.expand_to_noun_compound(hyponym, doc)
 
             doc._.hearst_patterns.append(
                 (predicate, hypernym_extended, hyponym_extended)
             )
 
             for token in hyponym.conjuncts:
-
                 token_extended = self.expand_to_noun_compound(token, doc)
                 if token != hypernym and token is not None:
                     doc._.hearst_patterns.append(
                         (predicate, hypernym_extended, token_extended)
                     )
 
         return doc
```

### Comparing `scispacy-0.5.1/scispacy/linking.py` & `scispacy-0.5.2/scispacy/linking.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from spacy.tokens import Doc
 from spacy.tokens import Span
 from spacy.language import Language
 
 from scispacy.candidate_generation import CandidateGenerator
+from typing import Optional
 
 
 @Language.factory("scispacy_linker")
 class EntityLinker:
     """
     A spacy pipeline component which identifies entities in text which appear
     in a knowledge base.
@@ -62,24 +63,24 @@
         how many are nearest neighbours are found.
     linker_name: str, optional (default = None)
         The name of the pretrained entity linker to load.
     """
 
     def __init__(
         self,
-        nlp: Language = None,
+        nlp: Optional[Language] = None,
         name: str = "scispacy_linker",
-        candidate_generator: CandidateGenerator = None,
+        candidate_generator: Optional[CandidateGenerator] = None,
         resolve_abbreviations: bool = True,
         k: int = 30,
         threshold: float = 0.7,
         no_definition_threshold: float = 0.95,
         filter_for_definitions: bool = True,
         max_entities_per_mention: int = 5,
-        linker_name: str = None,
+        linker_name: Optional[str] = None,
     ):
         # TODO(Mark): Remove in scispacy v1.0.
         Span.set_extension("umls_ents", default=[], force=True)
         Span.set_extension("kb_ents", default=[], force=True)
 
         self.candidate_generator = candidate_generator or CandidateGenerator(
             name=linker_name
```

### Comparing `scispacy-0.5.1/scispacy/linking_utils.py` & `scispacy-0.5.2/scispacy/linking_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,21 @@
 from scispacy.umls_semantic_type_tree import (
     UmlsSemanticTypeTree,
     construct_umls_tree_from_tsv,
 )
 
 
 class Entity(NamedTuple):
-
     concept_id: str
     canonical_name: str
     aliases: List[str]
     types: List[str] = []
     definition: Optional[str] = None
 
     def __repr__(self):
-
         rep = ""
         num_aliases = len(self.aliases)
         rep = rep + f"CUI: {self.concept_id}, Name: {self.canonical_name}\n"
         rep = rep + f"Definition: {self.definition}\n"
         rep = rep + f"TUI(s): {', '.join(self.types)}\n"
         if num_aliases > 10:
             rep = (
@@ -32,15 +30,15 @@
         else:
             rep = (
                 rep + f"Aliases: (total: {num_aliases}): \n\t {', '.join(self.aliases)}"
             )
         return rep
 
 
-DEFAULT_UMLS_PATH = "https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/data/kbs/2020-10-09/umls_2020_aa_cat0129.jsonl"  # noqa
+DEFAULT_UMLS_PATH = "https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/data/kbs/2023-04-23/umls_2022_ab_cat0129.jsonl"  # noqa
 DEFAULT_UMLS_TYPES_PATH = "https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/data/umls_semantic_type_tree.tsv"
 
 
 class KnowledgeBase:
     """
     A class representing two commonly needed views of a Knowledge Base:
     1. A mapping from concept_id to an Entity NamedTuple with more information.
@@ -50,15 +48,15 @@
     ----------
     file_path: str, required.
         The file path to the json/jsonl representation of the KB to load.
     """
 
     def __init__(
         self,
-        file_path: str = None,
+        file_path: Optional[str] = None,
     ):
         if file_path is None:
             raise ValueError(
                 "Do not use the default arguments to KnowledgeBase. "
                 "Instead, use a subclass (e.g UmlsKnowledgeBase) or pass a path to a kb."
             )
         if file_path.endswith("jsonl"):
@@ -81,45 +79,44 @@
 
 class UmlsKnowledgeBase(KnowledgeBase):
     def __init__(
         self,
         file_path: str = DEFAULT_UMLS_PATH,
         types_file_path: str = DEFAULT_UMLS_TYPES_PATH,
     ):
-
         super().__init__(file_path)
 
         self.semantic_type_tree: UmlsSemanticTypeTree = construct_umls_tree_from_tsv(
             types_file_path
         )
 
 
 class Mesh(KnowledgeBase):
     def __init__(
         self,
-        file_path: str = "https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/kbs/2020-10-09/mesh_2020.jsonl",  # noqa
+        file_path: str = "https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/kbs/2023-04-23/umls_mesh_2022.jsonl",  # noqa
     ):
         super().__init__(file_path)
 
 
 class GeneOntology(KnowledgeBase):
     def __init__(
         self,
-        file_path: str = "https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/kbs/2020-10-09/umls_2020_go.jsonl",  # noqa
+        file_path: str = "https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/kbs/2023-04-23/umls_go_2022.jsonl",  # noqa
     ):
         super().__init__(file_path)
 
 
 class HumanPhenotypeOntology(KnowledgeBase):
     def __init__(
         self,
-        file_path: str = "https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/kbs/2020-10-09/umls_2020_hpo.jsonl",  # noqa
+        file_path: str = "https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/kbs/2023-04-23/umls_hpo_2022.jsonl",  # noqa
     ):
         super().__init__(file_path)
 
 
 class RxNorm(KnowledgeBase):
     def __init__(
         self,
-        file_path: str = "https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/kbs/2020-10-09/umls_2020_rxnorm.jsonl",  # noqa
+        file_path: str = "https://ai2-s2-scispacy.s3-us-west-2.amazonaws.com/data/kbs/2023-04-23/umls_rxnorm_2022.jsonl",  # noqa
     ):
         super().__init__(file_path)
```

### Comparing `scispacy-0.5.1/scispacy/per_class_scorer.py` & `scispacy-0.5.2/scispacy/per_class_scorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
         self._false_negatives: Dict[str, int] = defaultdict(int)
 
     def __call__(
         self,
         predicted_spans: List[Tuple[int, int, str]],
         gold_spans: List[Tuple[int, int, str]],
     ) -> None:
-
         gold_spans = copy.copy(gold_spans)
         predicted_spans = copy.copy(predicted_spans)
         untyped_gold_spans = {(x[0], x[1]) for x in gold_spans}
         untyped_predicted_spans = {(x[0], x[1]) for x in predicted_spans}
 
         for untyped_span, span in zip(untyped_predicted_spans, predicted_spans):
             if span in gold_spans:
```

### Comparing `scispacy-0.5.1/scispacy/train_utils.py` & `scispacy-0.5.2/scispacy/train_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import json
 
 import tqdm
 from spacy.language import Language
 
 from scispacy.per_class_scorer import PerClassScorer
+from typing import Optional
 
 
 def evaluate_ner(
-    nlp: Language, eval_data, dump_path: str = None, verbose: bool = False
+    nlp: Language, eval_data, dump_path: Optional[str] = None, verbose: bool = False
 ) -> PerClassScorer:
-
     scorer = PerClassScorer()
     print("Evaluating %d rows" % len(eval_data))
     for i, (text, gold_spans) in enumerate(tqdm.tqdm(eval_data)):
-
         # parse dev data with trained model
         doc = nlp(text)
         predicted_spans = [
             (ent.start_char, ent.end_char, ent.label_) for ent in doc.ents
         ]
         scorer(predicted_spans, gold_spans["entities"])
```

### Comparing `scispacy-0.5.1/scispacy/umls_semantic_type_tree.py` & `scispacy-0.5.2/scispacy/umls_semantic_type_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import NamedTuple, List, Dict, Deque, Any, Optional
 from collections import deque
 
 from scispacy.file_cache import cached_path
 
 
 class SemanticTypeNode(NamedTuple):
-
     type_id: str
     full_name: str
     children: List[Any]  # Mypy does not support nested types yet :(
     level: int
 
 
 class UmlsSemanticTypeTree:
@@ -77,15 +76,14 @@
         for node in self.get_nodes_at_depth(level):
             for child in self.get_children(node):
                 new_type_id_map[child.type_id] = node.type_id
         return new_type_id_map
 
 
 def construct_umls_tree_from_tsv(filepath: str) -> UmlsSemanticTypeTree:
-
     """
     Reads in a tsv file which is formatted as a depth first traversal of
     a hierarchy tree, where nodes are of the format:
 
     Name TAB UMLS Semantic Type TAB Tree Depth
 
     Event    T051    1
```

### Comparing `scispacy-0.5.1/scispacy/umls_utils.py` & `scispacy-0.5.2/scispacy/umls_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict
+from typing import Optional, List, Dict
 
 # TODO(Mark): Remove in scispacy v1.0, for backward compatability only.
 from scispacy.linking_utils import Entity as UmlsEntity, UmlsKnowledgeBase  # noqa
 
 # preferred definition sources (from S2)
 DEF_SOURCES_PREFERRED = {"NCI_BRIDG", "NCI_NCI-GLOSS", "NCI", "GO", "MSH", "NCI_FDA"}
 
@@ -33,15 +33,17 @@
             )  # ugly hack because all files end with an empty column
             if found_filename in filename:
                 return column_names
     assert False, f"Couldn't find column names for file {filename}"
     return None
 
 
-def read_umls_concepts(meta_path: str, concept_details: Dict, source: str = None):
+def read_umls_concepts(
+    meta_path: str, concept_details: Dict, source: Optional[str] = None
+):
     """
     Read the concepts file MRCONSO.RRF from a UMLS release and store it in
     concept_details dictionary. Each concept is represented with
     - concept_id
     - canonical_name
     - aliases
     - types
```

### Comparing `scispacy-0.5.1/scispacy/util.py` & `scispacy-0.5.2/scispacy/util.py`

 * *Files identical despite different names*

### Comparing `scispacy-0.5.1/scispacy.egg-info/PKG-INFO` & `scispacy-0.5.2/scispacy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scispacy
-Version: 0.5.1
+Version: 0.5.2
 Summary: A full SpaCy pipeline and models for scientific/biomedical documents.
 Home-page: https://allenai.github.io/SciSpaCy/
 Author: Allen Institute for Artificial Intelligence
 Author-email: ai2-info@allenai.org
 License: Apache
 Description: <p align="center"><img width="50%" src="docs/scispacy-logo.png" /></p>
         
@@ -35,23 +35,23 @@
         Additionally, scispacy uses modern features of Python and as such is only available for **Python 3.6 or greater**.
         
         
         
         #### Setting up a virtual environment
         
         [Conda](https://conda.io/) can be used set up a virtual environment with the
-        version of Python required for scispaCy.  If you already have a Python 3.6 or 3.7
+        version of Python required for scispaCy.  If you already have a Python
         environment you want to use, you can skip to the 'installing via pip' section.
         
         1.  [Follow the installation instructions for Conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html?highlight=conda#regular-installation).
         
-        2.  Create a Conda environment called "scispacy" with Python 3.6:
+        2.  Create a Conda environment called "scispacy" with Python 3.9 (any version >= 3.6 should work):
         
             ```bash
-            conda create -n scispacy python=3.6
+            conda create -n scispacy python=3.9
             ```
         
         3.  Activate the Conda environment. You will need to activate the Conda environment in each terminal in which you want to use scispaCy.
         
             ```bash
             source activate scispacy
             ```
```

### Comparing `scispacy-0.5.1/scispacy.egg-info/SOURCES.txt` & `scispacy-0.5.2/scispacy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scispacy-0.5.1/setup.py` & `scispacy-0.5.2/setup.py`

 * *Files identical despite different names*


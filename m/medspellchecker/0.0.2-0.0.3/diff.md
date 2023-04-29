# Comparing `tmp/medspellchecker-0.0.2.tar.gz` & `tmp/medspellchecker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medspellchecker-0.0.2.tar", last modified: Sat Apr 22 11:07:44 2023, max compression
+gzip compressed data, was "medspellchecker-0.0.3.tar", last modified: Sat Apr 29 17:52:57 2023, max compression
```

## Comparing `medspellchecker-0.0.2.tar` & `medspellchecker-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-22 11:07:44.716633 medspellchecker-0.0.2/
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    11357 2022-08-03 12:33:44.000000 medspellchecker-0.0.2/LICENSE
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4011 2023-04-22 11:07:44.716633 medspellchecker-0.0.2/PKG-INFO
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     3028 2023-04-02 21:46:08.000000 medspellchecker-0.0.2/README.md
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-22 11:07:44.708633 medspellchecker-0.0.2/medspellchecker/
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-22 11:07:44.712633 medspellchecker-0.0.2/medspellchecker/tool/
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     8720 2023-03-24 21:02:33.000000 medspellchecker-0.0.2/medspellchecker/tool/abstract_bert_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     3080 2023-03-24 21:02:33.000000 medspellchecker-0.0.2/medspellchecker/tool/abstract_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    14945 2022-12-16 21:23:05.000000 medspellchecker-0.0.2/medspellchecker/tool/candidate_generator.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      330 2022-12-14 21:21:48.000000 medspellchecker-0.0.2/medspellchecker/tool/candidate_word.py
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-22 11:07:44.712633 medspellchecker-0.0.2/medspellchecker/tool/data/
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)  4603445 2022-08-03 12:33:45.000000 medspellchecker-0.0.2/medspellchecker/tool/data/processed_lemmatized_all_dict.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      581 2022-12-16 21:23:05.000000 medspellchecker-0.0.2/medspellchecker/tool/distilbert_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4393 2022-12-14 21:21:48.000000 medspellchecker-0.0.2/medspellchecker/tool/edit_distance.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2434 2022-12-14 21:21:48.000000 medspellchecker-0.0.2/medspellchecker/tool/gpu_utils.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    13812 2023-04-10 20:03:39.000000 medspellchecker-0.0.2/medspellchecker/tool/medspellchecker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      169 2023-03-23 20:05:58.000000 medspellchecker-0.0.2/medspellchecker/tool/mistake_type.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4089 2023-04-10 18:03:51.000000 medspellchecker-0.0.2/medspellchecker/tool/pre_post_processor.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      568 2022-12-16 21:23:05.000000 medspellchecker-0.0.2/medspellchecker/tool/roberta_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      569 2022-12-16 23:37:30.000000 medspellchecker-0.0.2/medspellchecker/tool/rubert_tiny2_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      556 2023-03-17 18:40:55.000000 medspellchecker-0.0.2/medspellchecker/tool/rubioberta_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      563 2023-03-17 18:40:55.000000 medspellchecker-0.0.2/medspellchecker/tool/rubioroberta_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      938 2023-04-08 20:00:29.000000 medspellchecker-0.0.2/medspellchecker/tool/word.py
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-22 11:07:44.708633 medspellchecker-0.0.2/medspellchecker.egg-info/
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4011 2023-04-22 11:07:44.000000 medspellchecker-0.0.2/medspellchecker.egg-info/PKG-INFO
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      950 2023-04-22 11:07:44.000000 medspellchecker-0.0.2/medspellchecker.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        1 2023-04-22 11:07:44.000000 medspellchecker-0.0.2/medspellchecker.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      173 2023-04-22 11:07:44.000000 medspellchecker-0.0.2/medspellchecker.egg-info/requires.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       16 2023-04-22 11:07:44.000000 medspellchecker-0.0.2/medspellchecker.egg-info/top_level.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       38 2023-04-22 11:07:44.716633 medspellchecker-0.0.2/setup.cfg
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2036 2023-04-22 11:07:33.000000 medspellchecker-0.0.2/setup.py
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-29 17:52:57.527343 medspellchecker-0.0.3/
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    11357 2022-08-03 12:33:44.000000 medspellchecker-0.0.3/LICENSE
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       36 2023-04-29 17:52:50.000000 medspellchecker-0.0.3/MANIFEST.in
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     6333 2023-04-29 17:24:30.000000 medspellchecker-0.0.3/PACKAGE.md
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     7316 2023-04-29 17:52:57.527343 medspellchecker-0.0.3/PKG-INFO
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-29 17:52:57.519343 medspellchecker-0.0.3/medspellchecker/
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-29 17:52:57.523342 medspellchecker-0.0.3/medspellchecker/tool/
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     8720 2023-03-24 21:02:33.000000 medspellchecker-0.0.3/medspellchecker/tool/abstract_bert_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     3080 2023-03-24 21:02:33.000000 medspellchecker-0.0.3/medspellchecker/tool/abstract_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    14945 2022-12-16 21:23:05.000000 medspellchecker-0.0.3/medspellchecker/tool/candidate_generator.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      330 2022-12-14 21:21:48.000000 medspellchecker-0.0.3/medspellchecker/tool/candidate_word.py
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-29 17:52:57.523342 medspellchecker-0.0.3/medspellchecker/tool/data/
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)  4603445 2022-08-03 12:33:45.000000 medspellchecker-0.0.3/medspellchecker/tool/data/processed_lemmatized_all_dict.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      581 2022-12-16 21:23:05.000000 medspellchecker-0.0.3/medspellchecker/tool/distilbert_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4393 2022-12-14 21:21:48.000000 medspellchecker-0.0.3/medspellchecker/tool/edit_distance.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2434 2022-12-14 21:21:48.000000 medspellchecker-0.0.3/medspellchecker/tool/gpu_utils.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    13812 2023-04-22 11:19:05.000000 medspellchecker-0.0.3/medspellchecker/tool/medspellchecker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      169 2023-03-23 20:05:58.000000 medspellchecker-0.0.3/medspellchecker/tool/mistake_type.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4089 2023-04-10 18:03:51.000000 medspellchecker-0.0.3/medspellchecker/tool/pre_post_processor.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      568 2022-12-16 21:23:05.000000 medspellchecker-0.0.3/medspellchecker/tool/roberta_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      569 2022-12-16 23:37:30.000000 medspellchecker-0.0.3/medspellchecker/tool/rubert_tiny2_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      556 2023-03-17 18:40:55.000000 medspellchecker-0.0.3/medspellchecker/tool/rubioberta_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      563 2023-03-17 18:40:55.000000 medspellchecker-0.0.3/medspellchecker/tool/rubioroberta_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      938 2023-04-08 20:00:29.000000 medspellchecker-0.0.3/medspellchecker/tool/word.py
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-29 17:52:57.523342 medspellchecker-0.0.3/medspellchecker.egg-info/
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     7316 2023-04-29 17:52:57.000000 medspellchecker-0.0.3/medspellchecker.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      963 2023-04-29 17:52:57.000000 medspellchecker-0.0.3/medspellchecker.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        1 2023-04-29 17:52:57.000000 medspellchecker-0.0.3/medspellchecker.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      173 2023-04-29 17:52:57.000000 medspellchecker-0.0.3/medspellchecker.egg-info/requires.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       16 2023-04-29 17:52:57.000000 medspellchecker-0.0.3/medspellchecker.egg-info/top_level.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       38 2023-04-29 17:52:57.527343 medspellchecker-0.0.3/setup.cfg
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2019 2023-04-29 17:50:35.000000 medspellchecker-0.0.3/setup.py
```

### Comparing `medspellchecker-0.0.2/LICENSE` & `medspellchecker-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker/tool/abstract_bert_candidate_ranker.py` & `medspellchecker-0.0.3/medspellchecker/tool/abstract_bert_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker/tool/abstract_candidate_ranker.py` & `medspellchecker-0.0.3/medspellchecker/tool/abstract_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker/tool/candidate_generator.py` & `medspellchecker-0.0.3/medspellchecker/tool/candidate_generator.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker/tool/data/processed_lemmatized_all_dict.txt` & `medspellchecker-0.0.3/medspellchecker/tool/data/processed_lemmatized_all_dict.txt`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker/tool/distilbert_candidate_ranker.py` & `medspellchecker-0.0.3/medspellchecker/tool/distilbert_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker/tool/edit_distance.py` & `medspellchecker-0.0.3/medspellchecker/tool/edit_distance.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker/tool/gpu_utils.py` & `medspellchecker-0.0.3/medspellchecker/tool/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker/tool/medspellchecker.py` & `medspellchecker-0.0.3/medspellchecker/tool/medspellchecker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker/tool/pre_post_processor.py` & `medspellchecker-0.0.3/medspellchecker/tool/pre_post_processor.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker/tool/roberta_candidate_ranker.py` & `medspellchecker-0.0.3/medspellchecker/tool/roberta_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker/tool/rubert_tiny2_candidate_ranker.py` & `medspellchecker-0.0.3/medspellchecker/tool/rubert_tiny2_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker/tool/rubioberta_candidate_ranker.py` & `medspellchecker-0.0.3/medspellchecker/tool/rubioberta_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker/tool/rubioroberta_candidate_ranker.py` & `medspellchecker-0.0.3/medspellchecker/tool/rubioroberta_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker/tool/word.py` & `medspellchecker-0.0.3/medspellchecker/tool/word.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.2/medspellchecker.egg-info/SOURCES.txt` & `medspellchecker-0.0.3/medspellchecker.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
-README.md
+MANIFEST.in
+PACKAGE.md
 setup.py
 medspellchecker.egg-info/PKG-INFO
 medspellchecker.egg-info/SOURCES.txt
 medspellchecker.egg-info/dependency_links.txt
 medspellchecker.egg-info/requires.txt
 medspellchecker.egg-info/top_level.txt
 medspellchecker/tool/abstract_bert_candidate_ranker.py
```

### Comparing `medspellchecker-0.0.2/setup.py` & `medspellchecker-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import pathlib
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
-
+print(here / 'PACKAGE.md')
 # Get the long description from the README file
-long_description = (here / 'README.md').read_text(encoding='utf-8')
-
-print(find_packages(where='spellchecker'))
+long_description = (here / 'PACKAGE.md').read_text(encoding='utf-8')
 
 setup(
     name='medspellchecker',
-    version='0.0.2',
+    version='0.0.3',
     description='Fast and effective spellchecker for Russian medical texts',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/DmitryPogrebnoy/MedSpellChecker',
     author='Dmitry Pogrebnoy',
     author_email='pogrebnoy.inc@gmail.com',
     license='Apache License 2.0',
```


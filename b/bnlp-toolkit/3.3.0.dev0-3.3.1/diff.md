# Comparing `tmp/bnlp_toolkit-3.3.0.dev0.tar.gz` & `tmp/bnlp_toolkit-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bnlp_toolkit-3.3.0.dev0.tar", last modified: Thu Nov 17 09:00:45 2022, max compression
+gzip compressed data, was "bnlp_toolkit-3.3.1.tar", last modified: Sat Apr 29 03:41:10 2023, max compression
```

## Comparing `bnlp_toolkit-3.3.0.dev0.tar` & `bnlp_toolkit-3.3.1.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2022-11-17 09:00:45.000000 bnlp_toolkit-3.3.0.dev0/
--rw-rw-r--   0 sagor     (1000) sagor     (1000)     1069 2021-12-17 16:43:41.000000 bnlp_toolkit-3.3.0.dev0/LICENSE
--rw-rw-r--   0 sagor     (1000) sagor     (1000)    21174 2022-11-17 09:00:45.000000 bnlp_toolkit-3.3.0.dev0/PKG-INFO
--rw-rw-r--   0 sagor     (1000) sagor     (1000)    20642 2022-11-12 08:36:07.000000 bnlp_toolkit-3.3.0.dev0/README.md
-drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2022-11-17 09:00:45.000000 bnlp_toolkit-3.3.0.dev0/bnlp/
--rw-rw-r--   0 sagor     (1000) sagor     (1000)      390 2022-11-17 07:48:10.000000 bnlp_toolkit-3.3.0.dev0/bnlp/__init__.py
-drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2022-11-17 09:00:45.000000 bnlp_toolkit-3.3.0.dev0/bnlp/corpus/
--rw-rw-r--   0 sagor     (1000) sagor     (1000)     8139 2021-12-17 16:43:41.000000 bnlp_toolkit-3.3.0.dev0/bnlp/corpus/__init__.py
--rw-rw-r--   0 sagor     (1000) sagor     (1000)      390 2021-12-17 16:43:41.000000 bnlp_toolkit-3.3.0.dev0/bnlp/corpus/util.py
-drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2022-11-17 09:00:45.000000 bnlp_toolkit-3.3.0.dev0/bnlp/embedding/
--rw-rw-r--   0 sagor     (1000) sagor     (1000)        0 2021-12-17 16:43:41.000000 bnlp_toolkit-3.3.0.dev0/bnlp/embedding/__init__.py
--rw-rw-r--   0 sagor     (1000) sagor     (1000)     3411 2022-11-12 08:35:23.000000 bnlp_toolkit-3.3.0.dev0/bnlp/embedding/doc2vec.py
--rw-rw-r--   0 sagor     (1000) sagor     (1000)     3124 2021-12-17 16:43:41.000000 bnlp_toolkit-3.3.0.dev0/bnlp/embedding/fasttext.py
--rw-rw-r--   0 sagor     (1000) sagor     (1000)     1086 2021-12-17 16:43:41.000000 bnlp_toolkit-3.3.0.dev0/bnlp/embedding/glove.py
--rw-rw-r--   0 sagor     (1000) sagor     (1000)     6192 2021-12-17 16:43:41.000000 bnlp_toolkit-3.3.0.dev0/bnlp/embedding/word2vec.py
--rw-rw-r--   0 sagor     (1000) sagor     (1000)     4060 2022-11-17 05:14:52.000000 bnlp_toolkit-3.3.0.dev0/bnlp/ner.py
--rw-rw-r--   0 sagor     (1000) sagor     (1000)     3084 2021-12-17 16:43:41.000000 bnlp_toolkit-3.3.0.dev0/bnlp/pos.py
-drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2022-11-17 09:00:45.000000 bnlp_toolkit-3.3.0.dev0/bnlp/tokenizer/
--rw-rw-r--   0 sagor     (1000) sagor     (1000)        0 2021-12-17 16:43:41.000000 bnlp_toolkit-3.3.0.dev0/bnlp/tokenizer/__init__.py
--rw-rw-r--   0 sagor     (1000) sagor     (1000)     3129 2021-12-17 16:43:41.000000 bnlp_toolkit-3.3.0.dev0/bnlp/tokenizer/basic.py
--rw-rw-r--   0 sagor     (1000) sagor     (1000)     1076 2021-12-17 16:43:41.000000 bnlp_toolkit-3.3.0.dev0/bnlp/tokenizer/nltk.py
--rw-rw-r--   0 sagor     (1000) sagor     (1000)     1229 2021-12-17 16:43:41.000000 bnlp_toolkit-3.3.0.dev0/bnlp/tokenizer/sentencepiece.py
--rw-rw-r--   0 sagor     (1000) sagor     (1000)      291 2022-11-17 05:01:42.000000 bnlp_toolkit-3.3.0.dev0/bnlp/tokenizer/spacy.py
-drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2022-11-17 09:00:45.000000 bnlp_toolkit-3.3.0.dev0/bnlp_toolkit.egg-info/
--rw-rw-r--   0 sagor     (1000) sagor     (1000)    21174 2022-11-17 09:00:45.000000 bnlp_toolkit-3.3.0.dev0/bnlp_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 sagor     (1000) sagor     (1000)      579 2022-11-17 09:00:45.000000 bnlp_toolkit-3.3.0.dev0/bnlp_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 sagor     (1000) sagor     (1000)        1 2022-11-17 09:00:45.000000 bnlp_toolkit-3.3.0.dev0/bnlp_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 sagor     (1000) sagor     (1000)      124 2022-11-17 09:00:45.000000 bnlp_toolkit-3.3.0.dev0/bnlp_toolkit.egg-info/requires.txt
--rw-rw-r--   0 sagor     (1000) sagor     (1000)        9 2022-11-17 09:00:45.000000 bnlp_toolkit-3.3.0.dev0/bnlp_toolkit.egg-info/top_level.txt
-drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2022-11-17 09:00:45.000000 bnlp_toolkit-3.3.0.dev0/msc/
--rw-rw-r--   0 sagor     (1000) sagor     (1000)        0 2022-11-07 15:17:07.000000 bnlp_toolkit-3.3.0.dev0/msc/__init__.py
--rw-rw-r--   0 sagor     (1000) sagor     (1000)     5639 2022-11-17 05:18:20.000000 bnlp_toolkit-3.3.0.dev0/msc/test.py
--rw-rw-r--   0 sagor     (1000) sagor     (1000)       38 2022-11-17 09:00:45.000000 bnlp_toolkit-3.3.0.dev0/setup.cfg
--rw-rw-r--   0 sagor     (1000) sagor     (1000)      978 2022-11-17 07:47:36.000000 bnlp_toolkit-3.3.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.691246 bnlp_toolkit-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-04-29 03:41:10.691246 bnlp_toolkit-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22844 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.687246 bnlp_toolkit-3.3.1/bnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.687246 bnlp_toolkit-3.3.1/bnlp/cleantext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/cleantext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/cleantext/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/cleantext/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.687246 bnlp_toolkit-3.3.1/bnlp/corpus/
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/corpus/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.687246 bnlp_toolkit-3.3.1/bnlp/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/embedding/doc2vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/embedding/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/embedding/glove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/embedding/word2vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/pos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.687246 bnlp_toolkit-3.3.1/bnlp/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/tokenizer/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/tokenizer/nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/bnlp/tokenizer/sentencepiece.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.691246 bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-04-29 03:41:10.000000 bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-29 03:41:10.000000 bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 03:41:10.000000 bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-29 03:41:10.000000 bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 03:41:10.000000 bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 03:41:10.691246 bnlp_toolkit-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:41:10.691246 bnlp_toolkit-3.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-04-29 03:40:58.000000 bnlp_toolkit-3.3.1/tests/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bnlp_toolkit-3.3.0.dev0/LICENSE` & `bnlp_toolkit-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.0.dev0/PKG-INFO` & `bnlp_toolkit-3.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,96 @@
 Metadata-Version: 2.1
 Name: bnlp_toolkit
-Version: 3.3.0.dev0
+Version: 3.3.1
 Summary: BNLP is a natural language processing toolkit for Bengali Language
 Home-page: https://github.com/sagorbrur/bnlp
 Author: Sagor Sarker
 Author-email: sagorhem3532@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: spacy
-Provides-Extra: fasttext
 License-File: LICENSE
 
-<img align="left" height="70" src="bnlp.svg" alt="bnlp"/>
-
 # Bengali Natural Language Processing(BNLP)
 
-[![Build Status](https://travis-ci.org/sagorbrur/bnlp.svg?branch=master)](https://travis-ci.org/sagorbrur/bnlp)
 [![PyPI version](https://img.shields.io/pypi/v/bnlp_toolkit)](https://pypi.org/project/bnlp-toolkit/)
 [![Downloads](https://pepy.tech/badge/bnlp-toolkit)](https://pepy.tech/project/bnlp-toolkit)
-[![Documentation Status](https://readthedocs.org/projects/bnlp/badge/?version=latest)](https://bnlp.readthedocs.io/en/latest/?badge=latest)
-[![Gitter](https://badges.gitter.im/bnlp_toolkit/community.svg)](https://gitter.im/bnlp_toolkit/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
-BNLP is a natural language processing toolkit for Bengali Language. This tool will help you to **tokenize Bengali text**, **Embedding Bengali words**, **Embedding Bengali Document**, **Bengali POS Tagging**, **Bengali Name Entity Recognition**, **Construct Neural Model** for Bengali NLP purposes.
+BNLP is a natural language processing toolkit for Bengali Language. This tool will help you to **tokenize Bengali text**, **Embedding Bengali words**, **Embedding Bengali Document**, **Bengali POS Tagging**, **Bengali Name Entity Recognition**, **Bangla Text Cleaning** for Bengali NLP purposes.
 
+Table of contents
+=================
 
+<!--ts-->
+   * [Installation](#installation)
+      * [PIP installer](#pip-installer)
+   * [Pretrained Model](#pretrained-model)
+      * [Download Links](#download-links)
+      * [Training Details](#training-details)
+   * [Tokenization](#tokenization)
+      * [Basic Tokenizer](#basic-tokenizer)
+      * [NLTK Tokenization](#nltk-tokenization)
+      * [Bengali SentencePiece Tokenization](#bengali-sentencepiece-tokenization)
+         * [Tokenization using trained model](#tokenization-using-trained-model)
+         * [Training SentencePiece](#training-sentencepiece)
+   * [Word Embedding](#word-embedding)
+      * [Bengali Word2Vec](#bengali-word2vec)
+         * [Generate Vector using pretrain model](#generate-vector-using-pretrain-model)
+         * [Find Most Similar Word Using Pretrained Model](#find-most-similar-word-using-pretrained-model)
+         * [Train Bengali Word2Vec with your own data](#train-bengali-word2vec-with-your-own-data)
+         * [Pre-train or resume word2vec training with same or new corpus or tokenized sentences](#pre-train-or-resume-word2vec-training-with-same-or-new-corpus-or-tokenized-sentences)
+     * [Bengali FastText](#bengali-fasttext)
+        * [Generate Vector Using Pretrained Model](#generate-vector-using-pretrain-model)
+        * [Train Bengali FastText Model](#train-bengali-fasttext-model)
+        * [Generate Vector File from Fasttext Binary Model](#generate-vector-file-from-fasttext-binary-model)
+     * [Bengali GloVe Word Vectors](#bengali-glove-word-vectors)
+   * [Document Embedding](#document-embedding)
+      * [Bengali Doc2Vec](#bengali-doc2vec)
+         * [Get document vector from input document](#get-document-vector-from-input-document)
+         * [Find document similarity between two document](#find-document-similarity-between-two-document)
+         * [Train doc2vec vector with custom text files](#train-doc2vec-vector-with-custom-text-files)
+   * [Bengali POS Tagging](#bengali-pos-tagging)
+      * [Bengali CRF POS Tagging](#bengali-crf-pos-tagging)
+         * [Find Pos Tag Using Pretrained Model](#find-pos-tag-using-pretrained-model)
+         * [Train POS Tag Model](#train-pos-tag-model)
+   * [Bengali NER](#bengali-ner)
+      * [Bengali CRF NER](#bengali-crf-ner)
+         * [Find NER Tag Using Pretrained Model](#find-ner-tag-using-pretrained-model)
+         * [Train NER Tag Model](#train-ner-tag-model)
+   * [Bengali Corpus Class](#bengali-corpus-class)
+      * [Stopwords and Punctuations](#stopwords-and-punctuations)
+      * [Remove stopwords from Text](#remove-stopwords-from-text)
+   * [Bangla Text Cleaning](#text-cleaning)
+   * [Contributor Guide](#contributor-guide)
+<!--te-->
+---
 
 ## Installation
 
-### PIP installer(Python: 3.6, 3.7, 3.8 tested okay, OS: linux, windows tested okay )
+### PIP installer
 
   ```
   pip install bnlp_toolkit
   ```
   **or Upgrade**
 
   ```
   pip install -U bnlp_toolkit
-
   ```
+  - Python: 3.6, 3.7, 3.8, 3.9
+  - OS: Linux, Windows, Mac
 
 
 
 ## Pretrained Model
 
-### Download Link
+### Download Links
 
 Large model published in [huggingface](https://huggingface.co/) model hub.
 
 * [Bengali SentencePiece](https://github.com/sagorbrur/bnlp/tree/master/model)
 * [Bengali Word2Vec](https://huggingface.co/sagorsarker/bangla_word2vec)
 * [Bengali FastText](https://huggingface.co/sagorsarker/bangla-fasttext)
 * [Bengali GloVe Wordvectors](https://huggingface.co/sagorsarker/bangla-glove-vectors)
@@ -63,360 +102,372 @@
 ### Training Details
 * Sentencepiece, Word2Vec, Fasttext, GloVe model trained with **Bengali Wikipedia Dump Dataset**
   - [Bengali Wiki Dump](https://dumps.wikimedia.org/bnwiki/latest/)
 * SentencePiece Training Vocab Size=50000
 * Fasttext trained with total words = 20M, vocab size = 1171011, epoch=50, embedding dimension = 300 and the training loss = 0.318668,
 * Word2Vec word embedding dimension = 100, min_count=5, window=5, epochs=10
 * To Know Bengali GloVe Wordvector and training process follow [this](https://github.com/sagorbrur/GloVe-Bengali) repository
-* Bengali CRF POS Tagging was training with [nltr](https://github.com/abhishekgupta92/bangla_pos_tagger/tree/master/data) dataset with 80% accuracy. 
+* Bengali CRF POS Tagging was training with [nltr](https://github.com/abhishekgupta92/bangla_pos_tagger/tree/master/data) dataset with 80% accuracy.
 * Bengali CRF NER Tagging was train with [this](https://github.com/MISabic/NER-Bangla-Dataset) data with 90% accuracy.
 * Bengali news article doc2vec model train with 8 jsons of [this](https://www.kaggle.com/datasets/ebiswas/bangla-largest-newspaper-dataset) corpus with epochs 40 vector size 100 min_count=2, total news article 400013
 * Bengali wikipedia doc2vec model trained with wikipedia dump datasets. Total articles 110448, epochs: 40, vector_size: 100, min_count: 2
 
 
 ## Tokenization
 
-* **Basic Tokenizer**
-
- 
+### Basic Tokenizer
 
   ```py
   from bnlp import BasicTokenizer
+  
   basic_tokenizer = BasicTokenizer()
   raw_text = "আমি বাংলায় গান গাই।"
   tokens = basic_tokenizer.tokenize(raw_text)
   print(tokens)
-  
-  # output: ["আমি", "বাংলায়", "গান", "গাই", "।"]
 
+  # output: ["আমি", "বাংলায়", "গান", "গাই", "।"]
   ```
 
-* **NLTK Tokenization**
+### NLTK Tokenization
 
   ```py
   from bnlp import NLTKTokenizer
-  
+
   bnltk = NLTKTokenizer()
   text = "আমি ভাত খাই। সে বাজারে যায়। তিনি কি সত্যিই ভালো মানুষ?"
   word_tokens = bnltk.word_tokenize(text)
   sentence_tokens = bnltk.sentence_tokenize(text)
   print(word_tokens)
   print(sentence_tokens)
-  
+
   # output
   # word_token: ["আমি", "ভাত", "খাই", "।", "সে", "বাজারে", "যায়", "।", "তিনি", "কি", "সত্যিই", "ভালো", "মানুষ", "?"]
   # sentence_token: ["আমি ভাত খাই।", "সে বাজারে যায়।", "তিনি কি সত্যিই ভালো মানুষ?"]
-
   ```
 
 
-* **Bengali SentencePiece Tokenization**
-
-  - tokenization using trained model
-    ```py
-    from bnlp import SentencepieceTokenizer
-
-    bsp = SentencepieceTokenizer()
-    model_path = "./model/bn_spm.model"
-    input_text = "আমি ভাত খাই। সে বাজারে যায়।"
-    tokens = bsp.tokenize(model_path, input_text)
-    print(tokens)
-    text2id = bsp.text2id(model_path, input_text)
-    print(text2id)
-    id2text = bsp.id2text(model_path, text2id)
-    print(id2text)
-
-    ```
-  - Training SentencePiece
-    ```py
-    from bnlp import SentencepieceTokenizer
-    
-    bsp = SentencepieceTokenizer()
-    data = "raw_text.txt"
-    model_prefix = "test"
-    vocab_size = 5
-    bsp.train(data, model_prefix, vocab_size) 
-
-    ```
-
+### Bengali SentencePiece Tokenization
 
+#### Tokenization using trained model
+```py
+from bnlp import SentencepieceTokenizer
+
+bsp = SentencepieceTokenizer()
+model_path = "./model/bn_spm.model"
+input_text = "আমি ভাত খাই। সে বাজারে যায়।"
+tokens = bsp.tokenize(model_path, input_text)
+print(tokens)
+text2id = bsp.text2id(model_path, input_text)
+print(text2id)
+id2text = bsp.id2text(model_path, text2id)
+print(id2text)
+```
+
+#### Training SentencePiece
+```py
+from bnlp import SentencepieceTokenizer
+
+bsp = SentencepieceTokenizer()
+data = "raw_text.txt"
+model_prefix = "test"
+vocab_size = 5
+bsp.train(data, model_prefix, vocab_size)
+```
 
 ## Word Embedding
 
-* **Bengali Word2Vec**
+### Bengali Word2Vec
+
+#### Generate Vector using pretrain model
 
-  - Generate Vector using pretrain model
+```py
+from bnlp import BengaliWord2Vec
 
-    ```py
-    from bnlp import BengaliWord2Vec
+bwv = BengaliWord2Vec()
+model_path = "bengali_word2vec.model"
+word = 'গ্রাম'
+vector = bwv.generate_word_vector(model_path, word)
+print(vector.shape)
+print(vector)
+```
 
-    bwv = BengaliWord2Vec()
-    model_path = "bengali_word2vec.model"
-    word = 'গ্রাম'
-    vector = bwv.generate_word_vector(model_path, word)
-    print(vector.shape)
-    print(vector)
+#### Find Most Similar Word Using Pretrained Model
 
-    ```
+```py
+from bnlp import BengaliWord2Vec
 
-  - Find Most Similar Word Using Pretrained Model
+bwv = BengaliWord2Vec()
+model_path = "bengali_word2vec.model"
+word = 'গ্রাম'
+similar = bwv.most_similar(model_path, word, topn=10)
+print(similar)
+```
+#### Train Bengali Word2Vec with your own data
 
-    ```py
-    from bnlp import BengaliWord2Vec
+Train Bengali word2vec with your custom raw data or tokenized sentences.
 
-    bwv = BengaliWord2Vec()
-    model_path = "bengali_word2vec.model"
-    word = 'গ্রাম'
-    similar = bwv.most_similar(model_path, word, topn=10)
-    print(similar)
+Custom tokenized sentence format example:
+```py
+sentences = [['আমি', 'ভাত', 'খাই', '।'], ['সে', 'বাজারে', 'যায়', '।']]
+```
+Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
 
-    ```
-  - Train Bengali Word2Vec with your own data
+```py
+from bnlp import BengaliWord2Vec
+bwv = BengaliWord2Vec()
+data_file = "raw_text.txt" # or you can pass custom sentence tokens as list of list
+model_name = "test_model.model"
+vector_name = "test_vector.vector"
+bwv.train(data_file, model_name, vector_name, epochs=5)
+```
 
-    Train Bengali word2vec with your custom raw data or tokenized sentences.
+#### Pre-train or resume word2vec training with same or new corpus or tokenized sentences
 
-    custom tokenized sentence format example:
-    ```
-    sentences = [['আমি', 'ভাত', 'খাই', '।'], ['সে', 'বাজারে', 'যায়', '।']]
-    ```
-    Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
+Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
 
-    ```py
-    from bnlp import BengaliWord2Vec
-    bwv = BengaliWord2Vec()
-    data_file = "raw_text.txt" # or you can pass custom sentence tokens as list of list
-    model_name = "test_model.model"
-    vector_name = "test_vector.vector"
-    bwv.train(data_file, model_name, vector_name, epochs=5)
+```py
+from bnlp import BengaliWord2Vec
+bwv = BengaliWord2Vec()
 
+trained_model_path = "mytrained_model.model"
+data_file = "raw_text.txt"
+model_name = "test_model.model"
+vector_name = "test_vector.vector"
+bwv.pretrain(trained_model_path, data_file, model_name, vector_name, epochs=5)
+```
 
-    ```
-  - Pre-train or resume word2vec training with same or new corpus or tokenized sentences
+### Bengali FastText
 
-    Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
+To use `fasttext` you need to install fasttext manually by `pip install fasttext==0.9.2`
 
-    ```py
-    from bnlp import BengaliWord2Vec
-    bwv = BengaliWord2Vec()
+NB: `fasttext` may not be worked in `windows`, it will only work in `linux`
 
-    trained_model_path = "mytrained_model.model"
-    data_file = "raw_text.txt"
-    model_name = "test_model.model"
-    vector_name = "test_vector.vector"
-    bwv.pretrain(trained_model_path, data_file, model_name, vector_name, epochs=5)
+### Generate Vector Using Pretrained Model
 
-    ```
-    
- * **Bengali FastText**
- 
-    To use `fasttext` you need to install fasttext manually by `pip install fasttext==0.9.2`
-    
-    NB: `fasttext` may not be worked in `windows`, it will only work in `linux`
+  ```py
+  from bnlp.embedding.fasttext import BengaliFasttext
 
-    - Generate Vector Using Pretrained Model
-      
+  bft = BengaliFasttext()
+  word = "গ্রাম"
+  model_path = "bengali_fasttext_wiki.bin"
+  word_vector = bft.generate_word_vector(model_path, word)
+  print(word_vector.shape)
+  print(word_vector)
+  ```
 
-      ```py
-      from bnlp.embedding.fasttext import BengaliFasttext
+### Train Bengali FastText Model
 
-      bft = BengaliFasttext()
-      word = "গ্রাম"
-      model_path = "bengali_fasttext_wiki.bin"
-      word_vector = bft.generate_word_vector(model_path, word)
-      print(word_vector.shape)
-      print(word_vector)
+Check [fasttext documentation](https://fasttext.cc/docs/en/options.html) for details of training parameter
 
+  ```py
+  from bnlp.embedding.fasttext import BengaliFasttext
 
-      ```
-    - Train Bengali FastText Model
+  bft = BengaliFasttext()
+  data = "raw_text.txt"
+  model_name = "saved_model.bin"
+  epoch = 50
+  bft.train(data, model_name, epoch)
+  ```
 
-      Check [fasttext documentation](https://fasttext.cc/docs/en/options.html) for details of training parameter
+### Generate Vector File from Fasttext Binary Model
 
-      ```py
-      from bnlp.embedding.fasttext import BengaliFasttext
+```py
+from bnlp.embedding.fasttext import BengaliFasttext
 
-      bft = BengaliFasttext()
-      data = "raw_text.txt"
-      model_name = "saved_model.bin"
-      epoch = 50
-      bft.train(data, model_name, epoch)
-      ```
+bft = BengaliFasttext()
 
-    - Generate Vector File from Fasttext Binary Model
-      ```py
-      from bnlp.embedding.fasttext import BengaliFasttext
+model_path = "mymodel.bin"
+out_vector_name = "myvector.txt"
+bft.bin2vec(model_path, out_vector_name)
+```
+
+## Bengali GloVe Word Vectors
+
+We trained glove model with bengali data(wiki+news articles) and published bengali glove word vectors</br>
+You can download and use it on your different machine learning purposes.
+
+```py
+from bnlp import BengaliGlove
+glove_path = "bn_glove.39M.100d.txt"
+word = "গ্রাম"
+bng = BengaliGlove()
+res = bng.closest_word(glove_path, word)
+print(res)
+vec = bng.word2vec(glove_path, word)
+print(vec)
+```
 
-      bft = BengaliFasttext()
+## Document Embedding
 
-      model_path = "mymodel.bin"
-      out_vector_name = "myvector.txt"
-      bft.bin2vec(model_path, out_vector_name)
-      ```
+### Bengali Doc2Vec
+#### Get document vector from input document
 
-* **Bengali GloVe Word Vectors**
+```py
+from bnlp import BengaliDoc2vec
 
-  We trained glove model with bengali data(wiki+news articles) and published bengali glove word vectors</br>
-  You can download and use it on your different machine learning purposes.
+bn_doc2vec = BengaliDoc2vec()
 
-  ```py
-  from bnlp import BengaliGlove
-  glove_path = "bn_glove.39M.100d.txt"
-  word = "গ্রাম"
-  bng = BengaliGlove()
-  res = bng.closest_word(glove_path, word)
-  print(res)
-  vec = bng.word2vec(glove_path, word)
-  print(vec)
+model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
+document = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
 
-  ```
+vector = bn_doc2vec.get_document_vector(model_path, text)
+print(vector)
+```
 
-## Document Embedding
-* __Bengali Doc2Vec__
-  - Get document vector from input document
+#### Find document similarity between two document
 
-    ```py
-    from bnlp import BengaliDoc2vec
-    
-    bn_doc2vec = BengaliDoc2vec()
-    
-    model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
-    document = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
-
-    vector = bn_doc2vec.get_document_vector(model_path, text)
-    print(vector)
-    ```
-
-  - Find document similarity between two document
-
-    ```py
-    from bnlp import BengaliDoc2vec
-    
-    bn_doc2vec = BengaliDoc2vec()
-    
-    model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
-    article_1 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
-    article_2 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
-
-    similarity = bn_doc2vec.get_document_similarity(
-      model_path,
-      article_1,
-      article_2
-    )
-    print(similarity)
-
-    ```
-
-  - Train doc2vec vector with custom text files
-
-    ```py
-    from bnlp import BengaliDoc2vec
-      
-    bn_doc2vec = BengaliDoc2vec()
-
-    text_files = "path/myfiles"
-    checkpoint_path = "msc/logs"
-
-    bn_doc2vec.train_doc2vec(
-      text_files, 
-      checkpoint_path=checkpoint_path,
-      vector_size=100,
-      min_count=2,
-      epochs=10
-    )
+```py
+from bnlp import BengaliDoc2vec
 
-    # it will train doc2vec with your text files and save the train model in checkpoint_path
+bn_doc2vec = BengaliDoc2vec()
 
-    ```
+model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
+article_1 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
+article_2 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
 
-## Bengali POS Tagging
-* **Bengali CRF POS Tagging** 
+similarity = bn_doc2vec.get_document_similarity(
+  model_path,
+  article_1,
+  article_2
+)
+print(similarity)
+```
 
+#### Train doc2vec vector with custom text files
 
-  - Find Pos Tag Using Pretrained Model
+```py
+from bnlp import BengaliDoc2vec
 
-    ```py
-    from bnlp import POS
-    bn_pos = POS()
-    model_path = "model/bn_pos.pkl"
-    text = "আমি ভাত খাই।" # or you can pass ['আমি', 'ভাত', 'খাই', '।']
-    res = bn_pos.tag(model_path, text)
-    print(res)
-    # [('আমি', 'PPR'), ('ভাত', 'NC'), ('খাই', 'VM'), ('।', 'PU')]
+bn_doc2vec = BengaliDoc2vec()
 
-    ```
-  - Train POS Tag Model
-  
-    ```py
-    from bnlp import POS
-    bn_pos = POS()
-    model_name = "pos_model.pkl"
-    train_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা', 'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
+text_files = "path/myfiles"
+checkpoint_path = "msc/logs"
 
-    test_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা', 'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
+bn_doc2vec.train_doc2vec(
+  text_files,
+  checkpoint_path=checkpoint_path,
+  vector_size=100,
+  min_count=2,
+  epochs=10
+)
 
-    bn_pos.train(model_name, train_data, test_data)
+# it will train doc2vec with your text files and save the train model in checkpoint_path
+```
 
-    ```
+## Bengali POS Tagging
 
-## Bengali NER
-* **Bengali CRF NER** 
+### Bengali CRF POS Tagging
 
+#### Find Pos Tag Using Pretrained Model
 
-  - Find NER Tag Using Pretrained Model
+```py
+from bnlp import POS
+bn_pos = POS()
+model_path = "model/bn_pos.pkl"
+text = "আমি ভাত খাই।" # or you can pass ['আমি', 'ভাত', 'খাই', '।']
+res = bn_pos.tag(model_path, text)
+print(res)
+# [('আমি', 'PPR'), ('ভাত', 'NC'), ('খাই', 'VM'), ('।', 'PU')]
+```
+
+#### Train POS Tag Model
+
+```py
+from bnlp import POS
+bn_pos = POS()
+model_name = "pos_model.pkl"
+train_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা',  'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
 
-    ```py
-    from bnlp import NER
-    bn_ner = NER()
-    model_path = "model/bn_ner.pkl"
-    text = "সে ঢাকায় থাকে।" # or you can pass ['সে', 'ঢাকায়', 'থাকে', '।']
-    result = bn_ner.tag(model_path, text)
-    print(result)
-    # [('সে', 'O'), ('ঢাকায়', 'S-LOC'), ('থাকে', 'O')]
+test_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা', 'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
 
-    ```
-  - Train NER Tag Model
-  
-    ```py
-    from bnlp import NER
-    bn_ner = NER()
-    model_name = "ner_model.pkl"
-    train_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
+bn_pos.train(model_name, train_data, test_data)
+```
 
-    test_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
+## Bengali NER
 
-    bn_ner.train(model_name, train_data, test_data)
+### Bengali CRF NER
 
-    ```
+#### Find NER Tag Using Pretrained Model
 
+```py
+from bnlp import NER
+bn_ner = NER()
+model_path = "model/bn_ner.pkl"
+text = "সে ঢাকায় থাকে।" # or you can pass ['সে', 'ঢাকায়', 'থাকে', '।']
+result = bn_ner.tag(model_path, text)
+print(result)
+# [('সে', 'O'), ('ঢাকায়', 'S-LOC'), ('থাকে', 'O')]
+```
+
+#### Train NER Tag Model
+
+```py
+from bnlp import NER
+bn_ner = NER()
+model_name = "ner_model.pkl"
+train_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
 
-## Bengali Corpus Class
+test_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
 
-* Stopwords and Punctuations
-  ```py
-  from bnlp.corpus import stopwords, punctuations, letters, digits
+bn_ner.train(model_name, train_data, test_data)
+```
 
-  print(stopwords)
-  print(punctuations)
-  print(letters)
-  print(digits)
 
-  ```
+## Bengali Corpus Class
 
-* Remove stopwords from Text
+### Stopwords and Punctuations
 
-    ```py
-    from bnlp.corpus import stopwords
-    from bnlp.corpus.util import remove_stopwords
-
-    raw_text = 'আমি ভাত খাই।' 
-    result = remove_stopwords(raw_text, stopwords)
-    print(result)
-    # ['ভাত', 'খাই', '।']
-    ```
+```py
+from bnlp.corpus import stopwords, punctuations, letters, digits
 
+print(stopwords)
+print(punctuations)
+print(letters)
+print(digits)
+```
+
+### Remove stopwords from Text
+
+```py
+from bnlp.corpus import stopwords
+from bnlp.corpus.util import remove_stopwords
+
+raw_text = 'আমি ভাত খাই।'
+result = remove_stopwords(raw_text, stopwords)
+print(result)
+# ['ভাত', 'খাই', '।']
+```
+
+## Text Cleaning
+We adopted different text cleaning formula, codes from [clean-text](https://github.com/jfilter/clean-text) and modified for Bangla. Now you can normalize and clean your text using the following methods.
+
+```py
+from bnlp import CleanText
+
+clean_text = CleanText(
+   fix_unicode=True,
+   unicode_norm=True,
+   unicode_norm_form="NFKC",
+   remove_url=False,
+   remove_email=False,
+   remove_emoji=False,
+   remove_number=False,
+   remove_digits=False,
+   remove_punct=False,
+   replace_with_url="<URL>",
+   replace_with_email="<EMAIL>",
+   replace_with_number="<NUMBER>",
+   replace_with_digit="<DIGIT>",
+   replace_with_punct = "<PUNC>"
+)
+
+input_text = "আমার সোনার বাংলা।"
+clean_text = clean_text(input_text)
+print(clean_text)
+```
 
 ## Contributor Guide
 
 Check [CONTRIBUTING.md](https://github.com/sagorbrur/bnlp/blob/master/CONTRIBUTING.md) page for details.
 
 
 ## Thanks To
```

### Comparing `bnlp_toolkit-3.3.0.dev0/README.md` & `bnlp_toolkit-3.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,81 @@
-<img align="left" height="70" src="bnlp.svg" alt="bnlp"/>
-
 # Bengali Natural Language Processing(BNLP)
 
-[![Build Status](https://travis-ci.org/sagorbrur/bnlp.svg?branch=master)](https://travis-ci.org/sagorbrur/bnlp)
 [![PyPI version](https://img.shields.io/pypi/v/bnlp_toolkit)](https://pypi.org/project/bnlp-toolkit/)
 [![Downloads](https://pepy.tech/badge/bnlp-toolkit)](https://pepy.tech/project/bnlp-toolkit)
-[![Documentation Status](https://readthedocs.org/projects/bnlp/badge/?version=latest)](https://bnlp.readthedocs.io/en/latest/?badge=latest)
-[![Gitter](https://badges.gitter.im/bnlp_toolkit/community.svg)](https://gitter.im/bnlp_toolkit/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
-BNLP is a natural language processing toolkit for Bengali Language. This tool will help you to **tokenize Bengali text**, **Embedding Bengali words**, **Embedding Bengali Document**, **Bengali POS Tagging**, **Bengali Name Entity Recognition**, **Construct Neural Model** for Bengali NLP purposes.
+BNLP is a natural language processing toolkit for Bengali Language. This tool will help you to **tokenize Bengali text**, **Embedding Bengali words**, **Embedding Bengali Document**, **Bengali POS Tagging**, **Bengali Name Entity Recognition**, **Bangla Text Cleaning** for Bengali NLP purposes.
 
+Table of contents
+=================
 
+<!--ts-->
+   * [Installation](#installation)
+      * [PIP installer](#pip-installer)
+   * [Pretrained Model](#pretrained-model)
+      * [Download Links](#download-links)
+      * [Training Details](#training-details)
+   * [Tokenization](#tokenization)
+      * [Basic Tokenizer](#basic-tokenizer)
+      * [NLTK Tokenization](#nltk-tokenization)
+      * [Bengali SentencePiece Tokenization](#bengali-sentencepiece-tokenization)
+         * [Tokenization using trained model](#tokenization-using-trained-model)
+         * [Training SentencePiece](#training-sentencepiece)
+   * [Word Embedding](#word-embedding)
+      * [Bengali Word2Vec](#bengali-word2vec)
+         * [Generate Vector using pretrain model](#generate-vector-using-pretrain-model)
+         * [Find Most Similar Word Using Pretrained Model](#find-most-similar-word-using-pretrained-model)
+         * [Train Bengali Word2Vec with your own data](#train-bengali-word2vec-with-your-own-data)
+         * [Pre-train or resume word2vec training with same or new corpus or tokenized sentences](#pre-train-or-resume-word2vec-training-with-same-or-new-corpus-or-tokenized-sentences)
+     * [Bengali FastText](#bengali-fasttext)
+        * [Generate Vector Using Pretrained Model](#generate-vector-using-pretrain-model)
+        * [Train Bengali FastText Model](#train-bengali-fasttext-model)
+        * [Generate Vector File from Fasttext Binary Model](#generate-vector-file-from-fasttext-binary-model)
+     * [Bengali GloVe Word Vectors](#bengali-glove-word-vectors)
+   * [Document Embedding](#document-embedding)
+      * [Bengali Doc2Vec](#bengali-doc2vec)
+         * [Get document vector from input document](#get-document-vector-from-input-document)
+         * [Find document similarity between two document](#find-document-similarity-between-two-document)
+         * [Train doc2vec vector with custom text files](#train-doc2vec-vector-with-custom-text-files)
+   * [Bengali POS Tagging](#bengali-pos-tagging)
+      * [Bengali CRF POS Tagging](#bengali-crf-pos-tagging)
+         * [Find Pos Tag Using Pretrained Model](#find-pos-tag-using-pretrained-model)
+         * [Train POS Tag Model](#train-pos-tag-model)
+   * [Bengali NER](#bengali-ner)
+      * [Bengali CRF NER](#bengali-crf-ner)
+         * [Find NER Tag Using Pretrained Model](#find-ner-tag-using-pretrained-model)
+         * [Train NER Tag Model](#train-ner-tag-model)
+   * [Bengali Corpus Class](#bengali-corpus-class)
+      * [Stopwords and Punctuations](#stopwords-and-punctuations)
+      * [Remove stopwords from Text](#remove-stopwords-from-text)
+   * [Bangla Text Cleaning](#text-cleaning)
+   * [Contributor Guide](#contributor-guide)
+<!--te-->
+---
 
 ## Installation
 
-### PIP installer(Python: 3.6, 3.7, 3.8 tested okay, OS: linux, windows tested okay )
+### PIP installer
 
   ```
   pip install bnlp_toolkit
   ```
   **or Upgrade**
 
   ```
   pip install -U bnlp_toolkit
-
   ```
+  - Python: 3.6, 3.7, 3.8, 3.9
+  - OS: Linux, Windows, Mac
 
 
 
 ## Pretrained Model
 
-### Download Link
+### Download Links
 
 Large model published in [huggingface](https://huggingface.co/) model hub.
 
 * [Bengali SentencePiece](https://github.com/sagorbrur/bnlp/tree/master/model)
 * [Bengali Word2Vec](https://huggingface.co/sagorsarker/bangla_word2vec)
 * [Bengali FastText](https://huggingface.co/sagorsarker/bangla-fasttext)
 * [Bengali GloVe Wordvectors](https://huggingface.co/sagorsarker/bangla-glove-vectors)
@@ -46,360 +87,372 @@
 ### Training Details
 * Sentencepiece, Word2Vec, Fasttext, GloVe model trained with **Bengali Wikipedia Dump Dataset**
   - [Bengali Wiki Dump](https://dumps.wikimedia.org/bnwiki/latest/)
 * SentencePiece Training Vocab Size=50000
 * Fasttext trained with total words = 20M, vocab size = 1171011, epoch=50, embedding dimension = 300 and the training loss = 0.318668,
 * Word2Vec word embedding dimension = 100, min_count=5, window=5, epochs=10
 * To Know Bengali GloVe Wordvector and training process follow [this](https://github.com/sagorbrur/GloVe-Bengali) repository
-* Bengali CRF POS Tagging was training with [nltr](https://github.com/abhishekgupta92/bangla_pos_tagger/tree/master/data) dataset with 80% accuracy. 
+* Bengali CRF POS Tagging was training with [nltr](https://github.com/abhishekgupta92/bangla_pos_tagger/tree/master/data) dataset with 80% accuracy.
 * Bengali CRF NER Tagging was train with [this](https://github.com/MISabic/NER-Bangla-Dataset) data with 90% accuracy.
 * Bengali news article doc2vec model train with 8 jsons of [this](https://www.kaggle.com/datasets/ebiswas/bangla-largest-newspaper-dataset) corpus with epochs 40 vector size 100 min_count=2, total news article 400013
 * Bengali wikipedia doc2vec model trained with wikipedia dump datasets. Total articles 110448, epochs: 40, vector_size: 100, min_count: 2
 
 
 ## Tokenization
 
-* **Basic Tokenizer**
-
- 
+### Basic Tokenizer
 
   ```py
   from bnlp import BasicTokenizer
+  
   basic_tokenizer = BasicTokenizer()
   raw_text = "আমি বাংলায় গান গাই।"
   tokens = basic_tokenizer.tokenize(raw_text)
   print(tokens)
-  
-  # output: ["আমি", "বাংলায়", "গান", "গাই", "।"]
 
+  # output: ["আমি", "বাংলায়", "গান", "গাই", "।"]
   ```
 
-* **NLTK Tokenization**
+### NLTK Tokenization
 
   ```py
   from bnlp import NLTKTokenizer
-  
+
   bnltk = NLTKTokenizer()
   text = "আমি ভাত খাই। সে বাজারে যায়। তিনি কি সত্যিই ভালো মানুষ?"
   word_tokens = bnltk.word_tokenize(text)
   sentence_tokens = bnltk.sentence_tokenize(text)
   print(word_tokens)
   print(sentence_tokens)
-  
+
   # output
   # word_token: ["আমি", "ভাত", "খাই", "।", "সে", "বাজারে", "যায়", "।", "তিনি", "কি", "সত্যিই", "ভালো", "মানুষ", "?"]
   # sentence_token: ["আমি ভাত খাই।", "সে বাজারে যায়।", "তিনি কি সত্যিই ভালো মানুষ?"]
-
   ```
 
 
-* **Bengali SentencePiece Tokenization**
-
-  - tokenization using trained model
-    ```py
-    from bnlp import SentencepieceTokenizer
-
-    bsp = SentencepieceTokenizer()
-    model_path = "./model/bn_spm.model"
-    input_text = "আমি ভাত খাই। সে বাজারে যায়।"
-    tokens = bsp.tokenize(model_path, input_text)
-    print(tokens)
-    text2id = bsp.text2id(model_path, input_text)
-    print(text2id)
-    id2text = bsp.id2text(model_path, text2id)
-    print(id2text)
-
-    ```
-  - Training SentencePiece
-    ```py
-    from bnlp import SentencepieceTokenizer
-    
-    bsp = SentencepieceTokenizer()
-    data = "raw_text.txt"
-    model_prefix = "test"
-    vocab_size = 5
-    bsp.train(data, model_prefix, vocab_size) 
-
-    ```
-
+### Bengali SentencePiece Tokenization
 
+#### Tokenization using trained model
+```py
+from bnlp import SentencepieceTokenizer
+
+bsp = SentencepieceTokenizer()
+model_path = "./model/bn_spm.model"
+input_text = "আমি ভাত খাই। সে বাজারে যায়।"
+tokens = bsp.tokenize(model_path, input_text)
+print(tokens)
+text2id = bsp.text2id(model_path, input_text)
+print(text2id)
+id2text = bsp.id2text(model_path, text2id)
+print(id2text)
+```
+
+#### Training SentencePiece
+```py
+from bnlp import SentencepieceTokenizer
+
+bsp = SentencepieceTokenizer()
+data = "raw_text.txt"
+model_prefix = "test"
+vocab_size = 5
+bsp.train(data, model_prefix, vocab_size)
+```
 
 ## Word Embedding
 
-* **Bengali Word2Vec**
+### Bengali Word2Vec
+
+#### Generate Vector using pretrain model
 
-  - Generate Vector using pretrain model
+```py
+from bnlp import BengaliWord2Vec
 
-    ```py
-    from bnlp import BengaliWord2Vec
+bwv = BengaliWord2Vec()
+model_path = "bengali_word2vec.model"
+word = 'গ্রাম'
+vector = bwv.generate_word_vector(model_path, word)
+print(vector.shape)
+print(vector)
+```
 
-    bwv = BengaliWord2Vec()
-    model_path = "bengali_word2vec.model"
-    word = 'গ্রাম'
-    vector = bwv.generate_word_vector(model_path, word)
-    print(vector.shape)
-    print(vector)
+#### Find Most Similar Word Using Pretrained Model
 
-    ```
+```py
+from bnlp import BengaliWord2Vec
 
-  - Find Most Similar Word Using Pretrained Model
+bwv = BengaliWord2Vec()
+model_path = "bengali_word2vec.model"
+word = 'গ্রাম'
+similar = bwv.most_similar(model_path, word, topn=10)
+print(similar)
+```
+#### Train Bengali Word2Vec with your own data
 
-    ```py
-    from bnlp import BengaliWord2Vec
+Train Bengali word2vec with your custom raw data or tokenized sentences.
 
-    bwv = BengaliWord2Vec()
-    model_path = "bengali_word2vec.model"
-    word = 'গ্রাম'
-    similar = bwv.most_similar(model_path, word, topn=10)
-    print(similar)
+Custom tokenized sentence format example:
+```py
+sentences = [['আমি', 'ভাত', 'খাই', '।'], ['সে', 'বাজারে', 'যায়', '।']]
+```
+Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
 
-    ```
-  - Train Bengali Word2Vec with your own data
+```py
+from bnlp import BengaliWord2Vec
+bwv = BengaliWord2Vec()
+data_file = "raw_text.txt" # or you can pass custom sentence tokens as list of list
+model_name = "test_model.model"
+vector_name = "test_vector.vector"
+bwv.train(data_file, model_name, vector_name, epochs=5)
+```
 
-    Train Bengali word2vec with your custom raw data or tokenized sentences.
+#### Pre-train or resume word2vec training with same or new corpus or tokenized sentences
 
-    custom tokenized sentence format example:
-    ```
-    sentences = [['আমি', 'ভাত', 'খাই', '।'], ['সে', 'বাজারে', 'যায়', '।']]
-    ```
-    Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
+Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
 
-    ```py
-    from bnlp import BengaliWord2Vec
-    bwv = BengaliWord2Vec()
-    data_file = "raw_text.txt" # or you can pass custom sentence tokens as list of list
-    model_name = "test_model.model"
-    vector_name = "test_vector.vector"
-    bwv.train(data_file, model_name, vector_name, epochs=5)
+```py
+from bnlp import BengaliWord2Vec
+bwv = BengaliWord2Vec()
 
+trained_model_path = "mytrained_model.model"
+data_file = "raw_text.txt"
+model_name = "test_model.model"
+vector_name = "test_vector.vector"
+bwv.pretrain(trained_model_path, data_file, model_name, vector_name, epochs=5)
+```
 
-    ```
-  - Pre-train or resume word2vec training with same or new corpus or tokenized sentences
+### Bengali FastText
 
-    Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
+To use `fasttext` you need to install fasttext manually by `pip install fasttext==0.9.2`
 
-    ```py
-    from bnlp import BengaliWord2Vec
-    bwv = BengaliWord2Vec()
+NB: `fasttext` may not be worked in `windows`, it will only work in `linux`
 
-    trained_model_path = "mytrained_model.model"
-    data_file = "raw_text.txt"
-    model_name = "test_model.model"
-    vector_name = "test_vector.vector"
-    bwv.pretrain(trained_model_path, data_file, model_name, vector_name, epochs=5)
+### Generate Vector Using Pretrained Model
 
-    ```
-    
- * **Bengali FastText**
- 
-    To use `fasttext` you need to install fasttext manually by `pip install fasttext==0.9.2`
-    
-    NB: `fasttext` may not be worked in `windows`, it will only work in `linux`
+  ```py
+  from bnlp.embedding.fasttext import BengaliFasttext
 
-    - Generate Vector Using Pretrained Model
-      
+  bft = BengaliFasttext()
+  word = "গ্রাম"
+  model_path = "bengali_fasttext_wiki.bin"
+  word_vector = bft.generate_word_vector(model_path, word)
+  print(word_vector.shape)
+  print(word_vector)
+  ```
 
-      ```py
-      from bnlp.embedding.fasttext import BengaliFasttext
+### Train Bengali FastText Model
 
-      bft = BengaliFasttext()
-      word = "গ্রাম"
-      model_path = "bengali_fasttext_wiki.bin"
-      word_vector = bft.generate_word_vector(model_path, word)
-      print(word_vector.shape)
-      print(word_vector)
+Check [fasttext documentation](https://fasttext.cc/docs/en/options.html) for details of training parameter
 
+  ```py
+  from bnlp.embedding.fasttext import BengaliFasttext
 
-      ```
-    - Train Bengali FastText Model
+  bft = BengaliFasttext()
+  data = "raw_text.txt"
+  model_name = "saved_model.bin"
+  epoch = 50
+  bft.train(data, model_name, epoch)
+  ```
 
-      Check [fasttext documentation](https://fasttext.cc/docs/en/options.html) for details of training parameter
+### Generate Vector File from Fasttext Binary Model
 
-      ```py
-      from bnlp.embedding.fasttext import BengaliFasttext
+```py
+from bnlp.embedding.fasttext import BengaliFasttext
 
-      bft = BengaliFasttext()
-      data = "raw_text.txt"
-      model_name = "saved_model.bin"
-      epoch = 50
-      bft.train(data, model_name, epoch)
-      ```
+bft = BengaliFasttext()
 
-    - Generate Vector File from Fasttext Binary Model
-      ```py
-      from bnlp.embedding.fasttext import BengaliFasttext
+model_path = "mymodel.bin"
+out_vector_name = "myvector.txt"
+bft.bin2vec(model_path, out_vector_name)
+```
+
+## Bengali GloVe Word Vectors
+
+We trained glove model with bengali data(wiki+news articles) and published bengali glove word vectors</br>
+You can download and use it on your different machine learning purposes.
+
+```py
+from bnlp import BengaliGlove
+glove_path = "bn_glove.39M.100d.txt"
+word = "গ্রাম"
+bng = BengaliGlove()
+res = bng.closest_word(glove_path, word)
+print(res)
+vec = bng.word2vec(glove_path, word)
+print(vec)
+```
 
-      bft = BengaliFasttext()
+## Document Embedding
 
-      model_path = "mymodel.bin"
-      out_vector_name = "myvector.txt"
-      bft.bin2vec(model_path, out_vector_name)
-      ```
+### Bengali Doc2Vec
+#### Get document vector from input document
 
-* **Bengali GloVe Word Vectors**
+```py
+from bnlp import BengaliDoc2vec
 
-  We trained glove model with bengali data(wiki+news articles) and published bengali glove word vectors</br>
-  You can download and use it on your different machine learning purposes.
+bn_doc2vec = BengaliDoc2vec()
 
-  ```py
-  from bnlp import BengaliGlove
-  glove_path = "bn_glove.39M.100d.txt"
-  word = "গ্রাম"
-  bng = BengaliGlove()
-  res = bng.closest_word(glove_path, word)
-  print(res)
-  vec = bng.word2vec(glove_path, word)
-  print(vec)
+model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
+document = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
 
-  ```
+vector = bn_doc2vec.get_document_vector(model_path, text)
+print(vector)
+```
 
-## Document Embedding
-* __Bengali Doc2Vec__
-  - Get document vector from input document
+#### Find document similarity between two document
 
-    ```py
-    from bnlp import BengaliDoc2vec
-    
-    bn_doc2vec = BengaliDoc2vec()
-    
-    model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
-    document = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
-
-    vector = bn_doc2vec.get_document_vector(model_path, text)
-    print(vector)
-    ```
-
-  - Find document similarity between two document
-
-    ```py
-    from bnlp import BengaliDoc2vec
-    
-    bn_doc2vec = BengaliDoc2vec()
-    
-    model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
-    article_1 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
-    article_2 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
-
-    similarity = bn_doc2vec.get_document_similarity(
-      model_path,
-      article_1,
-      article_2
-    )
-    print(similarity)
-
-    ```
-
-  - Train doc2vec vector with custom text files
-
-    ```py
-    from bnlp import BengaliDoc2vec
-      
-    bn_doc2vec = BengaliDoc2vec()
-
-    text_files = "path/myfiles"
-    checkpoint_path = "msc/logs"
-
-    bn_doc2vec.train_doc2vec(
-      text_files, 
-      checkpoint_path=checkpoint_path,
-      vector_size=100,
-      min_count=2,
-      epochs=10
-    )
+```py
+from bnlp import BengaliDoc2vec
 
-    # it will train doc2vec with your text files and save the train model in checkpoint_path
+bn_doc2vec = BengaliDoc2vec()
 
-    ```
+model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
+article_1 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
+article_2 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
 
-## Bengali POS Tagging
-* **Bengali CRF POS Tagging** 
+similarity = bn_doc2vec.get_document_similarity(
+  model_path,
+  article_1,
+  article_2
+)
+print(similarity)
+```
 
+#### Train doc2vec vector with custom text files
 
-  - Find Pos Tag Using Pretrained Model
+```py
+from bnlp import BengaliDoc2vec
 
-    ```py
-    from bnlp import POS
-    bn_pos = POS()
-    model_path = "model/bn_pos.pkl"
-    text = "আমি ভাত খাই।" # or you can pass ['আমি', 'ভাত', 'খাই', '।']
-    res = bn_pos.tag(model_path, text)
-    print(res)
-    # [('আমি', 'PPR'), ('ভাত', 'NC'), ('খাই', 'VM'), ('।', 'PU')]
+bn_doc2vec = BengaliDoc2vec()
 
-    ```
-  - Train POS Tag Model
-  
-    ```py
-    from bnlp import POS
-    bn_pos = POS()
-    model_name = "pos_model.pkl"
-    train_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা', 'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
+text_files = "path/myfiles"
+checkpoint_path = "msc/logs"
 
-    test_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা', 'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
+bn_doc2vec.train_doc2vec(
+  text_files,
+  checkpoint_path=checkpoint_path,
+  vector_size=100,
+  min_count=2,
+  epochs=10
+)
 
-    bn_pos.train(model_name, train_data, test_data)
+# it will train doc2vec with your text files and save the train model in checkpoint_path
+```
 
-    ```
+## Bengali POS Tagging
 
-## Bengali NER
-* **Bengali CRF NER** 
+### Bengali CRF POS Tagging
 
+#### Find Pos Tag Using Pretrained Model
 
-  - Find NER Tag Using Pretrained Model
+```py
+from bnlp import POS
+bn_pos = POS()
+model_path = "model/bn_pos.pkl"
+text = "আমি ভাত খাই।" # or you can pass ['আমি', 'ভাত', 'খাই', '।']
+res = bn_pos.tag(model_path, text)
+print(res)
+# [('আমি', 'PPR'), ('ভাত', 'NC'), ('খাই', 'VM'), ('।', 'PU')]
+```
+
+#### Train POS Tag Model
+
+```py
+from bnlp import POS
+bn_pos = POS()
+model_name = "pos_model.pkl"
+train_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা',  'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
 
-    ```py
-    from bnlp import NER
-    bn_ner = NER()
-    model_path = "model/bn_ner.pkl"
-    text = "সে ঢাকায় থাকে।" # or you can pass ['সে', 'ঢাকায়', 'থাকে', '।']
-    result = bn_ner.tag(model_path, text)
-    print(result)
-    # [('সে', 'O'), ('ঢাকায়', 'S-LOC'), ('থাকে', 'O')]
+test_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা', 'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
 
-    ```
-  - Train NER Tag Model
-  
-    ```py
-    from bnlp import NER
-    bn_ner = NER()
-    model_name = "ner_model.pkl"
-    train_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
+bn_pos.train(model_name, train_data, test_data)
+```
 
-    test_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
+## Bengali NER
 
-    bn_ner.train(model_name, train_data, test_data)
+### Bengali CRF NER
 
-    ```
+#### Find NER Tag Using Pretrained Model
 
+```py
+from bnlp import NER
+bn_ner = NER()
+model_path = "model/bn_ner.pkl"
+text = "সে ঢাকায় থাকে।" # or you can pass ['সে', 'ঢাকায়', 'থাকে', '।']
+result = bn_ner.tag(model_path, text)
+print(result)
+# [('সে', 'O'), ('ঢাকায়', 'S-LOC'), ('থাকে', 'O')]
+```
+
+#### Train NER Tag Model
+
+```py
+from bnlp import NER
+bn_ner = NER()
+model_name = "ner_model.pkl"
+train_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
 
-## Bengali Corpus Class
+test_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
 
-* Stopwords and Punctuations
-  ```py
-  from bnlp.corpus import stopwords, punctuations, letters, digits
+bn_ner.train(model_name, train_data, test_data)
+```
 
-  print(stopwords)
-  print(punctuations)
-  print(letters)
-  print(digits)
 
-  ```
+## Bengali Corpus Class
 
-* Remove stopwords from Text
+### Stopwords and Punctuations
 
-    ```py
-    from bnlp.corpus import stopwords
-    from bnlp.corpus.util import remove_stopwords
-
-    raw_text = 'আমি ভাত খাই।' 
-    result = remove_stopwords(raw_text, stopwords)
-    print(result)
-    # ['ভাত', 'খাই', '।']
-    ```
+```py
+from bnlp.corpus import stopwords, punctuations, letters, digits
 
+print(stopwords)
+print(punctuations)
+print(letters)
+print(digits)
+```
+
+### Remove stopwords from Text
+
+```py
+from bnlp.corpus import stopwords
+from bnlp.corpus.util import remove_stopwords
+
+raw_text = 'আমি ভাত খাই।'
+result = remove_stopwords(raw_text, stopwords)
+print(result)
+# ['ভাত', 'খাই', '।']
+```
+
+## Text Cleaning
+We adopted different text cleaning formula, codes from [clean-text](https://github.com/jfilter/clean-text) and modified for Bangla. Now you can normalize and clean your text using the following methods.
+
+```py
+from bnlp import CleanText
+
+clean_text = CleanText(
+   fix_unicode=True,
+   unicode_norm=True,
+   unicode_norm_form="NFKC",
+   remove_url=False,
+   remove_email=False,
+   remove_emoji=False,
+   remove_number=False,
+   remove_digits=False,
+   remove_punct=False,
+   replace_with_url="<URL>",
+   replace_with_email="<EMAIL>",
+   replace_with_number="<NUMBER>",
+   replace_with_digit="<DIGIT>",
+   replace_with_punct = "<PUNC>"
+)
+
+input_text = "আমার সোনার বাংলা।"
+clean_text = clean_text(input_text)
+print(clean_text)
+```
 
 ## Contributor Guide
 
 Check [CONTRIBUTING.md](https://github.com/sagorbrur/bnlp/blob/master/CONTRIBUTING.md) page for details.
 
 
 ## Thanks To
```

### Comparing `bnlp_toolkit-3.3.0.dev0/bnlp/embedding/doc2vec.py` & `bnlp_toolkit-3.3.1/bnlp/embedding/doc2vec.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,38 +4,39 @@
 from tqdm import tqdm
 from scipy import spatial
 from gensim.models.doc2vec import Doc2Vec
 from bnlp.tokenizer.basic import BasicTokenizer
 
 default_tokenizer = BasicTokenizer()
 
+
 def read_corpus(files, tokenizer=None):
     for i, file in tqdm(enumerate(files)):
-      with open(file) as f:
-        text = f.read()
-        if tokenizer:
-            tokens = tokenizer(text)
-        else:
-            tokens = default_tokenizer.tokenize(text)
-        yield gensim.models.doc2vec.TaggedDocument(tokens, [i])
-          
+        with open(file) as f:
+            text = f.read()
+            if tokenizer:
+                tokens = tokenizer(text)
+            else:
+                tokens = default_tokenizer.tokenize(text)
+            yield gensim.models.doc2vec.TaggedDocument(tokens, [i])
+
 
 class BengaliDoc2vec:
     def __init__(self, tokenizer=None):
         self.tokenizer = tokenizer
 
     def get_document_vector(self, model_path, document):
         """Get document vector using trained doc2vec model
 
         Args:
             model_path (bin): trained doc2vec model path
             document (str): input documents
 
         Returns:
-            ndarray: generated vector 
+            ndarray: generated vector
         """
         model = Doc2Vec.load(model_path)
         if self.tokenizer:
             tokens = self.tokenizer(document)
         else:
             tokens = default_tokenizer.tokenize(document)
 
@@ -62,34 +63,45 @@
             document_2_tokens = default_tokenizer.tokenize(document_2)
 
         model = Doc2Vec.load(model_path)
 
         document_1_vector = model.infer_vector(document_1_tokens)
         document_2_vector = model.infer_vector(document_2_tokens)
 
-        similarity = round(1 - spatial.distance.cosine(document_1_vector, document_2_vector), 2)
+        similarity = round(
+            1 - spatial.distance.cosine(document_1_vector, document_2_vector), 2
+        )
 
         return similarity
 
-    def train_doc2vec(self, text_files, checkpoint_path='ckpt', vector_size=100, min_count=2, epochs=10):
+    def train_doc2vec(
+        self,
+        text_files,
+        checkpoint_path="ckpt",
+        vector_size=100,
+        min_count=2,
+        epochs=10,
+    ):
         """Train doc2vec with custom text files
 
         Args:
             text_files (str): path contains the text files with extension .txt
             checkpoint_path (str, optional): checkpoint save path. Defaults to 'ckpt'.
             vector_size (int, optional): size of the vector. Defaults to 100.
             min_count (int, optional): minimum word count. Defaults to 2.
             epochs (int, optional): training iteration number. Defaults to 10.
         """
-        text_files = glob.glob(text_files + '/*.txt')
+        text_files = glob.glob(text_files + "/*.txt")
         if self.tokenizer:
             train_corpus = list(read_corpus(text_files, self.tokenizer))
         else:
             train_corpus = list(read_corpus(text_files))
 
         model = Doc2Vec(vector_size=vector_size, min_count=min_count, epochs=epochs)
         model.build_vocab(train_corpus)
-        model.train(train_corpus, total_examples=model.corpus_count, epochs=model.epochs)
-        
+        model.train(
+            train_corpus, total_examples=model.corpus_count, epochs=model.epochs
+        )
+
         os.makedirs(checkpoint_path, exist_ok=True)
-        output_model_name = os.path.join(checkpoint_path, 'custom_doc2vec_model.model')
+        output_model_name = os.path.join(checkpoint_path, "custom_doc2vec_model.model")
         model.save(output_model_name)
```

### Comparing `bnlp_toolkit-3.3.0.dev0/bnlp/embedding/fasttext.py` & `bnlp_toolkit-3.3.1/bnlp/embedding/fasttext.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 import multiprocessing
-from wasabi import msg
+
 try:
     import fasttext
 except ImportError:
     print("fasttext not installed. Install it by 'pip install fasttext'")
 
+
 class BengaliFasttext:
-    
-    def train(self, data, model_name, epoch, lr=0.05, dim=300, ws=5, minCount=5, 
-        minn=3, maxn=6, neg=5, wordNgrams=1, loss="ns", bucket=2000000,
-        thread=multiprocessing.cpu_count() - 1):
+    def train(
+        self,
+        data,
+        model_name,
+        epoch,
+        lr=0.05,
+        dim=300,
+        ws=5,
+        minCount=5,
+        minn=3,
+        maxn=6,
+        neg=5,
+        wordNgrams=1,
+        loss="ns",
+        bucket=2000000,
+        thread=multiprocessing.cpu_count() - 1,
+    ):
         """train fasttext with raw text data
 
         Args:
             data (str): raw text data path
             model_name (str): name of output trained model with extension
             epoch (int): number of training iteration
             lr (float, optional): learning rate. Defaults to 0.05.
@@ -24,54 +38,54 @@
             maxn (int, optional): [description]. Defaults to 6.
             neg (int, optional): negative sampling. Defaults to 5.
             wordNgrams (int, optional): [description]. Defaults to 1.
             loss (str, optional): loss type . Defaults to "ns".
             bucket (int, optional): [description]. Defaults to 2000000.
             thread ([type], optional): [description]. Defaults to multiprocessing.cpu_count()-1.
         """
-        msg.info('training started.....')
+        print("training started.....")
         model = fasttext.train_unsupervised(
-            data, 
-            model='skipgram',
+            data,
+            model="skipgram",
             epoch=epoch,
             lr=lr,
             dim=dim,
             ws=ws,
             minCount=minCount,
             minn=minn,
             maxn=maxn,
             neg=neg,
             wordNgrams=wordNgrams,
             loss=loss,
             bucket=bucket,
-            thread=thread
+            thread=thread,
         )
-        msg.good(f'training done! saving as {model_name}')
+        print(f"training done! saving as {model_name}")
         model.save_model(model_name)
 
     def bin2vec(self, bin_model, vector_name):
         """Generate vector text file from fasttext binary model
 
         Args:
             bin_model (bin): fasttext trained binary model
             vector_name (str): name of the output vector with extension
         """
-        output_vector = open(vector_name, 'w')
+        output_vector = open(vector_name, "w")
 
         f = fasttext.load_model(bin_model)
         words = f.get_words()
         vocab_len = str(len(words))
         dimension = str(f.get_dimension())
-        output_vector.write(vocab_len+" "+dimension+"\n")
+        output_vector.write(vocab_len + " " + dimension + "\n")
         for w in words:
             v = f.get_word_vector(w)
             vstr = ""
             for vi in v:
                 vstr += " " + str(vi)
-            output_vector.write(w + vstr+ "\n")
+            output_vector.write(w + vstr + "\n")
         output_vector.close()
 
     def generate_word_vector(self, model_path, word):
         """generate word vector from given input word
 
         Args:
             model_path (str): fasttext trained model path
```

### Comparing `bnlp_toolkit-3.3.0.dev0/bnlp/embedding/glove.py` & `bnlp_toolkit-3.3.1/bnlp/embedding/glove.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import numpy as np
 import scipy
 from scipy import spatial
-#print(np.__version__) #1.17.4
-#print(scipy.__version__) #1.3.3
 
+# print(np.__version__) #1.17.4
+# print(scipy.__version__) #1.3.3
 
 
 class BengaliGlove:
-  
-  def word2vec(self, glove_path, test_word):
-      embeddings_dict = {}
-      with open(glove_path, 'r') as f:
-          for line in f:
-              values = line.split()
-              word = values[0]
-              vector = np.asarray(values[1:], "float32")
-              embeddings_dict[word] = vector
-      result_vec = embeddings_dict[test_word]
-      return result_vec
-
-  def closest_word(self,glove_path, test_word):
-
-    def find_closest_embeddings(embedding):
-      return sorted(embeddings_dict.keys(), key=lambda word: spatial.distance.euclidean(embeddings_dict[word], embedding))
-    
-    
-    embeddings_dict = {}
-    with open(glove_path, 'r') as f:
-        for line in f:
-            values = line.split()
-            word = values[0]
-            vector = np.asarray(values[1:], "float32")
-            embeddings_dict[word] = vector
-    result = find_closest_embeddings(embeddings_dict[test_word])[:10]
-    return result
-
-
+    def word2vec(self, glove_path, test_word):
+        embeddings_dict = {}
+        with open(glove_path, "r") as f:
+            for line in f:
+                values = line.split()
+                word = values[0]
+                vector = np.asarray(values[1:], "float32")
+                embeddings_dict[word] = vector
+        result_vec = embeddings_dict[test_word]
+        return result_vec
+
+    def closest_word(self, glove_path, test_word):
+        def find_closest_embeddings(embedding):
+            return sorted(
+                embeddings_dict.keys(),
+                key=lambda word: spatial.distance.euclidean(
+                    embeddings_dict[word], embedding
+                ),
+            )
+
+        embeddings_dict = {}
+        with open(glove_path, "r") as f:
+            for line in f:
+                values = line.split()
+                word = values[0]
+                vector = np.asarray(values[1:], "float32")
+                embeddings_dict[word] = vector
+        result = find_closest_embeddings(embeddings_dict[test_word])[:10]
+        return result
```

### Comparing `bnlp_toolkit-3.3.0.dev0/bnlp/embedding/word2vec.py` & `bnlp_toolkit-3.3.1/bnlp/embedding/word2vec.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,53 +2,73 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import print_function
 
 import os
 import sys
 import multiprocessing
-from wasabi import msg
 from gensim.models import Word2Vec
 from gensim.models.word2vec import LineSentence
 from bnlp.tokenizer.nltk import NLTKTokenizer
 
+
 class MyCorpus:
     """An iterator that yields sentences (lists of str).
-        We used NLTKTokenizer from bnlp to tokenize sentence words
+    We used NLTKTokenizer from bnlp to tokenize sentence words
     """
+
     def __init__(self, data_path):
         self.data_path = data_path
         self.bnltk = NLTKTokenizer()
 
     def __iter__(self):
         for line in open(self.data_path):
             sentences = self.bnltk.sentence_tokenize(line)
             for sentence in sentences:
                 tokens = self.bnltk.word_tokenize(sentence)
                 yield tokens
 
+
 class BengaliWord2Vec:
-    def train(self, data_path, model_name, vector_name, vector_size=100,
-        alpha=0.025, min_alpha=0.0001, sg=0, hs=0, negative=5, ns_exponent=0.75, 
-        window=5, min_count=5, max_vocab_size=None, workers=3, epochs=5, 
-        sample=1e-3, cbow_mean=1, compute_loss=True, callbacks=()):
+    def train(
+        self,
+        data_path,
+        model_name,
+        vector_name,
+        vector_size=100,
+        alpha=0.025,
+        min_alpha=0.0001,
+        sg=0,
+        hs=0,
+        negative=5,
+        ns_exponent=0.75,
+        window=5,
+        min_count=5,
+        max_vocab_size=None,
+        workers=3,
+        epochs=5,
+        sample=1e-3,
+        cbow_mean=1,
+        compute_loss=True,
+        callbacks=(),
+    ):
         """train bengali word2vec
 
         Args:
             data_path (str/list): raw text data path as string with extension or
                                   sentence token list. example: [[], []]
             model_name (str): output model name ex: mymodel.model
             vector_name (str): output vector name ex: myvector.txt
             vector_size (int, optional): vector dimension. Defaults to 100.
             alpha (float, optional): initial learning rate. Defaults to 0.025.
             min_alpha (float, optional): minimum learning rate. Defaults to 0.0001.
             sg (int, optional): skip-gram model or cbow model. if 1 then skip-gram. Defaults to 0.
             hs (int, optional): hierarchical softmax. Defaults to 0.
             negative (int, optional): negative sampling. Defaults to 5.
-            ns_exponent (float, optional): The exponent used to shape the 
+            ns_exponent (float, optional): The exponent used to shape the
                         negative sampling distribution. Defaults to 0.75.
             window (int, optional): window size. Defaults to 5.
             min_count (int, optional): minimum word count to ignore. Defaults to 5.
             max_vocab_size ([type], optional): maximum vocab size. Defaults to None.
             workers (int, optional): worker number. Defaults to 3.
             epochs (int, optional): number of training iteration. Defaults to 5.
             sample ([type], optional): sampling rate. Defaults to 1e-3.
@@ -57,78 +77,81 @@
             callbacks (tuple, optional): callback sequence. Defaults to ().
         """
         if isinstance(data_path, list):
             sentences = data_path
         else:
             sentences = MyCorpus(data_path)
 
-        msg.info("training started.......")
-        msg.info("please wait.....it will take time according to your data size and computation capability")
+        print("training started.......")
+        print(
+            "please wait.....it will take time according to your data size and computation capability"
+        )
         model = Word2Vec(
-            sentences=sentences, 
+            sentences=sentences,
             vector_size=vector_size,
             alpha=alpha,
             min_alpha=min_alpha,
             sg=sg,
             hs=hs,
             negative=negative,
             ns_exponent=ns_exponent,
             sample=sample,
             cbow_mean=cbow_mean,
-            window=window, 
-            min_count=min_count, 
-            max_vocab_size=max_vocab_size, 
+            window=window,
+            min_count=min_count,
+            max_vocab_size=max_vocab_size,
             workers=workers,
-            epochs=epochs, 
+            epochs=epochs,
             compute_loss=compute_loss,
-            callbacks=callbacks
+            callbacks=callbacks,
         )
         # getting the training loss value
         training_loss = model.get_latest_training_loss()
 
-        msg.good('train completed successfully')
-        msg.good(f"trianing loss: {training_loss}")
-        msg.info(f"model and vector saving...")
+        print("train completed successfully")
+        print(f"trianing loss: {training_loss}")
+        print(f"model and vector saving...")
         model.save(model_name)
         model.wv.save_word2vec_format(vector_name, binary=False)
-        msg.good(f"model and vector saved as {model_name} and {vector_name}")
+        print(f"model and vector saved as {model_name} and {vector_name}")
 
-    def pretrain(self, model_path, new_sentences, output_model_name, 
-        output_vector_name, epochs=5):
+    def pretrain(
+        self, model_path, new_sentences, output_model_name, output_vector_name, epochs=5
+    ):
         """resume training from saved word2vec model
 
         Args:
             model_path (bin): path of trained word2vec model
             new_sentences (list): list of new sentences
             output_model_name (str): output model name
             output_vector_name (str): output vector name
             epoch(int): number of training iteration
         """
         if isinstance(new_sentences, str):
             new_sentences = MyCorpus(new_sentences)
-        msg.info(f"model loading ....")
+        print(f"model loading ....")
         model = Word2Vec.load(model_path)
-        msg.info(f"vocab building with new sentences")
+        print(f"vocab building with new sentences")
         model.build_vocab(new_sentences, update=True)
-        msg.info("pre-training started.......")
-        msg.info("please wait.....it will take time according to your data size and computation capability")
-        model.train(
-            new_sentences, 
-            total_examples=model.corpus_count,
-            epochs=epochs
+        print("pre-training started.......")
+        print(
+            "please wait.....it will take time according to your data size and computation capability"
         )
+        model.train(new_sentences, total_examples=model.corpus_count, epochs=epochs)
         # getting the training loss value
         training_loss = model.get_latest_training_loss()
 
-        msg.good('pre-train completed successfully')
-        msg.good(f"pre-trianing loss: {training_loss}")
-        msg.info(f"model and vector saving...")
+        print("pre-train completed successfully")
+        print(f"pre-trianing loss: {training_loss}")
+        print(f"model and vector saving...")
         model.save(output_model_name)
         model.wv.save_word2vec_format(output_vector_name, binary=False)
-        msg.good(f"model and vector saved as {output_model_name} and {output_vector_name}")
+        print(
+            f"model and vector saved as {output_model_name} and {output_vector_name}"
+        )
 
     def generate_word_vector(self, model_path, input_word):
         """
         :model_name: (str) model path with file name and extension
         :input_word: (str) word to generate vector
 
         """
```

### Comparing `bnlp_toolkit-3.3.0.dev0/bnlp/pos.py` & `bnlp_toolkit-3.3.1/bnlp/ner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,83 +1,90 @@
 """
-tool: We used sklearn crf_suite for bengali pos tagging
+tool: We used sklearn crf_suite for bengali name entity recognition
 https://sklearn-crfsuite.readthedocs.io/en/latest/
+
 """
 
 import pickle
+import string
 from sklearn_crfsuite import CRF
 from sklearn_crfsuite import metrics
 from nltk.tag.util import untag
 from bnlp.tokenizer.basic import BasicTokenizer
 
+
 def features(sentence, index):
-        """ sentence: [w1, w2, ...], index: the index of the word """
-        return {
-            'word': sentence[index],
-            'is_first': index == 0,
-            'is_last': index == len(sentence) - 1,
-            'is_capitalized': sentence[index][0].upper() == sentence[index][0],
-            'is_all_caps': sentence[index].upper() == sentence[index],
-            'is_all_lower': sentence[index].lower() == sentence[index],
-            'prefix-1': sentence[index][0],
-            'prefix-2': sentence[index][:2],
-            'prefix-3': sentence[index][:3],
-            'suffix-1': sentence[index][-1],
-            'suffix-2': sentence[index][-2:],
-            'suffix-3': sentence[index][-3:],
-            'prev_word': '' if index == 0 else sentence[index - 1],
-            'next_word': '' if index == len(sentence) - 1 else sentence[index + 1],
-            'has_hyphen': '-' in sentence[index],
-            'is_numeric': sentence[index].isdigit(),
-            'capitals_inside': sentence[index][1:].lower() != sentence[index][1:]
-        }
+    """sentence: [w1, w2, ...], index: the index of the word"""
+    return {
+        "word": sentence[index],
+        "is_first": index == 0,
+        "is_last": index == len(sentence) - 1,
+        "is_capitalized": sentence[index][0].upper() == sentence[index][0],
+        "is_all_caps": sentence[index].upper() == sentence[index],
+        "is_all_lower": sentence[index].lower() == sentence[index],
+        "prefix-1": sentence[index][0],
+        "prefix-2": sentence[index][:2],
+        "prefix-3": sentence[index][:3],
+        "suffix-1": sentence[index][-1],
+        "suffix-2": sentence[index][-2:],
+        "suffix-3": sentence[index][-3:],
+        "prev_word": "" if index == 0 else sentence[index - 1],
+        "next_word": "" if index == len(sentence) - 1 else sentence[index + 1],
+        "has_hyphen": "-" in sentence[index],
+        "is_numeric": sentence[index].isdigit(),
+        "capitals_inside": sentence[index][1:].lower() != sentence[index][1:],
+    }
+
 
 def transform_to_dataset(tagged_sentences):
     X, y = [], []
-     
+
     for tagged in tagged_sentences:
         try:
             X.append([features(untag(tagged), index) for index in range(len(tagged))])
             y.append([tag for _, tag in tagged])
         except Exception as e:
             print(e)
- 
+
     return X, y
 
-class POS:
+
+class NER:
     def tag(self, model_path, text):
-        with open(model_path, 'rb') as pkl_model:
+        punctuations = string.punctuation + "।"
+        with open(model_path, "rb") as pkl_model:
             model = pickle.load(pkl_model)
             if not isinstance(text, list):
                 basic_t = BasicTokenizer()
                 tokens = basic_t.tokenize(text)
+                tokens = [x for x in tokens if x not in punctuations]
             else:
                 tokens = text
-            sentence_features = [features(tokens, index) for index in range(len(tokens))]
+            sentence_features = [
+                features(tokens, index) for index in range(len(tokens))
+            ]
             result = list(zip(tokens, model.predict([sentence_features])[0]))
             pkl_model.close()
             return result
 
     def train(self, model_name, train_data, test_data, average="micro"):
-       
+
         X_train, y_train = transform_to_dataset(train_data)
         X_test, y_test = transform_to_dataset(test_data)
         print(len(X_train))
         print(len(X_test))
 
-
         print("Training Started........")
-        print("it will take time according to your dataset size..")
+        print("It will take time according to your dataset size...")
         model = CRF()
         model.fit(X_train, y_train)
         print("Training Finished!")
-        
+
         print("Evaluating with Test Data...")
         y_pred = model.predict(X_test)
         print("Accuracy is: ")
         print(metrics.flat_accuracy_score(y_test, y_pred))
-
         print(f"F1 Score({average}) is: ")
         print(metrics.flat_f1_score(y_test, y_pred, average=average))
-        
-        pickle.dump(model, open(model_name, 'wb'))
+
+        pickle.dump(model, open(model_name, "wb"))
         print("Model Saved!")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bnlp_toolkit-3.3.0.dev0/bnlp/tokenizer/basic.py` & `bnlp_toolkit-3.3.1/bnlp/tokenizer/basic.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,110 +1,111 @@
 """
 Basic Tokenization
 Basic tokenization tokenize sentence using white spaces, punctuation mark
-Code shamelessly copied from BERT tokenization 
+Code shamelessly copied from BERT tokenization
 To check Original Code: https://github.com/google-research/bert/blob/master/tokenization.py
 """
 import six
 import unicodedata
 
+
 def convert_to_unicode(text):
-  """Converts `text` to Unicode (if it's not already), assuming utf-8 input."""
-  if six.PY3:
-    if isinstance(text, str):
-      return text
-    elif isinstance(text, bytes):
-      return text.decode("utf-8", "ignore")
-    else:
-      raise ValueError("Unsupported string type: %s" % (type(text)))
-  elif six.PY2:
-    if isinstance(text, str):
-      return text.decode("utf-8", "ignore")
-    elif isinstance(text, unicode):
-      return text
+    """Converts `text` to Unicode (if it's not already), assuming utf-8 input."""
+    if six.PY3:
+        if isinstance(text, str):
+            return text
+        elif isinstance(text, bytes):
+            return text.decode("utf-8", "ignore")
+        else:
+            raise ValueError("Unsupported string type: %s" % (type(text)))
+    elif six.PY2:
+        if isinstance(text, str):
+            return text.decode("utf-8", "ignore")
+        elif isinstance(text, unicode):
+            return text
+        else:
+            raise ValueError("Unsupported string type: %s" % (type(text)))
     else:
-      raise ValueError("Unsupported string type: %s" % (type(text)))
-  else:
-    raise ValueError("Not running on Python2 or Python 3?")
+        raise ValueError("Not running on Python2 or Python 3?")
+
 
 def whitespace_tokenize(text):
-  """Runs basic whitespace cleaning and splitting on a piece of text."""
-  text = text.strip()
-  # print("Text: ", text)
-  if not text:
-    return []
-  tokens = text.split()
-  # print("tokens : ", tokens)
-  return tokens
+    """Runs basic whitespace cleaning and splitting on a piece of text."""
+    text = text.strip()
+    # print("Text: ", text)
+    if not text:
+        return []
+    tokens = text.split()
+    # print("tokens : ", tokens)
+    return tokens
 
 
 def _is_punctuation(char):
-  """Checks whether `chars` is a punctuation character."""
-  cp = ord(char)
-  # We treat all non-letter/number ASCII as punctuation.
-  # Characters such as "^", "$", and "`" are not in the Unicode
-  # Punctuation class but we treat them as punctuation anyways, for
-  # consistency.
-  if ((cp >= 33 and cp <= 47) or (cp >= 58 and cp <= 64) or
-      (cp >= 91 and cp <= 96) or (cp >= 123 and cp <= 126)):
-    return True
-  cat = unicodedata.category(char)
-  if cat.startswith("P"):
-    return True
-  return False
+    """Checks whether `chars` is a punctuation character."""
+    cp = ord(char)
+    # We treat all non-letter/number ASCII as punctuation.
+    # Characters such as "^", "$", and "`" are not in the Unicode
+    # Punctuation class but we treat them as punctuation anyways, for
+    # consistency.
+    if (
+        (cp >= 33 and cp <= 47)
+        or (cp >= 58 and cp <= 64)
+        or (cp >= 91 and cp <= 96)
+        or (cp >= 123 and cp <= 126)
+    ):
+        return True
+    cat = unicodedata.category(char)
+    if cat.startswith("P"):
+        return True
+    return False
+
 
 class BasicTokenizer:
-  """Runs basic tokenization (punctuation splitting, lower casing, etc.)."""
+    """Runs basic tokenization (punctuation splitting, lower casing, etc.)."""
 
-  def tokenize(self, text):
-    """Tokenizes a piece of text."""
-    text = convert_to_unicode(text)
-
-
-    orig_tokens = whitespace_tokenize(text)
-    # print("original tokens: ", orig_tokens)
-    split_tokens = []
-    for token in orig_tokens:
-      # if self.do_lower_case:
-      #   token = token.lower()
-      #   token = self._run_strip_accents(token)
-      split_tokens.extend(self._run_split_on_punc(token))
-
-    # print("split tokens: ", split_tokens)
-    output_tokens = whitespace_tokenize(" ".join(split_tokens))
-    return output_tokens
-
-  def _run_strip_accents(self, text):
-    """Strips accents from a piece of text."""
-    text = unicodedata.normalize("NFD", text)
-    output = []
-    for char in text:
-      cat = unicodedata.category(char)
-      if cat == "Mn":
-        continue
-      output.append(char)
-    return "".join(output)
-
-  def _run_split_on_punc(self, text):
-    """Splits punctuation on a piece of text."""
-    chars = list(text)
-    i = 0
-    start_new_word = True
-    output = []
-    while i < len(chars):
-      char = chars[i]
-      if _is_punctuation(char):
-        output.append([char])
+    def tokenize(self, text):
+        """Tokenizes a piece of text."""
+        text = convert_to_unicode(text)
+
+        orig_tokens = whitespace_tokenize(text)
+        # print("original tokens: ", orig_tokens)
+        split_tokens = []
+        for token in orig_tokens:
+            # if self.do_lower_case:
+            #   token = token.lower()
+            #   token = self._run_strip_accents(token)
+            split_tokens.extend(self._run_split_on_punc(token))
+
+        # print("split tokens: ", split_tokens)
+        output_tokens = whitespace_tokenize(" ".join(split_tokens))
+        return output_tokens
+
+    def _run_strip_accents(self, text):
+        """Strips accents from a piece of text."""
+        text = unicodedata.normalize("NFD", text)
+        output = []
+        for char in text:
+            cat = unicodedata.category(char)
+            if cat == "Mn":
+                continue
+            output.append(char)
+        return "".join(output)
+
+    def _run_split_on_punc(self, text):
+        """Splits punctuation on a piece of text."""
+        chars = list(text)
+        i = 0
         start_new_word = True
-      else:
-        if start_new_word:
-          output.append([])
-        start_new_word = False
-        output[-1].append(char)
-      i += 1
-
-    return ["".join(x) for x in output]
-
-
-
+        output = []
+        while i < len(chars):
+            char = chars[i]
+            if _is_punctuation(char):
+                output.append([char])
+                start_new_word = True
+            else:
+                if start_new_word:
+                    output.append([])
+                start_new_word = False
+                output[-1].append(char)
+            i += 1
 
- 
+        return ["".join(x) for x in output]
```

### Comparing `bnlp_toolkit-3.3.0.dev0/bnlp/tokenizer/nltk.py` & `bnlp_toolkit-3.3.1/bnlp/tokenizer/nltk.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 import nltk
 
 try:
-    nltk.data.find('tokenizers/punkt')
+    nltk.data.find("tokenizers/punkt")
 except LookupError:
     print("punkt not found. downloading...")
-    nltk.download('punkt')
+    nltk.download("punkt")
 
 
 class NLTKTokenizer:
     def word_tokenize(self, text):
         tokens = nltk.word_tokenize(text)
         new_tokens = []
         for token in tokens:
-            if token[-1] == "।" and len(token)>1:
+            if token[-1] == "।" and len(token) > 1:
                 token_1 = token[:-1]
                 token_2 = token[-1]
                 new_tokens.append(token_1)
                 new_tokens.append(token_2)
             else:
-              new_tokens.append(token)
+                new_tokens.append(token)
         return new_tokens
-    
+
     def sentence_tokenize(self, text):
-        text = text.replace(".", "<dummy_bangla_token>") # to deal with abbreviations
+        text = text.replace(".", "<dummy_bangla_token>")  # to deal with abbreviations
         text = text.replace("।", ".")
         tokens = nltk.tokenize.sent_tokenize(text)
         new_tokens = []
         for token in tokens:
-            token = token.replace(".","।") # do operation in reverse order
-            token = token.replace("<dummy_bangla_token>",".")
+            token = token.replace(".", "।")  # do operation in reverse order
+            token = token.replace("<dummy_bangla_token>", ".")
             new_tokens.append(token)
         return new_tokens
-
-
-
-
```

### Comparing `bnlp_toolkit-3.3.0.dev0/bnlp/tokenizer/sentencepiece.py` & `bnlp_toolkit-3.3.1/bnlp/tokenizer/sentencepiece.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 import os
 import sentencepiece as bsp
 
 
 class SentencepieceTokenizer:
-    
     def train(self, data, model_prefix, vocab_size):
         """
         :data: (str) data path with extension
         :model_prefix: (str) model name prefix
         :vocab_size: (int) size of train vocabulary
 
         """
-        train_args = "--model_prefix="+model_prefix+" --input="+data+" --vocab_size="+str(vocab_size)
+        train_args = (
+            "--model_prefix="
+            + model_prefix
+            + " --input="
+            + data
+            + " --vocab_size="
+            + str(vocab_size)
+        )
         bsp.SentencePieceTrainer.train(train_args)
-        print("%s.model and %s.vocab is saved on your current directory"%(model_prefix, model_prefix))
+        print(
+            "%s.model and %s.vocab is saved on your current directory"
+            % (model_prefix, model_prefix)
+        )
 
     def tokenize(self, model_path, text):
         """
         :model_path: (str) path of the model with extension
         :text: (str) input text for tokenization
 
         """
         model = bsp.SentencePieceProcessor()
         model.Load(model_path)
         tokens = model.EncodeAsPieces(text)
 
         return tokens
-    
+
     def text2id(self, model_path, text):
         model = bsp.SentencePieceProcessor()
         model.Load(model_path)
         ids = model.EncodeAsIds(text)
         return ids
+
     def id2text(self, model_path, ids):
         model = bsp.SentencePieceProcessor()
         model.Load(model_path)
         text = model.DecodeIds(ids)
         return text
-
-
-
-
```

### Comparing `bnlp_toolkit-3.3.0.dev0/bnlp_toolkit.egg-info/PKG-INFO` & `bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,96 @@
 Metadata-Version: 2.1
 Name: bnlp-toolkit
-Version: 3.3.0.dev0
+Version: 3.3.1
 Summary: BNLP is a natural language processing toolkit for Bengali Language
 Home-page: https://github.com/sagorbrur/bnlp
 Author: Sagor Sarker
 Author-email: sagorhem3532@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: spacy
-Provides-Extra: fasttext
 License-File: LICENSE
 
-<img align="left" height="70" src="bnlp.svg" alt="bnlp"/>
-
 # Bengali Natural Language Processing(BNLP)
 
-[![Build Status](https://travis-ci.org/sagorbrur/bnlp.svg?branch=master)](https://travis-ci.org/sagorbrur/bnlp)
 [![PyPI version](https://img.shields.io/pypi/v/bnlp_toolkit)](https://pypi.org/project/bnlp-toolkit/)
 [![Downloads](https://pepy.tech/badge/bnlp-toolkit)](https://pepy.tech/project/bnlp-toolkit)
-[![Documentation Status](https://readthedocs.org/projects/bnlp/badge/?version=latest)](https://bnlp.readthedocs.io/en/latest/?badge=latest)
-[![Gitter](https://badges.gitter.im/bnlp_toolkit/community.svg)](https://gitter.im/bnlp_toolkit/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
-BNLP is a natural language processing toolkit for Bengali Language. This tool will help you to **tokenize Bengali text**, **Embedding Bengali words**, **Embedding Bengali Document**, **Bengali POS Tagging**, **Bengali Name Entity Recognition**, **Construct Neural Model** for Bengali NLP purposes.
+BNLP is a natural language processing toolkit for Bengali Language. This tool will help you to **tokenize Bengali text**, **Embedding Bengali words**, **Embedding Bengali Document**, **Bengali POS Tagging**, **Bengali Name Entity Recognition**, **Bangla Text Cleaning** for Bengali NLP purposes.
 
+Table of contents
+=================
 
+<!--ts-->
+   * [Installation](#installation)
+      * [PIP installer](#pip-installer)
+   * [Pretrained Model](#pretrained-model)
+      * [Download Links](#download-links)
+      * [Training Details](#training-details)
+   * [Tokenization](#tokenization)
+      * [Basic Tokenizer](#basic-tokenizer)
+      * [NLTK Tokenization](#nltk-tokenization)
+      * [Bengali SentencePiece Tokenization](#bengali-sentencepiece-tokenization)
+         * [Tokenization using trained model](#tokenization-using-trained-model)
+         * [Training SentencePiece](#training-sentencepiece)
+   * [Word Embedding](#word-embedding)
+      * [Bengali Word2Vec](#bengali-word2vec)
+         * [Generate Vector using pretrain model](#generate-vector-using-pretrain-model)
+         * [Find Most Similar Word Using Pretrained Model](#find-most-similar-word-using-pretrained-model)
+         * [Train Bengali Word2Vec with your own data](#train-bengali-word2vec-with-your-own-data)
+         * [Pre-train or resume word2vec training with same or new corpus or tokenized sentences](#pre-train-or-resume-word2vec-training-with-same-or-new-corpus-or-tokenized-sentences)
+     * [Bengali FastText](#bengali-fasttext)
+        * [Generate Vector Using Pretrained Model](#generate-vector-using-pretrain-model)
+        * [Train Bengali FastText Model](#train-bengali-fasttext-model)
+        * [Generate Vector File from Fasttext Binary Model](#generate-vector-file-from-fasttext-binary-model)
+     * [Bengali GloVe Word Vectors](#bengali-glove-word-vectors)
+   * [Document Embedding](#document-embedding)
+      * [Bengali Doc2Vec](#bengali-doc2vec)
+         * [Get document vector from input document](#get-document-vector-from-input-document)
+         * [Find document similarity between two document](#find-document-similarity-between-two-document)
+         * [Train doc2vec vector with custom text files](#train-doc2vec-vector-with-custom-text-files)
+   * [Bengali POS Tagging](#bengali-pos-tagging)
+      * [Bengali CRF POS Tagging](#bengali-crf-pos-tagging)
+         * [Find Pos Tag Using Pretrained Model](#find-pos-tag-using-pretrained-model)
+         * [Train POS Tag Model](#train-pos-tag-model)
+   * [Bengali NER](#bengali-ner)
+      * [Bengali CRF NER](#bengali-crf-ner)
+         * [Find NER Tag Using Pretrained Model](#find-ner-tag-using-pretrained-model)
+         * [Train NER Tag Model](#train-ner-tag-model)
+   * [Bengali Corpus Class](#bengali-corpus-class)
+      * [Stopwords and Punctuations](#stopwords-and-punctuations)
+      * [Remove stopwords from Text](#remove-stopwords-from-text)
+   * [Bangla Text Cleaning](#text-cleaning)
+   * [Contributor Guide](#contributor-guide)
+<!--te-->
+---
 
 ## Installation
 
-### PIP installer(Python: 3.6, 3.7, 3.8 tested okay, OS: linux, windows tested okay )
+### PIP installer
 
   ```
   pip install bnlp_toolkit
   ```
   **or Upgrade**
 
   ```
   pip install -U bnlp_toolkit
-
   ```
+  - Python: 3.6, 3.7, 3.8, 3.9
+  - OS: Linux, Windows, Mac
 
 
 
 ## Pretrained Model
 
-### Download Link
+### Download Links
 
 Large model published in [huggingface](https://huggingface.co/) model hub.
 
 * [Bengali SentencePiece](https://github.com/sagorbrur/bnlp/tree/master/model)
 * [Bengali Word2Vec](https://huggingface.co/sagorsarker/bangla_word2vec)
 * [Bengali FastText](https://huggingface.co/sagorsarker/bangla-fasttext)
 * [Bengali GloVe Wordvectors](https://huggingface.co/sagorsarker/bangla-glove-vectors)
@@ -63,360 +102,372 @@
 ### Training Details
 * Sentencepiece, Word2Vec, Fasttext, GloVe model trained with **Bengali Wikipedia Dump Dataset**
   - [Bengali Wiki Dump](https://dumps.wikimedia.org/bnwiki/latest/)
 * SentencePiece Training Vocab Size=50000
 * Fasttext trained with total words = 20M, vocab size = 1171011, epoch=50, embedding dimension = 300 and the training loss = 0.318668,
 * Word2Vec word embedding dimension = 100, min_count=5, window=5, epochs=10
 * To Know Bengali GloVe Wordvector and training process follow [this](https://github.com/sagorbrur/GloVe-Bengali) repository
-* Bengali CRF POS Tagging was training with [nltr](https://github.com/abhishekgupta92/bangla_pos_tagger/tree/master/data) dataset with 80% accuracy. 
+* Bengali CRF POS Tagging was training with [nltr](https://github.com/abhishekgupta92/bangla_pos_tagger/tree/master/data) dataset with 80% accuracy.
 * Bengali CRF NER Tagging was train with [this](https://github.com/MISabic/NER-Bangla-Dataset) data with 90% accuracy.
 * Bengali news article doc2vec model train with 8 jsons of [this](https://www.kaggle.com/datasets/ebiswas/bangla-largest-newspaper-dataset) corpus with epochs 40 vector size 100 min_count=2, total news article 400013
 * Bengali wikipedia doc2vec model trained with wikipedia dump datasets. Total articles 110448, epochs: 40, vector_size: 100, min_count: 2
 
 
 ## Tokenization
 
-* **Basic Tokenizer**
-
- 
+### Basic Tokenizer
 
   ```py
   from bnlp import BasicTokenizer
+  
   basic_tokenizer = BasicTokenizer()
   raw_text = "আমি বাংলায় গান গাই।"
   tokens = basic_tokenizer.tokenize(raw_text)
   print(tokens)
-  
-  # output: ["আমি", "বাংলায়", "গান", "গাই", "।"]
 
+  # output: ["আমি", "বাংলায়", "গান", "গাই", "।"]
   ```
 
-* **NLTK Tokenization**
+### NLTK Tokenization
 
   ```py
   from bnlp import NLTKTokenizer
-  
+
   bnltk = NLTKTokenizer()
   text = "আমি ভাত খাই। সে বাজারে যায়। তিনি কি সত্যিই ভালো মানুষ?"
   word_tokens = bnltk.word_tokenize(text)
   sentence_tokens = bnltk.sentence_tokenize(text)
   print(word_tokens)
   print(sentence_tokens)
-  
+
   # output
   # word_token: ["আমি", "ভাত", "খাই", "।", "সে", "বাজারে", "যায়", "।", "তিনি", "কি", "সত্যিই", "ভালো", "মানুষ", "?"]
   # sentence_token: ["আমি ভাত খাই।", "সে বাজারে যায়।", "তিনি কি সত্যিই ভালো মানুষ?"]
-
   ```
 
 
-* **Bengali SentencePiece Tokenization**
-
-  - tokenization using trained model
-    ```py
-    from bnlp import SentencepieceTokenizer
-
-    bsp = SentencepieceTokenizer()
-    model_path = "./model/bn_spm.model"
-    input_text = "আমি ভাত খাই। সে বাজারে যায়।"
-    tokens = bsp.tokenize(model_path, input_text)
-    print(tokens)
-    text2id = bsp.text2id(model_path, input_text)
-    print(text2id)
-    id2text = bsp.id2text(model_path, text2id)
-    print(id2text)
-
-    ```
-  - Training SentencePiece
-    ```py
-    from bnlp import SentencepieceTokenizer
-    
-    bsp = SentencepieceTokenizer()
-    data = "raw_text.txt"
-    model_prefix = "test"
-    vocab_size = 5
-    bsp.train(data, model_prefix, vocab_size) 
-
-    ```
-
+### Bengali SentencePiece Tokenization
 
+#### Tokenization using trained model
+```py
+from bnlp import SentencepieceTokenizer
+
+bsp = SentencepieceTokenizer()
+model_path = "./model/bn_spm.model"
+input_text = "আমি ভাত খাই। সে বাজারে যায়।"
+tokens = bsp.tokenize(model_path, input_text)
+print(tokens)
+text2id = bsp.text2id(model_path, input_text)
+print(text2id)
+id2text = bsp.id2text(model_path, text2id)
+print(id2text)
+```
+
+#### Training SentencePiece
+```py
+from bnlp import SentencepieceTokenizer
+
+bsp = SentencepieceTokenizer()
+data = "raw_text.txt"
+model_prefix = "test"
+vocab_size = 5
+bsp.train(data, model_prefix, vocab_size)
+```
 
 ## Word Embedding
 
-* **Bengali Word2Vec**
+### Bengali Word2Vec
+
+#### Generate Vector using pretrain model
 
-  - Generate Vector using pretrain model
+```py
+from bnlp import BengaliWord2Vec
 
-    ```py
-    from bnlp import BengaliWord2Vec
+bwv = BengaliWord2Vec()
+model_path = "bengali_word2vec.model"
+word = 'গ্রাম'
+vector = bwv.generate_word_vector(model_path, word)
+print(vector.shape)
+print(vector)
+```
 
-    bwv = BengaliWord2Vec()
-    model_path = "bengali_word2vec.model"
-    word = 'গ্রাম'
-    vector = bwv.generate_word_vector(model_path, word)
-    print(vector.shape)
-    print(vector)
+#### Find Most Similar Word Using Pretrained Model
 
-    ```
+```py
+from bnlp import BengaliWord2Vec
 
-  - Find Most Similar Word Using Pretrained Model
+bwv = BengaliWord2Vec()
+model_path = "bengali_word2vec.model"
+word = 'গ্রাম'
+similar = bwv.most_similar(model_path, word, topn=10)
+print(similar)
+```
+#### Train Bengali Word2Vec with your own data
 
-    ```py
-    from bnlp import BengaliWord2Vec
+Train Bengali word2vec with your custom raw data or tokenized sentences.
 
-    bwv = BengaliWord2Vec()
-    model_path = "bengali_word2vec.model"
-    word = 'গ্রাম'
-    similar = bwv.most_similar(model_path, word, topn=10)
-    print(similar)
+Custom tokenized sentence format example:
+```py
+sentences = [['আমি', 'ভাত', 'খাই', '।'], ['সে', 'বাজারে', 'যায়', '।']]
+```
+Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
 
-    ```
-  - Train Bengali Word2Vec with your own data
+```py
+from bnlp import BengaliWord2Vec
+bwv = BengaliWord2Vec()
+data_file = "raw_text.txt" # or you can pass custom sentence tokens as list of list
+model_name = "test_model.model"
+vector_name = "test_vector.vector"
+bwv.train(data_file, model_name, vector_name, epochs=5)
+```
 
-    Train Bengali word2vec with your custom raw data or tokenized sentences.
+#### Pre-train or resume word2vec training with same or new corpus or tokenized sentences
 
-    custom tokenized sentence format example:
-    ```
-    sentences = [['আমি', 'ভাত', 'খাই', '।'], ['সে', 'বাজারে', 'যায়', '।']]
-    ```
-    Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
+Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
 
-    ```py
-    from bnlp import BengaliWord2Vec
-    bwv = BengaliWord2Vec()
-    data_file = "raw_text.txt" # or you can pass custom sentence tokens as list of list
-    model_name = "test_model.model"
-    vector_name = "test_vector.vector"
-    bwv.train(data_file, model_name, vector_name, epochs=5)
+```py
+from bnlp import BengaliWord2Vec
+bwv = BengaliWord2Vec()
 
+trained_model_path = "mytrained_model.model"
+data_file = "raw_text.txt"
+model_name = "test_model.model"
+vector_name = "test_vector.vector"
+bwv.pretrain(trained_model_path, data_file, model_name, vector_name, epochs=5)
+```
 
-    ```
-  - Pre-train or resume word2vec training with same or new corpus or tokenized sentences
+### Bengali FastText
 
-    Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
+To use `fasttext` you need to install fasttext manually by `pip install fasttext==0.9.2`
 
-    ```py
-    from bnlp import BengaliWord2Vec
-    bwv = BengaliWord2Vec()
+NB: `fasttext` may not be worked in `windows`, it will only work in `linux`
 
-    trained_model_path = "mytrained_model.model"
-    data_file = "raw_text.txt"
-    model_name = "test_model.model"
-    vector_name = "test_vector.vector"
-    bwv.pretrain(trained_model_path, data_file, model_name, vector_name, epochs=5)
+### Generate Vector Using Pretrained Model
 
-    ```
-    
- * **Bengali FastText**
- 
-    To use `fasttext` you need to install fasttext manually by `pip install fasttext==0.9.2`
-    
-    NB: `fasttext` may not be worked in `windows`, it will only work in `linux`
+  ```py
+  from bnlp.embedding.fasttext import BengaliFasttext
 
-    - Generate Vector Using Pretrained Model
-      
+  bft = BengaliFasttext()
+  word = "গ্রাম"
+  model_path = "bengali_fasttext_wiki.bin"
+  word_vector = bft.generate_word_vector(model_path, word)
+  print(word_vector.shape)
+  print(word_vector)
+  ```
 
-      ```py
-      from bnlp.embedding.fasttext import BengaliFasttext
+### Train Bengali FastText Model
 
-      bft = BengaliFasttext()
-      word = "গ্রাম"
-      model_path = "bengali_fasttext_wiki.bin"
-      word_vector = bft.generate_word_vector(model_path, word)
-      print(word_vector.shape)
-      print(word_vector)
+Check [fasttext documentation](https://fasttext.cc/docs/en/options.html) for details of training parameter
 
+  ```py
+  from bnlp.embedding.fasttext import BengaliFasttext
 
-      ```
-    - Train Bengali FastText Model
+  bft = BengaliFasttext()
+  data = "raw_text.txt"
+  model_name = "saved_model.bin"
+  epoch = 50
+  bft.train(data, model_name, epoch)
+  ```
 
-      Check [fasttext documentation](https://fasttext.cc/docs/en/options.html) for details of training parameter
+### Generate Vector File from Fasttext Binary Model
 
-      ```py
-      from bnlp.embedding.fasttext import BengaliFasttext
+```py
+from bnlp.embedding.fasttext import BengaliFasttext
 
-      bft = BengaliFasttext()
-      data = "raw_text.txt"
-      model_name = "saved_model.bin"
-      epoch = 50
-      bft.train(data, model_name, epoch)
-      ```
+bft = BengaliFasttext()
 
-    - Generate Vector File from Fasttext Binary Model
-      ```py
-      from bnlp.embedding.fasttext import BengaliFasttext
+model_path = "mymodel.bin"
+out_vector_name = "myvector.txt"
+bft.bin2vec(model_path, out_vector_name)
+```
+
+## Bengali GloVe Word Vectors
+
+We trained glove model with bengali data(wiki+news articles) and published bengali glove word vectors</br>
+You can download and use it on your different machine learning purposes.
+
+```py
+from bnlp import BengaliGlove
+glove_path = "bn_glove.39M.100d.txt"
+word = "গ্রাম"
+bng = BengaliGlove()
+res = bng.closest_word(glove_path, word)
+print(res)
+vec = bng.word2vec(glove_path, word)
+print(vec)
+```
 
-      bft = BengaliFasttext()
+## Document Embedding
 
-      model_path = "mymodel.bin"
-      out_vector_name = "myvector.txt"
-      bft.bin2vec(model_path, out_vector_name)
-      ```
+### Bengali Doc2Vec
+#### Get document vector from input document
 
-* **Bengali GloVe Word Vectors**
+```py
+from bnlp import BengaliDoc2vec
 
-  We trained glove model with bengali data(wiki+news articles) and published bengali glove word vectors</br>
-  You can download and use it on your different machine learning purposes.
+bn_doc2vec = BengaliDoc2vec()
 
-  ```py
-  from bnlp import BengaliGlove
-  glove_path = "bn_glove.39M.100d.txt"
-  word = "গ্রাম"
-  bng = BengaliGlove()
-  res = bng.closest_word(glove_path, word)
-  print(res)
-  vec = bng.word2vec(glove_path, word)
-  print(vec)
+model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
+document = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
 
-  ```
+vector = bn_doc2vec.get_document_vector(model_path, text)
+print(vector)
+```
 
-## Document Embedding
-* __Bengali Doc2Vec__
-  - Get document vector from input document
+#### Find document similarity between two document
 
-    ```py
-    from bnlp import BengaliDoc2vec
-    
-    bn_doc2vec = BengaliDoc2vec()
-    
-    model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
-    document = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
-
-    vector = bn_doc2vec.get_document_vector(model_path, text)
-    print(vector)
-    ```
-
-  - Find document similarity between two document
-
-    ```py
-    from bnlp import BengaliDoc2vec
-    
-    bn_doc2vec = BengaliDoc2vec()
-    
-    model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
-    article_1 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
-    article_2 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
-
-    similarity = bn_doc2vec.get_document_similarity(
-      model_path,
-      article_1,
-      article_2
-    )
-    print(similarity)
-
-    ```
-
-  - Train doc2vec vector with custom text files
-
-    ```py
-    from bnlp import BengaliDoc2vec
-      
-    bn_doc2vec = BengaliDoc2vec()
-
-    text_files = "path/myfiles"
-    checkpoint_path = "msc/logs"
-
-    bn_doc2vec.train_doc2vec(
-      text_files, 
-      checkpoint_path=checkpoint_path,
-      vector_size=100,
-      min_count=2,
-      epochs=10
-    )
+```py
+from bnlp import BengaliDoc2vec
 
-    # it will train doc2vec with your text files and save the train model in checkpoint_path
+bn_doc2vec = BengaliDoc2vec()
 
-    ```
+model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
+article_1 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
+article_2 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
 
-## Bengali POS Tagging
-* **Bengali CRF POS Tagging** 
+similarity = bn_doc2vec.get_document_similarity(
+  model_path,
+  article_1,
+  article_2
+)
+print(similarity)
+```
 
+#### Train doc2vec vector with custom text files
 
-  - Find Pos Tag Using Pretrained Model
+```py
+from bnlp import BengaliDoc2vec
 
-    ```py
-    from bnlp import POS
-    bn_pos = POS()
-    model_path = "model/bn_pos.pkl"
-    text = "আমি ভাত খাই।" # or you can pass ['আমি', 'ভাত', 'খাই', '।']
-    res = bn_pos.tag(model_path, text)
-    print(res)
-    # [('আমি', 'PPR'), ('ভাত', 'NC'), ('খাই', 'VM'), ('।', 'PU')]
+bn_doc2vec = BengaliDoc2vec()
 
-    ```
-  - Train POS Tag Model
-  
-    ```py
-    from bnlp import POS
-    bn_pos = POS()
-    model_name = "pos_model.pkl"
-    train_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা', 'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
+text_files = "path/myfiles"
+checkpoint_path = "msc/logs"
 
-    test_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা', 'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
+bn_doc2vec.train_doc2vec(
+  text_files,
+  checkpoint_path=checkpoint_path,
+  vector_size=100,
+  min_count=2,
+  epochs=10
+)
 
-    bn_pos.train(model_name, train_data, test_data)
+# it will train doc2vec with your text files and save the train model in checkpoint_path
+```
 
-    ```
+## Bengali POS Tagging
 
-## Bengali NER
-* **Bengali CRF NER** 
+### Bengali CRF POS Tagging
 
+#### Find Pos Tag Using Pretrained Model
 
-  - Find NER Tag Using Pretrained Model
+```py
+from bnlp import POS
+bn_pos = POS()
+model_path = "model/bn_pos.pkl"
+text = "আমি ভাত খাই।" # or you can pass ['আমি', 'ভাত', 'খাই', '।']
+res = bn_pos.tag(model_path, text)
+print(res)
+# [('আমি', 'PPR'), ('ভাত', 'NC'), ('খাই', 'VM'), ('।', 'PU')]
+```
+
+#### Train POS Tag Model
+
+```py
+from bnlp import POS
+bn_pos = POS()
+model_name = "pos_model.pkl"
+train_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা',  'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
 
-    ```py
-    from bnlp import NER
-    bn_ner = NER()
-    model_path = "model/bn_ner.pkl"
-    text = "সে ঢাকায় থাকে।" # or you can pass ['সে', 'ঢাকায়', 'থাকে', '।']
-    result = bn_ner.tag(model_path, text)
-    print(result)
-    # [('সে', 'O'), ('ঢাকায়', 'S-LOC'), ('থাকে', 'O')]
+test_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা', 'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
 
-    ```
-  - Train NER Tag Model
-  
-    ```py
-    from bnlp import NER
-    bn_ner = NER()
-    model_name = "ner_model.pkl"
-    train_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
+bn_pos.train(model_name, train_data, test_data)
+```
 
-    test_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
+## Bengali NER
 
-    bn_ner.train(model_name, train_data, test_data)
+### Bengali CRF NER
 
-    ```
+#### Find NER Tag Using Pretrained Model
 
+```py
+from bnlp import NER
+bn_ner = NER()
+model_path = "model/bn_ner.pkl"
+text = "সে ঢাকায় থাকে।" # or you can pass ['সে', 'ঢাকায়', 'থাকে', '।']
+result = bn_ner.tag(model_path, text)
+print(result)
+# [('সে', 'O'), ('ঢাকায়', 'S-LOC'), ('থাকে', 'O')]
+```
+
+#### Train NER Tag Model
+
+```py
+from bnlp import NER
+bn_ner = NER()
+model_name = "ner_model.pkl"
+train_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
 
-## Bengali Corpus Class
+test_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
 
-* Stopwords and Punctuations
-  ```py
-  from bnlp.corpus import stopwords, punctuations, letters, digits
+bn_ner.train(model_name, train_data, test_data)
+```
 
-  print(stopwords)
-  print(punctuations)
-  print(letters)
-  print(digits)
 
-  ```
+## Bengali Corpus Class
 
-* Remove stopwords from Text
+### Stopwords and Punctuations
 
-    ```py
-    from bnlp.corpus import stopwords
-    from bnlp.corpus.util import remove_stopwords
-
-    raw_text = 'আমি ভাত খাই।' 
-    result = remove_stopwords(raw_text, stopwords)
-    print(result)
-    # ['ভাত', 'খাই', '।']
-    ```
+```py
+from bnlp.corpus import stopwords, punctuations, letters, digits
 
+print(stopwords)
+print(punctuations)
+print(letters)
+print(digits)
+```
+
+### Remove stopwords from Text
+
+```py
+from bnlp.corpus import stopwords
+from bnlp.corpus.util import remove_stopwords
+
+raw_text = 'আমি ভাত খাই।'
+result = remove_stopwords(raw_text, stopwords)
+print(result)
+# ['ভাত', 'খাই', '।']
+```
+
+## Text Cleaning
+We adopted different text cleaning formula, codes from [clean-text](https://github.com/jfilter/clean-text) and modified for Bangla. Now you can normalize and clean your text using the following methods.
+
+```py
+from bnlp import CleanText
+
+clean_text = CleanText(
+   fix_unicode=True,
+   unicode_norm=True,
+   unicode_norm_form="NFKC",
+   remove_url=False,
+   remove_email=False,
+   remove_emoji=False,
+   remove_number=False,
+   remove_digits=False,
+   remove_punct=False,
+   replace_with_url="<URL>",
+   replace_with_email="<EMAIL>",
+   replace_with_number="<NUMBER>",
+   replace_with_digit="<DIGIT>",
+   replace_with_punct = "<PUNC>"
+)
+
+input_text = "আমার সোনার বাংলা।"
+clean_text = clean_text(input_text)
+print(clean_text)
+```
 
 ## Contributor Guide
 
 Check [CONTRIBUTING.md](https://github.com/sagorbrur/bnlp/blob/master/CONTRIBUTING.md) page for details.
 
 
 ## Thanks To
```

### Comparing `bnlp_toolkit-3.3.0.dev0/bnlp_toolkit.egg-info/SOURCES.txt` & `bnlp_toolkit-3.3.1/bnlp_toolkit.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 LICENSE
 README.md
 setup.py
 bnlp/__init__.py
 bnlp/ner.py
 bnlp/pos.py
+bnlp/cleantext/__init__.py
+bnlp/cleantext/clean.py
+bnlp/cleantext/constants.py
 bnlp/corpus/__init__.py
 bnlp/corpus/util.py
 bnlp/embedding/__init__.py
 bnlp/embedding/doc2vec.py
 bnlp/embedding/fasttext.py
 bnlp/embedding/glove.py
 bnlp/embedding/word2vec.py
 bnlp/tokenizer/__init__.py
 bnlp/tokenizer/basic.py
 bnlp/tokenizer/nltk.py
 bnlp/tokenizer/sentencepiece.py
-bnlp/tokenizer/spacy.py
 bnlp_toolkit.egg-info/PKG-INFO
 bnlp_toolkit.egg-info/SOURCES.txt
 bnlp_toolkit.egg-info/dependency_links.txt
 bnlp_toolkit.egg-info/requires.txt
 bnlp_toolkit.egg-info/top_level.txt
-msc/__init__.py
-msc/test.py
+tests/test.py
```

### Comparing `bnlp_toolkit-3.3.0.dev0/setup.py` & `bnlp_toolkit-3.3.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 import codecs
 import setuptools
 
 
 setuptools.setup(
     name="bnlp_toolkit",
-    version="3.3.0dev",
+    version="3.3.1",
     author="Sagor Sarker",
     author_email="sagorhem3532@gmail.com",
     description="BNLP is a natural language processing toolkit for Bengali Language",
     long_description=codecs.open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/sagorbrur/bnlp",
     license="MIT",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires=">=3.6",
     install_requires=[
         "sentencepiece",
-        "gensim==4.0.1",
+        "gensim",
         "nltk",
         "numpy",
         "scipy",
         "sklearn-crfsuite",
-        "wasabi",
-        "tqdm"
+        "tqdm",
+        "ftfy",
+        "emoji==1.7.0",
     ],
-    extras_require={
-        'spacy': ["spacy==3.4.3"],
-        'fasttext': ["fasttext==0.9.2"]
-    },
 )
```


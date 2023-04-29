# Comparing `tmp/nlptoolssna-0.3.5.tar.gz` & `tmp/nlptoolssna-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.3.5.tar", last modified: Wed Apr 19 21:40:33 2023, max compression
+gzip compressed data, was "nlptoolssna-0.3.6.tar", last modified: Sat Apr 29 08:50:52 2023, max compression
```

## Comparing `nlptoolssna-0.3.5.tar` & `nlptoolssna-0.3.6.tar`

### file list

```diff
@@ -1,58 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.980403 nlptoolssna-0.3.5/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1821 2023-04-19 21:40:33.980403 nlptoolssna-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.902891 nlptoolssna-0.3.5/docs/
--rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/authors.rst
--rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/history.rst
--rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/installation.rst
--rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/readme.rst
--rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.911047 nlptoolssna-0.3.5/nlptools/
-drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.911047 nlptoolssna-0.3.5/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.3.5/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     2569 2023-04-18 22:20:52.000000 nlptoolssna-0.3.5/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/nlptools/__init__.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.920300 nlptoolssna-0.3.5/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.3.5/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.920300 nlptoolssna-0.3.5/nlptools/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.3.5/nlptools/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.3.5/nlptools/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.941124 nlptoolssna-0.3.5/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.3.5/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.3.5/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.3.5/nlptools/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0     7505 2023-04-19 21:39:18.000000 nlptoolssna-0.3.5/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.3.5/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.3.5/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.941124 nlptoolssna-0.3.5/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.3.5/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.3.5/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.951335 nlptoolssna-0.3.5/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.3.5/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.3.5/nlptools/salma/implication.py
--rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.3.5/nlptools/salma/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.974601 nlptoolssna-0.3.5/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-04-19 21:40:33.000000 nlptoolssna-0.3.5/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-04-19 21:40:33.000000 nlptoolssna-0.3.5/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 21:40:33.000000 nlptoolssna-0.3.5/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-19 21:40:33.000000 nlptoolssna-0.3.5/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.3.5/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-04-19 21:40:33.000000 nlptoolssna-0.3.5/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 21:40:33.000000 nlptoolssna-0.3.5/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-04-19 21:40:33.980403 nlptoolssna-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1843 2023-04-18 21:50:46.000000 nlptoolssna-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 21:40:33.980403 nlptoolssna-0.3.5/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.3.5/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.318354 nlptoolssna-0.3.6/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1821 2023-04-29 08:50:52.318354 nlptoolssna-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.146482 nlptoolssna-0.3.6/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.3.6/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.093352 nlptoolssna-0.3.6/docs/build/
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.093407 nlptoolssna-0.3.6/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.146482 nlptoolssna-0.3.6/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.3.6/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.178885 nlptoolssna-0.3.6/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.3.6/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.3.6/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.3.6/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.3.6/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.3.6/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.223258 nlptoolssna-0.3.6/docs/source/
+-rw-rw-rw-   0        0        0      318 2023-04-27 09:55:38.000000 nlptoolssna-0.3.6/docs/source/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.234340 nlptoolssna-0.3.6/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.3.6/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.235367 nlptoolssna-0.3.6/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.266745 nlptoolssna-0.3.6/docs/source/api/morph/
+-rw-rw-rw-   0        0        0       48 2023-04-26 20:02:35.000000 nlptoolssna-0.3.6/docs/source/api/morph/charsets.rst
+-rw-rw-rw-   0        0        0       66 2023-04-26 20:02:52.000000 nlptoolssna-0.3.6/docs/source/api/morph/lemmatizeSentence.rst
+-rw-rw-rw-   0        0        0      127 2023-04-27 18:16:11.000000 nlptoolssna-0.3.6/docs/source/api/morph/morph_tagger.rst
+-rw-rw-rw-   0        0        0       65 2023-04-26 20:03:13.000000 nlptoolssna-0.3.6/docs/source/api/morph/tokenizers_words.rst
+-rw-rw-rw-   0        0        0      280 2023-04-27 12:17:19.000000 nlptoolssna-0.3.6/docs/source/api/morph.rst
+-rw-rw-rw-   0        0        0      140 2023-04-26 20:11:06.000000 nlptoolssna-0.3.6/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.3.6/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.3.6/docs/source/conf.py
+-rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.3.6/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.3.6/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.270939 nlptoolssna-0.3.6/nlptools/
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.275109 nlptoolssna-0.3.6/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.3.6/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     2527 2023-04-27 21:39:46.000000 nlptoolssna-0.3.6/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/nlptools/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.276639 nlptoolssna-0.3.6/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.3.6/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.284828 nlptoolssna-0.3.6/nlptools/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.3.6/nlptools/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.3.6/nlptools/jaccard/jaccardFunction.py
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.293431 nlptoolssna-0.3.6/nlptools/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.3.6/nlptools/morph/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.3.6/nlptools/morph/charsets.py
+-rw-rw-rw-   0        0        0     7467 2023-04-29 08:48:51.000000 nlptoolssna-0.3.6/nlptools/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.3.6/nlptools/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.3.6/nlptools/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.293431 nlptoolssna-0.3.6/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.3.6/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.3.6/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.301537 nlptoolssna-0.3.6/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.3.6/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.3.6/nlptools/salma/implication.py
+-rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.3.6/nlptools/salma/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.310194 nlptoolssna-0.3.6/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1821 2023-04-29 08:50:51.000000 nlptoolssna-0.3.6/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1479 2023-04-29 08:50:52.000000 nlptoolssna-0.3.6/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 08:50:51.000000 nlptoolssna-0.3.6/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-29 08:50:51.000000 nlptoolssna-0.3.6/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.3.6/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-04-29 08:50:51.000000 nlptoolssna-0.3.6/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-29 08:50:51.000000 nlptoolssna-0.3.6/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-04-29 08:50:52.318354 nlptoolssna-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1843 2023-04-18 21:50:46.000000 nlptoolssna-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.318354 nlptoolssna-0.3.6/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.3.5/CONTRIBUTING.rst` & `nlptoolssna-0.3.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.5/LICENSE` & `nlptoolssna-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.5/PKG-INFO` & `nlptoolssna-0.3.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.3.5/README.rst` & `nlptoolssna-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.5/docs/Makefile` & `nlptoolssna-0.3.6/docs/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line.
+SOURCEDIR     = source
 SPHINXOPTS    =
-SPHINXBUILD   = python -msphinx
+SPHINXBUILD   = sphinx-build -c $(SOURCEDIR) -c $(SOURCEDIR)/config
 SPHINXPROJ    = nlptools
-SOURCEDIR     = .
 BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+    @$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+    @$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `nlptoolssna-0.3.5/docs/conf.py` & `nlptoolssna-0.3.6/docs/source/conf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,113 +1,140 @@
-#!/usr/bin/env python
+# -*- coding: utf-8 -*-
 #
-# nlptools documentation build configuration file, created by
-# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
+# Configuration file for the Sphinx documentation builder.
 #
-# This file is execfile()d with the current directory set to its
-# containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
+# This file does only contain a selection of the most common options. For a
+# full list see the documentation:
+# http://www.sphinx-doc.org/en/master/config
+
+# -- Path setup --------------------------------------------------------------
 
-# If extensions (or modules to document with autodoc) are in another
-# directory, add these directories to sys.path here. If the directory is
-# relative to the documentation root, use os.path.abspath to make it
-# absolute, like shown here.
+# If extensions (or modules to document with autodoc) are in another directory,
+# add these directories to sys.path here. If the directory is relative to the
+# documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
-sys.path.insert(0, os.path.abspath('..'))
 
-import nlptools
+# # Path to the parent directory of the documentation directory
+# parent_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
+
+# # Path to the nlptools package directory
+# nlptools_dir = os.path.join(parent_dir, 'nlptools')
+
+# # Insert the nlptools directory at the beginning of the system path
+# #sys.path.insert(0, nlptools_dir)
+sys.path.insert(0, os.path.abspath('../..'))
 
-# -- General configuration ---------------------------------------------
+# -- Extension Imports -------------------------------------------------------
+
+
+from recommonmark.parser import CommonMarkParser
+
+# -- Project information -----------------------------------------------------
+
+project = 'nlptools'
+copyright = '2023, Birzeit University'
+author = 'Alaa Omar'
+
+# The short X.Y version
+version = '0.3.5'
+# The full version, including alpha/beta/rc tags
+release = '0.3.5'
+
+
+# -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
+# ones.
+extensions = [
+    'sphinx.ext.napoleon',
+    'sphinx.ext.autodoc',
+    'sphinx.ext.githubpages',
+    'sphinx.ext.intersphinx'
+]
+
+intersphinx_mapping = {
+    'python': ('https://docs.python.org/3', None)
+}
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
+# Source parsers
+source_parsers = {
+    '.md': CommonMarkParser,
+}
+
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
-# source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ['.rst', '.md']
+# source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
-# General information about the project.
-project = 'nlptools'
-copyright = "2023, Alaa' Omar"
-author = "Alaa' Omar"
-
-# The version info for the project you're documenting, acts as replacement
-# for |version| and |release|, also used in various other places throughout
-# the built documents.
-#
-# The short X.Y version.
-version = nlptools.__version__
-# The full version, including alpha/beta/rc tags.
-release = nlptools.__version__
-
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-# This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+# This pattern also affects html_static_path and html_extra_path.
+exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
-
-# If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = False
+pygments_style = None
 
 
-# -- Options for HTML output -------------------------------------------
+# -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = 'sphinx_rtd_theme'
 
-# Theme options are theme-specific and customize the look and feel of a
-# theme further.  For a list of options available for each theme, see the
+# Theme options are theme-specific and customize the look and feel of a theme
+# further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
+# Custom sidebar templates, must be a dictionary that maps document names
+# to template names.
+#
+# The default sidebars (for documents that don't match any pattern) are
+# defined by theme itself.  Builtin themes are using these templates by
+# default: ``['localtoc.html', 'relations.html', 'sourcelink.html',
+# 'searchbox.html']``.
+#
+# html_sidebars = {}
 
-# -- Options for HTMLHelp output ---------------------------------------
+
+# -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'nlptoolsdoc'
+htmlhelp_basename = 'nlptools_doc'
 
 
-# -- Options for LaTeX output ------------------------------------------
+# -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
 
     # The font size ('10pt', '11pt' or '12pt').
@@ -120,43 +147,62 @@
 
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title, author, documentclass
-# [howto, manual, or own class]).
+# (source start file, target name, title,
+#  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'nlptools.tex',
-     'nlptools Documentation',
-     'Alaa' Omar', 'manual'),
+    (master_doc, 'nlptools.tex', 'NLP Tools Documentation',
+     'Alaa Omar', 'manual'),
 ]
 
 
-# -- Options for manual page output ------------------------------------
+# -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'nlptools',
-     'nlptools Documentation',
+    (master_doc, 'nlptools', 'nlptools Documentation',
      [author], 1)
 ]
 
 
-# -- Options for Texinfo output ----------------------------------------
+# -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'nlptools',
-     'nlptools Documentation',
-     author,
-     'nlptools',
-     'One line description of project.',
+    (master_doc, 'nlptools', 'nlptools Documentation',
+     author, 'nlptools',
+     'Arabic NLP tools'
+     ,
      'Miscellaneous'),
 ]
 
 
+# -- Options for Epub output -------------------------------------------------
+
+# Bibliographic Dublin Core info.
+epub_title = project
 
+# The unique identifier of the text. This can be a ISBN number
+# or the project homepage.
+#
+# epub_identifier = ''
+
+# A unique identification for the text.
+#
+# epub_uid = ''
+
+# A list of files that should not be packed into the epub file.
+epub_exclude_files = ['search.html']
+
+
+# -- Extension configuration -------------------------------------------------
+
+autodoc_mock_imports = [
+    'kenlm'
+]
```

### Comparing `nlptoolssna-0.3.5/docs/installation.rst` & `nlptoolssna-0.3.6/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.5/docs/make.bat` & `nlptoolssna-0.3.6/docs/make.bat`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 @ECHO OFF
 
 pushd %~dp0
 
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=python -msphinx
+	set SPHINXBUILD=sphinx-build
 )
-set SOURCEDIR=.
-set BUILDDIR=_build
-set SPHINXPROJ=nlptools
+set SOURCEDIR=source
+set BUILDDIR=build
 
 if "%1" == "" goto help
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
-	echo.The Sphinx module was not found. Make sure you have Sphinx installed,
-	echo.then set the SPHINXBUILD environment variable to point to the full
-	echo.path of the 'sphinx-build' executable. Alternatively you may add the
-	echo.Sphinx directory to PATH.
+	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
+	echo.installed, then set the SPHINXBUILD environment variable to point
+	echo.to the full path of the 'sphinx-build' executable. Alternatively you
+	echo.may add the Sphinx directory to PATH.
 	echo.
 	echo.If you don't have Sphinx installed, grab it from
 	echo.http://sphinx-doc.org/
 	exit /b 1
 )
 
 %SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
```

### Comparing `nlptoolssna-0.3.5/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.3.6/nlptools/DataDownload/downloader.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import sys
 from pathlib import Path
 import requests  
 import zipfile
 from tqdm import tqdm
 
 urls = {
-    'morph':'https://portal.sina.birzeit.edu/20230418test27012000.pickle',
-    'ner': 'http://portal.sina.birzeit.edu/867530901NED20230418modelv28.zip',
-    'salma': 'http://portal.sina.birzeit.edu/98765432128.zip',
-    'salma2021': 'http://portal.sina.birzeit.edu/98765432128_02_22_May_2021.zip'
+    'morph':'https://portal.sina.birzeit.edu/ALMA27012000.pickle',
+    'ner': 'http://portal.sina.birzeit.edu/Wj27012000.zip',
+    'salma': 'http://portal.sina.birzeit.edu/SALMA27012000.zip',
+    'salma2021': 'http://portal.sina.birzeit.edu/SALMA_v2.zip'
 }
 
 def get_appdatadir():
     home = str(Path.home())
 
     if 'google.colab' in sys.modules:
         return Path('/content/nlptools')
```

### Comparing `nlptoolssna-0.3.5/nlptools/data/my_data.pickle` & `nlptoolssna-0.3.6/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.5/nlptools/jaccard/jaccardFunction.py` & `nlptoolssna-0.3.6/nlptools/jaccard/jaccardFunction.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.5/nlptools/morph/charsets.py` & `nlptoolssna-0.3.6/nlptools/morph/charsets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-
+# We acknoledge that this file  charsets.py is imported from Camel tools citation. url
+#
 
 import unicodedata
 
 from six import unichr
 
 
 UNICODE_PUNCT_CHARSET = frozenset(
```

### Comparing `nlptoolssna-0.3.5/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.3.6/nlptools/morph/morph_tagger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,87 +1,89 @@
 import pickle
 from nlptools.morph import settings 
 import re
-from nlptools.morph.lemmatizeSentence import lemmatize_sentence
 from nlptools.morph.tokenizers_words import simple_word_tokenize
 from nlptools.parse.parser import arStrip
 import os.path
 from nlptools.DataDownload import downloader
 
 def load_ALMA_dic():
    # Open the Pickle file in binary mode
-    filename = '20230418test27012000.pickle'
+    filename = 'ALMA27012000.pickle'
     path =downloader.get_appdatadir()
     file_path = os.path.join(path, filename)
     
 
     with open(file_path, 'rb') as f:
        #Load the serialized data from the file
        ALMA_dic = pickle.load(f)
        #print(ALMA_dic)
        return ALMA_dic
 
-def tag(word, lang, task):
+def tag(token, language, task):
     """
-    given a token, this method retrives the possible morphological solutions (lemma, pos, and frequency) filterd by spesific
+    Given a token, this method retrives the possible morphological solutions (lemma, pos, frequency, task and language) filterd by spesific
     language and task.
-     
-       in a dictionary to find its lemma, part of speech, and frequency,
-    filtered by the specified language and task. The dictionary used is assumed to be a nested dictionary where keys
-    are words and values are lists of lemma entries, where each lemma entry is a list of the form
-    [form_id, form, pos_ar, lemma, lemma_freq, lang, task].
-
+          
     Args:
-        word (str): The Arabic word to be morphologcaly tagged.
-        lang (str): The language to filter the results by [MSA, Pal, ].
-        task (str): The task to filter the results by [lemmatizer, pos, full].
+        token (str): The Arabic token to be morphologcaly tagged.
+        language (str): The language to filter the results by, [MSA, Pal, ].
+        task (str): The task to filter the results by [lemmatizer, pos, full]. The defualt task if not specisifd is `full`.
 
     Returns:
-        list: A list of [word, lemma, pos_ar, lemma_freq, lang, task], where:
-            - word: the original input word
-            - lemma: the lemma of the word
-            - pos_ar: the part of speech of the word in Arabic
-            - lemma_freq: the frequency of the lemma in the dictionary @check:returen or not
-            - lang: the input language value
-            - task: the input task languge
+        list: A list of [token, lemma, pos_ar, lemma_freq, language, task], where:
+            - token: the original input token
+            - lemma: the lemma of the token
+            - pos_ar: the part of speech of the token in Arabic
+            - lemma_freq: the frequency of the lemma in the dictionary
+            - language: the input language 
+            - task: the input task 
 
-            If no sloution is found for this word, an empty list is returned.
+            If no sloution is found for this token, an empty list is returned.
     """
-    if word in settings.div_dic.keys():
+    if token in settings.div_dic.keys():
 
-        soluation =settings.div_dic[word][1]
-        if task =='full' and soluation[-2] == lang:
-            return  [word, soluation[3], soluation[2],  soluation[-2], soluation[-1]]
-        elif soluation[-2] == lang and soluation[-1] ==task:
-            return [word, soluation[3], soluation[2],  soluation[-2], soluation[-1]]
+        soluation =settings.div_dic[token][1]
+        if task =='full' and soluation[-2] == language:
+            return  [token, soluation[3], soluation[2],  soluation[-2], soluation[-1]]
+        elif soluation[-2] == language and soluation[-1] ==task:
+            return [token, soluation[3], soluation[2],  soluation[-2], soluation[-1]]
         return []
     else:
         return []
 
-def lemmatize_sentence(text ,lang, task):
+def lemmatize_sentence(text ,language, task):
    """
-    This method takes a text as input and returns a morphological solution for each token in this text, Based
-    on the input language and task, such that:
-    if task == lemmatizaer, then the morphological soltuion is only the lemma.
-       task == pos, then the morphological soltuion is only the pos.
-       task == full, the the morphological soltuion is both the lemma and the pos.
+    This method takes a text as input and returns a morphological solution for each token in this text, Based on the input language and task, such that:
+    if:
+         - task is lemmatizaer, then the morphological soltuion is only the lemma.
+         - task is pos, then the morphological soltuion is only the pos.
+         - task is full, the the morphological soltuion is both the lemma and the pos.
      
-    the lang arguemet is used to help the morphological analysis to return more accurate solutions, for example if the sentence
-    is MSA, or Palestinian dilect.
+    The language arguemet is used to help the morphological analysis to return more accurate solutions, for example if the text is MSA, or dialects (Palestinian dilect, pppp).
    
-
     Args:
-    - text (str): The input text to morphologicaly analyzed.
-    - task (str): The type of task being performed (e.g., 'lemmatizer', 'pos', or 'full').
-    - lang (str): The language of the input sentence (e.g., 'MSA').
-
+          - text (str): The input text to morphologicaly analyzed.
+          - language (str): The language of the input text (e.g., 'MSA').
+          - task (str): The type of task being performed (e.g., 'lemmatizer', 'pos', or 'full').
+         
     Returns:
     - output_list (list): A list of morphological solution for each token in the input text.
 
+    **Example:**
+
+    .. highlight:: python
+    .. code-block:: python
+
+         from nlptools.morph import morph_tagger
+      
+         # Return the morpological solution for each token in this text
+         morph_tagger.tagger('ذهب الولد الى المدرسة')
     """
+
    output_list = []
    # tokenize sentence into words
    words = simple_word_tokenize(text)
    # for each word 
    for word in words:
          result_word =[]
          # Trim spaces 
@@ -99,79 +101,75 @@
 
          # if word is english, update pos to be ENGLISH
          elif re.match("^[a-zA-Z]*$", word):
             solution[2] = "ENGLISH"
 
          else:
             # search for a word (as is) in ALMA dictionary   
-            result_word = tag(word,lang, task)
+            result_word = tag(word,language, task)
             
             if len(re.sub(r'^[ﻝ]','',re.sub(r'^[ﺍ]','',word))) > 5 and result_word == []:
                # try with remove remove AL
-               result_word = tag(re.sub(r'^[ﻝ]','',re.sub(r'^[ﺍ]','',word)), lang, task)
+               result_word = tag(re.sub(r'^[ﻝ]','',re.sub(r'^[ﺍ]','',word)), language, task)
 
             if result_word == []:
               # try with replace ﻩ with ﺓ
-               result_word = tag(re.sub(r'[ﻩ]$','ﺓ',word), lang, task)
+               result_word = tag(re.sub(r'[ﻩ]$','ﺓ',word), language, task)
 
             if result_word == []:
                # try with unify Alef
                word_with_unify_alef = arStrip(word , False , False , False , False , True , False) # Unify Alef
-               result_word = tag(word_with_unify_alef, lang, task)
+               result_word = tag(word_with_unify_alef, language, task)
             
             if result_word == []:
                # try with remove diac
                word_undiac = arStrip(word , True , False , True , True , False , False) # remove diacs, shaddah ,  digit
-               result_word = tag(word_undiac, lang, task)
+               result_word = tag(word_undiac, language, task)
 
             if result_word == []:
                # try with remove diac and unify alef
                word_undiac = arStrip(word , True , True , True , False, True , False) # diacs , smallDiacs , shaddah ,  alif
-               result_word = tag(word_undiac, lang, task)
-         
+               result_word = tag(word_undiac, language, task)
+
          if result_word != []:
                # if solution found
                tmp_solution = [word,word+"_0","",0]               
                tmp_solution[1] = result_word[2] # lemma
                tmp_solution[2] = result_word[1] # pos_ar
                tmp_solution[3] = result_word[3] # lemma_freq
                output_list.append(tmp_solution)
          else:
             # if no solution is found
             output_list.append(solution)
+
    return output_list               
         
-def tagger(text: str, task = 'full', lang = 'MSA') -> list:
+def tagger(text: str, task = 'full', language = 'MSA') -> list:
 
     """
-    This method takes an Arabic text as input, tokenize it into tokens and calles 
-    the morphological tagger to return the morpological solution for each token in this text.
-    There is not limit for the text size, but one should be resonable based on the available resources (computational power).
-    @check
-
-   @comment : text or sentence. 
-    
+    This method takes an Arabic text as input, tokenize it into tokens and calles the morphological tagger to return the morpological solution for each token in this text.
+    There is no limit for the text size, but one should be resonable based on the available resources (computational power).
+   
     Args:
-        text (str): The input Arabic sentence to be morphologically analyzed and tagged.
-        task (str): The type of morphological analysis and tagging to be performed. Default is 'full'.
-        lang (str): The language of the input sentence. Default is 'MSA' (Modern Standard Arabic).
+        - text (str): The input Arabic text to be morphologically analyzed and tagged.
+        - task (str): The type of morphological analysis and tagging to be performed. Default is 'full'.
+        - language (str): The language of the input text. Default is 'MSA' (Modern Standard Arabic).
         
     Returns:
-        list: A list of lists, where each sublist contains information about a word in the input text, including 
-              the original word, its lemma, its part of speech (POS) tag, and its lemma frequency.
+        list: A list of lists, where each sublist contains information about a token in the input text, including the original tokem, its lemma, its part of speech (POS) tag, its lemma frequency, the task and the language.
     """
     
     # Check if the ALMA dictionary has been loaded
     if settings.flag == True:
         settings.flag = False
     settings.div_dic = load_ALMA_dic()
    
     
     # Perform lemmatization on the input sentence
-    output_list = lemmatize_sentence(text,lang, task)
+    output_list = lemmatize_sentence(text,language, task)
     
     # Return the list of lemmatized words
     return output_list
```

### Comparing `nlptoolssna-0.3.5/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.3.6/nlptools/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.5/nlptools/parse/parser.py` & `nlptoolssna-0.3.6/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.5/nlptools/salma/implication.py` & `nlptoolssna-0.3.6/nlptools/salma/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.5/nlptools/salma/tokenizers_words.py` & `nlptoolssna-0.3.6/nlptools/salma/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.5/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.3.6/nlptoolssna.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.3.5/setup.cfg` & `nlptoolssna-0.3.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.5/setup.py` & `nlptoolssna-0.3.6/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/insights-extractor-0.1.3.tar.gz` & `tmp/insights-extractor-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/insights-extractor/insights-extractor/dist/.tmp-lrxn8f7b/insights-extractor-0.1.3.tar", last modified: Fri Apr 28 20:34:03 2023, max compression
+gzip compressed data, was "/home/runner/work/insights-extractor/insights-extractor/dist/.tmp-3wlvixic/insights-extractor-0.1.4.tar", last modified: Sat Apr 29 15:01:55 2023, max compression
```

## Comparing `insights-extractor-0.1.3.tar` & `insights-extractor-0.1.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/dist/insights-extractor-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/dist/insights_extractor-0.1.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/extractlib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/extractlib/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/classification/prep_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/extractlib/classification/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/classification/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/classification/utils/keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/extractlib/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/document/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/document/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/document/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/document/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/extractlib/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/extractlib/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/models/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/extractlib/ner/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/ner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/extractlib/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/nlp/pre_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/nlp/stopwords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/extractlib/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/settings/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/extractlib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/extractlib/utils/temp_dir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/insights_extractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/insights_extractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/insights_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/insights_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/insights_extractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/insights_extractor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/src/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/src/requirements/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:34:03.000000 insights-extractor-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/tests/pre_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/tests/prep_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-28 20:33:47.000000 insights-extractor-0.1.3/tests/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/dist/insights-extractor-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/dist/insights_extractor-0.1.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/classification/prep_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/classification/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/classification/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/classification/utils/keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/document/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/document/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/document/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/document/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/models/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/ner/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/ner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/nlp/pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/nlp/stopwords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/settings/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/utils/temp_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/insights_extractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/insights_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/insights_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/insights_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/insights_extractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/insights_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/requirements/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/tests/pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/tests/prep_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/tests/table.py
```

### Comparing `insights-extractor-0.1.3/.github/workflows/python-publish.yml` & `insights-extractor-0.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/LICENSE` & `insights-extractor-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/PKG-INFO` & `insights-extractor-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insights-extractor
-Version: 0.1.3
+Version: 0.1.4
 Summary: Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities.
 Author-email: Trae Moore <trae.dev@gmail.com>
 Project-URL: Homepage, https://github.com/traemoore/insights-extractor
 Project-URL: Tests, https://github.com/traemoore/insights-extractor-test
 Project-URL: Bug Tracker, https://github.com/traemoore/insights-extractor/issues
 Keywords: nltk,spaCy,Pymupdf,Camelot,OpenCV,Ghostscript,insight-extractor,pdf extraction,pdf data extraction,pdf data,classification,keyword extraction
 Classifier: Programming Language :: Python :: 3
```

### Comparing `insights-extractor-0.1.3/README.md` & `insights-extractor-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/dist/insights-extractor-0.1.0.tar.gz` & `insights-extractor-0.1.4/dist/insights-extractor-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/dist/insights_extractor-0.1.0-py3-none-any.whl` & `insights-extractor-0.1.4/dist/insights_extractor-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/pyproject.toml` & `insights-extractor-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   "nltk == 3.8.1; python_version >= '3.7'",
   "PyMuPDF == 1.21.1; python_version >= '3.7'",
   "camelot-py == 0.11.0; python_version >= '3.6'",
   "opencv-python == 4.7.0.72; python_version >= '3.6'",
   "ghostscript == 0.7; python_version >= '3.6'"
 ]
 name = "insights-extractor"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Trae Moore", email="trae.dev@gmail.com" },
 ]
 description = "Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["nltk", "spaCy", "Pymupdf", "Camelot", "OpenCV", "Ghostscript", "insight-extractor", "pdf extraction", "pdf data extraction", "pdf data", "classification", "keyword extraction"]
```

### Comparing `insights-extractor-0.1.3/src/extractlib/classification/prep_utils.py` & `insights-extractor-0.1.4/src/extractlib/classification/prep_utils.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/src/extractlib/classification/utils/keywords.py` & `insights-extractor-0.1.4/src/extractlib/classification/utils/keywords.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/src/extractlib/document/page.py` & `insights-extractor-0.1.4/src/extractlib/document/page.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/src/extractlib/document/process.py` & `insights-extractor-0.1.4/src/extractlib/document/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,10 +136,16 @@
                     # 'classification_training_data': "" #clean_text(training_data, remove_punctuation=True),
                     # 'kvps': []
                 }
             }
 
             return data
         except Exception as e:
+            data = {
+                'page': index,
+                'error': str(e)
+            }
+            print(f'Error processing page {index} of {file_path}:\n {e}')
             # Raise an error if an exception occurs while processing the page
-            raise PageProcessingError(
-                f'Error processing page {index} of {file_path}: {e}')
+            # raise PageProcessingError(
+            #     f'Error processing page {index} of {file_path}: {e}')
+            return data
```

### Comparing `insights-extractor-0.1.3/src/extractlib/document/table.py` & `insights-extractor-0.1.4/src/extractlib/document/table.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/src/extractlib/document/utils.py` & `insights-extractor-0.1.4/src/extractlib/document/utils.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/src/extractlib/ner/__init__.py` & `insights-extractor-0.1.4/src/extractlib/ner/__init__.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/src/extractlib/nlp/pre_process.py` & `insights-extractor-0.1.4/src/extractlib/nlp/pre_process.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/src/extractlib/settings/config.py` & `insights-extractor-0.1.4/src/extractlib/settings/config.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/src/extractlib/utils/json_utils.py` & `insights-extractor-0.1.4/src/extractlib/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/src/insights_extractor.egg-info/PKG-INFO` & `insights-extractor-0.1.4/src/insights_extractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insights-extractor
-Version: 0.1.3
+Version: 0.1.4
 Summary: Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities.
 Author-email: Trae Moore <trae.dev@gmail.com>
 Project-URL: Homepage, https://github.com/traemoore/insights-extractor
 Project-URL: Tests, https://github.com/traemoore/insights-extractor-test
 Project-URL: Bug Tracker, https://github.com/traemoore/insights-extractor/issues
 Keywords: nltk,spaCy,Pymupdf,Camelot,OpenCV,Ghostscript,insight-extractor,pdf extraction,pdf data extraction,pdf data,classification,keyword extraction
 Classifier: Programming Language :: Python :: 3
```

### Comparing `insights-extractor-0.1.3/src/insights_extractor.egg-info/SOURCES.txt` & `insights-extractor-0.1.4/src/insights_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/tests/pre_process.py` & `insights-extractor-0.1.4/tests/pre_process.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/tests/prep_utils.py` & `insights-extractor-0.1.4/tests/prep_utils.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.3/tests/table.py` & `insights-extractor-0.1.4/tests/table.py`

 * *Files identical despite different names*


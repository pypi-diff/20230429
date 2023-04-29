# Comparing `tmp/insights-extractor-0.1.4.tar.gz` & `tmp/insights-extractor-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/insights-extractor/insights-extractor/dist/.tmp-3wlvixic/insights-extractor-0.1.4.tar", last modified: Sat Apr 29 15:01:55 2023, max compression
+gzip compressed data, was "/home/runner/work/insights-extractor/insights-extractor/dist/.tmp-pb8uwas5/insights-extractor-0.1.5.tar", last modified: Sat Apr 29 20:27:34 2023, max compression
```

## Comparing `insights-extractor-0.1.4.tar` & `insights-extractor-0.1.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/dist/insights-extractor-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/dist/insights_extractor-0.1.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/classification/prep_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/classification/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/classification/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/classification/utils/keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/document/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/document/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/document/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/document/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/models/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/ner/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/ner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/nlp/pre_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/nlp/stopwords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/settings/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/extractlib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/extractlib/utils/temp_dir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/insights_extractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/insights_extractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/insights_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/insights_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/insights_extractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/insights_extractor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/src/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/src/requirements/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:01:55.000000 insights-extractor-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/tests/pre_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/tests/prep_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-29 15:01:43.000000 insights-extractor-0.1.4/tests/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/dist/insights-extractor-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/dist/insights_extractor-0.1.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/extractlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/extractlib/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/classification/prep_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/extractlib/classification/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/classification/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/classification/utils/keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/extractlib/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/document/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/document/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/document/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/document/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/extractlib/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/extractlib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/models/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/extractlib/ner/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/ner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/extractlib/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/nlp/pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/nlp/stopwords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/extractlib/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/settings/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/extractlib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/extractlib/utils/temp_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/insights_extractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/insights_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/insights_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/insights_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/insights_extractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/insights_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/src/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/src/requirements/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:27:34.000000 insights-extractor-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/tests/pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/tests/prep_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-29 20:27:20.000000 insights-extractor-0.1.5/tests/table.py
```

### Comparing `insights-extractor-0.1.4/.github/workflows/python-publish.yml` & `insights-extractor-0.1.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.4/LICENSE` & `insights-extractor-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.4/PKG-INFO` & `insights-extractor-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insights-extractor
-Version: 0.1.4
+Version: 0.1.5
 Summary: Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities.
 Author-email: Trae Moore <trae.dev@gmail.com>
 Project-URL: Homepage, https://github.com/traemoore/insights-extractor
 Project-URL: Tests, https://github.com/traemoore/insights-extractor-test
 Project-URL: Bug Tracker, https://github.com/traemoore/insights-extractor/issues
 Keywords: nltk,spaCy,Pymupdf,Camelot,OpenCV,Ghostscript,insight-extractor,pdf extraction,pdf data extraction,pdf data,classification,keyword extraction
 Classifier: Programming Language :: Python :: 3
```

### Comparing `insights-extractor-0.1.4/README.md` & `insights-extractor-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.4/dist/insights-extractor-0.1.0.tar.gz` & `insights-extractor-0.1.5/dist/insights-extractor-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.4/dist/insights_extractor-0.1.0-py3-none-any.whl` & `insights-extractor-0.1.5/dist/insights_extractor-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.4/pyproject.toml` & `insights-extractor-0.1.5/pyproject.toml`

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
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Trae Moore", email="trae.dev@gmail.com" },
 ]
 description = "Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["nltk", "spaCy", "Pymupdf", "Camelot", "OpenCV", "Ghostscript", "insight-extractor", "pdf extraction", "pdf data extraction", "pdf data", "classification", "keyword extraction"]
```

### Comparing `insights-extractor-0.1.4/src/extractlib/classification/prep_utils.py` & `insights-extractor-0.1.5/src/extractlib/classification/prep_utils.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.4/src/extractlib/classification/utils/keywords.py` & `insights-extractor-0.1.5/src/extractlib/classification/utils/keywords.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.4/src/extractlib/document/page.py` & `insights-extractor-0.1.5/src/extractlib/document/page.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.4/src/extractlib/document/process.py` & `insights-extractor-0.1.5/src/extractlib/document/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .utils import split_document_pages
 from ..models.table import Table
 from ..settings import config
 from ..utils.json_utils import cleanse_and_tag_json_structure
 from ..exceptions import DocumentProcessingError, PageProcessingError
 
 
-def process_document(file: str, exclude_pages=None, use_multithreading=False,  split_pages_output_dir=None, delete_split_pages=True):
+def process_document(file: str, settings: dict = None, use_multithreading: bool = False, split_pages_output_dir: str = None, delete_split_pages: bool = True):
     """
     Process a document by splitting it into pages and processing each page individually.
 
     Args:
         file (str): The path to the input document file.
         pages (list): A list of page numbers to exclude (non-zero based index). If None, all pages are processed (default=None).
         use_multithreading (bool): Whether to use multi-threading to process the pages (default=False).
@@ -28,17 +28,20 @@
         dict: A dictionary containing the processed data for each page. The dictionary has the following keys:
             - 'pages': A list of dictionaries containing the processed data for each page. Each dictionary has the following keys:
                 - 'page': An integer identifying the page number.
                 - 'content': A dictionary containing the extracted content for the page.
 
     Raises: DocumentProcessingError if an error occurs while processing the document.
     """
+
+    config.update(settings)
+
     result = {
         'document_name': os.path.basename(file),
-        'excluded_pages': exclude_pages if exclude_pages is not None else None,
+        'excluded_pages': config.exclude_pages if config.exclude_pages is not None else None,
         'pages': []
     }
 
     try:
         # Split the input document into individual pages
         target_dir, files = split_document_pages(
             file, split_pages_output_dir)
@@ -47,28 +50,28 @@
     
     # Process each page in the document
     if use_multithreading:
         # If multi-threading is enabled, process each page in a separate thread
         with ThreadPoolExecutor() as executor:
             futures = []
             for i, file_path in enumerate(files):
-                if exclude_pages is None or i+1 not in exclude_pages:
+                if config.exclude_pages is None or i+1 not in config.exclude_pages:
                     futures.append(executor.submit(
                         process_page, file_path, i+1))
 
             # Wait for all threads to complete and collect the results
             for future in futures:
                 result['pages'].append(future.result())
         
             # Sort the pages list by page number
         result['pages'] = sorted(result['pages'], key=lambda x: x['page'])
     else:
         # If multi-threading is disabled, process each page sequentially in the main thread
         for i, file_path in enumerate(files):
-            if exclude_pages is None or i+1 not in exclude_pages:
+            if config.exclude_pages is None or i+1 not in config.exclude_pages:
                 result['pages'].append(process_page(file_path, i+1))
 
     # Delete the extracted pages if the delete_extracted_pages flag is set
     if delete_split_pages:
         shutil.rmtree(target_dir)
 
     return result
```

### Comparing `insights-extractor-0.1.4/src/extractlib/document/table.py` & `insights-extractor-0.1.5/src/extractlib/document/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 
 
 def corrilate_table_data(table_elements, table_data):
     # Initialize an empty dictionary to store tables
     tables = {}
     
+    if not table_elements or not table_data:
+        return None
+
     # Iterate through each table in table_data
     tbl_idx = 0
     while tbl_idx < len(table_data):
         table = table_data[tbl_idx]
 
         # Iterate through each row in the table's JSON data
         row_idx = 0
@@ -65,15 +68,15 @@
                         col_idx += 1
                         break
 
             # Increment the row index
             row_idx += 1
 
         # If there are no more elements with 'table': 0, increment the table index
-        if not any(element.get('table') == 0 for element in table_elements):
+        if all(element.get('table') != 0 for element in table_elements):
             tbl_idx += 1
     
     # Sort the elements in each table by their row and column values
     sorted_tables = {key: sorted(tables[key], key=lambda x: (x['row'], x['column'])) for key in tables}
     
     # Return the sorted tables if table_elements is empty, otherwise return None
     return sorted_tables if not any(table_elements) else None
```

### Comparing `insights-extractor-0.1.4/src/extractlib/document/utils.py` & `insights-extractor-0.1.5/src/extractlib/document/utils.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.4/src/extractlib/ner/__init__.py` & `insights-extractor-0.1.5/src/extractlib/ner/__init__.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.4/src/extractlib/nlp/pre_process.py` & `insights-extractor-0.1.5/src/extractlib/nlp/pre_process.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.4/src/extractlib/utils/json_utils.py` & `insights-extractor-0.1.5/src/extractlib/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.4/src/insights_extractor.egg-info/PKG-INFO` & `insights-extractor-0.1.5/src/insights_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insights-extractor
-Version: 0.1.4
+Version: 0.1.5
 Summary: Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities.
 Author-email: Trae Moore <trae.dev@gmail.com>
 Project-URL: Homepage, https://github.com/traemoore/insights-extractor
 Project-URL: Tests, https://github.com/traemoore/insights-extractor-test
 Project-URL: Bug Tracker, https://github.com/traemoore/insights-extractor/issues
 Keywords: nltk,spaCy,Pymupdf,Camelot,OpenCV,Ghostscript,insight-extractor,pdf extraction,pdf data extraction,pdf data,classification,keyword extraction
 Classifier: Programming Language :: Python :: 3
```

### Comparing `insights-extractor-0.1.4/src/insights_extractor.egg-info/SOURCES.txt` & `insights-extractor-0.1.5/src/insights_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.4/tests/pre_process.py` & `insights-extractor-0.1.5/tests/pre_process.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.4/tests/prep_utils.py` & `insights-extractor-0.1.5/tests/prep_utils.py`

 * *Files identical despite different names*


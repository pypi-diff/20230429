# Comparing `tmp/openai-to-sqlite-0.2.tar.gz` & `tmp/openai-to-sqlite-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-to-sqlite-0.2.tar", last modified: Fri Jan 13 17:00:49 2023, max compression
+gzip compressed data, was "openai-to-sqlite-0.3.tar", last modified: Sat Apr 29 06:20:04 2023, max compression
```

## Comparing `openai-to-sqlite-0.2.tar` & `openai-to-sqlite-0.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 17:00:49.964858 openai-to-sqlite-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-13 17:00:29.000000 openai-to-sqlite-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-01-13 17:00:49.964858 openai-to-sqlite-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-01-13 17:00:29.000000 openai-to-sqlite-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 17:00:49.964858 openai-to-sqlite-0.2/openai_to_sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 17:00:29.000000 openai-to-sqlite-0.2/openai_to_sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-13 17:00:29.000000 openai-to-sqlite-0.2/openai_to_sqlite/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-01-13 17:00:29.000000 openai-to-sqlite-0.2/openai_to_sqlite/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 17:00:49.964858 openai-to-sqlite-0.2/openai_to_sqlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-01-13 17:00:49.000000 openai-to-sqlite-0.2/openai_to_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-01-13 17:00:49.000000 openai-to-sqlite-0.2/openai_to_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 17:00:49.000000 openai-to-sqlite-0.2/openai_to_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-13 17:00:49.000000 openai-to-sqlite-0.2/openai_to_sqlite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-13 17:00:49.000000 openai-to-sqlite-0.2/openai_to_sqlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-13 17:00:49.000000 openai-to-sqlite-0.2/openai_to_sqlite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 17:00:49.964858 openai-to-sqlite-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-01-13 17:00:29.000000 openai-to-sqlite-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:04.399422 openai-to-sqlite-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 06:19:44.000000 openai-to-sqlite-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-29 06:20:04.399422 openai-to-sqlite-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-04-29 06:19:44.000000 openai-to-sqlite-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:04.399422 openai-to-sqlite-0.3/openai_to_sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:44.000000 openai-to-sqlite-0.3/openai_to_sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-29 06:19:44.000000 openai-to-sqlite-0.3/openai_to_sqlite/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-04-29 06:19:44.000000 openai-to-sqlite-0.3/openai_to_sqlite/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:04.399422 openai-to-sqlite-0.3/openai_to_sqlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-29 06:20:04.000000 openai-to-sqlite-0.3/openai_to_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-29 06:20:04.000000 openai-to-sqlite-0.3/openai_to_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:20:04.000000 openai-to-sqlite-0.3/openai_to_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 06:20:04.000000 openai-to-sqlite-0.3/openai_to_sqlite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-29 06:20:04.000000 openai-to-sqlite-0.3/openai_to_sqlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-29 06:20:04.000000 openai-to-sqlite-0.3/openai_to_sqlite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 06:20:04.399422 openai-to-sqlite-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-29 06:19:44.000000 openai-to-sqlite-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:04.399422 openai-to-sqlite-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-29 06:19:44.000000 openai-to-sqlite-0.3/tests/test_openai_to_sqlite.py
```

### Comparing `openai-to-sqlite-0.2/LICENSE` & `openai-to-sqlite-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-to-sqlite-0.2/PKG-INFO` & `openai-to-sqlite-0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,18 @@
-Metadata-Version: 2.1
-Name: openai-to-sqlite
-Version: 0.2
-Summary: Save OpenAI API results to a SQLite database
-Home-page: https://github.com/simonw/openai-to-sqlite
-Author: Simon Willison
-License: Apache License, Version 2.0
-Project-URL: Issues, https://github.com/simonw/openai-to-sqlite/issues
-Project-URL: CI, https://github.com/simonw/openai-to-sqlite/actions
-Project-URL: Changelog, https://github.com/simonw/openai-to-sqlite/releases
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # openai-to-sqlite
 
 [![PyPI](https://img.shields.io/pypi/v/openai-to-sqlite.svg)](https://pypi.org/project/openai-to-sqlite/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/openai-to-sqlite?include_prereleases&label=changelog)](https://github.com/simonw/openai-to-sqlite/releases)
 [![Tests](https://github.com/simonw/openai-to-sqlite/workflows/Test/badge.svg)](https://github.com/simonw/openai-to-sqlite/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/openai-to-sqlite/blob/master/LICENSE)
 
 This tool provides utilities for interacting with OpenAI APIs and storing the results in a SQLite database.
 
+See [Semantic search answers: Q&A against documentation with GPT3 + OpenAI embeddings](https://simonwillison.net/2023/Jan/13/semantic-search-answers/) for background on this project.
+
 ## Installation
 
 Install this tool using `pip`:
 
     pip install openai-to-sqlite
 
 ## Configuration
@@ -36,14 +23,46 @@
 
 You can then either set the API key as an environment variable:
 
     export OPENAI_API_KEY=sk-...
 
 Or pass it to each command using the `--token sk-...` option.
 
+## Calling OpenAI APIs with SQL functions
+
+The `openai-to-sqlite query` command can be used to execute SQL queries that call OpenAI APIs.
+
+Functions available are:
+
+- `chatgpt(prompt)` - call the OpenAI Chat API using model `gpt-3.5-turbo` with the specified prompt.
+- `chatgpt(prompt, system)` - call that API with the prompt and the specified system prompt.
+
+More functions are planned in the future.
+
+Here's how to use this command to run basic sentiment analysis against content in a table:
+```
+openai-to-sqlite query database.db "
+  update messages set sentiment = chatgpt(
+    'Sentiment analysis for this message: ' || message ||
+    ' - ONLY return a lowercase string from: positive, negative, neutral, unknown'
+  )
+  where sentiment not in ('positive', 'negative', 'neutral', 'unknown')
+    or sentiment is null
+"
+```
+This updates the `sentiment` column in a table called `messages`. It populates it with the response from the specified prompt.
+
+The command will display a progress bar indicating how many rows are being processed.
+
+You can add an empty `sentiment` column to a table using [sqlite-utils](https://sqlite-utils.datasette.io/) like this:
+
+```
+sqlite-utils add-column database.db messages sentiment
+```
+
 ## Embeddings
 
 The `embeddings` command can be used to calculate and store [OpenAI embeddings](https://beta.openai.com/docs/guides/embeddings) for strings of text.
 
 Each embedding has a cost, so be sure to familiarize yourself with [the pricing](https://openai.com/api/pricing/) for the embedding model.
 
 The command can accept data in four different ways:
```

### Comparing `openai-to-sqlite-0.2/README.md` & `openai-to-sqlite-0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,33 @@
+Metadata-Version: 2.1
+Name: openai-to-sqlite
+Version: 0.3
+Summary: Save OpenAI API results to a SQLite database
+Home-page: https://github.com/simonw/openai-to-sqlite
+Author: Simon Willison
+License: Apache License, Version 2.0
+Project-URL: Issues, https://github.com/simonw/openai-to-sqlite/issues
+Project-URL: CI, https://github.com/simonw/openai-to-sqlite/actions
+Project-URL: Changelog, https://github.com/simonw/openai-to-sqlite/releases
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # openai-to-sqlite
 
 [![PyPI](https://img.shields.io/pypi/v/openai-to-sqlite.svg)](https://pypi.org/project/openai-to-sqlite/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/openai-to-sqlite?include_prereleases&label=changelog)](https://github.com/simonw/openai-to-sqlite/releases)
 [![Tests](https://github.com/simonw/openai-to-sqlite/workflows/Test/badge.svg)](https://github.com/simonw/openai-to-sqlite/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/openai-to-sqlite/blob/master/LICENSE)
 
 This tool provides utilities for interacting with OpenAI APIs and storing the results in a SQLite database.
 
+See [Semantic search answers: Q&A against documentation with GPT3 + OpenAI embeddings](https://simonwillison.net/2023/Jan/13/semantic-search-answers/) for background on this project.
+
 ## Installation
 
 Install this tool using `pip`:
 
     pip install openai-to-sqlite
 
 ## Configuration
@@ -21,14 +38,46 @@
 
 You can then either set the API key as an environment variable:
 
     export OPENAI_API_KEY=sk-...
 
 Or pass it to each command using the `--token sk-...` option.
 
+## Calling OpenAI APIs with SQL functions
+
+The `openai-to-sqlite query` command can be used to execute SQL queries that call OpenAI APIs.
+
+Functions available are:
+
+- `chatgpt(prompt)` - call the OpenAI Chat API using model `gpt-3.5-turbo` with the specified prompt.
+- `chatgpt(prompt, system)` - call that API with the prompt and the specified system prompt.
+
+More functions are planned in the future.
+
+Here's how to use this command to run basic sentiment analysis against content in a table:
+```
+openai-to-sqlite query database.db "
+  update messages set sentiment = chatgpt(
+    'Sentiment analysis for this message: ' || message ||
+    ' - ONLY return a lowercase string from: positive, negative, neutral, unknown'
+  )
+  where sentiment not in ('positive', 'negative', 'neutral', 'unknown')
+    or sentiment is null
+"
+```
+This updates the `sentiment` column in a table called `messages`. It populates it with the response from the specified prompt.
+
+The command will display a progress bar indicating how many rows are being processed.
+
+You can add an empty `sentiment` column to a table using [sqlite-utils](https://sqlite-utils.datasette.io/) like this:
+
+```
+sqlite-utils add-column database.db messages sentiment
+```
+
 ## Embeddings
 
 The `embeddings` command can be used to calculate and store [OpenAI embeddings](https://beta.openai.com/docs/guides/embeddings) for strings of text.
 
 Each embedding has a cost, so be sure to familiarize yourself with [the pricing](https://openai.com/api/pricing/) for the embedding model.
 
 The command can accept data in four different ways:
```

### Comparing `openai-to-sqlite-0.2/openai_to_sqlite.egg-info/PKG-INFO` & `openai-to-sqlite-0.3/openai_to_sqlite.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-to-sqlite
-Version: 0.2
+Version: 0.3
 Summary: Save OpenAI API results to a SQLite database
 Home-page: https://github.com/simonw/openai-to-sqlite
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/openai-to-sqlite/issues
 Project-URL: CI, https://github.com/simonw/openai-to-sqlite/actions
 Project-URL: Changelog, https://github.com/simonw/openai-to-sqlite/releases
@@ -18,14 +18,16 @@
 [![PyPI](https://img.shields.io/pypi/v/openai-to-sqlite.svg)](https://pypi.org/project/openai-to-sqlite/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/openai-to-sqlite?include_prereleases&label=changelog)](https://github.com/simonw/openai-to-sqlite/releases)
 [![Tests](https://github.com/simonw/openai-to-sqlite/workflows/Test/badge.svg)](https://github.com/simonw/openai-to-sqlite/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/openai-to-sqlite/blob/master/LICENSE)
 
 This tool provides utilities for interacting with OpenAI APIs and storing the results in a SQLite database.
 
+See [Semantic search answers: Q&A against documentation with GPT3 + OpenAI embeddings](https://simonwillison.net/2023/Jan/13/semantic-search-answers/) for background on this project.
+
 ## Installation
 
 Install this tool using `pip`:
 
     pip install openai-to-sqlite
 
 ## Configuration
@@ -36,14 +38,46 @@
 
 You can then either set the API key as an environment variable:
 
     export OPENAI_API_KEY=sk-...
 
 Or pass it to each command using the `--token sk-...` option.
 
+## Calling OpenAI APIs with SQL functions
+
+The `openai-to-sqlite query` command can be used to execute SQL queries that call OpenAI APIs.
+
+Functions available are:
+
+- `chatgpt(prompt)` - call the OpenAI Chat API using model `gpt-3.5-turbo` with the specified prompt.
+- `chatgpt(prompt, system)` - call that API with the prompt and the specified system prompt.
+
+More functions are planned in the future.
+
+Here's how to use this command to run basic sentiment analysis against content in a table:
+```
+openai-to-sqlite query database.db "
+  update messages set sentiment = chatgpt(
+    'Sentiment analysis for this message: ' || message ||
+    ' - ONLY return a lowercase string from: positive, negative, neutral, unknown'
+  )
+  where sentiment not in ('positive', 'negative', 'neutral', 'unknown')
+    or sentiment is null
+"
+```
+This updates the `sentiment` column in a table called `messages`. It populates it with the response from the specified prompt.
+
+The command will display a progress bar indicating how many rows are being processed.
+
+You can add an empty `sentiment` column to a table using [sqlite-utils](https://sqlite-utils.datasette.io/) like this:
+
+```
+sqlite-utils add-column database.db messages sentiment
+```
+
 ## Embeddings
 
 The `embeddings` command can be used to calculate and store [OpenAI embeddings](https://beta.openai.com/docs/guides/embeddings) for strings of text.
 
 Each embedding has a cost, so be sure to familiarize yourself with [the pricing](https://openai.com/api/pricing/) for the embedding model.
 
 The command can accept data in four different ways:
```

### Comparing `openai-to-sqlite-0.2/setup.py` & `openai-to-sqlite-0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.2"
+VERSION = "0.3"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -27,11 +27,11 @@
     license="Apache License, Version 2.0",
     version=VERSION,
     packages=["openai_to_sqlite"],
     entry_points="""
         [console_scripts]
         openai-to-sqlite=openai_to_sqlite.cli:cli
     """,
-    install_requires=["click", "httpx", "sqlite-utils>=3.28"],
-    extras_require={"test": ["pytest", "pytest-httpx"]},
+    install_requires=["click", "httpx", "sqlite-utils>=3.28", "openai"],
+    extras_require={"test": ["pytest", "pytest-httpx", "pytest-mock"]},
     python_requires=">=3.7",
 )
```


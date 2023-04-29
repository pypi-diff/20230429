# Comparing `tmp/gTTS-2.3.1.tar.gz` & `tmp/gTTS-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gTTS-2.3.1.tar", last modified: Mon Jan 16 07:40:42 2023, max compression
+gzip compressed data, was "gTTS-2.3.2.tar", last modified: Sat Apr 29 06:21:05 2023, max compression
```

## Comparing `gTTS-2.3.1.tar` & `gTTS-2.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 07:40:42.739301 gTTS-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-01-16 07:40:27.000000 gTTS-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-01-16 07:40:42.739301 gTTS-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-01-16 07:40:27.000000 gTTS-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 07:40:42.731301 gTTS-2.3.1/gTTS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-01-16 07:40:42.000000 gTTS-2.3.1/gTTS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-01-16 07:40:42.000000 gTTS-2.3.1/gTTS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 07:40:42.000000 gTTS-2.3.1/gTTS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-16 07:40:42.000000 gTTS-2.3.1/gTTS.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-16 07:40:42.000000 gTTS-2.3.1/gTTS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-16 07:40:42.000000 gTTS-2.3.1/gTTS.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 07:40:42.735301 gTTS-2.3.1/gtts/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/accents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/langs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 07:40:42.735301 gTTS-2.3.1/gtts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 07:40:42.735301 gTTS-2.3.1/gtts/tests/input_files/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tests/input_files/test_cli_test_ascii.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tests/input_files/test_cli_test_utf8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tests/test_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tests/test_tts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 07:40:42.735301 gTTS-2.3.1/gtts/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tokenizer/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tokenizer/pre_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tokenizer/symbols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 07:40:42.739301 gTTS-2.3.1/gtts/tokenizer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tokenizer/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tokenizer/tests/test_pre_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tokenizer/tests/test_tokenizer_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tokenizer/tokenizer_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/tts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-16 07:40:27.000000 gTTS-2.3.1/gtts/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-01-16 07:40:27.000000 gTTS-2.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 07:40:42.739301 gTTS-2.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:05.493319 gTTS-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-29 06:20:51.000000 gTTS-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-29 06:21:05.493319 gTTS-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-29 06:20:51.000000 gTTS-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:05.485319 gTTS-2.3.2/gTTS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-29 06:21:05.000000 gTTS-2.3.2/gTTS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-29 06:21:05.000000 gTTS-2.3.2/gTTS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:21:05.000000 gTTS-2.3.2/gTTS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-29 06:21:05.000000 gTTS-2.3.2/gTTS.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-29 06:21:05.000000 gTTS-2.3.2/gTTS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 06:21:05.000000 gTTS-2.3.2/gTTS.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:05.489319 gTTS-2.3.2/gtts/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/accents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/langs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:05.489319 gTTS-2.3.2/gtts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:05.489319 gTTS-2.3.2/gtts/tests/input_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tests/input_files/test_cli_test_ascii.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tests/input_files/test_cli_test_utf8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tests/test_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tests/test_tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:05.493319 gTTS-2.3.2/gtts/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tokenizer/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tokenizer/pre_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tokenizer/symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:05.493319 gTTS-2.3.2/gtts/tokenizer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tokenizer/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tokenizer/tests/test_pre_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tokenizer/tests/test_tokenizer_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tokenizer/tokenizer_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 06:20:51.000000 gTTS-2.3.2/gtts/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-29 06:20:51.000000 gTTS-2.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 06:21:05.493319 gTTS-2.3.2/setup.cfg
```

### Comparing `gTTS-2.3.1/LICENSE` & `gTTS-2.3.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright © 2014-2022 Pierre Nicolas Durette
+Copyright © 2014-2023 Pierre Nicolas Durette
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `gTTS-2.3.1/PKG-INFO` & `gTTS-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gTTS
-Version: 2.3.1
+Version: 2.3.2
 Summary: gTTS (Google Text-to-Speech), a Python library and CLI tool to interface with Google Translate text-to-speech API
 Author-email: Pierre Nicolas Durette <pndurette@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/pndurette/gTTS
 Project-URL: documentation, https://gtts.readthedocs.io
 Project-URL: repository, https://github.com/pndurette/gTTS
 Project-URL: changelog, https://github.com/pndurette/gTTS/blob/main/CHANGELOG.md
@@ -75,8 +75,8 @@
 
 -   [Questions & community](https://github.com/pndurette/gTTS/discussions)
 -   [Changelog](CHANGELOG.rst)
 -   [Contributing](CONTRIBUTING.rst)
 
 ### Licence
 
-[The MIT License (MIT)](LICENSE) Copyright © 2014-2022 Pierre Nicolas Durette & [Contributors](https://github.com/pndurette/gTTS/graphs/contributors)
+[The MIT License (MIT)](LICENSE) Copyright © 2014-2023 Pierre Nicolas Durette & [Contributors](https://github.com/pndurette/gTTS/graphs/contributors)
```

### Comparing `gTTS-2.3.1/README.md` & `gTTS-2.3.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
 -   [Questions & community](https://github.com/pndurette/gTTS/discussions)
 -   [Changelog](CHANGELOG.rst)
 -   [Contributing](CONTRIBUTING.rst)
 
 ### Licence
 
-[The MIT License (MIT)](LICENSE) Copyright © 2014-2022 Pierre Nicolas Durette & [Contributors](https://github.com/pndurette/gTTS/graphs/contributors)
+[The MIT License (MIT)](LICENSE) Copyright © 2014-2023 Pierre Nicolas Durette & [Contributors](https://github.com/pndurette/gTTS/graphs/contributors)
```

### Comparing `gTTS-2.3.1/gTTS.egg-info/PKG-INFO` & `gTTS-2.3.2/gTTS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gTTS
-Version: 2.3.1
+Version: 2.3.2
 Summary: gTTS (Google Text-to-Speech), a Python library and CLI tool to interface with Google Translate text-to-speech API
 Author-email: Pierre Nicolas Durette <pndurette@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/pndurette/gTTS
 Project-URL: documentation, https://gtts.readthedocs.io
 Project-URL: repository, https://github.com/pndurette/gTTS
 Project-URL: changelog, https://github.com/pndurette/gTTS/blob/main/CHANGELOG.md
@@ -75,8 +75,8 @@
 
 -   [Questions & community](https://github.com/pndurette/gTTS/discussions)
 -   [Changelog](CHANGELOG.rst)
 -   [Contributing](CONTRIBUTING.rst)
 
 ### Licence
 
-[The MIT License (MIT)](LICENSE) Copyright © 2014-2022 Pierre Nicolas Durette & [Contributors](https://github.com/pndurette/gTTS/graphs/contributors)
+[The MIT License (MIT)](LICENSE) Copyright © 2014-2023 Pierre Nicolas Durette & [Contributors](https://github.com/pndurette/gTTS/graphs/contributors)
```

### Comparing `gTTS-2.3.1/gTTS.egg-info/SOURCES.txt` & `gTTS-2.3.2/gTTS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/gtts/accents.py` & `gTTS-2.3.2/gtts/accents.py`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/gtts/cli.py` & `gTTS-2.3.2/gtts/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 from gtts import gTTS, gTTSError, __version__
-from gtts.lang import tts_langs
+from gtts.lang import tts_langs, _fallback_deprecated_lang
 import click
 import logging
 import logging.config
 
 # Click settings
 CONTEXT_SETTINGS = {"help_option_names": ["-h", "--help"]}
 
@@ -42,14 +42,17 @@
 def validate_lang(ctx, param, lang):
     """Validation callback for the <lang> option.
     Ensures <lang> is a supported language unless the <nocheck> flag is set
     """
     if ctx.params["nocheck"]:
         return lang
 
+    # Fallback from deprecated language if needed
+    lang = _fallback_deprecated_lang(lang)
+
     try:
         if lang not in tts_langs():
             raise click.UsageError(
                 "'%s' not in list of supported languages.\n"
                 "Use --all to list languages or "
                 "add --nocheck to disable language check." % lang
             )
```

### Comparing `gTTS-2.3.1/gtts/lang.py` & `gTTS-2.3.2/gtts/lang.py`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/gtts/langs.py` & `gTTS-2.3.2/gtts/langs.py`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/gtts/tests/test_cli.py` & `gTTS-2.3.2/gtts/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/gtts/tests/test_lang.py` & `gTTS-2.3.2/gtts/tests/test_lang.py`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/gtts/tests/test_tts.py` & `gTTS-2.3.2/gtts/tests/test_tts.py`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/gtts/tests/test_utils.py` & `gTTS-2.3.2/gtts/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/gtts/tokenizer/core.py` & `gTTS-2.3.2/gtts/tokenizer/core.py`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/gtts/tokenizer/pre_processors.py` & `gTTS-2.3.2/gtts/tokenizer/pre_processors.py`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/gtts/tokenizer/tests/test_core.py` & `gTTS-2.3.2/gtts/tokenizer/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/gtts/tokenizer/tests/test_pre_processors.py` & `gTTS-2.3.2/gtts/tokenizer/tests/test_pre_processors.py`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/gtts/tokenizer/tests/test_tokenizer_cases.py` & `gTTS-2.3.2/gtts/tokenizer/tests/test_tokenizer_cases.py`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/gtts/tokenizer/tokenizer_cases.py` & `gTTS-2.3.2/gtts/tokenizer/tokenizer_cases.py`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/gtts/tts.py` & `gTTS-2.3.2/gtts/tts.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     Args:
         text (string): The text to be read.
         tld (string): Top-level domain for the Google Translate host,
             i.e `https://translate.google.<tld>`. Different Google domains
             can produce different localized 'accents' for a given
             language. This is also useful when ``google.com`` might be blocked
             within a network but a local or different Google host
-            (e.g. ``google.cn``) is not. Default is ``com``.
+            (e.g. ``google.com.hk``) is not. Default is ``com``.
         lang (string, optional): The language (IETF language tag) to
             read the text in. Default is ``en``.
         slow (bool, optional): Reads text more slowly. Defaults to ``False``.
         lang_check (bool, optional): Strictly enforce an existing ``lang``,
             to catch a language error early. If set to ``True``,
             a ``ValueError`` is raised if ``lang`` doesn't exist.
             Setting ``lang_check`` to ``False`` skips Web requests
@@ -360,14 +360,16 @@
             status = rsp.status_code
             reason = rsp.reason
 
             premise = "{:d} ({}) from TTS API".format(status, reason)
 
             if status == 403:
                 cause = "Bad token or upstream API changes"
+            elif status == 404 and tts.tld != "com":
+                cause = "Unsupported tld '{}'".format(tts.tld)
             elif status == 200 and not tts.lang_check:
                 cause = (
                     "No audio stream in response. Unsupported language '%s'"
                     % self.tts.lang
                 )
             elif status >= 500:
                 cause = "Uptream API error. Try again later."
```

### Comparing `gTTS-2.3.1/gtts/utils.py` & `gTTS-2.3.2/gtts/utils.py`

 * *Files identical despite different names*

### Comparing `gTTS-2.3.1/pyproject.toml` & `gTTS-2.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gTTS"
-version = "2.3.1"
+version = "2.3.2"
 description = "gTTS (Google Text-to-Speech), a Python library and CLI tool to interface with Google Translate text-to-speech API"
 authors = [{name = "Pierre Nicolas Durette", email = "pndurette@gmail.com"}]
 requires-python = ">=3.7"
 readme = "README.md"
 license = {text = "MIT"}
 keywords = [
     "gtts",
```


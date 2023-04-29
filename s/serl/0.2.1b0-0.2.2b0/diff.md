# Comparing `tmp/serl-0.2.1b0.tar.gz` & `tmp/serl-0.2.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serl-0.2.1b0.tar", last modified: Thu Apr 27 13:39:34 2023, max compression
+gzip compressed data, was "serl-0.2.2b0.tar", last modified: Sat Apr 29 17:36:04 2023, max compression
```

## Comparing `serl-0.2.1b0.tar` & `serl-0.2.2b0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 13:39:34.700956 serl-0.2.1b0/
--rw-rw-rw-   0        0        0     1091 2023-03-30 16:03:47.000000 serl-0.2.1b0/LICENSE
--rw-rw-rw-   0        0        0     2294 2023-04-27 13:39:34.700956 serl-0.2.1b0/PKG-INFO
--rw-rw-rw-   0        0        0      652 2023-04-27 13:33:45.000000 serl-0.2.1b0/README.md
--rw-rw-rw-   0        0        0       84 2023-03-30 16:03:47.000000 serl-0.2.1b0/pyproject.toml
--rw-rw-rw-   0        0        0      897 2023-04-27 13:39:34.708213 serl-0.2.1b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 13:39:34.602521 serl-0.2.1b0/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 13:39:34.665261 serl-0.2.1b0/src/serl/
--rw-rw-rw-   0        0        0        0 2023-03-30 16:03:47.000000 serl-0.2.1b0/src/serl/__init__.py
--rw-rw-rw-   0        0        0       74 2023-03-30 16:03:47.000000 serl-0.2.1b0/src/serl/__main__.py
--rw-rw-rw-   0        0        0     2726 2023-04-17 21:26:43.000000 serl-0.2.1b0/src/serl/config.py
--rw-rw-rw-   0        0        0     3691 2023-04-27 13:38:14.000000 serl-0.2.1b0/src/serl/constants.py
--rw-rw-rw-   0        0        0     3820 2023-04-26 14:50:50.000000 serl-0.2.1b0/src/serl/highlight.py
--rw-rw-rw-   0        0        0     3731 2023-04-26 14:18:07.000000 serl-0.2.1b0/src/serl/lexer.py
--rw-rw-rw-   0        0        0     3359 2023-04-17 20:35:29.000000 serl-0.2.1b0/src/serl/logger.py
--rw-rw-rw-   0        0        0    18751 2023-04-27 13:20:48.000000 serl-0.2.1b0/src/serl/main.py
--rw-rw-rw-   0        0        0     4893 2023-04-27 13:16:35.000000 serl-0.2.1b0/src/serl/parser.py
--rw-rw-rw-   0        0        0     2933 2023-04-21 14:34:29.000000 serl-0.2.1b0/src/serl/schema.py
--rw-rw-rw-   0        0        0     4819 2023-04-27 13:25:04.000000 serl-0.2.1b0/src/serl/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:39:34.689372 serl-0.2.1b0/src/serl.egg-info/
--rw-rw-rw-   0        0        0     2294 2023-04-27 13:39:34.000000 serl-0.2.1b0/src/serl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-04-27 13:39:34.000000 serl-0.2.1b0/src/serl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 13:39:34.000000 serl-0.2.1b0/src/serl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-27 13:39:34.000000 serl-0.2.1b0/src/serl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2023-04-27 13:39:34.000000 serl-0.2.1b0/src/serl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-27 13:39:34.000000 serl-0.2.1b0/src/serl.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 13:39:34.699895 serl-0.2.1b0/tests/
--rw-rw-rw-   0        0        0      572 2023-04-17 18:50:19.000000 serl-0.2.1b0/tests/test_config.py
--rw-rw-rw-   0        0        0      807 2023-04-04 06:33:54.000000 serl-0.2.1b0/tests/test_highlight.py
--rw-rw-rw-   0        0        0     2156 2023-04-26 14:06:44.000000 serl-0.2.1b0/tests/test_lexer.py
--rw-rw-rw-   0        0        0     4461 2023-04-20 22:48:18.000000 serl-0.2.1b0/tests/test_main.py
--rw-rw-rw-   0        0        0     2390 2023-04-17 18:00:20.000000 serl-0.2.1b0/tests/test_parser.py
--rw-rw-rw-   0        0        0     1896 2023-04-17 08:06:23.000000 serl-0.2.1b0/tests/test_schema.py
--rw-rw-rw-   0        0        0     5486 2023-04-25 06:59:43.000000 serl-0.2.1b0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:36:04.767347 serl-0.2.2b0/
+-rw-rw-rw-   0        0        0     1091 2023-03-30 16:03:47.000000 serl-0.2.2b0/LICENSE
+-rw-rw-rw-   0        0        0     2294 2023-04-29 17:36:04.767347 serl-0.2.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0      652 2023-04-27 13:33:45.000000 serl-0.2.2b0/README.md
+-rw-rw-rw-   0        0        0       84 2023-03-30 16:03:47.000000 serl-0.2.2b0/pyproject.toml
+-rw-rw-rw-   0        0        0      897 2023-04-29 17:36:04.774681 serl-0.2.2b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 17:36:04.651546 serl-0.2.2b0/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 17:36:04.715644 serl-0.2.2b0/src/serl/
+-rw-rw-rw-   0        0        0        0 2023-03-30 16:03:47.000000 serl-0.2.2b0/src/serl/__init__.py
+-rw-rw-rw-   0        0        0       74 2023-03-30 16:03:47.000000 serl-0.2.2b0/src/serl/__main__.py
+-rw-rw-rw-   0        0        0     2726 2023-04-17 21:26:43.000000 serl-0.2.2b0/src/serl/config.py
+-rw-rw-rw-   0        0        0     3691 2023-04-29 17:34:44.000000 serl-0.2.2b0/src/serl/constants.py
+-rw-rw-rw-   0        0        0     3768 2023-04-28 08:16:32.000000 serl-0.2.2b0/src/serl/highlight.py
+-rw-rw-rw-   0        0        0     3731 2023-04-26 14:18:07.000000 serl-0.2.2b0/src/serl/lexer.py
+-rw-rw-rw-   0        0        0     3359 2023-04-17 20:35:29.000000 serl-0.2.2b0/src/serl/logger.py
+-rw-rw-rw-   0        0        0    18751 2023-04-27 13:50:07.000000 serl-0.2.2b0/src/serl/main.py
+-rw-rw-rw-   0        0        0     4893 2023-04-27 13:16:35.000000 serl-0.2.2b0/src/serl/parser.py
+-rw-rw-rw-   0        0        0     2933 2023-04-21 14:34:29.000000 serl-0.2.2b0/src/serl/schema.py
+-rw-rw-rw-   0        0        0     4819 2023-04-27 13:25:04.000000 serl-0.2.2b0/src/serl/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:36:04.748816 serl-0.2.2b0/src/serl.egg-info/
+-rw-rw-rw-   0        0        0     2294 2023-04-29 17:36:04.000000 serl-0.2.2b0/src/serl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-04-29 17:36:04.000000 serl-0.2.2b0/src/serl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 17:36:04.000000 serl-0.2.2b0/src/serl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-29 17:36:04.000000 serl-0.2.2b0/src/serl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2023-04-29 17:36:04.000000 serl-0.2.2b0/src/serl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-29 17:36:04.000000 serl-0.2.2b0/src/serl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 17:36:04.765060 serl-0.2.2b0/tests/
+-rw-rw-rw-   0        0        0      572 2023-04-17 18:50:19.000000 serl-0.2.2b0/tests/test_config.py
+-rw-rw-rw-   0        0        0      807 2023-04-04 06:33:54.000000 serl-0.2.2b0/tests/test_highlight.py
+-rw-rw-rw-   0        0        0     2156 2023-04-26 14:06:44.000000 serl-0.2.2b0/tests/test_lexer.py
+-rw-rw-rw-   0        0        0     4461 2023-04-20 22:48:18.000000 serl-0.2.2b0/tests/test_main.py
+-rw-rw-rw-   0        0        0     2390 2023-04-17 18:00:20.000000 serl-0.2.2b0/tests/test_parser.py
+-rw-rw-rw-   0        0        0     1896 2023-04-17 08:06:23.000000 serl-0.2.2b0/tests/test_schema.py
+-rw-rw-rw-   0        0        0     5486 2023-04-25 06:59:43.000000 serl-0.2.2b0/tests/test_utils.py
```

### Comparing `serl-0.2.1b0/LICENSE` & `serl-0.2.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/PKG-INFO` & `serl-0.2.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serl
-Version: 0.2.1b0
+Version: 0.2.2b0
 Summary: Serialized Language (serl)
 Author: Harry Downing
 Author-email: harry.downing17@gmail.com
 License: MIT
 Project-URL: Repository, https://github.com/harrydowning/serl
 Project-URL: Documentation, https://serl.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
```

### Comparing `serl-0.2.1b0/README.md` & `serl-0.2.2b0/README.md`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/setup.cfg` & `serl-0.2.2b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/src/serl/config.py` & `serl-0.2.2b0/src/serl/config.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/src/serl/constants.py` & `serl-0.2.2b0/src/serl/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 NAME = __package__
-VERSION = '0.2.1-beta'
+VERSION = '0.2.2-beta'
 
 SYSTEM_CONFIG_DIR = f'.{NAME}'
 SYSTEM_CONFIG_ENV_DIR = 'environments'
 SHELL_CHAR = '$'
 VENV_CONFIG = 'pyvenv.cfg'
 EXCEPTION_ATTR = 'serl_loc'
```

### Comparing `serl-0.2.1b0/src/serl/highlight.py` & `serl-0.2.2b0/src/serl/highlight.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from pygments.style import Style, StyleMeta
 from pygments.util import ClassNotFound
 from pygments.lexer import RegexLexer
 from pygments.token import string_to_tokentype, Token, Comment, Whitespace
 from pygments.formatters import get_formatter_by_name
 from pygments.styles import get_style_by_name
 
-# SerlToken = string_to_tokentype('Token.Serl')
+SerlToken = string_to_tokentype('Token.Serl')
 def get_pygments_lexer(_tokens: dict, ignore: str, tokentypes: dict):
     tokentypes = {t: ttype.title() for t, ttype in tokentypes.items()}
     class PygmentsLexer(RegexLexer):
         flags = re.VERBOSE
 
         tokens = {
             'root': [
                 (_tokens.get(name_or_pattern, name_or_pattern), 
                  string_to_tokentype(ttype)) 
                 for name_or_pattern, ttype in tokentypes.items()
             ] + [(r'\s', Whitespace)]
         }
         if ignore:
             tokens['root'].append((ignore, Comment))
-        # tokens['root'].append(('.', SerlToken))
+        tokens['root'].append(('.', SerlToken))
     try:
         return PygmentsLexer()
     except ValueError as err:
         logger.error(f'Syntax highlighter lexer error: {err}', code=1)
 
 def get_pygments_style(style: StyleMeta, user_styles: dict[str, str]):
     attrs = {
@@ -38,15 +38,15 @@
         if not attr.startswith('_')
     }
 
     attrs['styles'] = attrs.get('styles', {}) | {
         string_to_tokentype(tokentype.title()): user_style
         for tokentype, user_style in user_styles.items()
     }
-    # attrs['styles'][SerlToken] = attrs['styles'][Token]
+    attrs['styles'][SerlToken] = attrs['styles'][Token]
     # Create class with type(...) to allow dynamic creation of attrs
     PygmentsStyle = type('PygmentsStyle', (Style,), attrs)
     return PygmentsStyle
 
 def parse_key_value(input: str) -> dict:
     result = {}
     str_re = r'(?s)([\'\"])(.*?)\1'
@@ -77,24 +77,23 @@
     return result
 
 def get_pygments_output(src: str, tokens: dict[str, str], ignore: str, 
                        tokentypes: dict[str, str], user_styles: dict[str, str],
                        format: str, format_options: dict, style_defs_arg):
     lexer = get_pygments_lexer(tokens, ignore, tokentypes)
     
-    style_name = format_options.get('style', None)
-    if style_name:
-        try:
-            style = get_style_by_name(style_name)
-        except ClassNotFound:
-            logger.warning(f'No Pygment style found for \'{style_name}\'. '
-                           f'Default will be used.')
-            style = get_style_by_name('default')
-        
-        format_options['style'] = get_pygments_style(style, user_styles)
+    style_name = format_options.get('style', 'default')
+    try:
+        style = get_style_by_name(style_name)
+    except ClassNotFound:
+        logger.warning(f'No Pygment style found for \'{style_name}\'. '
+                        f'Default will be used.')
+        style = get_style_by_name('default')
+    
+    format_options['style'] = get_pygments_style(style, user_styles)
 
     try:
         formatter = get_formatter_by_name(format, **format_options)
     except ClassNotFound:
         logger.error(f'No Pygment formmatter found for \'{format}\'.', code=1)
     
     try:
```

### Comparing `serl-0.2.1b0/src/serl/lexer.py` & `serl-0.2.2b0/src/serl/lexer.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/src/serl/logger.py` & `serl-0.2.2b0/src/serl/logger.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/src/serl/main.py` & `serl-0.2.2b0/src/serl/main.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/src/serl/parser.py` & `serl-0.2.2b0/src/serl/parser.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/src/serl/schema.py` & `serl-0.2.2b0/src/serl/schema.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/src/serl/utils.py` & `serl-0.2.2b0/src/serl/utils.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/src/serl.egg-info/PKG-INFO` & `serl-0.2.2b0/src/serl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serl
-Version: 0.2.1b0
+Version: 0.2.2b0
 Summary: Serialized Language (serl)
 Author: Harry Downing
 Author-email: harry.downing17@gmail.com
 License: MIT
 Project-URL: Repository, https://github.com/harrydowning/serl
 Project-URL: Documentation, https://serl.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
```

### Comparing `serl-0.2.1b0/src/serl.egg-info/SOURCES.txt` & `serl-0.2.2b0/src/serl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/tests/test_config.py` & `serl-0.2.2b0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/tests/test_highlight.py` & `serl-0.2.2b0/tests/test_highlight.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/tests/test_lexer.py` & `serl-0.2.2b0/tests/test_lexer.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/tests/test_main.py` & `serl-0.2.2b0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/tests/test_parser.py` & `serl-0.2.2b0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/tests/test_schema.py` & `serl-0.2.2b0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.1b0/tests/test_utils.py` & `serl-0.2.2b0/tests/test_utils.py`

 * *Files identical despite different names*


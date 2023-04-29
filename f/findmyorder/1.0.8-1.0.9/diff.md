# Comparing `tmp/findmyorder-1.0.8.tar.gz` & `tmp/findmyorder-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.0.8.tar", max compression
+gzip compressed data, was "findmyorder-1.0.9.tar", max compression
```

## Comparing `findmyorder-1.0.8.tar` & `findmyorder-1.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-27 06:57:13.622135 findmyorder-1.0.8/LICENSE
--rw-r--r--   0        0        0     1426 2023-04-27 06:57:13.622135 findmyorder-1.0.8/README.md
--rw-r--r--   0        0        0      106 2023-04-27 06:57:14.362153 findmyorder-1.0.8/findmyorder/__init__.py
--rw-r--r--   0        0        0      723 2023-04-27 06:57:13.622135 findmyorder-1.0.8/findmyorder/config.py
--rw-r--r--   0        0        0      120 2023-04-27 06:57:13.622135 findmyorder-1.0.8/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     3409 2023-04-27 06:57:13.622135 findmyorder-1.0.8/findmyorder/main.py
--rw-r--r--   0        0        0     1194 2023-04-27 06:57:14.362153 findmyorder-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 findmyorder-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-27 08:02:56.393167 findmyorder-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1426 2023-04-27 08:02:56.393167 findmyorder-1.0.9/README.md
+-rw-r--r--   0        0        0      106 2023-04-27 08:02:57.129178 findmyorder-1.0.9/findmyorder/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-27 08:02:56.393167 findmyorder-1.0.9/findmyorder/config.py
+-rw-r--r--   0        0        0      120 2023-04-27 08:02:56.393167 findmyorder-1.0.9/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     3322 2023-04-27 08:02:56.393167 findmyorder-1.0.9/findmyorder/main.py
+-rw-r--r--   0        0        0     1213 2023-04-27 08:02:57.125178 findmyorder-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 findmyorder-1.0.9/PKG-INFO
```

### Comparing `findmyorder-1.0.8/LICENSE` & `findmyorder-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.8/README.md` & `findmyorder-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.8/findmyorder/config.py` & `findmyorder-1.0.9/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.8/findmyorder/main.py` & `findmyorder-1.0.9/findmyorder/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio, logging, re
 from datetime import datetime
 
 from findmyorder.config import settings
 
-from pyparsing import Word, alphas, nums, oneOf, Optional, Regex, Suppress, LineEnd, Group, delimitedList
+from pyparsing import one_of, Word, alphas, Regex, Optional
 
 
 class findmyorder:
 
     def __init__(self,
                  ):
         self.logger =  logging.getLogger(__name__)
@@ -28,15 +28,15 @@
         self.logger.debug(f"error search {e}")
         return False
 
     def identify_order(self,mystring: str = None,):
       self.logger.debug(f"identify_order for {mystring}")
       try:
         #parsing
-        action = oneOf("BUY SELL LONG SHORT")
+        action = oneOf(strs="BUY SELL LONG SHORT",caseless=True)
         currency_pair = Word(alphas, exact=6)
         market = Optional(Word(alphas, exact=4))
         percentage = Regex(r'\d+(\.\d+)?%')
         # quantity = Regex(r'\d+(\.\d+)?')('quantity')
         # stop_loss = Regex(r'sl=\d+')['stop_loss']
         # take_profit1 = Regex(r'tp1=\d+')['take_profit1']
         # take_profit2 = Regex(r'tp2=\d+')['take_profit2']
@@ -46,15 +46,15 @@
         #order grammar
         order_grammar = action('action') + currency_pair('currency_pair') + percentage('percentage') 
                         # + Optional(quantity)
                         # + Optional(stop_loss) 
                         # + Optional(take_profit1) 
                         # + Optional(take_profit2)  
                         # + Optional(comment)
-        self.logger.debug(f"order_grammar  {order_grammar}")
+
         result = order_grammar.parseString(mystring)
         self.logger.debug(f"identify_order result {result}")
         return results
 
 
       except Exception as e:
           self.logger.debug(f"error identify_order {e}")
```

### Comparing `findmyorder-1.0.8/pyproject.toml` & `findmyorder-1.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.0.8"
+version = "1.0.9"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 
 
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/findmyorder/discussions"
 "Issues" =  "https://github.com/mraniki/findmyorder/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
-asyncio = "*"
-dynaconf = "*"
-pyparsing = "*"
+asyncio = ">=3.4.3"
+dynaconf = ">=3.1.12"
+pyparsing = ">=3.0.9"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
 python_classes = [
```

### Comparing `findmyorder-1.0.8/PKG-INFO` & `findmyorder-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: asyncio
-Requires-Dist: dynaconf
-Requires-Dist: pyparsing
+Requires-Dist: asyncio (>=3.4.3)
+Requires-Dist: dynaconf (>=3.1.12)
+Requires-Dist: pyparsing (>=3.0.9)
 Project-URL: Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
 Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
 Description-Content-Type: text/markdown
 
 # Find my order.
```


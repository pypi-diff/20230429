# Comparing `tmp/SnakeMD-2.0.0b2.tar.gz` & `tmp/snakemd-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SnakeMD-2.0.0b2.tar", last modified: Mon Apr 10 17:10:39 2023, max compression
+gzip compressed data, was "snakemd-2.1.0.tar", max compression
```

## Comparing `SnakeMD-2.0.0b2.tar` & `snakemd-2.1.0.tar`

### file list

```diff
@@ -1,29 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:39.686669 SnakeMD-2.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-04-10 17:10:39.682669 SnakeMD-2.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:39.682669 SnakeMD-2.0.0b2/SnakeMD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-04-10 17:10:39.000000 SnakeMD-2.0.0b2/SnakeMD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-10 17:10:39.000000 SnakeMD-2.0.0b2/SnakeMD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:10:39.000000 SnakeMD-2.0.0b2/SnakeMD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 17:10:39.000000 SnakeMD-2.0.0b2/SnakeMD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:10:39.686669 SnakeMD-2.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:39.682669 SnakeMD-2.0.0b2/snakemd/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/snakemd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/snakemd/document.py
--rw-r--r--   0 runner    (1001) docker     (123)    39935 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/snakemd/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/snakemd/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:39.682669 SnakeMD-2.0.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_heading.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_horizontal_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_md_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_paragraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-10 17:10:27.000000 SnakeMD-2.0.0b2/tests/test_table_of_contents.py
+-rw-r--r--   0        0        0     1071 2023-04-29 18:06:06.129025 snakemd-2.1.0/LICENSE
+-rw-r--r--   0        0        0     7060 2023-04-29 18:06:06.129025 snakemd-2.1.0/README.md
+-rw-r--r--   0        0        0     1414 2023-04-29 18:06:06.133025 snakemd-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      594 2023-04-29 18:06:06.133025 snakemd-2.1.0/snakemd/__init__.py
+-rw-r--r--   0        0        0    13530 2023-04-29 18:06:06.133025 snakemd-2.1.0/snakemd/document.py
+-rw-r--r--   0        0        0    40086 2023-04-29 18:06:06.133025 snakemd-2.1.0/snakemd/elements.py
+-rw-r--r--   0        0        0     3319 2023-04-29 18:06:06.133025 snakemd-2.1.0/snakemd/templates.py
+-rw-r--r--   0        0        0     8213 1970-01-01 00:00:00.000000 snakemd-2.1.0/PKG-INFO
```

### Comparing `SnakeMD-2.0.0b2/LICENSE` & `snakemd-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SnakeMD-2.0.0b2/PKG-INFO` & `snakemd-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 Metadata-Version: 2.1
-Name: SnakeMD
-Version: 2.0.0b2
+Name: snakemd
+Version: 2.1.0
 Summary: A markdown generation library for Python.
-Home-page: https://github.com/TheRenegadeCoder/SnakeMD
-Author: The Renegade Coder
+Home-page: https://www.snakemd.io
+License: MIT
+Author: Jeremy Grifski
 Author-email: jeremy.grifski@therenegadecoder.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Documentation :: Sphinx
-Requires-Python: >=3.8
+Project-URL: Documentation, https://www.snakemd.io/en/latest/docs/
+Project-URL: Repository, https://github.com/TheRenegadeCoder/SnakeMD
+Project-URL: changelog, https://www.snakemd.io/en/latest/version-history/
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Welcome to SnakeMD
 
 SnakeMD is your ticket to generating Markdown in Python. To prove it to you, we've generated this entire README using SnakeMD. See readme.py for how it was done. To get started, download and install SnakeMD:
 
 ```shell
 pip install snakemd
```

### Comparing `SnakeMD-2.0.0b2/README.md` & `snakemd-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `SnakeMD-2.0.0b2/snakemd/__init__.py` & `snakemd-2.1.0/snakemd/__init__.py`

 * *Files identical despite different names*

### Comparing `SnakeMD-2.0.0b2/snakemd/document.py` & `snakemd-2.1.0/snakemd/document.py`

 * *Files identical despite different names*

### Comparing `SnakeMD-2.0.0b2/snakemd/elements.py` & `snakemd-2.1.0/snakemd/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,20 @@
     types of elements in the collection. In short, elements must
     be able to be converted to their markdown representation using
     the built-in :py:class:`str` constructor. 
     """
 
     @abstractmethod
     def __str__(self) -> str:
-        pass
+        """
+        The default string method to be implemented by all inheriting
+        classes. 
+
+        :return: a string representation of the element
+        """
 
 
 class Inline(Element):
     """
     The basic unit of text in markdown. All components which contain
     text are built using this class instead of strings directly. That
     way, those elements capture all styling information.
@@ -834,15 +839,15 @@
             >>> paragraph = Paragraph("I come in piece").replace("piece", "peace")
             >>> str(paragraph)
             'I come in peace'
 
         :param str target: 
             the target string to replace
         :param str replacement: 
-            the Inline object to insert in place of the target
+            the string to insert in place of the target
         :param int count: 
             the number of targets to replace; defaults to -1 (all)
         :return: 
             self
         """
         return self._replace_any(target, Inline(replacement), count)
 
@@ -1052,15 +1057,15 @@
         indent: int = 0
     ) -> None:
         logger.debug(f"Initializing table\n{(header, body, align)}")
         super().__init__()
         self._header: list[Paragraph]
         self._body: list[list[Paragraph]]
         self._header, self._body = self._process_table(header, body)
-        if len(self._body) > 1 and not all(len(self._body[0]) == len(x) for x in self._body[1:]):
+        if len(self._body) > 1 and not all([len(self._body[0]) == len(x) for x in self._body[1:]]):
             raise ValueError("Table rows are not all the same length")
         elif body and len(self._header) != len(self._body[0]):
             raise ValueError("Table header and rows have different lengths")
         self._widths: list[int] = self._process_widths(
             self._header,
             self._body
         )
```

### Comparing `SnakeMD-2.0.0b2/snakemd/templates.py` & `snakemd-2.1.0/snakemd/templates.py`

 * *Files identical despite different names*


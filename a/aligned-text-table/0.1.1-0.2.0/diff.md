# Comparing `tmp/aligned_text_table-0.1.1.tar.gz` & `tmp/aligned_text_table-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligned_text_table-0.1.1.tar", max compression
+gzip compressed data, was "aligned_text_table-0.2.0.tar", max compression
```

## Comparing `aligned_text_table-0.1.1.tar` & `aligned_text_table-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      654 2023-04-28 23:55:20.419467 aligned_text_table-0.1.1/README.md
--rw-r--r--   0        0        0       21 2023-04-28 22:29:05.027773 aligned_text_table-0.1.1/aligned_text_table/__init__.py
--rw-r--r--   0        0        0     2375 2023-04-28 23:58:30.730870 aligned_text_table-0.1.1/aligned_text_table/parser.py
--rw-r--r--   0        0        0      525 2023-04-29 00:06:15.949455 aligned_text_table-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 aligned_text_table-0.1.1/setup.py
--rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 aligned_text_table-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      654 2023-04-28 23:55:20.419467 aligned_text_table-0.2.0/README.md
+-rw-r--r--   0        0        0       21 2023-04-28 22:29:05.027773 aligned_text_table-0.2.0/aligned_text_table/__init__.py
+-rw-r--r--   0        0        0     2057 2023-04-29 00:38:42.566669 aligned_text_table-0.2.0/aligned_text_table/parser.py
+-rw-r--r--   0        0        0      464 2023-04-29 00:39:26.491256 aligned_text_table-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 aligned_text_table-0.2.0/setup.py
+-rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 aligned_text_table-0.2.0/PKG-INFO
```

### Comparing `aligned_text_table-0.1.1/README.md` & `aligned_text_table-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aligned_text_table-0.1.1/setup.py` & `aligned_text_table-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['aligned_text_table']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'aligned-text-table',
-    'version': '0.1.1',
+    'version': '0.2.0',
     'description': 'Parser for space-aligned tables in plain text',
     'long_description': '# Aligned text table\n\nA parser for tables in plain text that are aligned with spaces, e.g.:\n\n```\nThis is     Column two   This one\ncolumn one               is column\n                         three\n```\n\n## Usage\n\n```\n>>> from aligned_text_table import parse_row\n\n>>> parse_row(\n...     lines=[\n...         "This is     Column two   This one ",\n...         "column one               is column",\n...         "three    "\n...     ],\n...     keys=["one", "two", "three"]\n... )\n\n{\n    "one": "This is column one",\n    "two": "Column two",\n    "three": "This one is column three"\n}\n```\n\n## Tests\n\nTo run tests, install and run Tox:\n\n```\npip3 install tox\ntox\n```\n',
     'author': 'Robin Winslow',
     'author_email': 'robin@robinwinslow.co.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nottrobin/aligned-text-table',
```

### Comparing `aligned_text_table-0.1.1/PKG-INFO` & `aligned_text_table-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligned-text-table
-Version: 0.1.1
+Version: 0.2.0
 Summary: Parser for space-aligned tables in plain text
 Home-page: https://github.com/nottrobin/aligned-text-table
 License: Public domain
 Author: Robin Winslow
 Author-email: robin@robinwinslow.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```


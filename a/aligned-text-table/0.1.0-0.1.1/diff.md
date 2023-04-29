# Comparing `tmp/aligned_text_table-0.1.0.tar.gz` & `tmp/aligned_text_table-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligned_text_table-0.1.0.tar", max compression
+gzip compressed data, was "aligned_text_table-0.1.1.tar", max compression
```

## Comparing `aligned_text_table-0.1.0.tar` & `aligned_text_table-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      654 2023-04-28 23:55:20.419467 aligned_text_table-0.1.0/README.md
--rw-r--r--   0        0        0       21 2023-04-28 22:29:05.027773 aligned_text_table-0.1.0/aligned_text_table/__init__.py
--rw-r--r--   0        0        0     2375 2023-04-28 23:58:30.730870 aligned_text_table-0.1.0/aligned_text_table/parser.py
--rw-r--r--   0        0        0      401 2023-04-28 22:19:31.229882 aligned_text_table-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 aligned_text_table-0.1.0/setup.py
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 aligned_text_table-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      654 2023-04-28 23:55:20.419467 aligned_text_table-0.1.1/README.md
+-rw-r--r--   0        0        0       21 2023-04-28 22:29:05.027773 aligned_text_table-0.1.1/aligned_text_table/__init__.py
+-rw-r--r--   0        0        0     2375 2023-04-28 23:58:30.730870 aligned_text_table-0.1.1/aligned_text_table/parser.py
+-rw-r--r--   0        0        0      525 2023-04-29 00:06:15.949455 aligned_text_table-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 aligned_text_table-0.1.1/setup.py
+-rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 aligned_text_table-0.1.1/PKG-INFO
```

### Comparing `aligned_text_table-0.1.0/README.md` & `aligned_text_table-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aligned_text_table-0.1.0/aligned_text_table/parser.py` & `aligned_text_table-0.1.1/aligned_text_table/parser.py`

 * *Files identical despite different names*

### Comparing `aligned_text_table-0.1.0/setup.py` & `aligned_text_table-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 ['aligned_text_table']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'aligned-text-table',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Parser for space-aligned tables in plain text',
     'long_description': '# Aligned text table\n\nA parser for tables in plain text that are aligned with spaces, e.g.:\n\n```\nThis is     Column two   This one\ncolumn one               is column\n                         three\n```\n\n## Usage\n\n```\n>>> from aligned_text_table import parse_row\n\n>>> parse_row(\n...     lines=[\n...         "This is     Column two   This one ",\n...         "column one               is column",\n...         "three    "\n...     ],\n...     keys=["one", "two", "three"]\n... )\n\n{\n    "one": "This is column one",\n    "two": "Column two",\n    "three": "This one is column three"\n}\n```\n\n## Tests\n\nTo run tests, install and run Tox:\n\n```\npip3 install tox\ntox\n```\n',
     'author': 'Robin Winslow',
     'author_email': 'robin@robinwinslow.co.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/nottrobin/aligned-text-table',
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```


# Comparing `tmp/rpp-0.4.tar.gz` & `tmp/rpp-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rpp-0.4.tar", last modified: Tue Dec 19 19:12:10 2017, max compression
+gzip compressed data, was "rpp-0.5.tar", last modified: Sat Apr 29 18:43:35 2023, max compression
```

## Comparing `rpp-0.4.tar` & `rpp-0.5.tar`

### file list

```diff
@@ -1,21 +1,28 @@
-drwxr-xr-x   0 sviatoslav  (1000) sviatoslav  (1000)        0 2017-12-19 19:12:10.000000 rpp-0.4/
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)     1509 2017-12-19 18:24:51.000000 rpp-0.4/LICENSE.rst
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)       20 2017-12-19 18:24:51.000000 rpp-0.4/MANIFEST.in
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)     3299 2017-12-19 19:12:10.000000 rpp-0.4/PKG-INFO
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)     1897 2017-12-19 18:24:51.000000 rpp-0.4/README.rst
-drwxr-xr-x   0 sviatoslav  (1000) sviatoslav  (1000)        0 2017-12-19 19:12:10.000000 rpp-0.4/rpp/
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)      291 2017-12-19 18:24:51.000000 rpp-0.4/rpp/__init__.py
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)     1197 2017-12-19 18:24:51.000000 rpp-0.4/rpp/decoder.py
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)     2310 2017-12-19 18:24:51.000000 rpp-0.4/rpp/element.py
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)     1877 2017-12-19 18:24:51.000000 rpp-0.4/rpp/encoder.py
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)      366 2017-12-19 18:24:51.000000 rpp-0.4/rpp/rpp.py
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)     2225 2017-12-19 18:24:51.000000 rpp-0.4/rpp/scanner.py
-drwxr-xr-x   0 sviatoslav  (1000) sviatoslav  (1000)        0 2017-12-19 19:12:10.000000 rpp-0.4/rpp.egg-info/
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)     3299 2017-12-19 19:12:10.000000 rpp-0.4/rpp.egg-info/PKG-INFO
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)      300 2017-12-19 19:12:10.000000 rpp-0.4/rpp.egg-info/SOURCES.txt
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)        1 2017-12-19 19:12:10.000000 rpp-0.4/rpp.egg-info/dependency_links.txt
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)        1 2017-12-19 18:46:43.000000 rpp-0.4/rpp.egg-info/not-zip-safe
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)       10 2017-12-19 19:12:10.000000 rpp-0.4/rpp.egg-info/requires.txt
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)        4 2017-12-19 19:12:10.000000 rpp-0.4/rpp.egg-info/top_level.txt
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)      125 2017-12-19 19:12:10.000000 rpp-0.4/setup.cfg
--rw-r--r--   0 sviatoslav  (1000) sviatoslav  (1000)     1076 2017-12-19 18:24:51.000000 rpp-0.4/setup.py
+drwxr-xr-x   0 sviatoslav   (501) staff       (20)        0 2023-04-29 18:43:35.144122 rpp-0.5/
+-rw-r--r--   0 sviatoslav   (501) staff       (20)      603 2023-04-29 18:36:19.000000 rpp-0.5/CHANGES.rst
+-rw-r--r--   0 sviatoslav   (501) staff       (20)     1479 2023-04-29 16:58:54.000000 rpp-0.5/LICENSE.rst
+-rw-r--r--   0 sviatoslav   (501) staff       (20)       92 2023-04-29 18:31:31.000000 rpp-0.5/MANIFEST.in
+-rw-r--r--   0 sviatoslav   (501) staff       (20)     2749 2023-04-29 18:43:35.143956 rpp-0.5/PKG-INFO
+-rw-r--r--   0 sviatoslav   (501) staff       (20)     1876 2023-04-29 18:37:59.000000 rpp-0.5/README.rst
+-rw-r--r--   0 sviatoslav   (501) staff       (20)     1029 2023-04-29 17:56:38.000000 rpp-0.5/pyproject.toml
+drwxr-xr-x   0 sviatoslav   (501) staff       (20)        0 2023-04-29 18:43:35.141881 rpp-0.5/rpp/
+-rw-r--r--   0 sviatoslav   (501) staff       (20)      291 2023-04-29 18:36:19.000000 rpp-0.5/rpp/__init__.py
+-rw-r--r--   0 sviatoslav   (501) staff       (20)     1187 2023-04-29 17:35:10.000000 rpp-0.5/rpp/decoder.py
+-rw-r--r--   0 sviatoslav   (501) staff       (20)     2251 2023-04-29 17:35:10.000000 rpp-0.5/rpp/element.py
+-rw-r--r--   0 sviatoslav   (501) staff       (20)     1881 2023-04-29 17:35:10.000000 rpp-0.5/rpp/encoder.py
+-rw-r--r--   0 sviatoslav   (501) staff       (20)      366 2023-04-29 16:58:54.000000 rpp-0.5/rpp/rpp.py
+-rw-r--r--   0 sviatoslav   (501) staff       (20)     2204 2023-04-29 17:56:38.000000 rpp-0.5/rpp/scanner.py
+drwxr-xr-x   0 sviatoslav   (501) staff       (20)        0 2023-04-29 18:43:35.142627 rpp-0.5/rpp.egg-info/
+-rw-r--r--   0 sviatoslav   (501) staff       (20)     2749 2023-04-29 18:43:35.000000 rpp-0.5/rpp.egg-info/PKG-INFO
+-rw-r--r--   0 sviatoslav   (501) staff       (20)      370 2023-04-29 18:43:35.000000 rpp-0.5/rpp.egg-info/SOURCES.txt
+-rw-r--r--   0 sviatoslav   (501) staff       (20)        1 2023-04-29 18:43:35.000000 rpp-0.5/rpp.egg-info/dependency_links.txt
+-rw-r--r--   0 sviatoslav   (501) staff       (20)       10 2023-04-29 18:43:35.000000 rpp-0.5/rpp.egg-info/requires.txt
+-rw-r--r--   0 sviatoslav   (501) staff       (20)        4 2023-04-29 18:43:35.000000 rpp-0.5/rpp.egg-info/top_level.txt
+-rw-r--r--   0 sviatoslav   (501) staff       (20)       38 2023-04-29 18:43:35.144171 rpp-0.5/setup.cfg
+drwxr-xr-x   0 sviatoslav   (501) staff       (20)        0 2023-04-29 18:43:35.143078 rpp-0.5/tests/
+drwxr-xr-x   0 sviatoslav   (501) staff       (20)        0 2023-04-29 18:43:35.143528 rpp-0.5/tests/data/
+-rw-r--r--   0 sviatoslav   (501) staff       (20)     3349 2023-04-29 16:58:54.000000 rpp-0.5/tests/data/empty.RPP
+-rw-r--r--   0 sviatoslav   (501) staff       (20)    10433 2023-04-29 17:22:03.000000 rpp-0.5/tests/data/vst.RPP
+-rw-r--r--   0 sviatoslav   (501) staff       (20)     1768 2023-04-29 16:58:54.000000 rpp-0.5/tests/test_element.py
+-rw-r--r--   0 sviatoslav   (501) staff       (20)     5177 2023-04-29 17:56:38.000000 rpp-0.5/tests/test_rpp.py
+-rw-r--r--   0 sviatoslav   (501) staff       (20)      167 2023-04-29 17:56:38.000000 rpp-0.5/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rpp-0.4/LICENSE.rst` & `rpp-0.5/LICENSE.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-Copyright (c) 2015 by Sviatoslav Abakumov.
-
-All rights reserved.
+Copyright 2015 Sviatoslav Abakumov
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `rpp-0.4/PKG-INFO` & `rpp-0.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,91 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: rpp
-Version: 0.4
-Summary: REAPER Project File Parser
-Home-page: https://github.com/Perlence/rpp
-Author: Sviatoslav Abakumov
-Author-email: dust.harvesting@gmail.com
-License: BSD
-Download-URL: https://github.com/Perlence/rpp/archive/0.4.tar.gz
-Description-Content-Type: UNKNOWN
-Description: RPP
-        ===
-        
-        Description
-        -----------
-        
-        RPP is a format used to describe `REAPER <http://reaper.fm>`_ projects. This package is designed to be RPP
-        parser/emitter and uses `PLY <http://www.dabeaz.com/ply/>`_ as parser framework.
-        
-        
-        Examples
-        --------
-        
-        Import the package:
-        
-        .. code-block:: python
-        
-           >>> import rpp
-        
-        Decode RPP:
-        
-        .. code-block:: python
-        
-           >>> r = rpp.loads("""\
-           <REAPER_PROJECT 0.1 "4.32" 1372525904
-             RIPPLE 0
-             GROUPOVERRIDE 0 0 0
-             AUTOXFADE 1
-           >
-           """)
-           >>> r
-           Element(tag='REAPER_PROJECT', attrib=['0.1', '4.32', '1372525904'], children=[
-               ['RIPPLE', '0'],
-               ['GROUPOVERRIDE', '0', '0', '0'],
-               ['AUTOXFADE', '1'],
-           ])
-        
-        Transform elements into RPP:
-        
-        .. code-block:: python
-        
-           >>> from rpp import Element
-           >>> rpp.dumps(
-           ...     Element(tag='REAPER_PROJECT', attrib=['0.1', '4.32', '1372525904'], children=[
-           ...         ['RIPPLE', '0'],
-           ...         ['GROUPOVERRIDE', '0', '0', '0'],
-           ...         ['AUTOXFADE', '1'],
-           ...     ]))
-           '<REAPER_PROJECT 0.1 4.32 1372525904\n  RIPPLE 0\n  GROUPOVERRIDE 0 0 0\n  AUTOXFADE 1\n>\n'
-        
-        ``Element`` mimics the interface of xml.etree.ElementTree.Element_. You can perform quering operations with ``findall``,
-        ``find``, ``iterfind``. Note that attribute and text predicates are not supported.
-        
-        .. _xml.etree.ElementTree.Element: https://docs.python.org/3/library/xml.etree.elementtree.html#xml.etree.ElementTree.Element
-        
-        .. code-block:: python
-        
-           >>> groupoverride = r.find('.//GROUPOVERRIDE')
-           >>> groupoverride
-           ['GROUPOVERRIDE', '0', '0', '0']
-           >>> groupoverride[1:] = ['9', '9', '9']
-           >>> r
-           Element(tag='REAPER_PROJECT', attrib=['0.1', '4.32', '1372525904'], children=[
-               ['RIPPLE', '0'],
-               ['GROUPOVERRIDE', '9', '9', '9'],
-               ['AUTOXFADE', '1'],
-           ])
-        
-        
-        Dependencies
-        ------------
-        
-        - `attrs <https://attrs.readthedocs.org/>`_
-        - `ply <http://www.dabeaz.com/ply/>`_
-        
-Platform: UNKNOWN
+Version: 0.5
+Summary: Read and write Reaper RPP files with Python.
+Author-email: Sviatoslav Abakumov <dust.harvesting@gmail.com>
+License: BSD-3-Clause
+Project-URL: Source code, https://github.com/Perlence/rpp
+Project-URL: Issue tracker, https://github.com/Perlence/rpp/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE.rst
+
+RPP
+===
+
+RPP is a format used to describe `REAPER <http://reaper.fm>`_ projects. This package is designed to be an RPP
+parser/emitter and uses `PLY <http://www.dabeaz.com/ply/>`_ as a parser framework.
+
+Examples
+--------
+
+Import the package:
+
+.. code-block:: python
+
+   >>> import rpp
+
+Decode RPP:
+
+.. code-block:: python
+
+   >>> r = rpp.loads("""\
+   <REAPER_PROJECT 0.1 "4.32" 1372525904
+     RIPPLE 0
+     GROUPOVERRIDE 0 0 0
+     AUTOXFADE 1
+   >
+   """)
+   >>> r
+   Element(tag='REAPER_PROJECT', attrib=['0.1', '4.32', '1372525904'], children=[
+       ['RIPPLE', '0'],
+       ['GROUPOVERRIDE', '0', '0', '0'],
+       ['AUTOXFADE', '1'],
+   ])
+
+Transform elements into RPP:
+
+.. code-block:: python
+
+   >>> from rpp import Element
+   >>> rpp.dumps(
+   ...     Element(tag='REAPER_PROJECT', attrib=['0.1', '4.32', '1372525904'], children=[
+   ...         ['RIPPLE', '0'],
+   ...         ['GROUPOVERRIDE', '0', '0', '0'],
+   ...         ['AUTOXFADE', '1'],
+   ...     ]))
+   '<REAPER_PROJECT 0.1 4.32 1372525904\n  RIPPLE 0\n  GROUPOVERRIDE 0 0 0\n  AUTOXFADE 1\n>\n'
+
+``Element`` mimics the interface of xml.etree.ElementTree.Element_. You can perform querying operations with
+``findall``, ``find``, ``iterfind``. Note that attribute and text predicates are not supported.
+
+.. _xml.etree.ElementTree.Element: https://docs.python.org/3/library/xml.etree.elementtree.html#xml.etree.ElementTree.Element
+
+.. code-block:: python
+
+   >>> groupoverride = r.find('.//GROUPOVERRIDE')
+   >>> groupoverride
+   ['GROUPOVERRIDE', '0', '0', '0']
+   >>> groupoverride[1:] = ['9', '9', '9']
+   >>> r
+   Element(tag='REAPER_PROJECT', attrib=['0.1', '4.32', '1372525904'], children=[
+       ['RIPPLE', '0'],
+       ['GROUPOVERRIDE', '9', '9', '9'],
+       ['AUTOXFADE', '1'],
+   ])
+
+Dependencies
+------------
+
+- `attrs <https://attrs.readthedocs.org/>`_
+- `ply <http://www.dabeaz.com/ply/>`_
```

### Comparing `rpp-0.4/README.rst` & `rpp-0.5/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 RPP
 ===
 
-Description
------------
-
-RPP is a format used to describe `REAPER <http://reaper.fm>`_ projects. This package is designed to be RPP
-parser/emitter and uses `PLY <http://www.dabeaz.com/ply/>`_ as parser framework.
-
+RPP is a format used to describe `REAPER <http://reaper.fm>`_ projects. This package is designed to be an RPP
+parser/emitter and uses `PLY <http://www.dabeaz.com/ply/>`_ as a parser framework.
 
 Examples
 --------
 
 Import the package:
 
 .. code-block:: python
@@ -44,16 +40,16 @@
    ...     Element(tag='REAPER_PROJECT', attrib=['0.1', '4.32', '1372525904'], children=[
    ...         ['RIPPLE', '0'],
    ...         ['GROUPOVERRIDE', '0', '0', '0'],
    ...         ['AUTOXFADE', '1'],
    ...     ]))
    '<REAPER_PROJECT 0.1 4.32 1372525904\n  RIPPLE 0\n  GROUPOVERRIDE 0 0 0\n  AUTOXFADE 1\n>\n'
 
-``Element`` mimics the interface of xml.etree.ElementTree.Element_. You can perform quering operations with ``findall``,
-``find``, ``iterfind``. Note that attribute and text predicates are not supported.
+``Element`` mimics the interface of xml.etree.ElementTree.Element_. You can perform querying operations with
+``findall``, ``find``, ``iterfind``. Note that attribute and text predicates are not supported.
 
 .. _xml.etree.ElementTree.Element: https://docs.python.org/3/library/xml.etree.elementtree.html#xml.etree.ElementTree.Element
 
 .. code-block:: python
 
    >>> groupoverride = r.find('.//GROUPOVERRIDE')
    >>> groupoverride
@@ -62,13 +58,12 @@
    >>> r
    Element(tag='REAPER_PROJECT', attrib=['0.1', '4.32', '1372525904'], children=[
        ['RIPPLE', '0'],
        ['GROUPOVERRIDE', '9', '9', '9'],
        ['AUTOXFADE', '1'],
    ])
 
-
 Dependencies
 ------------
 
 - `attrs <https://attrs.readthedocs.org/>`_
 - `ply <http://www.dabeaz.com/ply/>`_
```

### Comparing `rpp-0.4/rpp/decoder.py` & `rpp-0.5/rpp/decoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,9 +56,9 @@
         t[0] += t[2]
 
 
 def p_error(t):
     if t is None:
         message = 'syntax error at EOF'
     else:
-        message = 'syntax error at line {}, token={}'.format(t.lineno or 1, t.type)
+        message = f'syntax error at line {t.lineno or 1}, token={t.type}'
     raise ValueError(message)
```

### Comparing `rpp-0.4/rpp/element.py` & `rpp-0.5/rpp/element.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import xml.etree.ElementPath
 
 import attr
 
 
 @attr.s
-class Element(object):
+class Element:
     tag = attr.ib()
     attrib = attr.ib(default=())
     children = attr.ib(default=attr.Factory(list))
 
     def append(self, element):
         self.children.append(element)
 
@@ -49,15 +49,15 @@
         self.children[index] = element
 
     def __len__(self):
         return len(self.children)
 
 
 @attr.s
-class QueryableElement(object):
+class QueryableElement:
     element = attr.ib()
 
     @property
     def tag(self):
         return self.element.tag
 
     def iter(self, tag=None):
@@ -68,15 +68,15 @@
             if isinstance(item, Element):
                 yield QueryableElement(item)
             elif isinstance(item, list):
                 yield ListBackedElement(item)
 
 
 @attr.s
-class ListBackedElement(object):
+class ListBackedElement:
     list = attr.ib()
 
     @property
     def tag(self):
         return self.list[0]
 
     def iter(self, tag=None):
@@ -88,11 +88,10 @@
 
 
 def iterate_element(element, tag):
     if tag is None or element.tag == tag:
         yield element
     for item in element:
         if hasattr(item, 'iter'):
-            for subitem in item.iter(tag):
-                yield subitem
+            yield from item.iter(tag)
         elif tag is None:
             yield item
```

### Comparing `rpp-0.4/rpp/encoder.py` & `rpp-0.5/rpp/encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections import Iterable
+from collections.abc import Iterable
 from decimal import Decimal
 
 from .element import Element
 from .scanner import starts_with_quote, starts_with_pipe
 
 
 def encode(element, indent=2, level=0):
```

### Comparing `rpp-0.4/rpp/scanner.py` & `rpp-0.5/rpp/scanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     return iter(lex)
 
 
 def lexer():
     return Lexer()
 
 
-class Lexer(object):
+class Lexer:
     _input = None
     _iter = None
 
     def input(self, s):
         self._input = s
         self._iter = iter(self)
 
@@ -40,30 +40,30 @@
                         elif line.startswith(CLOSE):
                             yield LexToken('CLOSE', CLOSE, lineno)
                             line = line[1:]
                         elif starts_with_pipe(line):
                             yield LexToken('STRING', line, lineno)
                             line = ''
                     if line:
-                        pair = line.split(None, 1)
+                        pair = line.split(maxsplit=1)
                         thing, rest = pair if len(pair) > 1 else (pair[0], '')
                         yield LexToken('STRING', thing, lineno)
                         line = rest
                 is_first_token_in_line = False
             yield LexToken('NEWLINE', '\n', lineno)
 
     def _find_closing_quote(self, line, lineno):
         try:
             return line.index(line[0], 1)
         except ValueError:
-            raise ValueError('closing quote not found at line {}'.format(lineno))
+            raise ValueError(f'closing quote not found at line {lineno}')
 
 
 @attr.s
-class LexToken(object):
+class LexToken:
     type = attr.ib()
     value = attr.ib()
     lineno = attr.ib()
 
 
 def starts_with_quote(s):
     quotes = '"\'`'
```

### Comparing `rpp-0.4/rpp.egg-info/PKG-INFO` & `rpp-0.5/rpp.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,91 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: rpp
-Version: 0.4
-Summary: REAPER Project File Parser
-Home-page: https://github.com/Perlence/rpp
-Author: Sviatoslav Abakumov
-Author-email: dust.harvesting@gmail.com
-License: BSD
-Download-URL: https://github.com/Perlence/rpp/archive/0.4.tar.gz
-Description-Content-Type: UNKNOWN
-Description: RPP
-        ===
-        
-        Description
-        -----------
-        
-        RPP is a format used to describe `REAPER <http://reaper.fm>`_ projects. This package is designed to be RPP
-        parser/emitter and uses `PLY <http://www.dabeaz.com/ply/>`_ as parser framework.
-        
-        
-        Examples
-        --------
-        
-        Import the package:
-        
-        .. code-block:: python
-        
-           >>> import rpp
-        
-        Decode RPP:
-        
-        .. code-block:: python
-        
-           >>> r = rpp.loads("""\
-           <REAPER_PROJECT 0.1 "4.32" 1372525904
-             RIPPLE 0
-             GROUPOVERRIDE 0 0 0
-             AUTOXFADE 1
-           >
-           """)
-           >>> r
-           Element(tag='REAPER_PROJECT', attrib=['0.1', '4.32', '1372525904'], children=[
-               ['RIPPLE', '0'],
-               ['GROUPOVERRIDE', '0', '0', '0'],
-               ['AUTOXFADE', '1'],
-           ])
-        
-        Transform elements into RPP:
-        
-        .. code-block:: python
-        
-           >>> from rpp import Element
-           >>> rpp.dumps(
-           ...     Element(tag='REAPER_PROJECT', attrib=['0.1', '4.32', '1372525904'], children=[
-           ...         ['RIPPLE', '0'],
-           ...         ['GROUPOVERRIDE', '0', '0', '0'],
-           ...         ['AUTOXFADE', '1'],
-           ...     ]))
-           '<REAPER_PROJECT 0.1 4.32 1372525904\n  RIPPLE 0\n  GROUPOVERRIDE 0 0 0\n  AUTOXFADE 1\n>\n'
-        
-        ``Element`` mimics the interface of xml.etree.ElementTree.Element_. You can perform quering operations with ``findall``,
-        ``find``, ``iterfind``. Note that attribute and text predicates are not supported.
-        
-        .. _xml.etree.ElementTree.Element: https://docs.python.org/3/library/xml.etree.elementtree.html#xml.etree.ElementTree.Element
-        
-        .. code-block:: python
-        
-           >>> groupoverride = r.find('.//GROUPOVERRIDE')
-           >>> groupoverride
-           ['GROUPOVERRIDE', '0', '0', '0']
-           >>> groupoverride[1:] = ['9', '9', '9']
-           >>> r
-           Element(tag='REAPER_PROJECT', attrib=['0.1', '4.32', '1372525904'], children=[
-               ['RIPPLE', '0'],
-               ['GROUPOVERRIDE', '9', '9', '9'],
-               ['AUTOXFADE', '1'],
-           ])
-        
-        
-        Dependencies
-        ------------
-        
-        - `attrs <https://attrs.readthedocs.org/>`_
-        - `ply <http://www.dabeaz.com/ply/>`_
-        
-Platform: UNKNOWN
+Version: 0.5
+Summary: Read and write Reaper RPP files with Python.
+Author-email: Sviatoslav Abakumov <dust.harvesting@gmail.com>
+License: BSD-3-Clause
+Project-URL: Source code, https://github.com/Perlence/rpp
+Project-URL: Issue tracker, https://github.com/Perlence/rpp/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE.rst
+
+RPP
+===
+
+RPP is a format used to describe `REAPER <http://reaper.fm>`_ projects. This package is designed to be an RPP
+parser/emitter and uses `PLY <http://www.dabeaz.com/ply/>`_ as a parser framework.
+
+Examples
+--------
+
+Import the package:
+
+.. code-block:: python
+
+   >>> import rpp
+
+Decode RPP:
+
+.. code-block:: python
+
+   >>> r = rpp.loads("""\
+   <REAPER_PROJECT 0.1 "4.32" 1372525904
+     RIPPLE 0
+     GROUPOVERRIDE 0 0 0
+     AUTOXFADE 1
+   >
+   """)
+   >>> r
+   Element(tag='REAPER_PROJECT', attrib=['0.1', '4.32', '1372525904'], children=[
+       ['RIPPLE', '0'],
+       ['GROUPOVERRIDE', '0', '0', '0'],
+       ['AUTOXFADE', '1'],
+   ])
+
+Transform elements into RPP:
+
+.. code-block:: python
+
+   >>> from rpp import Element
+   >>> rpp.dumps(
+   ...     Element(tag='REAPER_PROJECT', attrib=['0.1', '4.32', '1372525904'], children=[
+   ...         ['RIPPLE', '0'],
+   ...         ['GROUPOVERRIDE', '0', '0', '0'],
+   ...         ['AUTOXFADE', '1'],
+   ...     ]))
+   '<REAPER_PROJECT 0.1 4.32 1372525904\n  RIPPLE 0\n  GROUPOVERRIDE 0 0 0\n  AUTOXFADE 1\n>\n'
+
+``Element`` mimics the interface of xml.etree.ElementTree.Element_. You can perform querying operations with
+``findall``, ``find``, ``iterfind``. Note that attribute and text predicates are not supported.
+
+.. _xml.etree.ElementTree.Element: https://docs.python.org/3/library/xml.etree.elementtree.html#xml.etree.ElementTree.Element
+
+.. code-block:: python
+
+   >>> groupoverride = r.find('.//GROUPOVERRIDE')
+   >>> groupoverride
+   ['GROUPOVERRIDE', '0', '0', '0']
+   >>> groupoverride[1:] = ['9', '9', '9']
+   >>> r
+   Element(tag='REAPER_PROJECT', attrib=['0.1', '4.32', '1372525904'], children=[
+       ['RIPPLE', '0'],
+       ['GROUPOVERRIDE', '9', '9', '9'],
+       ['AUTOXFADE', '1'],
+   ])
+
+Dependencies
+------------
+
+- `attrs <https://attrs.readthedocs.org/>`_
+- `ply <http://www.dabeaz.com/ply/>`_
```


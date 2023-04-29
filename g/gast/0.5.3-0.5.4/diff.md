# Comparing `tmp/gast-0.5.3.tar.gz` & `tmp/gast-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gast-0.5.3.tar", last modified: Sat Nov 13 21:38:54 2021, max compression
+gzip compressed data, was "gast-0.5.4.tar", last modified: Sat Apr 29 19:36:59 2023, max compression
```

## Comparing `gast-0.5.3.tar` & `gast-0.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 sguelton (114786) sguelton (114786)        0 2021-11-13 21:38:54.000000 gast-0.5.3/
--rw-r--r--   0 sguelton (114786) sguelton (114786)     1490 2019-01-04 22:04:28.000000 gast-0.5.3/LICENSE
-drwxr-xr-x   0 sguelton (114786) sguelton (114786)        0 2021-11-13 21:38:54.000000 gast-0.5.3/gast/
--rw-r--r--   0 sguelton (114786) sguelton (114786)      117 2021-08-09 08:14:10.000000 gast-0.5.3/gast/__init__.py
--rw-r--r--   0 sguelton (114786) sguelton (114786)    15475 2021-11-13 21:36:36.000000 gast-0.5.3/gast/gast.py
--rw-r--r--   0 sguelton (114786) sguelton (114786)    14977 2021-07-23 21:21:44.000000 gast-0.5.3/gast/ast3.py
--rw-r--r--   0 sguelton (114786) sguelton (114786)       22 2021-11-13 21:37:58.000000 gast-0.5.3/gast/version.py
--rw-r--r--   0 sguelton (114786) sguelton (114786)     1057 2021-07-23 21:21:44.000000 gast-0.5.3/gast/astn.py
--rw-r--r--   0 sguelton (114786) sguelton (114786)    38638 2021-11-13 21:36:36.000000 gast-0.5.3/gast/unparser.py
--rw-r--r--   0 sguelton (114786) sguelton (114786)    13384 2021-06-28 20:16:16.000000 gast-0.5.3/gast/ast2.py
--rw-r--r--   0 sguelton (114786) sguelton (114786)       45 2019-01-04 22:04:28.000000 gast-0.5.3/MANIFEST.in
-drwxr-xr-x   0 sguelton (114786) sguelton (114786)        0 2021-11-13 21:38:54.000000 gast-0.5.3/gast.egg-info/
--rw-r--r--   0 sguelton (114786) sguelton (114786)        1 2021-11-13 21:38:54.000000 gast-0.5.3/gast.egg-info/dependency_links.txt
--rw-r--r--   0 sguelton (114786) sguelton (114786)      329 2021-11-13 21:38:54.000000 gast-0.5.3/gast.egg-info/SOURCES.txt
--rw-r--r--   0 sguelton (114786) sguelton (114786)        5 2021-11-13 21:38:54.000000 gast-0.5.3/gast.egg-info/top_level.txt
--rw-r--r--   0 sguelton (114786) sguelton (114786)     1316 2021-11-13 21:38:54.000000 gast-0.5.3/gast.egg-info/PKG-INFO
--rw-r--r--   0 sguelton (114786) sguelton (114786)       38 2021-11-13 21:38:54.000000 gast-0.5.3/setup.cfg
--rw-r--r--   0 sguelton (114786) sguelton (114786)     1316 2021-11-13 21:38:54.000000 gast-0.5.3/PKG-INFO
--rw-r--r--   0 sguelton (114786) sguelton (114786)     9474 2021-07-23 21:21:44.000000 gast-0.5.3/README.rst
--rw-r--r--   0 sguelton (114786) sguelton (114786)     1863 2021-11-13 21:36:36.000000 gast-0.5.3/setup.py
-drwxr-xr-x   0 sguelton (114786) sguelton (114786)        0 2021-11-13 21:38:54.000000 gast-0.5.3/tests/
--rw-r--r--   0 sguelton (114786) sguelton (114786)       46 2019-01-04 22:04:28.000000 gast-0.5.3/tests/__init__.py
--rw-r--r--   0 sguelton (114786) sguelton (114786)    17108 2021-07-23 21:21:44.000000 gast-0.5.3/tests/test_compat.py
--rw-r--r--   0 sguelton (114786) sguelton (114786)     4500 2021-11-13 21:36:36.000000 gast-0.5.3/tests/test_api.py
--rw-r--r--   0 sguelton (114786) sguelton (114786)      833 2021-11-13 21:36:36.000000 gast-0.5.3/tests/test_self.py
+drwxr-xr-x   0 ssp       (1000) ssp       (1000)        0 2023-04-29 19:36:59.183535 gast-0.5.4/
+-rw-r--r--   0 ssp       (1000) ssp       (1000)     1490 2023-02-09 13:57:33.000000 gast-0.5.4/LICENSE
+-rw-r--r--   0 ssp       (1000) ssp       (1000)       45 2023-02-09 13:57:33.000000 gast-0.5.4/MANIFEST.in
+-rw-r--r--   0 ssp       (1000) ssp       (1000)     1327 2023-04-29 19:36:59.183535 gast-0.5.4/PKG-INFO
+-rw-r--r--   0 ssp       (1000) ssp       (1000)    10512 2023-04-16 16:26:44.000000 gast-0.5.4/README.rst
+drwxr-xr-x   0 ssp       (1000) ssp       (1000)        0 2023-04-29 19:36:59.182535 gast-0.5.4/gast/
+-rw-r--r--   0 ssp       (1000) ssp       (1000)      117 2023-02-09 13:57:33.000000 gast-0.5.4/gast/__init__.py
+-rw-r--r--   0 ssp       (1000) ssp       (1000)    13384 2023-02-09 13:57:33.000000 gast-0.5.4/gast/ast2.py
+-rw-r--r--   0 ssp       (1000) ssp       (1000)    14977 2023-02-09 13:57:33.000000 gast-0.5.4/gast/ast3.py
+-rw-r--r--   0 ssp       (1000) ssp       (1000)     1057 2023-02-09 13:57:33.000000 gast-0.5.4/gast/astn.py
+-rw-r--r--   0 ssp       (1000) ssp       (1000)    17346 2023-04-16 16:26:44.000000 gast-0.5.4/gast/gast.py
+-rw-r--r--   0 ssp       (1000) ssp       (1000)    38687 2023-02-09 13:57:33.000000 gast-0.5.4/gast/unparser.py
+-rw-r--r--   0 ssp       (1000) ssp       (1000)       22 2023-04-29 19:36:12.000000 gast-0.5.4/gast/version.py
+drwxr-xr-x   0 ssp       (1000) ssp       (1000)        0 2023-04-29 19:36:59.182535 gast-0.5.4/gast.egg-info/
+-rwxrwxrwx   0 ssp       (1000) ssp       (1000)     1327 2023-04-29 19:36:59.000000 gast-0.5.4/gast.egg-info/PKG-INFO
+-rwxrwxrwx   0 ssp       (1000) ssp       (1000)      329 2023-04-29 19:36:59.000000 gast-0.5.4/gast.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ssp       (1000) ssp       (1000)        1 2023-04-29 19:36:59.000000 gast-0.5.4/gast.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ssp       (1000) ssp       (1000)        5 2023-04-29 19:36:59.000000 gast-0.5.4/gast.egg-info/top_level.txt
+-rw-r--r--   0 ssp       (1000) ssp       (1000)       38 2023-04-29 19:36:59.183535 gast-0.5.4/setup.cfg
+-rw-r--r--   0 ssp       (1000) ssp       (1000)     1924 2023-04-16 16:26:44.000000 gast-0.5.4/setup.py
+drwxr-xr-x   0 ssp       (1000) ssp       (1000)        0 2023-04-29 19:36:59.182535 gast-0.5.4/tests/
+-rw-r--r--   0 ssp       (1000) ssp       (1000)       46 2023-02-09 13:57:33.000000 gast-0.5.4/tests/__init__.py
+-rw-r--r--   0 ssp       (1000) ssp       (1000)     4500 2023-02-09 13:57:33.000000 gast-0.5.4/tests/test_api.py
+-rw-r--r--   0 ssp       (1000) ssp       (1000)    24204 2023-04-16 16:26:44.000000 gast-0.5.4/tests/test_compat.py
+-rw-r--r--   0 ssp       (1000) ssp       (1000)      833 2023-02-09 13:57:33.000000 gast-0.5.4/tests/test_self.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gast-0.5.3/LICENSE` & `gast-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gast-0.5.3/gast/gast.py` & `gast-0.5.4/gast/gast.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 try:
     from ast import TypeIgnore
 except ImportError:
     class TypeIgnore(AST):
         pass
 
+try:
+    from ast import pattern
+except ImportError:
+    class pattern(AST):
+        pass
+
 
 def _make_node(Name, Fields, Attributes, Bases):
     NBFields = len(Fields)
 
     def create_node(self, *args, **kwargs):
         if args:
             if len(args) + len([k for k in kwargs if k in Fields]) != NBFields:
@@ -89,20 +95,26 @@
             (stmt,))),
     ('With', (('items', 'body', 'type_comment'),
               ('lineno', 'col_offset', 'end_lineno', 'end_col_offset',),
               (stmt,))),
     ('AsyncWith', (('items', 'body', 'type_comment'),
                    ('lineno', 'col_offset', 'end_lineno', 'end_col_offset',),
                    (stmt,))),
+    ('Match', (('subject', 'cases'),
+                   ('lineno', 'col_offset', 'end_lineno', 'end_col_offset',),
+                   (stmt,))),
     ('Raise', (('exc', 'cause',),
                ('lineno', 'col_offset', 'end_lineno', 'end_col_offset',),
                (stmt,))),
     ('Try', (('body', 'handlers', 'orelse', 'finalbody',),
              ('lineno', 'col_offset', 'end_lineno', 'end_col_offset',),
              (stmt,))),
+    ('TryStar', (('body', 'handlers', 'orelse', 'finalbody',),
+             ('lineno', 'col_offset', 'end_lineno', 'end_col_offset',),
+             (stmt,))),
     ('Assert', (('test', 'msg',),
                 ('lineno', 'col_offset', 'end_lineno', 'end_col_offset',),
                 (stmt,))),
     ('Import', (('names',),
                 ('lineno', 'col_offset', 'end_lineno', 'end_col_offset',),
                 (stmt,))),
     ('ImportFrom', (('module', 'names', 'level',),
@@ -286,14 +298,50 @@
     ('alias', (('name', 'asname'),
                ('lineno', 'col_offset', 'end_lineno', 'end_col_offset'),
                (AST,))),
 
     # withitem
     ('withitem', (('context_expr', 'optional_vars'), (), (AST,))),
 
+    # match_case
+    ('match_case', (('pattern', 'guard', 'body'), (), (AST,))),
+
+    # pattern
+    ('MatchValue', (('value',),
+                    ('lineno', 'col_offset', 'end_lineno', 'end_col_offset'),
+                    (pattern,))),
+    ('MatchSingleton', (('value',),
+                        ('lineno', 'col_offset',
+                         'end_lineno', 'end_col_offset'),
+                        (pattern,))),
+    ('MatchSequence', (('patterns',),
+                       ('lineno', 'col_offset',
+                        'end_lineno', 'end_col_offset'),
+                       (pattern,))),
+    ('MatchMapping', (('keys', 'patterns', 'rest'),
+                      ('lineno', 'col_offset',
+                       'end_lineno', 'end_col_offset'),
+                      (pattern,))),
+    ('MatchClass', (('cls', 'patterns', 'kwd_attrs', 'kwd_patterns'),
+                    ('lineno', 'col_offset',
+                     'end_lineno', 'end_col_offset'),
+                    (pattern,))),
+    ('MatchStar', (('name',),
+                   ('lineno', 'col_offset',
+                    'end_lineno', 'end_col_offset'),
+                   (pattern,))),
+    ('MatchAs', (('pattern', 'name'),
+                   ('lineno', 'col_offset',
+                    'end_lineno', 'end_col_offset'),
+                   (pattern,))),
+    ('MatchOr', (('patterns',),
+                 ('lineno', 'col_offset',
+                  'end_lineno', 'end_col_offset'),
+                 (pattern,))),
+
     # type_ignore
     ('type_ignore', ((), ('lineno', 'tag'), (TypeIgnore,))),
     )
 
 for name, descr in _nodes:
     _make_node(name, *descr)
 
@@ -304,15 +352,15 @@
 
 
 def parse(*args, **kwargs):
     return ast_to_gast(_ast.parse(*args, **kwargs))
 
 
 def unparse(gast_obj):
-    from gast.unparser import unparse
+    from .unparser import unparse
     return unparse(gast_obj)
 
 
 def literal_eval(node_or_string):
     if isinstance(node_or_string, AST):
         node_or_string = gast_to_ast(node_or_string)
     return _ast.literal_eval(node_or_string)
```

### Comparing `gast-0.5.3/gast/ast3.py` & `gast-0.5.4/gast/ast3.py`

 * *Files identical despite different names*

### Comparing `gast-0.5.3/gast/astn.py` & `gast-0.5.4/gast/astn.py`

 * *Files identical despite different names*

### Comparing `gast-0.5.3/gast/unparser.py` & `gast-0.5.4/gast/unparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 # products or services of Licensee, or any third party.
 #
 # 8. By copying, installing or otherwise using Python, Licensee
 # agrees to be bound by the terms and conditions of this License
 # Agreement.
 
 import sys
-from gast import *
+from . import *
 from contextlib import contextmanager
-from enum import auto, Enum
+from string import printable
 
 
 class nullcontext(object):
     def __init__(self, enter_result=None):
         self.enter_result = enter_result
 
     def __enter__(self):
@@ -92,22 +92,22 @@
     POWER = 15           # '**'
     AWAIT = 16           # 'await'
     ATOM = 17
 
 
 _SINGLE_QUOTES = ("'", '"')
 _MULTI_QUOTES = ('"""', "'''")
-_ALL_QUOTES = (*_SINGLE_QUOTES, *_MULTI_QUOTES)
+_ALL_QUOTES = _SINGLE_QUOTES + _MULTI_QUOTES
 
 class _Unparser(NodeVisitor):
     """Methods in this class recursively traverse an AST and
     output source code for the abstract syntax; original formatting
     is disregarded."""
 
-    def __init__(self, *, _avoid_backslashes=False):
+    def __init__(self, _avoid_backslashes=False):
         self._source = []
         self._buffer = []
         self._precedences = {}
         self._type_ignores = {}
         self._indent = 0
         self._avoid_backslashes = _avoid_backslashes
 
@@ -154,15 +154,15 @@
     @property
     def buffer(self):
         value = "".join(self._buffer)
         self._buffer.clear()
         return value
 
     @contextmanager
-    def block(self, *, extra = None):
+    def block(self, extra = None):
         """A context manager for preparing the source for blocks. It adds
         the character':', increases the indentation on enter and decreases
         the indentation on exit. If *extra* is given, it will be directly
         appended after the colon character.
         """
         self.write(":")
         if extra:
@@ -212,22 +212,22 @@
         node = node.value
         if isinstance(node, Constant) and isinstance(node.value, str):
             return node
 
     def get_type_comment(self, node):
         comment = self._type_ignores.get(node.lineno) or node.type_comment
         if comment is not None:
-            return f" # type: {comment}"
+            return " # type: {}".format(comment)
 
     def traverse(self, node):
         if isinstance(node, list):
             for item in node:
                 self.traverse(item)
         else:
-            super().visit(node)
+            super(_Unparser, self).visit(node)
 
     # Note: as visit() resets the output text, do NOT rely on
     # NodeVisitor.generic_visit to handle any nodes (as it calls back in to
     # the subclass visit() method, which resets self._source to an empty list)
     def visit(self, node):
         """Outputs a source code string that, if converted back to an ast
         (using ast.parse) will generate an AST equivalent to *node*"""
@@ -241,15 +241,15 @@
             self._write_docstring(docstring)
             self.traverse(node.body[1:])
         else:
             self.traverse(node.body)
 
     def visit_Module(self, node):
         self._type_ignores = {
-            ignore.lineno: f"ignore{ignore.tag}"
+            ignore.lineno: "ignore{}".format(ignore.tag)
             for ignore in node.type_ignores
         }
         self._write_docstring_and_traverse_body(node)
         self._type_ignores.clear()
 
     def visit_FunctionType(self, node):
         with self.delimit("(", ")"):
@@ -368,15 +368,15 @@
             self.set_precedence(_Precedence.ATOM, node.value)
             self.traverse(node.value)
 
     def visit_Raise(self, node):
         self.fill("raise")
         if not node.exc:
             if node.cause:
-                raise ValueError(f"Node can't use cause without an exception.")
+                raise ValueError("Node can't use cause without an exception.")
             return
         self.write(" ")
         self.traverse(node.exc)
         if node.cause:
             self.write(" from ")
             self.traverse(node.cause)
 
@@ -506,26 +506,26 @@
     def visit_AsyncWith(self, node):
         self.fill("async with ")
         self.interleave(lambda: self.write(", "), self.traverse, node.items)
         with self.block(extra=self.get_type_comment(node)):
             self.traverse(node.body)
 
     def _str_literal_helper(
-        self, string, *, quote_types=_ALL_QUOTES, escape_special_whitespace=False
+        self, string, quote_types=_ALL_QUOTES, escape_special_whitespace=False
     ):
         """Helper for writing string literals, minimizing escapes.
         Returns the tuple (string literal to write, possible quote types).
         """
         def escape_char(c):
             # \n and \t are non-printable, but we only escape them if
             # escape_special_whitespace is True
             if not escape_special_whitespace and c in "\n\t":
                 return c
             # Always escape backslashes and other non-printable characters
-            if c == "\\" or not c.isprintable():
+            if c == "\\" or not all(cc in printable for cc in c):
                 return c.encode("unicode_escape").decode("ascii")
             return c
 
         escaped_string = "".join(map(escape_char, string))
         possible_quotes = quote_types
         if "\n" in escaped_string:
             possible_quotes = [q for q in possible_quotes if q in _MULTI_QUOTES]
@@ -543,19 +543,19 @@
             # If we're using triple quotes and we'd need to escape a final
             # quote, escape it
             if possible_quotes[0][0] == escaped_string[-1]:
                 assert len(possible_quotes[0]) == 3
                 escaped_string = escaped_string[:-1] + "\\" + escaped_string[-1]
         return escaped_string, possible_quotes
 
-    def _write_str_avoiding_backslashes(self, string, *, quote_types=_ALL_QUOTES):
+    def _write_str_avoiding_backslashes(self, string, quote_types=_ALL_QUOTES):
         """Write string literal value with a best effort attempt to avoid backslashes."""
         string, quote_types = self._str_literal_helper(string, quote_types=quote_types)
         quote_type = quote_types[0]
-        self.write(f"{quote_type}{string}{quote_type}")
+        self.write("{0}{1}{0}".format(quote_type, string))
 
     def visit_JoinedStr(self, node):
         self.write("f")
         if self._avoid_backslashes:
             self._fstring_JoinedStr(node, self.buffer_writer)
             self._write_str_avoiding_backslashes(self.buffer)
             return
@@ -578,15 +578,15 @@
             value, quote_types = self._str_literal_helper(
                 value, quote_types=quote_types,
                 escape_special_whitespace=is_constant
             )
             new_buffer.append(value)
         value = "".join(new_buffer)
         quote_type = quote_types[0]
-        self.write(f"{quote_type}{value}{quote_type}")
+        self.write("{0}{1}{0}".format(quote_type, value))
 
     def visit_FormattedValue(self, node):
         self.write("f")
         self._fstring_FormattedValue(node, self.buffer_writer)
         self._write_str_avoiding_backslashes(self.buffer)
 
     def _fstring_JoinedStr(self, node, write):
@@ -610,15 +610,15 @@
         if "\\" in expr:
             raise ValueError("Unable to avoid backslash in f-string expression part")
         write(expr)
         if node.conversion != -1:
             conversion = chr(node.conversion)
             if conversion not in "sra":
                 raise ValueError("Unknown f-string conversion.")
-            write(f"!{conversion}")
+            write("!{}".format(conversion))
         if node.format_spec:
             write(":")
             meth = getattr(self, "_fstring_" + type(node.format_spec).__name__)
             meth(node.format_spec, write)
         write("}")
 
     def visit_Name(self, node):
@@ -633,27 +633,27 @@
     def _write_constant(self, value):
         if isinstance(value, (float, complex)):
             # Substitute overflowing decimal literal for AST infinities,
             # and inf - inf for NaNs.
             self.write(
                 repr(value)
                 .replace("inf", _INFSTR)
-                .replace("nan", f"({_INFSTR}-{_INFSTR})")
+                .replace("nan", "({0}-{0})".format(_INFSTR))
             )
         elif self._avoid_backslashes and isinstance(value, str):
             self._write_str_avoiding_backslashes(value)
         else:
             self.write(repr(value))
 
     def visit_Constant(self, node):
         value = node.value
         if isinstance(value, tuple):
             with self.delimit("(", ")"):
                 self.items_view(self._write_constant, value)
-        elif value is ...:
+        elif value is Ellipsis:
             self.write("...")
         else:
             if node.kind == "u":
                 self.write("u")
             self._write_constant(node.value)
 
     def visit_List(self, node):
@@ -807,15 +807,15 @@
                 right_precedence = operator_precedence
             else:
                 left_precedence = operator_precedence
                 right_precedence = operator_precedence + 1
 
             self.set_precedence(left_precedence, node.left)
             self.traverse(node.left)
-            self.write(f" {operator} ")
+            self.write(" {} ".format(operator))
             self.set_precedence(right_precedence, node.right)
             self.traverse(node.right)
 
     cmpops = {
         "Eq": "==",
         "NotEq": "!=",
         "Lt": "<",
@@ -837,24 +837,23 @@
                 self.traverse(e)
 
     boolops = {"And": "and", "Or": "or"}
     boolop_precedence = {"and": _Precedence.AND, "or": _Precedence.OR}
 
     def visit_BoolOp(self, node):
         operator = self.boolops[node.op.__class__.__name__]
-        operator_precedence = self.boolop_precedence[operator]
+        operator_precedence = [self.boolop_precedence[operator]]
 
         def increasing_level_traverse(node):
-            nonlocal operator_precedence
-            operator_precedence = operator_precedence + 1
-            self.set_precedence(operator_precedence, node)
+            operator_precedence[0] += 1
+            self.set_precedence(operator_precedence[0], node)
             self.traverse(node)
 
-        with self.require_parens(operator_precedence, node):
-            s = f" {operator} "
+        with self.require_parens(operator_precedence[0], node):
+            s = " {} ".format(operator)
             self.interleave(lambda: self.write(s), increasing_level_traverse, node.values)
 
     def visit_Attribute(self, node):
         self.set_precedence(_Precedence.ATOM, node.value)
         self.traverse(node.value)
         # Special case: 3.__abs__() is a syntax error, so if node.value
         # is an integer literal then we need to either parenthesize
@@ -1031,15 +1030,15 @@
                 lambda: self.write(", "), self.traverse, node.patterns
             )
 
     def visit_MatchStar(self, node):
         name = node.name
         if name is None:
             name = "_"
-        self.write(f"*{name}")
+        self.write("*{}".format(name))
 
     def visit_MatchMapping(self, node):
         def write_key_pattern_pair(pair):
             k, p = pair
             self.traverse(k)
             self.write(": ")
             self.traverse(p)
@@ -1051,29 +1050,29 @@
                 write_key_pattern_pair,
                 zip(keys, node.patterns, strict=True),
             )
             rest = node.rest
             if rest is not None:
                 if keys:
                     self.write(", ")
-                self.write(f"**{rest}")
+                self.write("**{}".format(rest))
 
     def visit_MatchClass(self, node):
         self.set_precedence(_Precedence.ATOM, node.cls)
         self.traverse(node.cls)
         with self.delimit("(", ")"):
             patterns = node.patterns
             self.interleave(
                 lambda: self.write(", "), self.traverse, patterns
             )
             attrs = node.kwd_attrs
             if attrs:
                 def write_attr_pattern(pair):
                     attr, pattern = pair
-                    self.write(f"{attr}=")
+                    self.write("{}=".format(attr))
                     self.traverse(pattern)
 
                 if patterns:
                     self.write(", ")
                 self.interleave(
                     lambda: self.write(", "),
                     write_attr_pattern,
@@ -1087,15 +1086,15 @@
             self.write("_")
         elif pattern is None:
             self.write(node.name)
         else:
             with self.require_parens(_Precedence.TEST, node):
                 self.set_precedence(_Precedence.BOR, node.pattern)
                 self.traverse(node.pattern)
-                self.write(f" as {node.name}")
+                self.write(" as {}".format(node.name))
 
     def visit_MatchOr(self, node):
         with self.require_parens(_Precedence.BOR, node):
             self.set_precedence(_Precedence.BOR + 1, *node.patterns)
             self.interleave(lambda: self.write(" | "), self.traverse, node.patterns)
 
 def unparse(ast_obj):
```

### Comparing `gast-0.5.3/gast/ast2.py` & `gast-0.5.4/gast/ast2.py`

 * *Files identical despite different names*

### Comparing `gast-0.5.3/gast.egg-info/PKG-INFO` & `gast-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: gast
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python AST that abstracts the underlying Python version
 Home-page: https://github.com/serge-sans-paille/gast/
 Author: serge-sans-paille
 Author-email: serge.guelton@telecom-bretagne.eu
 License: BSD 3-Clause
-Description: 
-        A generic AST to represent Python2 and Python3's Abstract Syntax Tree(AST).
-        
-        GAST provides a compatibility layer between the AST of various Python versions,
-        as produced by ``ast.parse`` from the standard ``ast`` module.
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -23,8 +17,16 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
+License-File: LICENSE
+
+
+A generic AST to represent Python2 and Python3's Abstract Syntax Tree(AST).
+
+GAST provides a compatibility layer between the AST of various Python versions,
+as produced by ``ast.parse`` from the standard ``ast`` module.
```

### Comparing `gast-0.5.3/PKG-INFO` & `gast-0.5.4/gast.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: gast
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python AST that abstracts the underlying Python version
 Home-page: https://github.com/serge-sans-paille/gast/
 Author: serge-sans-paille
 Author-email: serge.guelton@telecom-bretagne.eu
 License: BSD 3-Clause
-Description: 
-        A generic AST to represent Python2 and Python3's Abstract Syntax Tree(AST).
-        
-        GAST provides a compatibility layer between the AST of various Python versions,
-        as produced by ``ast.parse`` from the standard ``ast`` module.
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -23,8 +17,16 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
+License-File: LICENSE
+
+
+A generic AST to represent Python2 and Python3's Abstract Syntax Tree(AST).
+
+GAST provides a compatibility layer between the AST of various Python versions,
+as produced by ``ast.parse`` from the standard ``ast`` module.
```

### Comparing `gast-0.5.3/README.rst` & `gast-0.5.4/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 - 3.4
 - 3.5
 - 3.6
 - 3.7
 - 3.8
 - 3.9
 - 3.10
+- 3.11
 
 
 AST Changes
 -----------
 
 
 Python3
@@ -114,14 +115,17 @@
 
 - In Python3, ``None``, ``True`` and ``False`` are parsed as ``Constant``
   while they are parsed as regular ``Name`` in Python2.
 
 ASDL
 ****
 
+This closely matches the one from https://docs.python.org/3/library/ast.html#abstract-grammar, with a few
+trade-offs to cope with legacy ASTs.
+
 .. code::
 
     -- ASDL's six builtin types are identifier, int, string, bytes, object, singleton
 
     module Python
     {
         mod = Module(stmt* body, type_ignore *type_ignores)
@@ -159,16 +163,19 @@
               | For(expr target, expr iter, stmt* body, stmt* orelse, string? type_comment)
               | AsyncFor(expr target, expr iter, stmt* body, stmt* orelse, string? type_comment)
               | While(expr test, stmt* body, stmt* orelse)
               | If(expr test, stmt* body, stmt* orelse)
               | With(withitem* items, stmt* body, string? type_comment)
               | AsyncWith(withitem* items, stmt* body, string? type_comment)
 
+              | Match(expr subject, match_case* cases)
+
               | Raise(expr? exc, expr? cause)
               | Try(stmt* body, excepthandler* handlers, stmt* orelse, stmt* finalbody)
+              | TryStar(stmt* body, excepthandler* handlers, stmt* orelse, stmt* finalbody)
               | Assert(expr test, expr? msg)
 
               | Import(alias* names)
               | ImportFrom(identifier? module, alias* names, int? level)
 
               -- Doesn't capture requirement that locals must be
               -- defined if globals is
@@ -250,9 +257,25 @@
 
         -- import name with optional 'as' alias.
         alias = (identifier name, identifier? asname)
                 attributes (int lineno, int col_offset, int? end_lineno, int? end_col_offset)
 
         withitem = (expr context_expr, expr? optional_vars)
 
+        match_case = (pattern pattern, expr? guard, stmt* body)
+
+        pattern = MatchValue(expr value)
+                | MatchSingleton(constant value)
+                | MatchSequence(pattern* patterns)
+                | MatchMapping(expr* keys, pattern* patterns, identifier? rest)
+                | MatchClass(expr cls, pattern* patterns, identifier* kwd_attrs, pattern* kwd_patterns)
+
+                | MatchStar(identifier? name)
+                -- The optional "rest" MatchMapping parameter handles capturing extra mapping keys
+
+                | MatchAs(pattern? pattern, identifier? name)
+                | MatchOr(pattern* patterns)
+
+                 attributes (int lineno, int col_offset, int end_lineno, int end_col_offset)
+
         type_ignore = TypeIgnore(int lineno, string tag)
     }
```

### Comparing `gast-0.5.3/setup.py` & `gast-0.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,11 +37,12 @@
                    'Programming Language :: Python :: 3.4',
                    'Programming Language :: Python :: 3.5',
                    'Programming Language :: Python :: 3.6',
                    'Programming Language :: Python :: 3.7',
                    'Programming Language :: Python :: 3.8',
                    'Programming Language :: Python :: 3.9',
                    'Programming Language :: Python :: 3.10',
+                   'Programming Language :: Python :: 3.11',
                    ],
       python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*',
       **kw
       )
```

### Comparing `gast-0.5.3/tests/test_compat.py` & `gast-0.5.4/tests/test_compat.py`

 * *Files 25% similar despite different names*

```diff
@@ -118,14 +118,135 @@
                 compile(gast.gast_to_ast(tree), '<test>', 'exec')
                 norm = ("Module(body=[Expr(value=NamedExpr(target=Name(id='x',"
                         " ctx=Store(), annotation=None, type_comment=None), "
                         "value=Constant(value=1, kind=None)))], type_ignores="
                         "[])")
                 self.assertEqual(gast.dump(tree), norm)
 
+            if sys.version_info.minor >= 10:
+
+                def test_MatchValue(self):
+                    code = 'match v:\n  case "hello":...'
+                    tree = gast.parse(code)
+                    compile(gast.gast_to_ast(tree), '<test>', 'exec')
+                    norm = ("Module(body=[Match(subject=Name(id='v', ctx=Load"
+                            "(), annotation=None, type_comment=None), cases="
+                            "[match_case(pattern=MatchValue(value=Constant("
+                            "value='hello', kind=None)), guard=None, body="
+                            "[Expr(value=Constant(value=Ellipsis, kind=None))]"
+                            ")])], type_ignores=[])"
+                            )
+                    self.assertEqual(gast.dump(tree), norm)
+
+                def test_MatchSingleton(self):
+                    self.maxDiff = None
+                    code = 'match v:\n  case None:...'
+                    tree = gast.parse(code)
+                    compile(gast.gast_to_ast(tree), '<test>', 'exec')
+                    norm = ("Module(body=[Match(subject=Name(id='v', ctx=Load"
+                            "(), annotation=None, type_comment=None), cases=["
+                            "match_case(pattern=MatchSingleton(value=None), "
+                            "guard=None, body=[Expr(value=Constant(value="
+                            "Ellipsis, kind=None))])])], type_ignores=[])")
+                    self.assertEqual(gast.dump(tree), norm)
+
+                def test_MatchSequence(self):
+                    code = 'match v:\n  case a, b:...'
+                    tree = gast.parse(code)
+                    compile(gast.gast_to_ast(tree), '<test>', 'exec')
+                    norm = ("Module(body=[Match(subject=Name(id='v', ctx=Load"
+                            "(), annotation=None, type_comment=None), cases="
+                            "[match_case(pattern=MatchSequence(patterns=["
+                            "MatchAs(pattern=None, name='a'), MatchAs(pattern"
+                            "=None, name='b')]), guard=None, body=[Expr(value"
+                            "=Constant(value=Ellipsis, kind=None))])])], "
+                            "type_ignores=[])")
+                    self.assertEqual(gast.dump(tree), norm)
+
+                def test_MatchMapping(self):
+                    code = 'match v:\n  case {1: a}:...'
+                    tree = gast.parse(code)
+                    compile(gast.gast_to_ast(tree), '<test>', 'exec')
+                    norm = ("Module(body=[Match(subject=Name(id='v', ctx=Load"
+                            "(), annotation=None, type_comment=None), cases=["
+                            "match_case(pattern=MatchMapping(keys=[Constant("
+                            "value=1, kind=None)], patterns=[MatchAs(pattern"
+                            "=None, name='a')], rest=None), guard=None, body="
+                            "[Expr(value=Constant(value=Ellipsis, kind=None))]"
+                            ")])], type_ignores=[])")
+                    self.assertEqual(gast.dump(tree), norm)
+
+                def test_MatchClass(self):
+                    code = 'match v:\n  case Cls(attr=1):...'
+                    tree = gast.parse(code)
+                    compile(gast.gast_to_ast(tree), '<test>', 'exec')
+                    norm = ("Module(body=[Match(subject=Name(id='v', ctx=Load"
+                            "(), annotation=None, type_comment=None), cases=["
+                            "match_case(pattern=MatchClass(cls=Name(id='Cls'"
+                            ", ctx=Load(), annotation=None, type_comment=None"
+                            "), patterns=[], kwd_attrs=['attr'], kwd_patterns"
+                            "=[MatchValue(value=Constant(value=1, kind=None))"
+                            "]), guard=None, body=[Expr(value=Constant(value="
+                            "Ellipsis, kind=None))])])], type_ignores=[])")
+                    self.assertEqual(gast.dump(tree), norm)
+
+                def test_MatchStar(self):
+                    code = 'match v:\n  case [1, *other]:...'
+                    tree = gast.parse(code)
+                    compile(gast.gast_to_ast(tree), '<test>', 'exec')
+                    norm = ("Module(body=[Match(subject=Name(id='v', ctx=Load"
+                            "(), annotation=None, type_comment=None), cases=["
+                            "match_case(pattern=MatchSequence(patterns=["
+                            "MatchValue(value=Constant(value=1, kind=None)), "
+                            "MatchStar(name='other')]), guard=None, body="
+                            "[Expr(value=Constant(value=Ellipsis, kind=None)"
+                            ")])])], type_ignores=[])")
+                    self.assertEqual(gast.dump(tree), norm)
+
+                def test_MatchAs(self):
+                    code = 'match v:\n  case 1, other:...'
+                    tree = gast.parse(code)
+                    compile(gast.gast_to_ast(tree), '<test>', 'exec')
+                    norm = ("Module(body=[Match(subject=Name(id='v', ctx=Load"
+                            "(), annotation=None, type_comment=None), cases=["
+                            "match_case(pattern=MatchSequence(patterns=["
+                            "MatchValue(value=Constant(value=1, kind=None)), "
+                            "MatchAs(pattern=None, name='other')]), guard=None"
+                            ", body=[Expr(value=Constant(value=Ellipsis, kind"
+                            "=None))])])], type_ignores=[])")
+                    self.assertEqual(gast.dump(tree), norm)
+
+                def test_MatchOr(self):
+                    code = 'match v:\n  case 1 | 2:...'
+                    tree = gast.parse(code)
+                    compile(gast.gast_to_ast(tree), '<test>', 'exec')
+                    norm = ("Module(body=[Match(subject=Name(id='v', ctx=Load"
+                            "(), annotation=None, type_comment=None), cases=["
+                            "match_case(pattern=MatchOr(patterns=[MatchValue("
+                            "value=Constant(value=1, kind=None)), MatchValue("
+                            "value=Constant(value=2, kind=None))]), guard="
+                            "None, body=[Expr(value=Constant(value=Ellipsis, "
+                            "kind=None))])])], type_ignores=[])")
+                    self.assertEqual(gast.dump(tree), norm)
+
+
+                if sys.version_info.minor >= 11:
+
+                    def test_TryStar(self):
+                        code = '''
+                            try: ...
+                            except *ValueError: ...'''
+                        norm = ("Module(body=[TryStar(body=[Expr(value="
+                                "Constant(value=Ellipsis))], handlers=["
+                                "ExceptHandler(type=Name(id='ValueError', ctx"
+                                "=Load()), body=[Expr(value=Constant(value="
+                                "Ellipsis))])], orelse=[], finalbody=[])], "
+                                "type_ignores=[])")
+                        pass
+
         else:
 
             def test_Bytes(self):
                 code = 'b"0012"'
                 tree = gast.parse(code)
                 compile(gast.gast_to_ast(tree), '<test>', 'exec')
                 norm = ("Module(body=[Expr(value=Constant(value=b'0012', "
```

### Comparing `gast-0.5.3/tests/test_api.py` & `gast-0.5.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `gast-0.5.3/tests/test_self.py` & `gast-0.5.4/tests/test_self.py`

 * *Files identical despite different names*


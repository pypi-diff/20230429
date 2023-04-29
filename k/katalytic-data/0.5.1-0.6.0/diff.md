# Comparing `tmp/katalytic-data-0.5.1.tar.gz` & `tmp/katalytic-data-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-data-0.5.1.tar", last modified: Sat Apr 29 13:10:19 2023, max compression
+gzip compressed data, was "katalytic-data-0.6.0.tar", last modified: Sat Apr 29 20:11:18 2023, max compression
```

## Comparing `katalytic-data-0.5.1.tar` & `katalytic-data-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.5.1/.coveragerc
--rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.5.1/.gitignore
--rw-r--r--   0        0        0     3109 2023-04-27 17:15:54.916636 katalytic-data-0.5.1/.gitlab-ci.yml
--rw-r--r--   0        0        0    11874 2023-04-29 13:10:15.962382 katalytic-data-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0     2083 2023-04-16 12:25:23.268033 katalytic-data-0.5.1/README.md
--rw-r--r--   0        0        0     1245 2023-04-29 13:10:15.962382 katalytic-data-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    20454 2023-04-29 13:06:49.137033 katalytic-data-0.5.1/src/katalytic/data.py
--rw-r--r--   0        0        0    40111 2023-04-29 12:56:39.475521 katalytic-data-0.5.1/tests/test_data.py
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 katalytic-data-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.6.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.6.0/.gitignore
+-rw-r--r--   0        0        0     3109 2023-04-27 17:15:54.916636 katalytic-data-0.6.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0    12185 2023-04-29 20:11:15.675044 katalytic-data-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     2083 2023-04-16 12:25:23.268033 katalytic-data-0.6.0/README.md
+-rw-r--r--   0        0        0     1245 2023-04-29 20:11:15.675044 katalytic-data-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    20832 2023-04-29 20:04:37.808201 katalytic-data-0.6.0/src/katalytic/data.py
+-rw-r--r--   0        0        0    40893 2023-04-29 20:05:14.136232 katalytic-data-0.6.0/tests/test_data.py
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 katalytic-data-0.6.0/PKG-INFO
```

### Comparing `katalytic-data-0.5.1/.gitignore` & `katalytic-data-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.5.1/.gitlab-ci.yml` & `katalytic-data-0.6.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.5.1/CHANGELOG.md` & `katalytic-data-0.6.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.6.0 (2023-04-29)
+### feat
+- [[`52b8faf`](https://gitlab.com/katalytic/katalytic-data/commit/52b8faf9d53af06a791c4fab8c7b8a70001c1490)] **all_types_besides:** add "numbers" category
+- [[`c7c80ad`](https://gitlab.com/katalytic/katalytic-data/commit/c7c80ade75dfa858022855df849c6be6ccb3c4fc)] add all_types
+
+
 ## 0.5.1 (2023-04-29)
 ### fix
 - [[`1f727b0`](https://gitlab.com/katalytic/katalytic-data/commit/1f727b046ec1f5b38608139a2d3b20b363a58720)] **all_types_besides:** add "class" to the "callables" category
 
 
 ## 0.5.0 (2023-04-29)
 ### feat
```

### Comparing `katalytic-data-0.5.1/LICENSE.txt` & `katalytic-data-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.5.1/README.md` & `katalytic-data-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.5.1/pyproject.toml` & `katalytic-data-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-data"
-version = "0.5.1"
+version = "0.6.0"
 description = "This plugin adds utilities for working with data to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-data-0.5.1/src/katalytic/data.py` & `katalytic-data-0.6.0/src/katalytic/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import inspect
-import random
 from decimal import Decimal
 from fractions import Fraction
 from pathlib import Path
 
 from katalytic.checks import (
     is_any_of, is_iterable, is_iterator, is_none_of, is_primitive, is_dict_of_sequences_uniform, is_sequence_of_sequences_uniform,
     is_sequence_of_dicts_uniform
@@ -26,72 +24,91 @@
 def _generator():
     yield 1
 
 
 def _function():
     pass
 
+
 _lambda = lambda x: x
 _generator_expr = (x for x in [])
-__sequences = [[], (), range(1)]
-__dict_views = [{}.keys(), {}.values(), {}.items()]
-__iterators = [_generator, _generator_expr, iter([]), map(int, ''), enumerate([]), zip([], [])]
-__iterables = [*__dict_views, *__iterators, *__sequences, set(), {}]
-__collections = [(), set(), frozenset([]), {}, []]
-__singletons = [None, True, False]
-__primitives = [*__singletons, 0, 0.0, '', b'', bytearray(b'')]
-__callables = [_generator, _function, _lambda, _C_obj, _C]
+_sequences = [[], (), range(1)]
+_dict_views = [{}.keys(), {}.values(), {}.items()]
+_iterators = [_generator, _generator_expr, iter([]), map(int, ''), enumerate([]), zip([], [])]
+_iterables = [*_dict_views, *_iterators, *_sequences, set(), {}]
+_collections = [(), set(), frozenset([]), {}, []]
+_singletons = [None, True, False]
+_primitives = [*_singletons, 0, 0.0, '', b'', bytearray(b'')]
+_callables = [_generator, _function, _lambda, _C_obj, _C]
+_numbers = [0, 0.0, 0j, Decimal('0'), Fraction(0, 1)]
+_objects = [_obj, _C_obj]
+_generators = [_generator, _generator_expr]
+_functions = [_generator, _function, _lambda]
+
+_types = {
+    'bool': False,
+    'bytearray': bytearray(b''),
+    'bytes': b'',
+    'callables': _callables,
+    'callable object': _C_obj,
+    'class': _C,
+    'collections': _collections,
+    'complex': 0 + 0j,
+    'decimal': Decimal('0'),
+    'dict': {},
+    'dict_views': _dict_views,
+    'float': 0.0,
+    'fraction': Fraction(0, 1),
+    'frozenset': frozenset([]),
+    'functions': _functions,
+    'generator_expr': _generator_expr,
+    'generator_func': _generator,
+    'generators': _generators,
+    'int': 0,
+    'iterables': _iterables,
+    'iterators': _iterators,
+    'list': [],
+    'map': map(int, []),
+    'none': None,
+    'numbers': _numbers,
+    'objects': _objects,
+    'path': Path(''),
+    'primitives': _primitives,
+    'sequences': _sequences,
+    'set': set(),
+    'singletons': _singletons,
+    'str': '',
+    'tuple': (),
+}
+
+
+def all_types(whitelist=None):
+    if whitelist is None:
+        return flatten(_types.values())
+    elif not is_iterable(whitelist):
+        raise TypeError(f'<whitelist> must be iterable. Got {type(whitelist).__name__}')
+
+    unexpected = set(whitelist) - set(_types.keys())
+    if unexpected:
+        raise ValueError(f'Unexpected types in <whitelist>: {unexpected}')
+
+    return flatten(_types[t] for t in whitelist)
 
 
 def all_types_besides(blacklist):
     if not is_iterable(blacklist):
         raise TypeError(f'<blacklist> must be iterable. Got {type(blacklist).__name__}')
 
-    whitelist = {
-        'bool': False,
-        'bytearray': bytearray(b''),
-        'bytes': b'',
-        'callables': __callables,
-        'callable object': _C_obj,
-        'class': _C,
-        'collections': __collections,
-        'complex': 0 + 0j,
-        'decimal': Decimal('0'),
-        'dict': {},
-        'dict_views': __dict_views,
-        'float': 0,
-        'fraction': Fraction(0, 1),
-        'frozenset': frozenset([]),
-        'functions': [_generator, _function, _lambda],
-        'generator_expr': _generator_expr,
-        'generator_func': _generator,
-        'generators': [_generator, _generator_expr],
-        'int': 0,
-        'iterables': __iterables,
-        'iterators': __iterators,
-        'list': [],
-        'map': map(int, []),
-        'none': None,
-        'objects': [_obj, _C_obj],
-        'path': Path(''),
-        'primitives': __primitives,
-        'sequences': __sequences,
-        'set': set(),
-        'singletons': __singletons,
-        'str': '',
-        'tuple': (),
-    }
-
     blacklist = set(blacklist)
-    unexpected = blacklist - set(whitelist.keys())
+    unexpected = blacklist - set(_types.keys())
     if unexpected:
         raise ValueError(f'Unexpected types in <blacklist>: {unexpected}')
 
-    to_remove = flatten(whitelist[t] for t in blacklist)
-    all_types = flatten(whitelist.values())
+    to_remove = flatten(_types[t] for t in blacklist)
+    all_types = flatten(_types.values())
     kept = []
     for t in all_types:
         if t in to_remove:
             continue
 
         # remove duplicates too
         # I have to do it this way because python considers
```

### Comparing `katalytic-data-0.5.1/tests/test_data.py` & `katalytic-data-0.6.0/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from _decimal import Decimal
 from fractions import Fraction
-from pathlib import PosixPath
+from pathlib import Path, PosixPath
 
 import pytest
 
-from katalytic.checks import is_iterator, dicts_share_key_order, dicts_share_value_order, is_singleton, is_equal
+from katalytic.checks import is_iterator, dicts_share_key_order, dicts_share_value_order, is_equal
 from katalytic.data import (
-    _C, _C_obj, _function, _lambda, _obj, all_types_besides, as_list_of_dicts, as_list_of_lists, first, first_with_idx, flatten, flatten_recursive, last, last_with_idx, map_dict_keys, map_dict_values,
+    _C, _C_obj, _function, _iterables, _lambda, _obj, _objects, _types, all_types, all_types_besides, as_list_of_dicts, as_list_of_lists, first, first_with_idx, flatten, flatten_recursive, last, last_with_idx, map_dict_keys, map_dict_values,
     map_recursive, one, pick_all, pick_all_besides, pick_any, sort_dict_by_keys, sort_dict_by_keys_recursive, sort_dict_by_values, sort_dict_by_values_recursive,
     as_dict_of_lists, sort_recursive, xor, xor_with_idx, detect_fronts, detect_fronts_positive, detect_fronts_negative
 )
 
 
 def _is_list(x):
     return isinstance(x, list)
@@ -28,14 +28,36 @@
     return _is_num(x) and x % 2 == 1
 
 
 def _is_str(x):
     return isinstance(x, str)
 
 
+class Test_all_types:
+    @pytest.mark.parametrize('wrong_type', ['', 1, 1.0, True, False, object()])
+    def test_wrong_type(self, wrong_type):
+        with pytest.raises(TypeError):
+            all_types(wrong_type)
+
+    @pytest.mark.parametrize('unexpected', [
+        ['iterable', 'func', 'strong']
+    ])
+    def test_unexpected(self, unexpected):
+        with pytest.raises(ValueError):
+            all_types(unexpected)
+
+    @pytest.mark.parametrize('whitelist, expected', [
+        (None, flatten(_types.values())),
+        (['iterables'], _iterables),
+        (['iterables', 'objects', 'path'], [*_iterables, *_objects, Path('')]),
+    ])
+    def test_all_types(self, whitelist, expected):
+        assert all_types(whitelist) == expected
+
+
 class Test_all_types_besides:
     @pytest.mark.parametrize('wrong_type', ['', 1, 1.0, True, False, None, object()])
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
             all_types_besides(wrong_type)
 
     @pytest.mark.parametrize('unexpected', [
@@ -44,19 +66,19 @@
     def test_unexpected(self, unexpected):
         with pytest.raises(ValueError):
             all_types_besides(unexpected)
 
     @pytest.mark.parametrize('blacklist, expected', [
         (
             ['iterables'],
-            [False, bytearray(b''), b'', _function, _lambda, _C_obj, _C, 0j, Decimal('0'), 0, Fraction(0, 1), None, _obj, PosixPath('.'), True, 0.0, '']
+            [False, bytearray(b''), b'', _function, _lambda, _C_obj, _C, 0j, Decimal('0'), 0.0, Fraction(0, 1), 0, None, _obj, PosixPath('.'), True, '']
         ),
         (
             ['iterables', 'generators', 'functions', 'objects', 'path'],
-            [False, bytearray(b''), b'', _C, 0j, Decimal('0'), 0, Fraction(0, 1), None, True, 0.0, '']
+            [False, bytearray(b''), b'', _C, 0j, Decimal('0'), 0.0, Fraction(0, 1), 0, None, True, '']
         ),
     ])
     def test_all_types_besides(self, blacklist, expected):
         assert all_types_besides(blacklist) == expected
 
 
 class Test_as_dict_of_lists:
```

### Comparing `katalytic-data-0.5.1/PKG-INFO` & `katalytic-data-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-data
-Version: 0.5.1
+Version: 0.6.0
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```


# Comparing `tmp/katalytic-data-0.5.0.tar.gz` & `tmp/katalytic-data-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-data-0.5.0.tar", last modified: Sat Apr 29 13:02:35 2023, max compression
+gzip compressed data, was "katalytic-data-0.5.1.tar", last modified: Sat Apr 29 13:10:19 2023, max compression
```

## Comparing `katalytic-data-0.5.0.tar` & `katalytic-data-0.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.5.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.5.0/.gitignore
--rw-r--r--   0        0        0     3109 2023-04-27 17:15:54.916636 katalytic-data-0.5.0/.gitlab-ci.yml
--rw-r--r--   0        0        0    11670 2023-04-29 13:02:18.728364 katalytic-data-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     2083 2023-04-16 12:25:23.268033 katalytic-data-0.5.0/README.md
--rw-r--r--   0        0        0     1245 2023-04-29 13:02:18.728364 katalytic-data-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    20450 2023-04-29 12:57:50.375698 katalytic-data-0.5.0/src/katalytic/data.py
--rw-r--r--   0        0        0    40111 2023-04-29 12:56:39.475521 katalytic-data-0.5.0/tests/test_data.py
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 katalytic-data-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.5.1/.coveragerc
+-rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.5.1/.gitignore
+-rw-r--r--   0        0        0     3109 2023-04-27 17:15:54.916636 katalytic-data-0.5.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0    11874 2023-04-29 13:10:15.962382 katalytic-data-0.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     2083 2023-04-16 12:25:23.268033 katalytic-data-0.5.1/README.md
+-rw-r--r--   0        0        0     1245 2023-04-29 13:10:15.962382 katalytic-data-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    20454 2023-04-29 13:06:49.137033 katalytic-data-0.5.1/src/katalytic/data.py
+-rw-r--r--   0        0        0    40111 2023-04-29 12:56:39.475521 katalytic-data-0.5.1/tests/test_data.py
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 katalytic-data-0.5.1/PKG-INFO
```

### Comparing `katalytic-data-0.5.0/.gitignore` & `katalytic-data-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.5.0/.gitlab-ci.yml` & `katalytic-data-0.5.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.5.0/CHANGELOG.md` & `katalytic-data-0.5.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.5.1 (2023-04-29)
+### fix
+- [[`1f727b0`](https://gitlab.com/katalytic/katalytic-data/commit/1f727b046ec1f5b38608139a2d3b20b363a58720)] **all_types_besides:** add "class" to the "callables" category
+
+
 ## 0.5.0 (2023-04-29)
 ### feat
 - [[`27102cf`](https://gitlab.com/katalytic/katalytic-data/commit/27102cf2a974a2ae73e56afafab38eb66098940c)] **all_types_besides:** add "callables" category
 - [[`39cccc6`](https://gitlab.com/katalytic/katalytic-data/commit/39cccc664bd062e73fe80d63a21dedc8cffcb2d2)] add all_types_besides, flatten, flatten_recursive
 - [[`12706e2`](https://gitlab.com/katalytic/katalytic-data/commit/12706e2e40dc3127ca680c7121dd720e849d3fdc)] add are_equal
 - [[`fbe876b`](https://gitlab.com/katalytic/katalytic-data/commit/fbe876b80301be2ae917b93ee31954d576477af8)] add as_dict_of_lists(), and fix bugs in as_sequence_of_dicts() and as_sequence_of_sequences()
 - [[`2a4ac90`](https://gitlab.com/katalytic/katalytic-data/commit/2a4ac90ff94ced5ddbafc6d083d08a3720fb389c)] add as_sequence_of_dicts()
```

### Comparing `katalytic-data-0.5.0/LICENSE.txt` & `katalytic-data-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.5.0/README.md` & `katalytic-data-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.5.0/pyproject.toml` & `katalytic-data-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-data"
-version = "0.5.0"
+version = "0.5.1"
 description = "This plugin adds utilities for working with data to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-data-0.5.0/src/katalytic/data.py` & `katalytic-data-0.5.1/src/katalytic/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 __sequences = [[], (), range(1)]
 __dict_views = [{}.keys(), {}.values(), {}.items()]
 __iterators = [_generator, _generator_expr, iter([]), map(int, ''), enumerate([]), zip([], [])]
 __iterables = [*__dict_views, *__iterators, *__sequences, set(), {}]
 __collections = [(), set(), frozenset([]), {}, []]
 __singletons = [None, True, False]
 __primitives = [*__singletons, 0, 0.0, '', b'', bytearray(b'')]
-__callables = [_generator, _function, _lambda, _C_obj]
+__callables = [_generator, _function, _lambda, _C_obj, _C]
 
 
 def all_types_besides(blacklist):
     if not is_iterable(blacklist):
         raise TypeError(f'<blacklist> must be iterable. Got {type(blacklist).__name__}')
 
     whitelist = {
```

### Comparing `katalytic-data-0.5.0/tests/test_data.py` & `katalytic-data-0.5.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.5.0/PKG-INFO` & `katalytic-data-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-data
-Version: 0.5.0
+Version: 0.5.1
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```


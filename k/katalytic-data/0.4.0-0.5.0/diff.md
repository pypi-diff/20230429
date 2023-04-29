# Comparing `tmp/katalytic-data-0.4.0.tar.gz` & `tmp/katalytic-data-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-data-0.4.0.tar", last modified: Thu Apr 27 05:39:58 2023, max compression
+gzip compressed data, was "katalytic-data-0.5.0.tar", last modified: Sat Apr 29 13:02:35 2023, max compression
```

## Comparing `katalytic-data-0.4.0.tar` & `katalytic-data-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.4.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.4.0/.gitignore
--rw-r--r--   0        0        0     3109 2023-04-16 15:20:55.636719 katalytic-data-0.4.0/.gitlab-ci.yml
--rw-r--r--   0        0        0    11927 2023-04-27 05:39:51.262487 katalytic-data-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     2083 2023-04-16 12:25:23.268033 katalytic-data-0.4.0/README.md
--rw-r--r--   0        0        0     1548 2023-04-27 05:39:51.262487 katalytic-data-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5722 2023-04-25 05:47:11.165924 katalytic-data-0.4.0/src/katalytic/checks.py
--rw-r--r--   0        0        0    20361 2023-04-25 05:38:24.309384 katalytic-data-0.4.0/src/katalytic/data.py
--rw-r--r--   0        0        0    16327 2023-04-24 05:49:34.858602 katalytic-data-0.4.0/tests/test_checks.py
--rw-r--r--   0        0        0    39853 2023-04-25 05:42:40.065433 katalytic-data-0.4.0/tests/test_data.py
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 katalytic-data-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.5.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.5.0/.gitignore
+-rw-r--r--   0        0        0     3109 2023-04-27 17:15:54.916636 katalytic-data-0.5.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0    11670 2023-04-29 13:02:18.728364 katalytic-data-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     2083 2023-04-16 12:25:23.268033 katalytic-data-0.5.0/README.md
+-rw-r--r--   0        0        0     1245 2023-04-29 13:02:18.728364 katalytic-data-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    20450 2023-04-29 12:57:50.375698 katalytic-data-0.5.0/src/katalytic/data.py
+-rw-r--r--   0        0        0    40111 2023-04-29 12:56:39.475521 katalytic-data-0.5.0/tests/test_data.py
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 katalytic-data-0.5.0/PKG-INFO
```

### Comparing `katalytic-data-0.4.0/.gitignore` & `katalytic-data-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.4.0/.gitlab-ci.yml` & `katalytic-data-0.5.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.4.0/CHANGELOG.md` & `katalytic-data-0.5.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-## 0.4.0 (2023-04-27)
+## 0.5.0 (2023-04-29)
 ### feat
+- [[`27102cf`](https://gitlab.com/katalytic/katalytic-data/commit/27102cf2a974a2ae73e56afafab38eb66098940c)] **all_types_besides:** add "callables" category
 - [[`39cccc6`](https://gitlab.com/katalytic/katalytic-data/commit/39cccc664bd062e73fe80d63a21dedc8cffcb2d2)] add all_types_besides, flatten, flatten_recursive
 - [[`12706e2`](https://gitlab.com/katalytic/katalytic-data/commit/12706e2e40dc3127ca680c7121dd720e849d3fdc)] add are_equal
 - [[`fbe876b`](https://gitlab.com/katalytic/katalytic-data/commit/fbe876b80301be2ae917b93ee31954d576477af8)] add as_dict_of_lists(), and fix bugs in as_sequence_of_dicts() and as_sequence_of_sequences()
 - [[`2a4ac90`](https://gitlab.com/katalytic/katalytic-data/commit/2a4ac90ff94ced5ddbafc6d083d08a3720fb389c)] add as_sequence_of_dicts()
 - [[`ed4689c`](https://gitlab.com/katalytic/katalytic-data/commit/ed4689c231abf872c6f3fa130a286105548e69b1)] add as_sequence_of_sequences()
 - [[`f1222bf`](https://gitlab.com/katalytic/katalytic-data/commit/f1222bf4b6e54fe5361ad36a49534b1966a837b8)] add contains_all_of, contains_any_of, contains_none_of
 - [[`e17e02e`](https://gitlab.com/katalytic/katalytic-data/commit/e17e02e93bbc39c261a92c192fd1755d05a08873)] add detect_fronts, detect_fronts_positive, detect_fronts_negative
@@ -17,21 +18,33 @@
 - [[`563dc12`](https://gitlab.com/katalytic/katalytic-data/commit/563dc12952da62e486efc769a68f4103a2dd55ee)] add is_singleton()
 - [[`eeee05f`](https://gitlab.com/katalytic/katalytic-data/commit/eeee05fba6ae67ab439fa4030a1fd1a3901d41a3)] add one(), first(), last()
 - [[`5183859`](https://gitlab.com/katalytic/katalytic-data/commit/51838594613e4f47e34a91be19cf16fbef22dc2f)] add pick_all, pick_all_besides, pick_any,
 - [[`53cbf04`](https://gitlab.com/katalytic/katalytic-data/commit/53cbf0432bddac3f958be2c068a3d80e4a68e259)] add recursive_map(), sort_dict_by_keys_recursive()
 - [[`03767ca`](https://gitlab.com/katalytic/katalytic-data/commit/03767cac16935efbc459567f412a9d382d1a72d8)] add sort_dict_by_values_recursive()
 - [[`00d7045`](https://gitlab.com/katalytic/katalytic-data/commit/00d70456642dbfc4ecd7b32269a513dd6660723a)] add sort_recursive
 - [[`cb3b145`](https://gitlab.com/katalytic/katalytic-data/commit/cb3b145c1a7c08a6877744693690a981d7475691)] add xor, xor_with_idx
+- [[`5d107d9`](https://gitlab.com/katalytic/katalytic-data/commit/5d107d92b115a053b26d7a21aaddb623d4b1057d)] delete checks.py and tests. They were moved to katalytic-checks
 - [[`0b9be79`](https://gitlab.com/katalytic/katalytic-data/commit/0b9be79523d7fcdab4f93055ae9b8f0c56f1e595)] remove is_collection() and add is_iterable(), is_iterable_or_str(), is_iterator()
 - [[`d8d64aa`](https://gitlab.com/katalytic/katalytic-data/commit/d8d64aa37c1926303bc4f618bd0bd0fec23b5db4)] update as_sequence_of_dicts()
 ### fix
 - [[`a59bed1`](https://gitlab.com/katalytic/katalytic-data/commit/a59bed13380f4e1633e0515d4195361d6e4da7c8)] ImportError
 - [[`322a828`](https://gitlab.com/katalytic/katalytic-data/commit/322a82884728ae61ffc3b7bf88f2b2d801c6f197)] add missing import, use the correct kw arg
 - [[`7640b61`](https://gitlab.com/katalytic/katalytic-data/commit/7640b6192a19e0d2e2af8ea0e929ffe0d1e52daf)] dicts_share_value_order(), dicts_share_key_order()
 - [[`120950e`](https://gitlab.com/katalytic/katalytic-data/commit/120950ec78b1b2eba9535d06948b23bfa84a1593)] don't let python mix bools with 0 and 1
+- [[`e7f8161`](https://gitlab.com/katalytic/katalytic-data/commit/e7f81615643230c1384bea6cb8981d92898879cc)] release
+- [[`d25b099`](https://gitlab.com/katalytic/katalytic-data/commit/d25b09959d1a925d28399bc79f2644f2c6d197a7)] release
+- [[`a5944c0`](https://gitlab.com/katalytic/katalytic-data/commit/a5944c0bfa31e99e702333dd0862909b17a982a0)] release
+- [[`c05c712`](https://gitlab.com/katalytic/katalytic-data/commit/c05c71281084d8cbbba465415c88df689dd5d799)] release
+- [[`6b7ed67`](https://gitlab.com/katalytic/katalytic-data/commit/6b7ed670100f50728c00b6971137735ca0214221)] release
+- [[`11c54be`](https://gitlab.com/katalytic/katalytic-data/commit/11c54be3978ee6c2e1b8ef7f3f56802e2e631a69)] release
+- [[`122ece9`](https://gitlab.com/katalytic/katalytic-data/commit/122ece923011ab96e10023bae5a602b90025158b)] release
+- [[`6b7063f`](https://gitlab.com/katalytic/katalytic-data/commit/6b7063f694840f33f09a0ffd461a9868f365e03d)] release
+- [[`7bf31c7`](https://gitlab.com/katalytic/katalytic-data/commit/7bf31c71305029695de0a90f3546941863c98717)] release
+- [[`d377401`](https://gitlab.com/katalytic/katalytic-data/commit/d377401a2afb57ea1fe6270b27e01d50340175b8)] release
+- [[`cc167ec`](https://gitlab.com/katalytic/katalytic-data/commit/cc167ec169dbba15a46ba6ec1d39b99c673923f9)] release
 - [[`b144802`](https://gitlab.com/katalytic/katalytic-data/commit/b144802676ef160d297aa7b004a00d428f39fc1f)] rename recursive_map() -> map_recursive()
 - [[`15daadf`](https://gitlab.com/katalytic/katalytic-data/commit/15daadfc274b7de627a656dae8771ec5a7088662)] rename recursive_map() -> map_recursive()
 - [[`163f359`](https://gitlab.com/katalytic/katalytic-data/commit/163f359ada349a4cbcec44f1358dff2cf003b66c)] replace True with bool in map
 ### refactor
 - [[`b45f8c9`](https://gitlab.com/katalytic/katalytic-data/commit/b45f8c98fce269e9d4111b0e5f1381d3d7268fef)] call is_singleton()
 - [[`1eabb04`](https://gitlab.com/katalytic/katalytic-data/commit/1eabb045ba4ade3af6bfd54140e3f0e59ca81aad)] change arg names
 - [[`8293f3e`](https://gitlab.com/katalytic/katalytic-data/commit/8293f3ef6d8fd58b20e92791f5bb7a518e97a429)] is_iterable
@@ -40,58 +53,47 @@
 - [[`416e795`](https://gitlab.com/katalytic/katalytic-data/commit/416e7954e03f762ada53283c93f4f71dd7fa2ea9)] reposition a Test class
 - [[`e3fd9fe`](https://gitlab.com/katalytic/katalytic-data/commit/e3fd9feeb976e2cde6b5e5308a99a00e31ffe8cd)] simplify is_any_of
 
 
 ## 0.3.0 (2023-04-26)
 ### feat
 - [[`39cccc6`](https://gitlab.com/katalytic/katalytic-data/commit/39cccc664bd062e73fe80d63a21dedc8cffcb2d2)] add all_types_besides, flatten, flatten_recursive
-- [[`12706e2`](https://gitlab.com/katalytic/katalytic-data/commit/12706e2e40dc3127ca680c7121dd720e849d3fdc)] add are_equal
 - [[`fbe876b`](https://gitlab.com/katalytic/katalytic-data/commit/fbe876b80301be2ae917b93ee31954d576477af8)] add as_dict_of_lists(), and fix bugs in as_sequence_of_dicts() and as_sequence_of_sequences()
 - [[`2a4ac90`](https://gitlab.com/katalytic/katalytic-data/commit/2a4ac90ff94ced5ddbafc6d083d08a3720fb389c)] add as_sequence_of_dicts()
 - [[`ed4689c`](https://gitlab.com/katalytic/katalytic-data/commit/ed4689c231abf872c6f3fa130a286105548e69b1)] add as_sequence_of_sequences()
-- [[`f1222bf`](https://gitlab.com/katalytic/katalytic-data/commit/f1222bf4b6e54fe5361ad36a49534b1966a837b8)] add contains_all_of, contains_any_of, contains_none_of
 - [[`e17e02e`](https://gitlab.com/katalytic/katalytic-data/commit/e17e02e93bbc39c261a92c192fd1755d05a08873)] add detect_fronts, detect_fronts_positive, detect_fronts_negative
-- [[`32afee3`](https://gitlab.com/katalytic/katalytic-data/commit/32afee339e97a4dcb0238e76529ab26265f34db8)] add dicts_share_key_order() and dicts_share_value_order()
 - [[`a4f833b`](https://gitlab.com/katalytic/katalytic-data/commit/a4f833b15909de35a0940ea5e0656507e046218d)] add first_with_idx(), last_with_idx()
-- [[`1caaaba`](https://gitlab.com/katalytic/katalytic-data/commit/1caaaba0678f58725644736ec303385cfdc4fe70)] add is_any_of(), is_none_of()
-- [[`7b9b1b5`](https://gitlab.com/katalytic/katalytic-data/commit/7b9b1b55acde94f250399a42c01447bd787c7b5b)] add is_generator
-- [[`9caa741`](https://gitlab.com/katalytic/katalytic-data/commit/9caa741e7e273451e37cf2ee32cf1f25d3fa5c48)] add is_sequence() and is_sequence_or_str()
-- [[`d3fdf95`](https://gitlab.com/katalytic/katalytic-data/commit/d3fdf9576ff12bd3a717b2f393e4f24996c0bc2f)] add is_sequence_of_sequences(), is_sequence_of_dicts(), and is_dict_of_sequences()
-- [[`9a59d37`](https://gitlab.com/katalytic/katalytic-data/commit/9a59d37ee15047ddc250c55a2faaa2a577976dfa)] add is_sequence_of_sequences_uniform(), is_sequence_of_dicts_uniform(), is_dict_of_sequences_uniform()
-- [[`563dc12`](https://gitlab.com/katalytic/katalytic-data/commit/563dc12952da62e486efc769a68f4103a2dd55ee)] add is_singleton()
 - [[`eeee05f`](https://gitlab.com/katalytic/katalytic-data/commit/eeee05fba6ae67ab439fa4030a1fd1a3901d41a3)] add one(), first(), last()
 - [[`5183859`](https://gitlab.com/katalytic/katalytic-data/commit/51838594613e4f47e34a91be19cf16fbef22dc2f)] add pick_all, pick_all_besides, pick_any,
 - [[`53cbf04`](https://gitlab.com/katalytic/katalytic-data/commit/53cbf0432bddac3f958be2c068a3d80e4a68e259)] add recursive_map(), sort_dict_by_keys_recursive()
 - [[`03767ca`](https://gitlab.com/katalytic/katalytic-data/commit/03767cac16935efbc459567f412a9d382d1a72d8)] add sort_dict_by_values_recursive()
 - [[`00d7045`](https://gitlab.com/katalytic/katalytic-data/commit/00d70456642dbfc4ecd7b32269a513dd6660723a)] add sort_recursive
 - [[`cb3b145`](https://gitlab.com/katalytic/katalytic-data/commit/cb3b145c1a7c08a6877744693690a981d7475691)] add xor, xor_with_idx
-- [[`0b9be79`](https://gitlab.com/katalytic/katalytic-data/commit/0b9be79523d7fcdab4f93055ae9b8f0c56f1e595)] remove is_collection() and add is_iterable(), is_iterable_or_str(), is_iterator()
 - [[`d8d64aa`](https://gitlab.com/katalytic/katalytic-data/commit/d8d64aa37c1926303bc4f618bd0bd0fec23b5db4)] update as_sequence_of_dicts()
 ### fix
 - [[`a59bed1`](https://gitlab.com/katalytic/katalytic-data/commit/a59bed13380f4e1633e0515d4195361d6e4da7c8)] ImportError
 - [[`322a828`](https://gitlab.com/katalytic/katalytic-data/commit/322a82884728ae61ffc3b7bf88f2b2d801c6f197)] add missing import, use the correct kw arg
-- [[`7640b61`](https://gitlab.com/katalytic/katalytic-data/commit/7640b6192a19e0d2e2af8ea0e929ffe0d1e52daf)] dicts_share_value_order(), dicts_share_key_order()
 - [[`120950e`](https://gitlab.com/katalytic/katalytic-data/commit/120950ec78b1b2eba9535d06948b23bfa84a1593)] don't let python mix bools with 0 and 1
 - [[`b144802`](https://gitlab.com/katalytic/katalytic-data/commit/b144802676ef160d297aa7b004a00d428f39fc1f)] rename recursive_map() -> map_recursive()
 - [[`15daadf`](https://gitlab.com/katalytic/katalytic-data/commit/15daadfc274b7de627a656dae8771ec5a7088662)] rename recursive_map() -> map_recursive()
 - [[`163f359`](https://gitlab.com/katalytic/katalytic-data/commit/163f359ada349a4cbcec44f1358dff2cf003b66c)] replace True with bool in map
 ### refactor
 - [[`b45f8c9`](https://gitlab.com/katalytic/katalytic-data/commit/b45f8c98fce269e9d4111b0e5f1381d3d7268fef)] call is_singleton()
 - [[`1eabb04`](https://gitlab.com/katalytic/katalytic-data/commit/1eabb045ba4ade3af6bfd54140e3f0e59ca81aad)] change arg names
-- [[`8293f3e`](https://gitlab.com/katalytic/katalytic-data/commit/8293f3ef6d8fd58b20e92791f5bb7a518e97a429)] is_iterable
 - [[`4bad63c`](https://gitlab.com/katalytic/katalytic-data/commit/4bad63ca2bda10e41de30d6a1964f867cf395419)] rename are_equal to is_equal
 - [[`7d18c52`](https://gitlab.com/katalytic/katalytic-data/commit/7d18c529cc3db93717a00778e5fe488ff4fe3b7f)] rename are_equal to is_equal
 - [[`416e795`](https://gitlab.com/katalytic/katalytic-data/commit/416e7954e03f762ada53283c93f4f71dd7fa2ea9)] reposition a Test class
 - [[`e3fd9fe`](https://gitlab.com/katalytic/katalytic-data/commit/e3fd9feeb976e2cde6b5e5308a99a00e31ffe8cd)] simplify is_any_of
 
 
 ## 0.1.1 (2023-04-16)
 ## Fix
 * nothing
 
+
 ## 0.1.0 (2023-04-16)
 ### Feature
 * Add is_collection() ([`bf29261`](https://github.com/katalytic/katalytic-data/commit/bf2926172f56d000d1f09318ab212c7b9747a8b0))
 * Add is_primitive() ([`ed950cc`](https://github.com/katalytic/katalytic-data/commit/ed950ccdd8e4cd4d4439cb0ab9c763d55135461d))
 * Add sort_dict_by_values() ([`6b3c985`](https://github.com/katalytic/katalytic-data/commit/6b3c9856c69e088467087345743a38e6294def7a))
 * Add sort_dict_by_keys() ([`5c05e48`](https://github.com/katalytic/katalytic-data/commit/5c05e48c4cc8afaf6a861103784690ebc153dcc8))
 * Add map_dict_values() ([`ba289c5`](https://github.com/katalytic/katalytic-data/commit/ba289c5f5cb21ff66d89bb833f30e2be678e15da))
```

### Comparing `katalytic-data-0.4.0/LICENSE.txt` & `katalytic-data-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.4.0/README.md` & `katalytic-data-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.4.0/pyproject.toml` & `katalytic-data-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-data"
-version = "0.4.0"
+version = "0.5.0"
 description = "This plugin adds utilities for working with data to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -24,16 +24,16 @@
 	"high-level",
 	"data conversion",
 ]
 authors = [{name="Valentin Neagu", email="vali19th@protonmail.com"}]
 
 requires-python = ">=3.6"
 dependencies = [
-    "katalytic-pkg>=0.2.0",
     "katalytic-checks>=0.0.1",
+    "katalytic-pkg>=0.2.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov",
     "pytest-randomly",
@@ -42,27 +42,9 @@
 [project.urls]
 homepage = "https://gitlab.com/katalytic/katalytic-data.git"
 repository = "https://gitlab.com/katalytic/katalytic-data.git"
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
 
-[tool.tox]
-legacy_tox_ini = """
-[tox]
-env_list = py36, py37, py38, py39
-isolated_build = True
-
-[testenv]
-extras = dev
-deps = -e .
-
-commands = pytest --cov-fail-under=100 --cov=katalytic --cov-report term-missing
-"""
-
-[tool.semantic_release]
-version_variable = "pyproject.toml:version"
-branch = "main"
-
 [tool.flit.module]
 name = "katalytic.data"
-
```

### Comparing `katalytic-data-0.4.0/src/katalytic/data.py` & `katalytic-data-0.5.0/src/katalytic/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,24 +35,26 @@
 __sequences = [[], (), range(1)]
 __dict_views = [{}.keys(), {}.values(), {}.items()]
 __iterators = [_generator, _generator_expr, iter([]), map(int, ''), enumerate([]), zip([], [])]
 __iterables = [*__dict_views, *__iterators, *__sequences, set(), {}]
 __collections = [(), set(), frozenset([]), {}, []]
 __singletons = [None, True, False]
 __primitives = [*__singletons, 0, 0.0, '', b'', bytearray(b'')]
+__callables = [_generator, _function, _lambda, _C_obj]
 
 
 def all_types_besides(blacklist):
     if not is_iterable(blacklist):
         raise TypeError(f'<blacklist> must be iterable. Got {type(blacklist).__name__}')
 
     whitelist = {
         'bool': False,
         'bytearray': bytearray(b''),
         'bytes': b'',
+        'callables': __callables,
         'callable object': _C_obj,
         'class': _C,
         'collections': __collections,
         'complex': 0 + 0j,
         'decimal': Decimal('0'),
         'dict': {},
         'dict_views': __dict_views,
```

### Comparing `katalytic-data-0.4.0/tests/test_data.py` & `katalytic-data-0.5.0/tests/test_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def test_unexpected(self, unexpected):
         with pytest.raises(ValueError):
             all_types_besides(unexpected)
 
     @pytest.mark.parametrize('blacklist, expected', [
         (
             ['iterables'],
-            [False, bytearray(b''), b'', _C_obj, _C, 0j, Decimal('0'), 0, Fraction(0, 1), _function, _lambda, None, _obj, PosixPath('.'), True, 0.0, '']
+            [False, bytearray(b''), b'', _function, _lambda, _C_obj, _C, 0j, Decimal('0'), 0, Fraction(0, 1), None, _obj, PosixPath('.'), True, 0.0, '']
         ),
         (
             ['iterables', 'generators', 'functions', 'objects', 'path'],
             [False, bytearray(b''), b'', _C, 0j, Decimal('0'), 0, Fraction(0, 1), None, True, 0.0, '']
         ),
     ])
     def test_all_types_besides(self, blacklist, expected):
@@ -327,15 +327,20 @@
 
     @pytest.mark.parametrize('data, expected', [
         ((1, [(2, 3), (4, (5, 6))]), [1, (2, 3), (4, (5, 6))]),
         ([[1, (2, 3), (4, (5, 6))]], [1, (2, 3), (4, (5, 6))]),
         ({1, (2, 3), (4, (5, 6))}, [1, 2, 3, 4, (5, 6)]),
     ])
     def test_flattens_only_one_level(self, data, expected):
-        assert flatten(data) == expected
+        actual = flatten(data)
+        if isinstance(data, set):
+            actual = set(actual)
+            expected = set(expected)
+
+        assert actual == expected
 
 
 class Test_flatten_recursive:
     @pytest.mark.parametrize('wrong_type', [1, 1.0, True, False, None, '', object()])
     def test_should_be_an_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             flatten_recursive(wrong_type)
@@ -354,15 +359,20 @@
 
     @pytest.mark.parametrize('data, expected', [
         ((1, [(2, 3), (4, (5, 6))]), [1, 2, 3, 4, 5, 6]),
         ([[1, (2, 3), (4, (5, 6))]], [1, 2, 3, 4, 5, 6]),
         ({1, (2, 3), (4, (5, 6))}, [1, 2, 3, 4, 5, 6]),
     ])
     def test_flattens_all_levels(self, data, expected):
-        assert flatten_recursive(data) == expected
+        actual = flatten_recursive(data)
+        if isinstance(data, set):
+            actual = set(actual)
+            expected = set(expected)
+
+        assert actual == expected
 
 
 class Test_map_dict_keys:
     @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, None, False, 'string', object()])
     def test_mapping_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
             map_dict_keys(wrong_type, {})
```

### Comparing `katalytic-data-0.4.0/PKG-INFO` & `katalytic-data-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: katalytic-data
-Version: 0.4.0
+Version: 0.5.0
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Dist: katalytic-pkg>=0.2.0
 Requires-Dist: katalytic-checks>=0.0.1
+Requires-Dist: katalytic-pkg>=0.2.0
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-data.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-data.git
 Provides-Extra: dev
```


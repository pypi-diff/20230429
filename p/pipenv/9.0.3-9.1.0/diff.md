# Comparing `tmp/pipenv-9.0.3.tar.gz` & `tmp/pipenv-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pipenv-9.0.3.tar", last modified: Tue Jan 16 17:17:32 2018, max compression
+gzip compressed data, was "dist/pipenv-9.1.0.tar", last modified: Tue Feb 20 15:02:01 2018, max compression
```

## Comparing `pipenv-9.0.3.tar` & `pipenv-9.1.0.tar`

### file list

```diff
@@ -1,591 +1,585 @@
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:32.000000 pipenv-9.0.3/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    12083 2018-01-16 17:17:32.000000 pipenv-9.0.3/PKG-INFO
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    40754 2017-10-08 17:33:11.000000 pipenv-9.0.3/pipenv/pipenv.1
--rw-r--r--   0 kennethreitz   (501) admin       (80)      499 2017-09-28 17:43:43.000000 pipenv-9.0.3/pipenv/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      217 2018-01-16 17:17:17.000000 pipenv-9.0.3/pipenv/__version__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1222 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/pep508checker.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    92079 2018-01-16 17:16:10.000000 pipenv-9.0.3/pipenv/cli.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    47459 2018-01-16 17:16:10.000000 pipenv-9.0.3/pipenv/utils.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3181 2018-01-06 14:02:39.000000 pipenv-9.0.3/pipenv/environments.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5868 2017-09-30 13:19:31.000000 pipenv-9.0.3/pipenv/progress.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4364 2018-01-16 17:16:10.000000 pipenv-9.0.3/pipenv/patched/crayons.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/dotenv/
--rw-r--r--   0 kennethreitz   (501) admin       (80)      307 2017-11-29 18:44:07.000000 pipenv-9.0.3/pipenv/patched/dotenv/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2673 2017-11-29 18:44:07.000000 pipenv-9.0.3/pipenv/patched/dotenv/cli.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1293 2017-11-29 18:44:07.000000 pipenv-9.0.3/pipenv/patched/dotenv/ipython.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5759 2017-11-29 18:44:07.000000 pipenv-9.0.3/pipenv/patched/dotenv/main.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/piptools/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     5422 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/sync.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      128 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/click.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      846 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/logging.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)    21936 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/io.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     5501 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/cache.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/__init__.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/piptools/repositories/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2388 2017-10-06 13:44:19.000000 pipenv-9.0.3/pipenv/patched/piptools/repositories/local.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)       95 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/repositories/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     9746 2017-10-06 13:44:19.000000 pipenv-9.0.3/pipenv/patched/piptools/repositories/pypi.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1498 2017-10-06 13:44:19.000000 pipenv-9.0.3/pipenv/patched/piptools/repositories/base.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     6898 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/piptools/utils.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)    13314 2017-12-07 13:55:19.000000 pipenv-9.0.3/pipenv/patched/piptools/resolver.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/piptools/scripts/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3144 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/scripts/sync.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/scripts/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)    11421 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/piptools/scripts/compile.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1200 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/exceptions.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     6262 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/writer.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/piptools/_compat/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2826 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/_compat/tempfile.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      335 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/_compat/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     4562 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/_compat/contextlib.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      265 2017-09-27 17:39:10.000000 pipenv-9.0.3/pipenv/patched/piptools/__main__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      873 2017-11-29 18:44:07.000000 pipenv-9.0.3/pipenv/patched/piptools/locations.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/prettytoml/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)       19 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/_version.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/prettytoml/lexer/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     5192 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/lexer/test_lexer.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     4596 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/lexer/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3741 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/util.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      696 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1005 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/test_util.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/prettytoml/parser/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     4194 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/parser/test_parser.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      854 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/parser/tokenstream.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      838 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/parser/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2007 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/parser/elementsanitizer.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3837 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/parser/recdesc.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)    13563 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/parser/parser.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      439 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/parser/errors.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      384 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/test_prettifier.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2511 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/abstracttable.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2798 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_common.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2474 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/metadata.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1442 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_table.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      269 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_atomic.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2000 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_array.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      788 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_factory.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      897 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_metadata.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      371 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     5572 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/factory.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      410 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_tableheader.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2513 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/common.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/traversal/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1237 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/traversal/predicates.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     6725 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/traversal/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2898 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/inlinetable.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     4286 2017-09-25 20:59:41.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/table.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      354 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/errors.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3492 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/tableheader.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1792 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/atomic.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     4830 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/array.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1495 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_inlinetable.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      716 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_traversal.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      545 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/errors.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1518 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/deindentanonymoustable.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      524 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/test_tableindent.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1828 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/test_linelength.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1076 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/test_tableentrysort.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1280 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/tableassignment.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1353 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1627 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/tableindent.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1170 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/commentspace.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1343 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/tableentrysort.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      474 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/test_tablesep.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1568 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/common.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      512 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/test_commentspace.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      438 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/test_deindentanonymoustable.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      552 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/test_tableassignment.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1021 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/tablesep.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2265 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/linelength.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/prettytoml/tokens/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     4461 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/tokens/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3959 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/tokens/toml2py.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3150 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/tokens/test_toml2py.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      197 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/tokens/errors.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3052 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/prettytoml/tokens/test_py2toml.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     5046 2017-10-06 14:07:08.000000 pipenv-9.0.3/pipenv/patched/prettytoml/tokens/py2toml.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)        0 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/__init__.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    10465 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/baseparser.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/compat/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4912 2017-10-02 12:59:12.000000 pipenv-9.0.3/pipenv/patched/pip/compat/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    23096 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/compat/dictconfig.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    40552 2017-09-29 01:36:05.000000 pipenv-9.0.3/pipenv/patched/pip/index.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     9972 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/retrying.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    11556 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/version.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      513 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      421 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/utils.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4327 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/requirements.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1416 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/_structures.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     8230 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/markers.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      720 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/__about__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      860 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/_compat.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    28025 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    80176 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/ipaddress.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/webencodings/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     8979 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/webencodings/labels.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1305 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4306 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    10576 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     6562 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/webencodings/tests.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4094 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/ordereddict.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/progress/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3023 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/progress/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2685 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/progress/bar.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1314 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/progress/spinner.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2854 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/progress/helpers.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1502 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/progress/counter.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/_backport/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    25647 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/_backport/shutil.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      971 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/_backport/misc.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      274 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/_backport/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    92628 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/_backport/tarfile.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    26955 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/_backport/sysconfig.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    51013 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/locators.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    38833 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/metadata.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    23711 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/version.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    40801 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/compat.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    21085 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/index.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    14810 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/manifest.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    52991 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/util.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    49672 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/database.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      581 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     6282 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/markers.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    10766 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/resources.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    15224 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/scripts.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    39115 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/wheel.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/colorama/
--rw-r--r--   0 kennethreitz   (501) admin       (80)      240 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/colorama/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5365 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/colorama/win32.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     9668 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2524 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/colorama/ansi.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     6290 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/colorama/winterm.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1917 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/colorama/initialise.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/lockfile/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5506 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/lockfile/sqlitelockfile.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     9371 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/lockfile/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2652 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/lockfile/linklockfile.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3096 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/lockfile/mkdirlockfile.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2616 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/lockfile/symlinklockfile.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     6090 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/lockfile/pidlockfile.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     6536 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      498 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    13024 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      416 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2531 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4141 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4608 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      790 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      302 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1320 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/_cmd.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/caches/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3532 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      369 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      973 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4670 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/__init__.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    18208 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/cookies.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     8175 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/auth.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    25609 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/sessions.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      767 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/hooks.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1687 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/compat.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    30532 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/models.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      625 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/certs.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2326 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3316 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/status_codes.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5794 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/api.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    24163 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/utils.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    12536 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/langhungarianmodel.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    19590 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/mbcssm.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    11275 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/langthaimodel.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1157 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/compat.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    12784 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/langbulgarianmodel.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1675 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/euckrprober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3764 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/sjisprober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1782 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/cp949prober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1335 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/constants.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1295 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    34872 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/euctwfreq.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    11318 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/langhebrewmodel.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     9226 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/chardistribution.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5232 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/latin1prober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1902 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/charsetprober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1681 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/gb2312prober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3268 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/mbcharsetprober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    17725 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/langcyrillicmodel.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1676 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/euctwprober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2318 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/codingstatemachine.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3187 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/escprober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     6840 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/universaldetector.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2652 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/utf8prober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    36011 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/gb2312freq.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1967 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/mbcsgroupprober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2504 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/chardetect.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    12628 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/langgreekmodel.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3678 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/eucjpprober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    47315 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/jisfreq.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     7839 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/escsm.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4793 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/sbcharsetprober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    82594 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/big5freq.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    45978 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/euckrfreq.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1684 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/big5prober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    13359 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/hebrewprober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3791 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/charsetgroupprober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3291 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/sbcsgroupprober.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    19348 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/jpcntx.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1384 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/__init__.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2320 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/filepost.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5931 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/fields.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2128 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/request.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     9596 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/timeout.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      892 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2165 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/response.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    11622 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/ssl_.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    10664 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/retry.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5879 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/url.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4744 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/connection.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5988 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/request.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2852 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    13092 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/poolmanager.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    18615 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/response.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/
--rw-r--r--   0 kennethreitz   (501) admin       (80)        0 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5668 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/socks.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    11778 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     7937 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/appengine.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4531 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    11617 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/connection.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    10553 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/_collections.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/
--rw-r--r--   0 kennethreitz   (501) admin       (80)      109 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     8935 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/ordered_dict.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    30098 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/six.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/ssl_match_hostname/
--rw-r--r--   0 kennethreitz   (501) admin       (80)      460 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3778 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5599 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/exceptions.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    33591 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/connectionpool.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2860 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/exceptions.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)   344712 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/cacert.pem
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3012 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/structures.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    19740 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/adapters.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    22368 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/appdirs.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    25112 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/sanitizer.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2742 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/inject_meta_charset.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)        0 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      286 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/base.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      621 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/alphabeticalattributes.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    10534 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/optionaltags.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3365 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/lint.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1139 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/whitespace.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treewalkers/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     6309 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treewalkers/etree_lxml.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5544 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treewalkers/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4684 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treewalkers/etree.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2309 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treewalkers/genshi.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4939 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treewalkers/base.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1413 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treewalkers/dom.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treebuilders/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    14161 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treebuilders/etree_lxml.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3406 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treebuilders/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    12764 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treebuilders/etree.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    13942 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treebuilders/base.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     8835 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treebuilders/dom.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    32532 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_inputstream.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    16705 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_ihatexml.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    83387 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/constants.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)   117170 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/html5parser.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      780 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/__init__.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_trie/
--rw-r--r--   0 kennethreitz   (501) admin       (80)      979 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_trie/_base.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1178 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_trie/datrie.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      289 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_trie/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1775 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_trie/py.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treeadapters/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1661 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treeadapters/sax.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      208 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treeadapters/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1555 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treeadapters/genshi.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    14177 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/serializer.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    76580 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_tokenizer.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4096 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_utils.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    30098 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/six.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    38349 2017-09-28 23:15:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/distro.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/pkg_resources/
--rw-r--r--   0 kennethreitz   (501) admin       (80)   104325 2017-10-02 13:02:06.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      773 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/re-vendor.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)   224171 2017-09-28 23:15:32.000000 pipenv-9.0.3/pipenv/patched/pip/_vendor/pyparsing.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    16474 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/cmdoptions.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    32186 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/download.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)    11348 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      156 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/status_codes.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/utils/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1312 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/utils/build.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3327 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/utils/logging.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      971 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/utils/encoding.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2232 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/utils/deprecation.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    11597 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/utils/ui.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      899 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/utils/filesystem.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    27202 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/utils/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     8811 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/utils/appdirs.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      278 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/utils/setuptools_build.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2088 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/utils/packaging.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5455 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/utils/outdated.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2866 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/utils/hashes.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2939 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/utils/glibc.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/models/
--rw-r--r--   0 kennethreitz   (501) admin       (80)      487 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/models/index.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)       71 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/models/__init__.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/operations/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1590 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/operations/check.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)        0 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/operations/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5194 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/operations/freeze.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/req/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    46531 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/req/req_install.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    35581 2017-12-07 13:53:51.000000 pipenv-9.0.3/pipenv/patched/pip/req/req_set.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     6897 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/req/req_uninstall.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      276 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/req/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    11926 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/req/req_file.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/vcs/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    11197 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/vcs/git.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    12374 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/vcs/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3472 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/vcs/mercurial.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3803 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/vcs/bazaar.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     9350 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/vcs/subversion.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    10980 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/pep425tags.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     8121 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/exceptions.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/pip/commands/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5891 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/commands/show.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    11369 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/commands/list.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1382 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/commands/check.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2453 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/commands/completion.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     7810 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/commands/download.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2244 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/commands/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1597 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/commands/hash.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2884 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/commands/uninstall.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2835 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/commands/freeze.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4502 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/commands/search.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    17412 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/commands/install.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      982 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/commands/help.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     7729 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/commands/wheel.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    11910 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/basecommand.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      584 2017-09-28 23:15:30.000000 pipenv-9.0.3/pipenv/patched/pip/__main__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5626 2017-09-28 23:15:33.000000 pipenv-9.0.3/pipenv/patched/pip/locations.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    32046 2017-09-28 23:15:34.000000 pipenv-9.0.3/pipenv/patched/pip/wheel.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)  2208871 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/safety.zip
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/contoml/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)       19 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/_version.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/patched/contoml/file/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1707 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/file/cascadedict.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      333 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/file/test_peekableit.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1550 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/file/test_structurer.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3703 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/file/toplevels.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      455 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/file/raw.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      640 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/file/test_cascadedict.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)       29 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/file/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1226 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/file/freshtable.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     9881 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/file/file.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      573 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/file/test_entries.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      673 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/file/peekableit.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1501 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/file/array.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3989 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/file/structurer.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1226 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/patched/contoml/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)       59 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/__main__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    17449 2018-01-16 17:16:10.000000 pipenv-9.0.3/pipenv/project.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/vendor/
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/vendor/click_didyoumean/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1963 2017-02-13 15:52:52.000000 pipenv-9.0.3/pipenv/vendor/click_didyoumean/__init__.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/vendor/concurrent27/
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/vendor/concurrent27/futures/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    22424 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/concurrent27/futures/_base.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5094 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/concurrent27/futures/thread.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      893 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/concurrent27/futures/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    14988 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/concurrent27/futures/process.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)       76 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/concurrent27/__init__.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:32.000000 pipenv-9.0.3/pipenv/vendor/pytoml/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)       92 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/pytoml/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      509 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/pytoml/core.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)    10542 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/pytoml/parser.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3815 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/pytoml/writer.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:32.000000 pipenv-9.0.3/pipenv/vendor/markupsafe/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4795 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/markupsafe/_constants.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    10697 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/markupsafe/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1187 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/markupsafe/_native.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      565 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/markupsafe/_compat.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    10139 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/semver.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/vendor/iso8601/
--rw-r--r--   0 kennethreitz   (501) admin       (80)       23 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/iso8601/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     6670 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/iso8601/iso8601.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     7802 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/iso8601/test_iso8601.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    19784 2017-09-24 00:33:13.000000 pipenv-9.0.3/pipenv/vendor/docopt.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:32.000000 pipenv-9.0.3/pipenv/vendor/jinja2/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     7765 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/asyncsupport.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    62929 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/compiler.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)   589381 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/_stringdefs.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1626 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/constants.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    17382 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/loaders.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2565 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     8760 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/idtracking.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    26787 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/jinja2/runtime.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    35465 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/jinja2/parser.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    16707 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/jinja2/sandbox.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3316 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/jinja2/visitor.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    19941 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/jinja2/utils.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    12038 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/debug.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    28238 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/lexer.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    50848 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/environment.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1722 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/jinja2/optimizer.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4428 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/exceptions.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1323 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/defaults.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2596 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/_compat.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    29392 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/jinja2/nodes.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4428 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/jinja2/tests.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    12793 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/bccache.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    33424 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/filters.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    23867 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/ext.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4340 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/jinja2/meta.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4144 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/jinja2/asyncfilters.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/vendor/blindspin/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1934 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/blindspin/__init__.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/vendor/colorama/
--rw-r--r--   0 kennethreitz   (501) admin       (80)      240 2017-09-26 14:52:44.000000 pipenv-9.0.3/pipenv/vendor/colorama/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5365 2017-09-26 14:52:44.000000 pipenv-9.0.3/pipenv/vendor/colorama/win32.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     9668 2017-09-26 14:52:44.000000 pipenv-9.0.3/pipenv/vendor/colorama/ansitowin32.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2524 2017-09-26 14:52:44.000000 pipenv-9.0.3/pipenv/vendor/colorama/ansi.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     6290 2017-09-26 14:52:44.000000 pipenv-9.0.3/pipenv/vendor/colorama/winterm.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1917 2017-09-26 14:52:44.000000 pipenv-9.0.3/pipenv/vendor/colorama/initialise.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/vendor/fuzzywuzzy/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2437 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/fuzzywuzzy/StringMatcher.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)       47 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/fuzzywuzzy/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      780 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/fuzzywuzzy/string_processing.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2422 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/fuzzywuzzy/utils.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)    12569 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/fuzzywuzzy/process.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)    10561 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/fuzzywuzzy/fuzz.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     7094 2017-11-16 14:43:17.000000 pipenv-9.0.3/pipenv/vendor/delegator.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      879 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/background.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/vendor/click/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     7790 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/_winconsole.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4204 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/_unicodefun.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1198 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/_textwrap.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1515 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/globals.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2858 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    70254 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/core.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    18864 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/types.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     8889 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/formatting.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    15510 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/parser.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    21008 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/termui.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    14916 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/utils.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2423 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/_bashcomplete.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     6788 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/exceptions.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    21011 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/_compat.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    16395 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/_termui_impl.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    11002 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/testing.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    10941 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click/decorators.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)        0 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/__init__.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:32.000000 pipenv-9.0.3/pipenv/vendor/yarg/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     9990 2014-08-10 21:17:24.000000 pipenv-9.0.3/pipenv/vendor/yarg/package.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4298 2014-08-09 11:43:30.000000 pipenv-9.0.3/pipenv/vendor/yarg/release.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2122 2014-08-10 21:17:00.000000 pipenv-9.0.3/pipenv/vendor/yarg/client.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1959 2014-08-10 20:35:44.000000 pipenv-9.0.3/pipenv/vendor/yarg/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      188 2014-08-11 21:59:13.000000 pipenv-9.0.3/pipenv/vendor/yarg/__about__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2050 2014-08-09 11:47:15.000000 pipenv-9.0.3/pipenv/vendor/yarg/exceptions.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5406 2014-08-11 21:58:23.000000 pipenv-9.0.3/pipenv/vendor/yarg/parse.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:32.000000 pipenv-9.0.3/pipenv/vendor/requirements/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     8024 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/requirements/requirement.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      353 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/requirements/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1789 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/requirements/parser.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1298 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/requirements/fragment.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      405 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/requirements/vcs.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:32.000000 pipenv-9.0.3/pipenv/vendor/shutilwhich/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2202 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/shutilwhich/lib.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      205 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/shutilwhich/__init__.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/vendor/backports/
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/vendor/backports/shutil_get_terminal_size/
--rw-r--r--   0 kennethreitz   (501) admin       (80)      338 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/backports/shutil_get_terminal_size/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2913 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/backports/shutil_get_terminal_size/get_terminal_size.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)       75 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/backports/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    24720 2017-11-16 14:43:17.000000 pipenv-9.0.3/pipenv/vendor/appdirs.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:32.000000 pipenv-9.0.3/pipenv/vendor/pipfile/
--rw-r--r--   0 kennethreitz   (501) admin       (80)      409 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/pipfile/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5670 2017-09-30 13:16:15.000000 pipenv-9.0.3/pipenv/vendor/pipfile/api.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      681 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/pipfile/__about__.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:32.000000 pipenv-9.0.3/pipenv/vendor/pexpect/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    13716 2017-11-16 14:43:17.000000 pipenv-9.0.3/pipenv/vendor/pexpect/screen.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5665 2017-09-28 13:33:00.000000 pipenv-9.0.3/pipenv/vendor/pexpect/popen_spawn.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     6632 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/pexpect/run.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    10665 2017-11-16 14:43:17.000000 pipenv-9.0.3/pipenv/vendor/pexpect/expect.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5170 2017-09-28 13:33:00.000000 pipenv-9.0.3/pipenv/vendor/pexpect/replwrap.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    20641 2017-11-16 14:43:17.000000 pipenv-9.0.3/pipenv/vendor/pexpect/spawnbase.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    18876 2017-11-16 14:43:17.000000 pipenv-9.0.3/pipenv/vendor/pexpect/pxssh.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     3902 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/pexpect/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     5626 2017-11-16 14:43:17.000000 pipenv-9.0.3/pipenv/vendor/pexpect/fdpexpect.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     4942 2017-09-28 13:33:00.000000 pipenv-9.0.3/pipenv/vendor/pexpect/utils.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2621 2017-11-16 14:43:17.000000 pipenv-9.0.3/pipenv/vendor/pexpect/_async.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1068 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/pexpect/exceptions.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    12177 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/pexpect/ANSI.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    35090 2017-11-16 14:43:17.000000 pipenv-9.0.3/pipenv/vendor/pexpect/pty_spawn.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    13419 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/pexpect/FSM.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1733 2017-09-28 19:59:08.000000 pipenv-9.0.3/pipenv/vendor/first.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    54693 2017-11-16 14:43:17.000000 pipenv-9.0.3/pipenv/vendor/pathlib2.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:32.000000 pipenv-9.0.3/pipenv/vendor/ptyprocess/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2700 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/ptyprocess/util.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2328 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/ptyprocess/_fork_pty.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    30587 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/ptyprocess/ptyprocess.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      138 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/ptyprocess/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    30098 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/six.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:32.000000 pipenv-9.0.3/pipenv/vendor/pipreqs/
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)    26296 2017-06-30 12:37:40.000000 pipenv-9.0.3/pipenv/vendor/pipreqs/mapping
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)    13981 2017-06-30 12:37:40.000000 pipenv-9.0.3/pipenv/vendor/pipreqs/pipreqs.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)      118 2017-06-30 12:37:40.000000 pipenv-9.0.3/pipenv/vendor/pipreqs/__init__.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)    12204 2017-06-30 12:37:40.000000 pipenv-9.0.3/pipenv/vendor/pipreqs/stdlib
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv/vendor/Levenshtein/
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2198 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/Levenshtein/StringMatcher.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      112 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/Levenshtein/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    16099 2017-09-23 23:42:39.000000 pipenv-9.0.3/pipenv/vendor/click_completion.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)    43969 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/parse.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      182 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/timestamp.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     6150 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/strict_rfc3339.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    18922 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/pipdeptree.py
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:32.000000 pipenv-9.0.3/pipenv/vendor/psutil/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    31855 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/psutil/_pswindows.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    13658 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/psutil/_common.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    84917 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/psutil/__init__.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    15116 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/psutil/_psosx.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    29489 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/psutil/_psbsd.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    70357 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/psutil/_pslinux.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     8170 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/psutil/_compat.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     6283 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/psutil/_psposix.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)    24905 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/psutil/_pssunos.py
--rwxr-xr-x   0 kennethreitz   (501) admin       (80)    30910 2017-09-23 23:42:40.000000 pipenv-9.0.3/pipenv/vendor/toml.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)     1076 2017-09-23 23:42:39.000000 pipenv-9.0.3/LICENSE
--rw-r--r--   0 kennethreitz   (501) admin       (80)      227 2017-11-16 14:43:17.000000 pipenv-9.0.3/MANIFEST.in
--rw-r--r--   0 kennethreitz   (501) admin       (80)      179 2017-11-29 18:44:07.000000 pipenv-9.0.3/NOTICES
--rw-r--r--   0 kennethreitz   (501) admin       (80)     2790 2017-12-07 13:53:51.000000 pipenv-9.0.3/setup.py
--rw-r--r--   0 kennethreitz   (501) admin       (80)      196 2018-01-16 17:17:32.000000 pipenv-9.0.3/setup.cfg
--rw-r--r--   0 kennethreitz   (501) admin       (80)    20114 2018-01-16 17:16:41.000000 pipenv-9.0.3/HISTORY.txt
--rw-r--r--   0 kennethreitz   (501) admin       (80)     9241 2018-01-16 17:16:10.000000 pipenv-9.0.3/README.rst
-drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv.egg-info/
--rw-r--r--   0 kennethreitz   (501) admin       (80)    12083 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv.egg-info/PKG-INFO
--rw-r--r--   0 kennethreitz   (501) admin       (80)       66 2017-09-23 23:39:33.000000 pipenv-9.0.3/pipenv.egg-info/requires 2.txt
--rw-r--r--   0 kennethreitz   (501) admin       (80)    11455 2017-09-23 22:23:30.000000 pipenv-9.0.3/pipenv.egg-info/PKG-INFO 2
--rw-r--r--   0 kennethreitz   (501) admin       (80)    22698 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv.egg-info/SOURCES.txt
--rw-r--r--   0 kennethreitz   (501) admin       (80)       39 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv.egg-info/entry_points.txt
--rw-r--r--   0 kennethreitz   (501) admin       (80)    21245 2017-09-23 22:23:30.000000 pipenv-9.0.3/pipenv.egg-info/SOURCES 2.txt
--rw-r--r--   0 kennethreitz   (501) admin       (80)    21236 2017-09-23 23:39:33.000000 pipenv-9.0.3/pipenv.egg-info/SOURCES 3.txt
--rw-r--r--   0 kennethreitz   (501) admin       (80)       20 2017-09-23 23:39:33.000000 pipenv-9.0.3/pipenv.egg-info/top_level 2.txt
--rw-r--r--   0 kennethreitz   (501) admin       (80)       80 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv.egg-info/requires.txt
--rw-r--r--   0 kennethreitz   (501) admin       (80)        7 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv.egg-info/top_level.txt
--rw-r--r--   0 kennethreitz   (501) admin       (80)        1 2018-01-16 17:17:31.000000 pipenv-9.0.3/pipenv.egg-info/dependency_links.txt
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11915 2018-02-20 15:02:01.000000 pipenv-9.1.0/PKG-INFO
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    40758 2018-02-20 12:37:30.000000 pipenv-9.1.0/pipenv/pipenv.1
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      499 2017-09-28 17:43:43.000000 pipenv-9.1.0/pipenv/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    78176 2018-02-20 12:45:13.000000 pipenv-9.1.0/pipenv/core.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      217 2018-02-17 13:05:00.000000 pipenv-9.1.0/pipenv/__version__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1222 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/pep508checker.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    18252 2018-02-20 12:37:30.000000 pipenv-9.1.0/pipenv/cli.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    34194 2018-02-17 12:54:17.000000 pipenv-9.1.0/pipenv/utils.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3181 2018-01-06 14:02:39.000000 pipenv-9.1.0/pipenv/environments.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5868 2017-09-30 13:19:31.000000 pipenv-9.1.0/pipenv/progress.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4365 2018-02-04 15:37:06.000000 pipenv-9.1.0/pipenv/patched/crayons.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/dotenv/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      199 2018-02-04 15:37:06.000000 pipenv-9.1.0/pipenv/patched/dotenv/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2673 2017-11-29 18:44:07.000000 pipenv-9.1.0/pipenv/patched/dotenv/cli.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5862 2018-02-17 12:54:17.000000 pipenv-9.1.0/pipenv/patched/dotenv/main.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2596 2018-02-17 12:54:17.000000 pipenv-9.1.0/pipenv/patched/dotenv/test_main.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/piptools/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     5422 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/sync.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      128 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/click.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      846 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/logging.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)    21936 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/io.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     5501 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/cache.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/__init__.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/piptools/repositories/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2388 2017-10-06 13:44:19.000000 pipenv-9.1.0/pipenv/patched/piptools/repositories/local.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)       95 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/repositories/__init__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     9746 2017-10-06 13:44:19.000000 pipenv-9.1.0/pipenv/patched/piptools/repositories/pypi.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1498 2017-10-06 13:44:19.000000 pipenv-9.1.0/pipenv/patched/piptools/repositories/base.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     6898 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/piptools/utils.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)    13314 2017-12-07 13:55:19.000000 pipenv-9.1.0/pipenv/patched/piptools/resolver.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/piptools/scripts/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3144 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/scripts/sync.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/scripts/__init__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)    11421 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/piptools/scripts/compile.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1200 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/exceptions.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     6262 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/writer.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/piptools/_compat/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2826 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/_compat/tempfile.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      335 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/_compat/__init__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     4562 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/_compat/contextlib.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      265 2017-09-27 17:39:10.000000 pipenv-9.1.0/pipenv/patched/piptools/__main__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      873 2017-11-29 18:44:07.000000 pipenv-9.1.0/pipenv/patched/piptools/locations.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/prettytoml/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)       19 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/_version.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/prettytoml/lexer/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     5192 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/lexer/test_lexer.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     4596 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/lexer/__init__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3741 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/util.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      696 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/__init__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1005 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/test_util.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/prettytoml/parser/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     4194 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/parser/test_parser.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      854 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/parser/tokenstream.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      838 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/parser/__init__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2007 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/parser/elementsanitizer.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3837 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/parser/recdesc.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)    13563 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/parser/parser.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      439 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/parser/errors.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      384 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/test_prettifier.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2511 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/abstracttable.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2798 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_common.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2474 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/metadata.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1442 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_table.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      269 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_atomic.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2000 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_array.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      788 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_factory.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      897 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_metadata.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      371 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/__init__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     5572 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/factory.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      410 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_tableheader.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2513 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/common.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/traversal/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1237 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/traversal/predicates.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     6725 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/traversal/__init__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2898 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/inlinetable.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     4286 2017-09-25 20:59:41.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/table.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      354 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/errors.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3492 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/tableheader.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1792 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/atomic.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     4830 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/array.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1495 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_inlinetable.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      716 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_traversal.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      545 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/errors.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1518 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/deindentanonymoustable.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      524 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/test_tableindent.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1828 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/test_linelength.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1076 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/test_tableentrysort.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1280 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/tableassignment.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1353 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/__init__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1627 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/tableindent.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1170 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/commentspace.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1343 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/tableentrysort.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      474 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/test_tablesep.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1568 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/common.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      512 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/test_commentspace.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      438 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/test_deindentanonymoustable.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      552 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/test_tableassignment.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1021 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/tablesep.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     2265 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/linelength.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/prettytoml/tokens/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     4461 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/tokens/__init__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3959 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/tokens/toml2py.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3150 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/tokens/test_toml2py.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      197 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/tokens/errors.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3052 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/prettytoml/tokens/test_py2toml.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     5046 2017-10-06 14:07:08.000000 pipenv-9.1.0/pipenv/patched/prettytoml/tokens/py2toml.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)        0 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/__init__.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    10465 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/baseparser.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/compat/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4912 2017-10-02 12:59:12.000000 pipenv-9.1.0/pipenv/patched/pip/compat/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    23096 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/compat/dictconfig.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    40552 2017-09-29 01:36:05.000000 pipenv-9.1.0/pipenv/patched/pip/index.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     9972 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/retrying.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11556 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/version.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      513 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      421 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/utils.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4327 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1416 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     8230 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/markers.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      720 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      860 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/_compat.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    28025 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    80176 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/ipaddress.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/webencodings/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     8979 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1305 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4306 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    10576 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     6562 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4094 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/ordereddict.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/progress/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3023 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/progress/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2685 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/progress/bar.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1314 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/progress/spinner.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2854 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/progress/helpers.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1502 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/progress/counter.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/_backport/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    25647 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/_backport/shutil.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      971 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/_backport/misc.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      274 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/_backport/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    92628 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/_backport/tarfile.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    26955 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/_backport/sysconfig.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    51013 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/locators.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    38833 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    23711 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/version.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    40801 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/compat.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    21085 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/index.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    14810 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    52991 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/util.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    49672 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/database.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      581 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     6282 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/markers.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    10766 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/resources.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    15224 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    39115 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/wheel.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/colorama/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      240 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5365 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/colorama/win32.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     9668 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2524 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     6290 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1917 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/colorama/initialise.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/lockfile/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5506 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/lockfile/sqlitelockfile.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     9371 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/lockfile/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2652 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/lockfile/linklockfile.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3096 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/lockfile/mkdirlockfile.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2616 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/lockfile/symlinklockfile.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     6090 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/lockfile/pidlockfile.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     6536 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      498 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    13024 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      416 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2531 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4141 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4608 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      790 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      302 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1320 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/_cmd.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/caches/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3532 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      369 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      973 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4670 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/__init__.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    18208 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/cookies.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     8175 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/auth.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    25609 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/sessions.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      767 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/hooks.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1687 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/compat.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    30532 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/models.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      625 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/certs.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2326 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3316 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5794 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/api.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    24163 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/utils.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    12536 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/langhungarianmodel.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    19590 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/mbcssm.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11275 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/langthaimodel.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1157 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/compat.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    12784 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/langbulgarianmodel.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1675 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/euckrprober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3764 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/sjisprober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1782 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/cp949prober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1335 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/constants.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1295 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    34872 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/euctwfreq.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11318 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/langhebrewmodel.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     9226 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/chardistribution.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5232 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/latin1prober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1902 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/charsetprober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1681 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/gb2312prober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3268 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/mbcharsetprober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    17725 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/langcyrillicmodel.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1676 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/euctwprober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2318 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/codingstatemachine.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3187 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/escprober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     6840 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/universaldetector.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2652 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/utf8prober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    36011 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/gb2312freq.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1967 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/mbcsgroupprober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2504 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/chardetect.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    12628 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/langgreekmodel.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3678 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/eucjpprober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    47315 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/jisfreq.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     7839 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/escsm.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4793 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/sbcharsetprober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    82594 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/big5freq.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    45978 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/euckrfreq.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1684 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/big5prober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    13359 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/hebrewprober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3791 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/charsetgroupprober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3291 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/sbcsgroupprober.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    19348 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/jpcntx.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1384 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/__init__.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2320 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/filepost.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5931 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/fields.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2128 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/request.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     9596 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/timeout.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      892 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2165 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/response.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11622 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/ssl_.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    10664 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/retry.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5879 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/url.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4744 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/connection.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5988 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/request.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2852 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    13092 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/poolmanager.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    18615 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/response.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)        0 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5668 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/socks.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11778 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     7937 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/appengine.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4531 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11617 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/connection.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    10553 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/_collections.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      109 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     8935 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/ordered_dict.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    30098 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/six.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/ssl_match_hostname/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      460 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3778 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5599 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/exceptions.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    33591 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/connectionpool.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2860 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)   344712 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/cacert.pem
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3012 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/structures.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    19740 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/adapters.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    22368 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/appdirs.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    25112 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/sanitizer.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2742 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/inject_meta_charset.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)        0 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      286 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/base.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      621 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/alphabeticalattributes.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    10534 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/optionaltags.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3365 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/lint.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1139 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/whitespace.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treewalkers/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     6309 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treewalkers/etree_lxml.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5544 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treewalkers/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4684 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treewalkers/etree.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2309 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treewalkers/genshi.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4939 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treewalkers/base.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1413 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treewalkers/dom.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treebuilders/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    14161 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treebuilders/etree_lxml.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3406 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treebuilders/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    12764 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treebuilders/etree.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    13942 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treebuilders/base.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     8835 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treebuilders/dom.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    32532 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_inputstream.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    16705 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_ihatexml.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    83387 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/constants.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)   117170 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/html5parser.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      780 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/__init__.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_trie/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      979 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_trie/_base.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1178 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_trie/datrie.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      289 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_trie/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1775 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_trie/py.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treeadapters/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1661 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treeadapters/sax.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      208 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treeadapters/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1555 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treeadapters/genshi.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    14177 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/serializer.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    76580 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_tokenizer.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4096 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_utils.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    30098 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/six.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    38349 2017-09-28 23:15:31.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/distro.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/pkg_resources/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)   104325 2017-10-02 13:02:06.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      773 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/re-vendor.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)   224171 2017-09-28 23:15:32.000000 pipenv-9.1.0/pipenv/patched/pip/_vendor/pyparsing.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    16474 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/cmdoptions.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    32186 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/download.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)    11348 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      156 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/status_codes.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/utils/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1312 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/utils/build.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3327 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/utils/logging.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      971 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/utils/encoding.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2232 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/utils/deprecation.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11597 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/utils/ui.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      899 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/utils/filesystem.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    27202 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/utils/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     8811 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/utils/appdirs.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      278 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/utils/setuptools_build.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2088 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/utils/packaging.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5455 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/utils/outdated.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2866 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/utils/hashes.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2939 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/utils/glibc.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/models/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      487 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/models/index.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)       71 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/models/__init__.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/operations/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1590 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/operations/check.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)        0 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/operations/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5194 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/operations/freeze.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/req/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    46531 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/req/req_install.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    35581 2017-12-07 13:53:51.000000 pipenv-9.1.0/pipenv/patched/pip/req/req_set.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     6897 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/req/req_uninstall.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      276 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/req/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11926 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/req/req_file.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/vcs/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11197 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/vcs/git.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    12374 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/vcs/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3472 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/vcs/mercurial.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3803 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/vcs/bazaar.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     9350 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/vcs/subversion.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    10980 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/pep425tags.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     8121 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/exceptions.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/pip/commands/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5891 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/commands/show.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11369 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/commands/list.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1382 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/commands/check.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2453 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/commands/completion.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     7810 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/commands/download.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2244 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/commands/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1597 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/commands/hash.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2884 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/commands/uninstall.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2835 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/commands/freeze.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4502 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/commands/search.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    17412 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/commands/install.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      982 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/commands/help.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     7729 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/commands/wheel.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11910 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/basecommand.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      584 2017-09-28 23:15:30.000000 pipenv-9.1.0/pipenv/patched/pip/__main__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5626 2017-09-28 23:15:33.000000 pipenv-9.1.0/pipenv/patched/pip/locations.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    32046 2017-09-28 23:15:34.000000 pipenv-9.1.0/pipenv/patched/pip/wheel.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)  2208871 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/safety.zip
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/contoml/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)       19 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/_version.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/patched/contoml/file/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1707 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/file/cascadedict.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      333 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/file/test_peekableit.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1550 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/file/test_structurer.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3703 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/file/toplevels.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      455 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/file/raw.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      640 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/file/test_cascadedict.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)       29 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/file/__init__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1226 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/file/freshtable.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     9881 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/file/file.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      573 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/file/test_entries.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      673 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/file/peekableit.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1501 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/file/array.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3989 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/file/structurer.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1226 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/patched/contoml/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)       59 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/__main__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    17724 2018-02-17 12:54:17.000000 pipenv-9.1.0/pipenv/project.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/click_didyoumean/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1963 2017-02-13 15:52:52.000000 pipenv-9.1.0/pipenv/vendor/click_didyoumean/__init__.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/concurrent27/
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/concurrent27/futures/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    22424 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/concurrent27/futures/_base.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5094 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/concurrent27/futures/thread.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      893 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/concurrent27/futures/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    14988 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/concurrent27/futures/process.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)       76 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/concurrent27/__init__.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/pytoml/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)       92 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/pytoml/__init__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      509 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/pytoml/core.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)    10542 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/pytoml/parser.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     3815 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/pytoml/writer.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/markupsafe/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4795 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/markupsafe/_constants.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    10697 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/markupsafe/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1187 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/markupsafe/_native.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      565 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/markupsafe/_compat.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    10139 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/semver.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/iso8601/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)       23 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/iso8601/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     6670 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/iso8601/iso8601.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     7802 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/iso8601/test_iso8601.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    19784 2017-09-24 00:33:13.000000 pipenv-9.1.0/pipenv/vendor/docopt.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/jinja2/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     7765 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/asyncsupport.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    62929 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/compiler.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)   589381 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/_stringdefs.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1626 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/constants.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    17382 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/loaders.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2565 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     8760 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/idtracking.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    26787 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/jinja2/runtime.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    35465 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/jinja2/parser.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    16707 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/jinja2/sandbox.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3316 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/jinja2/visitor.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    19941 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/jinja2/utils.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    12038 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/debug.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    28238 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/lexer.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    50848 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/environment.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1722 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/jinja2/optimizer.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4428 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/exceptions.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1323 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/defaults.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2596 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/_compat.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    29392 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/jinja2/nodes.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4428 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/jinja2/tests.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    12793 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/bccache.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    33424 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/filters.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    23867 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/ext.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4340 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/jinja2/meta.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4144 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/jinja2/asyncfilters.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/blindspin/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1934 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/blindspin/__init__.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/colorama/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      240 2017-09-26 14:52:44.000000 pipenv-9.1.0/pipenv/vendor/colorama/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5365 2017-09-26 14:52:44.000000 pipenv-9.1.0/pipenv/vendor/colorama/win32.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     9668 2017-09-26 14:52:44.000000 pipenv-9.1.0/pipenv/vendor/colorama/ansitowin32.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2524 2017-09-26 14:52:44.000000 pipenv-9.1.0/pipenv/vendor/colorama/ansi.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     6290 2017-09-26 14:52:44.000000 pipenv-9.1.0/pipenv/vendor/colorama/winterm.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1917 2017-09-26 14:52:44.000000 pipenv-9.1.0/pipenv/vendor/colorama/initialise.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     7094 2017-11-16 14:43:17.000000 pipenv-9.1.0/pipenv/vendor/delegator.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      879 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/background.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/click/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     7790 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/_winconsole.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4204 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/_unicodefun.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1198 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/_textwrap.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1515 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/globals.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2858 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    70254 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/core.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    18864 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/types.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     8889 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/formatting.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    15510 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/parser.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    21008 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/termui.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    14916 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/utils.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2423 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/_bashcomplete.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     6788 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/exceptions.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    21011 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/_compat.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    16395 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/_termui_impl.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11002 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/testing.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    10941 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click/decorators.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)        0 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/__init__.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/yarg/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     9990 2014-08-10 21:17:24.000000 pipenv-9.1.0/pipenv/vendor/yarg/package.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4298 2014-08-09 11:43:30.000000 pipenv-9.1.0/pipenv/vendor/yarg/release.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2122 2014-08-10 21:17:00.000000 pipenv-9.1.0/pipenv/vendor/yarg/client.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1959 2014-08-10 20:35:44.000000 pipenv-9.1.0/pipenv/vendor/yarg/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      188 2014-08-11 21:59:13.000000 pipenv-9.1.0/pipenv/vendor/yarg/__about__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2050 2014-08-09 11:47:15.000000 pipenv-9.1.0/pipenv/vendor/yarg/exceptions.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5406 2014-08-11 21:58:23.000000 pipenv-9.1.0/pipenv/vendor/yarg/parse.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/requirements/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     8024 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/requirements/requirement.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      353 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/requirements/__init__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1789 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/requirements/parser.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)     1298 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/requirements/fragment.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      405 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/requirements/vcs.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/shutilwhich/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2202 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/shutilwhich/lib.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      205 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/shutilwhich/__init__.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/backports/
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/backports/shutil_get_terminal_size/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      338 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/backports/shutil_get_terminal_size/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2913 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/backports/shutil_get_terminal_size/get_terminal_size.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)       75 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/backports/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    24720 2017-11-16 14:43:17.000000 pipenv-9.1.0/pipenv/vendor/appdirs.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/pipfile/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      409 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/pipfile/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5670 2017-09-30 13:16:15.000000 pipenv-9.1.0/pipenv/vendor/pipfile/api.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      681 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/pipfile/__about__.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/pexpect/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    13716 2017-11-16 14:43:17.000000 pipenv-9.1.0/pipenv/vendor/pexpect/screen.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5665 2017-09-28 13:33:00.000000 pipenv-9.1.0/pipenv/vendor/pexpect/popen_spawn.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     6632 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/pexpect/run.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    10665 2017-11-16 14:43:17.000000 pipenv-9.1.0/pipenv/vendor/pexpect/expect.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5170 2017-09-28 13:33:00.000000 pipenv-9.1.0/pipenv/vendor/pexpect/replwrap.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    20641 2017-11-16 14:43:17.000000 pipenv-9.1.0/pipenv/vendor/pexpect/spawnbase.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    18876 2017-11-16 14:43:17.000000 pipenv-9.1.0/pipenv/vendor/pexpect/pxssh.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     3902 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/pexpect/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     5626 2017-11-16 14:43:17.000000 pipenv-9.1.0/pipenv/vendor/pexpect/fdpexpect.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     4942 2017-09-28 13:33:00.000000 pipenv-9.1.0/pipenv/vendor/pexpect/utils.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2621 2017-11-16 14:43:17.000000 pipenv-9.1.0/pipenv/vendor/pexpect/_async.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1068 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/pexpect/exceptions.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    12177 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/pexpect/ANSI.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    35090 2017-11-16 14:43:17.000000 pipenv-9.1.0/pipenv/vendor/pexpect/pty_spawn.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    13419 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/pexpect/FSM.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1733 2017-09-28 19:59:08.000000 pipenv-9.1.0/pipenv/vendor/first.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    54693 2017-11-16 14:43:17.000000 pipenv-9.1.0/pipenv/vendor/pathlib2.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/ptyprocess/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2700 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/ptyprocess/util.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2328 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/ptyprocess/_fork_pty.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    30587 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/ptyprocess/ptyprocess.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      138 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/ptyprocess/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    30098 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/six.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/pipreqs/
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)    26296 2017-06-30 12:37:40.000000 pipenv-9.1.0/pipenv/vendor/pipreqs/mapping
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)    13981 2017-06-30 12:37:40.000000 pipenv-9.1.0/pipenv/vendor/pipreqs/pipreqs.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)      118 2017-06-30 12:37:40.000000 pipenv-9.1.0/pipenv/vendor/pipreqs/__init__.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)    12204 2017-06-30 12:37:40.000000 pipenv-9.1.0/pipenv/vendor/pipreqs/stdlib
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/Levenshtein/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2198 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/Levenshtein/StringMatcher.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      112 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/Levenshtein/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    16099 2017-09-23 23:42:39.000000 pipenv-9.1.0/pipenv/vendor/click_completion.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)    43969 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/parse.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      182 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/timestamp.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     6150 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/strict_rfc3339.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    18922 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/pipdeptree.py
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv/vendor/psutil/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    31855 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/psutil/_pswindows.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    13658 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/psutil/_common.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    84917 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/psutil/__init__.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    15116 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/psutil/_psosx.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    29489 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/psutil/_psbsd.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    70357 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/psutil/_pslinux.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     8170 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/psutil/_compat.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     6283 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/psutil/_psposix.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    24905 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/psutil/_pssunos.py
+-rwxr-xr-x   0 kennethreitz   (501) admin       (80)    30910 2017-09-23 23:42:40.000000 pipenv-9.1.0/pipenv/vendor/toml.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     1076 2017-09-23 23:42:39.000000 pipenv-9.1.0/LICENSE
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      227 2017-11-16 14:43:17.000000 pipenv-9.1.0/MANIFEST.in
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      179 2017-11-29 18:44:07.000000 pipenv-9.1.0/NOTICES
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     2790 2017-12-07 13:53:51.000000 pipenv-9.1.0/setup.py
+-rw-r--r--   0 kennethreitz   (501) admin       (80)      196 2018-02-20 15:02:01.000000 pipenv-9.1.0/setup.cfg
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    20581 2018-02-20 15:00:33.000000 pipenv-9.1.0/HISTORY.txt
+-rw-r--r--   0 kennethreitz   (501) admin       (80)     9121 2018-02-04 15:37:06.000000 pipenv-9.1.0/README.rst
+drwxr-xr-x   0 kennethreitz   (501) admin       (80)        0 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv.egg-info/
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11915 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv.egg-info/PKG-INFO
+-rw-r--r--   0 kennethreitz   (501) admin       (80)       66 2017-09-23 23:39:33.000000 pipenv-9.1.0/pipenv.egg-info/requires 2.txt
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    11455 2017-09-23 22:23:30.000000 pipenv-9.1.0/pipenv.egg-info/PKG-INFO 2
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    22487 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv.egg-info/SOURCES.txt
+-rw-r--r--   0 kennethreitz   (501) admin       (80)       39 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv.egg-info/entry_points.txt
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    21245 2017-09-23 22:23:30.000000 pipenv-9.1.0/pipenv.egg-info/SOURCES 2.txt
+-rw-r--r--   0 kennethreitz   (501) admin       (80)    21236 2017-09-23 23:39:33.000000 pipenv-9.1.0/pipenv.egg-info/SOURCES 3.txt
+-rw-r--r--   0 kennethreitz   (501) admin       (80)       20 2017-09-23 23:39:33.000000 pipenv-9.1.0/pipenv.egg-info/top_level 2.txt
+-rw-r--r--   0 kennethreitz   (501) admin       (80)       80 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv.egg-info/requires.txt
+-rw-r--r--   0 kennethreitz   (501) admin       (80)        7 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv.egg-info/top_level.txt
+-rw-r--r--   0 kennethreitz   (501) admin       (80)        1 2018-02-20 15:02:01.000000 pipenv-9.1.0/pipenv.egg-info/dependency_links.txt
```

### Comparing `pipenv-9.0.3/PKG-INFO` & `pipenv-9.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pipenv
-Version: 9.0.3
+Version: 9.1.0
 Summary: Python Development Workflow for Humans.
 Home-page: https://github.com/pypa/pipenv
 Author: Kenneth Reitz
 Author-email: me@kennethreitz.org
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: 
@@ -50,20 +50,14 @@
         Installation
         ------------
         
         ::
         
             $ pip install pipenv
         
-        Or if you are on macOS, you can install Pipenv via `Homebrew <https://brew.sh/>`_ with:
-        
-        ::
-        
-            $ brew install pipenv
-        
         ✨🍰✨
         
         ☤ User Testimonials
         -------------------
         
         **Jannis Leidel**, former pip maintainer—
             *Pipenv is the porcelain I always wanted to build for pip. It fits my brain and mostly replaces virtualenvwrapper and manual pip calls for me. Use it.*
```

### Comparing `pipenv-9.0.3/pipenv/pipenv.1` & `pipenv-9.1.0/pipenv/pipenv.1`

 * *Files 0% similar despite different names*

```diff
@@ -755,15 +755,15 @@
 \fB\-\-skip\-lock\fP — Ignore the \fBPipfile.lock\fP and install from the \fBPipfile\fP\&. In addition, do not write out a \fBPipfile.lock\fP reflecting changes to the \fBPipfile\fP\&.
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .SS $ pipenv uninstall
 .sp
 \fB$ pipenv uninstall\fP supports all of the parameters in \fI\%pipenv install\fP,
-as well as one additonal, \fB\-\-all\fP\&.
+as well as one additional, \fB\-\-all\fP\&.
 .INDENT 0.0
 .INDENT 3.5
 .INDENT 0.0
 .IP \(bu 2
 \fB\-\-all\fP — This parameter will purge all files from the virtual environment,
 but leave the Pipfile untouched.
 .UNINDENT
@@ -796,15 +796,15 @@
 .INDENT 0.0
 .INDENT 3.5
 The shell launched in interactive mode. This means that if your shell reads its configuration from a specific file for interactive mode (e.g. bash by default looks for a \fB~/.bashrc\fP configuration file for interactive mode), then you\(aqll need to modify (or create) this file.
 .UNINDENT
 .UNINDENT
 .SS ☤ A Note about VCS Dependencies
 .sp
-Pipenv will resolve the sub–depencies of VCS dependencies, but only if they are editable, like so:
+Pipenv will resolve the sub–dependencies of VCS dependencies, but only if they are editable, like so:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 [packages]
 requests = {git = "https://github.com/requests/requests.git", editable=true}
@@ -1174,15 +1174,15 @@
 \fBPIPENV_VENV_IN_PROJECT\fP — If set, use \fB\&.venv\fP in your project directory
 instead of the global virtualenv manager \fBpew\fP\&.
 .IP \(bu 2
 \fBPIPENV_COLORBLIND\fP — Disable terminal colors, for some reason.
 .IP \(bu 2
 \fBPIPENV_NOSPIN\fP — Disable terminal spinner, for cleaner logs. Automatically set in CI environments.
 .IP \(bu 2
-\fBPIPENV_MAX_DEPTH\fP — Set to an integer for the maximum number of directories to resursively
+\fBPIPENV_MAX_DEPTH\fP — Set to an integer for the maximum number of directories to recursively
 search for a Pipfile.
 .IP \(bu 2
 \fBPIPENV_TIMEOUT\fP — Set to an integer for the max number of seconds Pipenv will
 wait for virtualenv creation to complete.  Defaults to 120 seconds.
 .IP \(bu 2
 \fBPIPENV_IGNORE_VIRTUALENVS\fP — Set to disable automatically using an activated virtualenv over
 the current project\(aqs own virtual environment.
```

### Comparing `pipenv-9.0.3/pipenv/pep508checker.py` & `pipenv-9.1.0/pipenv/pep508checker.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/cli.py` & `pipenv-9.1.0/pipenv/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # -*- coding: utf-8 -*-
+
 import contextlib
 import codecs
+import logging
 import os
 import sys
 import shutil
+import shlex
 import signal
 import time
 import tempfile
 from glob import glob
 import json as simplejson
 
 import urllib3
@@ -15,36 +18,31 @@
 import click
 import click_completion
 import crayons
 import dotenv
 import delegator
 import pexpect
 import requests
-import pip
 import pipfile
 import pipdeptree
-import requirements
 import semver
 import flake8.main.cli
 from pipreqs import pipreqs
 from blindspin import spinner
 from urllib3.exceptions import InsecureRequestWarning
-from pip.req.req_file import parse_requirements
-from click_didyoumean import DYMCommandCollection
 from .project import Project
 from .utils import (
     convert_deps_from_pip, convert_deps_to_pip, is_required_version,
     proper_case, pep423_name, split_file, merge_deps, resolve_deps, shellquote, is_vcs,
-    python_version, suggest_package, find_windows_executable, is_file,
-    prepare_pip_source_args, temp_environ, is_valid_url, download_file,
-    get_requirement, need_update_check, touch_update_stamp
+    python_version, find_windows_executable, is_file, prepare_pip_source_args,
+    temp_environ, is_valid_url, download_file, get_requirement, need_update_check,
+    touch_update_stamp
 )
 from .__version__ import __version__
 from . import pep508checker, progress
-from . import environments
 from .environments import (
     PIPENV_COLORBLIND, PIPENV_NOSPIN, PIPENV_SHELL_FANCY,
     PIPENV_VENV_IN_PROJECT, PIPENV_TIMEOUT, PIPENV_SKIP_VALIDATION,
     PIPENV_HIDE_EMOJIS, PIPENV_INSTALL_TIMEOUT, PYENV_ROOT,
     PYENV_INSTALLED, PIPENV_YES, PIPENV_DONT_LOAD_ENV,
     PIPENV_DEFAULT_PYTHON_VERSION, PIPENV_MAX_SUBPROCESS,
     PIPENV_DONT_USE_PYENV, SESSION_IS_INTERACTIVE, PIPENV_USE_SYSTEM,
@@ -53,28 +51,14 @@
 
 # Backport required for earlier versions of Python.
 if sys.version_info < (3, 3):
     from backports.shutil_get_terminal_size import get_terminal_size
 else:
     from shutil import get_terminal_size
 
-xyzzy = """
- _______   __                                           __
-/       \ /  |                                         /  |
-$$$$$$$  |$$/   ______    ______   _______   __     __ $$ |
-$$ |__$$ |/  | /      \  /      \ /       \ /  \   /  |$$ |
-$$    $$/ $$ |/$$$$$$  |/$$$$$$  |$$$$$$$  |$$  \ /$$/ $$ |
-$$$$$$$/  $$ |$$ |  $$ |$$    $$ |$$ |  $$ | $$  /$$/  $$/
-$$ |      $$ |$$ |__$$ |$$$$$$$$/ $$ |  $$ |  $$ $$/    __
-$$ |      $$ |$$    $$/ $$       |$$ |  $$ |   $$$/    /  |
-$$/       $$/ $$$$$$$/   $$$$$$$/ $$/   $$/     $/     $$/
-              $$ |
-              $$ |
-              $$/
-"""
 
 # Packages that should be ignored later.
 BAD_PACKAGES = (
     'setuptools', 'pip', 'wheel', 'six', 'packaging', 'distribute'
     'pyparsing', 'appdirs',
 )
 
@@ -118,14 +102,15 @@
 # Disable warnings for Python 2.6.
 urllib3.disable_warnings(InsecureRequestWarning)
 
 project = Project()
 
 
 def load_dot_env():
+    """Loads .env file into sys.environ."""
     if not PIPENV_DONT_LOAD_ENV:
         # If the project doesn't exist yet, check current directory for a .env file
         project_directory = project.project_directory or '.'
 
         denv = dotenv.find_dotenv(PIPENV_DOTENV_LOCATION or os.sep.join([project_directory, '.env']))
         if os.path.isfile(denv):
             click.echo(crayons.normal('Loading .env environment variables…', bold=True), err=True)
@@ -226,14 +211,16 @@
             c = delegator.run('"{0}" install {1} pip --upgrade'.format(which_pip(), windows), block=False)
             click.echo(crayons.blue(c.out))
     except AttributeError:
         pass
 
 
 def import_requirements(r=None, dev=False):
+    import pip
+    from pip.req.req_file import parse_requirements
     # Parse requirements.txt file with Pip's parser.
     # Pip requires a `PipSession` which is a subclass of requests.Session.
     # Since we're not making any network calls, it's initialized to nothing.
 
     if r:
         assert os.path.isfile(r)
 
@@ -293,25 +280,25 @@
                 rs.append(r)
         pkg_names = pipreqs.get_pkg_names(rs)
         return [proper_case(r) for r in pkg_names]
     except Exception:
         return []
 
 
-def ensure_pipfile(validate=True):
+def ensure_pipfile(validate=True, skip_requirements=False):
     """Creates a Pipfile for the project, if it doesn't exist."""
 
     global USING_DEFAULT_PYTHON
 
     # Assert Pipfile exists.
     if project.pipfile_is_empty:
 
         # If there's a requirements file, but no Pipfile...
-        if project.requirements_exists:
-            click.echo(crayons.normal(u'Requirements.txt found, instead of Pipfile! Converting…', bold=True))
+        if project.requirements_exists and not skip_requirements:
+            click.echo(crayons.normal(u'requirements.txt found, instead of Pipfile! Converting…', bold=True))
 
             # Create a Pipfile...
             python = which('python') if not USING_DEFAULT_PYTHON else False
             project.create_pipfile(python=python)
 
             with spinner():
                 # Import requirements.txt.
@@ -391,14 +378,15 @@
             'You can specify specific versions of Python with:\n  {0}'.format(
                 crayons.red('$ pipenv --python {0}'.format(os.sep.join(('path', 'to', 'python'))))
             ), err=True
         )
         sys.exit(1)
 
     def activate_pyenv():
+        import pip
         """Adds all pyenv installations to the PATH."""
         if PYENV_INSTALLED:
             if PYENV_ROOT:
                 pyenv_paths = {}
                 for found in glob(
                     '{0}{1}versions{1}*'.format(
                         PYENV_ROOT,
@@ -460,18 +448,18 @@
                     # TODO: Keep this up to date!
                     # These versions appear incompatible with pew:
                     # '2.5': '2.5.6',
                     '2.6': '2.6.9',
                     '2.7': '2.7.14',
                     # '3.1': '3.1.5',
                     # '3.2': '3.2.6',
-                    '3.3': '3.3.6',
+                    '3.3': '3.3.7',
                     '3.4': '3.4.7',
                     '3.5': '3.5.4',
-                    '3.6': '3.6.3',
+                    '3.6': '3.6.4',
                 }
                 try:
                     if len(python.split('.')) == 2:
                         # Find the latest version of Python available.
 
                         version = version_map[python]
                     else:
@@ -597,17 +585,21 @@
         # Remove the virtualenv.
         cleanup_virtualenv(bare=True)
 
         # Call this function again.
         ensure_virtualenv(three=three, python=python, site_packages=site_packages)
 
 
-def ensure_project(three=None, python=None, validate=True, system=False, warn=True, site_packages=False, deploy=False):
+def ensure_project(three=None, python=None, validate=True, system=False, warn=True, site_packages=False, deploy=False, skip_requirements=False):
     """Ensures both Pipfile and virtualenv exist for the project."""
 
+    # Automatically use an activated virtualenv.
+    if PIPENV_USE_SYSTEM:
+        system = True
+
     if not project.pipfile_exists:
         project.touch_pipfile()
 
     # Skip virtualenv creation when --system was used.
     if not system:
         ensure_virtualenv(three=three, python=python, site_packages=site_packages)
 
@@ -635,15 +627,15 @@
                             err=True
                         )
                     else:
                         click.echo(crayons.red('Deploy aborted.'), err=True)
                         sys.exit(1)
 
     # Ensure the Pipfile exists.
-    ensure_pipfile(validate=validate)
+    ensure_pipfile(validate=validate, skip_requirements=skip_requirements)
 
 
 def ensure_proper_casing(pfile):
     """Ensures proper casing of Pipfile packages, writes changes to disk."""
 
     casing_changed = proper_case_section(pfile.get('packages', {}))
     casing_changed |= proper_case_section(pfile.get('dev-packages', {}))
@@ -727,15 +719,18 @@
             click.echo(location)
 
 
 def do_install_dependencies(
     dev=False, only=False, bare=False, requirements=False, allow_global=False,
     ignore_hashes=False, skip_lock=False, verbose=False, concurrent=True
 ):
-    """"Executes the install functionality."""
+    """"Executes the install functionality.
+
+    If requirements is True, simply spits out a requirements format to stdout.
+    """
 
     def cleanup_procs(procs, concurrent):
         for c in procs:
 
             if concurrent:
                 c.block()
 
@@ -792,15 +787,29 @@
         dev=dev,
         requirements=requirements,
         ignore_hashes=ignore_hashes,
         blocking=blocking,
         only=only
     )
     failed_deps_list = []
+
     if requirements:
+
+        # Comment out packages that shouldn't be included in
+        # requirements.txt, for pip.
+
+        # Additional package selectors, specific to pip's --hash checking mode.
+        EXCLUDED_PACKAGES = list(BAD_PACKAGES) + ['-e .'] + ['-e file://'] + ['file://']
+        for l in (deps_list, dev_deps_list):
+            for i, dep in enumerate(l):
+                for bad_package in EXCLUDED_PACKAGES:
+                    if dep[0].startswith(bad_package):
+                        l[i] = list(l[i])
+                        l[i][0] = '# {0}'.format(l[i][0])
+
         # Output only default dependencies
         if not dev:
             click.echo('\n'.join(d[0] for d in deps_list))
             sys.exit(0)
 
         # Output only dev dependencies
         if dev:
@@ -903,15 +912,15 @@
 
     # The user wants the virtualenv in the project.
     if PIPENV_VENV_IN_PROJECT:
         cmd = ['virtualenv', project.virtualenv_location, '--prompt=({0})'.format(project.name)]
 
         # Pass site-packages flag to virtualenv, if desired...
         if site_packages:
-            cmd = [cmd] + ['--system-site-packages']
+            cmd.append('--system-site-packages')
     else:
         # Default: use pew.
         cmd = ['pew', 'new', project.virtualenv_name, '-d']
 
     # Pass a Python version to virtualenv, if needed.
     if python:
         click.echo(u'{0} {1} {2}'.format(
@@ -1034,15 +1043,16 @@
         sources=project.sources,
         verbose=verbose,
         python=python_version(which('python', allow_global=system)),
         clear=clear,
         which=which,
         which_pip=which_pip,
         project=project,
-        pre=pre
+        pre=pre,
+        allow_global=system
     )
 
     # Add develop dependencies to lockfile.
     for dep in results:
         # Add version information to lockfile.
         lockfile['develop'].update({dep['name']: {'version': '=={0}'.format(dep['version'])}})
 
@@ -1095,15 +1105,16 @@
         deps,
         sources=project.sources,
         verbose=verbose,
         python=python_version(which('python', allow_global=system)),
         which=which,
         which_pip=which_pip,
         project=project,
-        pre=pre
+        pre=pre,
+        allow_global=system
     )
 
     # Add default dependencies to lockfile.
     for dep in results:
         # Add version information to lockfile.
         lockfile['default'].update({dep['name']: {'version': '=={0}'.format(dep['version'])}})
 
@@ -1181,15 +1192,15 @@
         suffix = '.csh'
 
     # Escape any spaces located within the virtualenv path to allow
     # for proper activation.
     venv_location = project.virtualenv_location.replace(' ', r'\ ')
 
     if source:
-        return 'source {0}/bin/activate{1}'.format(venv_location, suffix)
+        return '. {0}/bin/activate{1}'.format(venv_location, suffix)
     else:
         return '{0}/bin/activate'.format(venv_location)
 
 
 def do_activate_virtualenv(bare=False):
     """Executes the activate virtualenv functionality."""
     # Check for environment marker, and skip if it's set.
@@ -1208,15 +1219,17 @@
     if downloads:
         if not bare:
             click.echo(crayons.normal(u'Clearing out downloads directory…', bold=True))
         shutil.rmtree(project.download_location)
         return
 
     freeze = delegator.run('"{0}" freeze'.format(which_pip(allow_global=allow_global))).out
-    installed = freeze.split()
+
+    # Remove comments from the output, if any.
+    installed = [line for line in freeze.splitlines() if not line.lstrip().startswith('#')]
 
     # Remove setuptools and friends from installed, if present.
     for package_name in BAD_PACKAGES:
         for i, package in enumerate(installed):
             if package.startswith(package_name):
                 del installed[i]
 
@@ -1318,17 +1331,19 @@
         do_activate_virtualenv()
 
 
 def pip_install(
     package_name=None, r=None, allow_global=False, ignore_hashes=False,
     no_deps=True, verbose=False, block=True, index=None, pre=False
 ):
+    import pip
 
     if verbose:
         click.echo(crayons.normal('Installing {0!r}'.format(package_name), bold=True), err=True)
+        pip.logger.setLevel(logging.INFO)
 
     # Create files for hash mode.
     if (not ignore_hashes) and (r is None):
         r = tempfile.mkstemp(prefix='pipenv-', suffix='-requirement.txt')[1]
         with open(r, 'w') as f:
             f.write(package_name)
 
@@ -1349,15 +1364,15 @@
         )
         sys.exit(1)
     if req:
         no_deps = False
 
         # Don't specify a source directory when using --system.
         if not allow_global and ('PIP_SRC' not in os.environ):
-            src = '--src {0}'.format(project.virtualenv_src_location)
+            src = '--src {0}'.format(shellquote(project.virtualenv_src_location))
         else:
             src = ''
     else:
         src = ''
 
     # Try installing for each source in project.sources.
     if index:
@@ -1585,207 +1600,69 @@
         # Windows built-in terminal lacks proper emoji taste.
         if PIPENV_HIDE_EMOJIS:
             click.echo(u'  PS: You have excellent taste!')
         else:
             click.echo(u'  PS: You have excellent taste! ✨ 🍰 ✨')
 
 
-CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
-
-
-@click.group(invoke_without_command=True, context_settings=CONTEXT_SETTINGS)
-@click.option('--update', is_flag=True, default=False, help="Update Pipenv & pip to latest.")
-@click.option('--where', is_flag=True, default=False, help="Output project home information.")
-@click.option('--venv', is_flag=True, default=False, help="Output virtualenv information.")
-@click.option('--py', is_flag=True, default=False, help="Output Python interpreter information.")
-@click.option('--envs', is_flag=True, default=False, help="Output Environment Variable options.")
-@click.option('--rm', is_flag=True, default=False, help="Remove the virtualenv.")
-@click.option('--bare', is_flag=True, default=False, help="Minimal output.")
-@click.option('--completion', is_flag=True, default=False, help="Output completion (to be eval'd).")
-@click.option('--man', is_flag=True, default=False, help="Display manpage.")
-@click.option('--three/--two', is_flag=True, default=None, help="Use Python 3/2 when creating virtualenv.")
-@click.option('--python', default=False, nargs=1, help="Specify which version of Python virtualenv should use.")
-@click.option('--site-packages', is_flag=True, default=False, help="Enable site-packages for the virtualenv.")
-@click.option('--jumbotron', is_flag=True, default=False, help="An easter egg, effectively.")
-@click.version_option(prog_name=crayons.normal('pipenv', bold=True), version=__version__)
-@click.pass_context
-def cli(
-    ctx, where=False, venv=False, rm=False, bare=False, three=False,
-    python=False, help=False, update=False, jumbotron=False, py=False,
-    site_packages=False, envs=False, man=False, completion=False
-):
-
-    if jumbotron:
-        # Awesome sauce.
-        click.echo(crayons.normal(xyzzy, bold=True))
-
-    if not update:
-        if need_update_check():
-            # Spun off in background thread, not unlike magic.
-            check_for_updates()
-    else:
-        # Update pip to latest version.
-        ensure_latest_pip()
-
-        # Upgrade self to latest version.
-        ensure_latest_self()
-
-        sys.exit()
-
-    if completion:
-        if PIPENV_SHELL:
-            os.environ['_PIPENV_COMPLETE'] = 'source-{0}'.format(PIPENV_SHELL.split(os.sep)[-1])
-        else:
-            click.echo(
-                'Please ensure that the {0} environment variable '
-                'is set.'.format(crayons.normal('SHELL', bold=True)), err=True)
-            sys.exit(1)
-
-        c = delegator.run('pipenv')
-        click.echo(c.out)
-        sys.exit(0)
-
-    if man:
-        if system_which('man'):
-            path = os.sep.join([os.path.dirname(__file__), 'pipenv.1'])
-            os.execle(system_which('man'), 'man', path, os.environ)
-        else:
-            click.echo('man does not appear to be available on your system.', err=True)
-
-    if envs:
-        click.echo('The following environment variables can be set, to do various things:\n')
-        for key in environments.__dict__:
-            if key.startswith('PIPENV'):
-                click.echo('  - {0}'.format(crayons.normal(key, bold=True)))
-
-        click.echo('\nYou can learn more at:\n   {0}'.format(
-            crayons.green('http://docs.pipenv.org/advanced.html#configuration-with-environment-variables')
-        ))
-        sys.exit(0)
-
-    warn_in_virtualenv()
-
-    if ctx.invoked_subcommand is None:
-        # --where was passed...
-        if where:
-            do_where(bare=True)
-            sys.exit(0)
 
-        elif py:
-            do_py()
-            sys.exit()
-
-        # --venv was passed...
-        elif venv:
-            # There is no virtualenv yet.
-            if not project.virtualenv_exists:
-                click.echo(crayons.red('No virtualenv has been created for this project yet!'), err=True)
-                sys.exit(1)
-            else:
-                click.echo(project.virtualenv_location)
-                sys.exit(0)
-
-        # --rm was passed...
-        elif rm:
-            # Abort if --system (or running in a virtualenv).
-            if PIPENV_USE_SYSTEM:
-                click.echo(
-                    crayons.red(
-                        'You are attempting to remove a virtualenv that '
-                        'Pipenv did not create. Aborting.'
-                    )
-                )
-                sys.exit(1)
-            if project.virtualenv_exists:
-                loc = project.virtualenv_location
-                click.echo(
-                    crayons.normal(
-                        u'{0} ({1})…'.format(
-                            crayons.normal('Removing virtualenv', bold=True),
-                            crayons.green(loc)
-                        )
-                    )
-                )
-
-                with spinner():
-                    # Remove the virtualenv.
-                    cleanup_virtualenv(bare=True)
-                sys.exit(0)
-            else:
-                click.echo(
-                    crayons.red(
-                        'No virtualenv has been created for this project yet!',
-                        bold=True
-                    ), err=True
-                )
-                sys.exit(1)
-
-    # --two / --three was passed...
-    if (python or three is not None) or site_packages:
-        ensure_project(three=three, python=python, warn=True, site_packages=site_packages)
-
-    # Check this again before exiting for empty ``pipenv`` command.
-    elif ctx.invoked_subcommand is None:
-        # Display help to user, if no commands were passed.
-        click.echo(format_help(ctx.get_help()))
 
 
 def do_py(system=False):
     try:
         click.echo(which('python', allow_global=system))
     except AttributeError:
         click.echo(crayons.red('No project found!'))
 
 
-@click.command(short_help="Installs provided packages and adds them to Pipfile, or (if none is given), installs all packages.", context_settings=dict(
-    ignore_unknown_options=True,
-    allow_extra_args=True
-))
-@click.argument('package_name', default=False)
-@click.argument('more_packages', nargs=-1)
-@click.option('--dev', '-d', is_flag=True, default=False, help="Install package(s) in [dev-packages].")
-@click.option('--three/--two', is_flag=True, default=None, help="Use Python 3/2 when creating virtualenv.")
-@click.option('--python', default=False, nargs=1, help="Specify which version of Python virtualenv should use.")
-@click.option('--system', is_flag=True, default=False, help="System pip management.")
-@click.option('--requirements', '-r', nargs=1, default=False, help="Import a requirements.txt file.")
-@click.option('--code', '-c', nargs=1, default=False, help="Import from codebase.")
-@click.option('--verbose', is_flag=True, default=False, help="Verbose mode.")
-@click.option('--ignore-pipfile', is_flag=True, default=False, help="Ignore Pipfile when installing, using the Pipfile.lock.")
-@click.option('--sequential', is_flag=True, default=False, help="Install dependencies one-at-a-time, instead of concurrently.")
-@click.option('--skip-lock', is_flag=True, default=False, help=u"Ignore locking mechanisms when installing—use the Pipfile, instead.")
-@click.option('--deploy', is_flag=True, default=False, help=u"Abort if the Pipfile.lock is out–of–date, or Python version is wrong.")
-@click.option('--pre', is_flag=True, default=False, help=u"Allow pre–releases.")
-def install(
+
+def do_install(
     package_name=False, more_packages=False, dev=False, three=False,
     python=False, system=False, lock=True, ignore_pipfile=False,
     skip_lock=False, verbose=False, requirements=False, sequential=False,
     pre=False, code=False, deploy=False
 ):
+    import pip
 
-    # Automatically use an activated virtualenv.
-    if PIPENV_USE_SYSTEM:
-        system = True
+    # Don't search for requirements.txt files if the user provides one
+    skip_requirements = True if requirements else False
 
     concurrent = (not sequential)
 
     # Ensure that virtualenv is available.
-    ensure_project(three=three, python=python, system=system, warn=True, deploy=deploy)
+    ensure_project(three=three, python=python, system=system, warn=True, deploy=deploy, skip_requirements=skip_requirements)
 
     # Load the --pre settings from the Pipfile.
     if not pre:
         pre = project.settings.get('allow_prereleases')
 
     remote = requirements and is_valid_url(requirements)
+
+    # Warn and exit if --system is used without a pipfile.
+    if system and package_name:
+        click.echo(
+            '{0}: --system is intended to be used for Pipfile installation, '
+            'not installation of specific packages. Aborting.'.format(
+                crayons.red('Warning', bold=True)
+            ), err=True
+        )
+        click.echo('See also: --deploy flag.', err=True)
+        sys.exit(1)
+
+    # Automatically use an activated virtualenv.
+    if PIPENV_USE_SYSTEM:
+        system = True
+
     # Check if the file is remote or not
     if remote:
         fd, temp_reqs = tempfile.mkstemp(prefix='pipenv-', suffix='-requirement.txt')
         requirements_url = requirements
 
         # Download requirements file
-        click.echo(crayons.normal(u'Remote requirements file provided! Downloading…',bold=True),err=True)
+        click.echo(crayons.normal(u'Remote requirements file provided! Downloading…', bold=True), err=True)
         try:
             download_file(requirements, temp_reqs)
         except IOError:
             click.echo(
                 crayons.red(
                    u'Unable to find requirements file at {0}.'.format(crayons.normal(requirements))
                 ),
@@ -1793,35 +1670,37 @@
             )
             sys.exit(1)
         # Replace the url with the temporary requirements file
         requirements = temp_reqs
         remote = True
 
     if requirements:
-        error, e = None, None
+        error, traceback = None, None
         click.echo(crayons.normal(u'Requirements file provided! Importing into Pipfile…', bold=True), err=True)
         try:
             import_requirements(r=project.path_to(requirements), dev=dev)
         except (UnicodeDecodeError, pip.exceptions.PipError) as e:
             # Don't print the temp file path if remote since it will be deleted.
             req_path = requirements_url if remote else project.path_to(requirements)
             error = (u'Unexpected syntax in {0}. Are you sure this is a '
                       'requirements.txt style file?'.format(req_path))
+            traceback = e
         except AssertionError as e:
             error = (u'Requirements file doesn\'t appear to exist. Please ensure the file exists in your '
                       'project directory or you provided the correct path.')
+            traceback = e
         finally:
             # If requirements file was provided by remote url delete the temporary file
             if remote:
                 os.close(fd)  # Close for windows to allow file cleanup.
                 os.remove(project.path_to(temp_reqs))
 
-            if error and e:
+            if error and traceback:
                 click.echo(crayons.red(error))
-                click.echo(crayons.blue(str(e)), err=True)
+                click.echo(crayons.blue(str(traceback)), err=True)
                 sys.exit(1)
 
     if code:
         click.echo(crayons.normal(u'Discovering imports from local codebase…', bold=True))
         for req in import_from_code(code):
             click.echo('  Found {0}!'.format(crayons.green(req)))
             project.add_package_to_pipfile(req)
@@ -1834,32 +1713,14 @@
     # Capture . argument and assign it to nothing
     if package_name == '.':
         package_name = False
 
     # Allow more than one package to be provided.
     package_names = [package_name, ] + more_packages
 
-    # Suggest a better package name, if appropriate.
-    if len(package_names) == 1:
-        # This can be False...
-        if package_names[0]:
-            if not package_names[0].startswith('-e '):
-                if not is_file(package_names[0]):
-                    if not any(op in package_names[0] for op in '!=<>~'):
-                        suggested_package = suggest_package(package_names[0])
-                        if suggested_package:
-                            if str(package_names[0].lower()) != str(suggested_package.lower()):
-                                if PIPENV_YES or click.confirm(
-                                    'Did you mean {0}?'.format(
-                                        crayons.normal(suggested_package, bold=True)
-                                    ),
-                                    default=True
-                                ):
-                                    package_names[0] = suggested_package
-
     # Install all dependencies, if none was provided.
     if package_name is False:
         # Update project settings with pre preference.
         if pre:
             project.update_settings({'allow_prereleases': pre})
 
         do_init(dev=dev, allow_global=system, ignore_pipfile=ignore_pipfile, system=system, skip_lock=skip_lock, verbose=verbose, concurrent=concurrent, deploy=deploy, pre=pre)
@@ -1930,25 +1791,15 @@
         # Ego boost.
         kr_easter_egg(package_name)
 
     if lock and not skip_lock:
         do_lock(system=system, pre=pre)
 
 
-@click.command(short_help="Un-installs a provided package and removes it from Pipfile.")
-@click.argument('package_name', default=False)
-@click.argument('more_packages', nargs=-1)
-@click.option('--three/--two', is_flag=True, default=None, help="Use Python 3/2 when creating virtualenv.")
-@click.option('--python', default=False, nargs=1, help="Specify which version of Python virtualenv should use.")
-@click.option('--system', is_flag=True, default=False, help="System pip management.")
-@click.option('--verbose', is_flag=True, default=False, help="Verbose mode.")
-@click.option('--lock', is_flag=True, default=True, help="Lock afterwards.")
-@click.option('--all-dev', is_flag=True, default=False, help="Un-install all package from [dev-packages].")
-@click.option('--all', is_flag=True, default=False, help="Purge all package(s) from virtualenv. Does not edit Pipfile.")
-def uninstall(
+def do_uninstall(
     package_name=False, more_packages=False, three=None, python=False,
     system=False, lock=False, all_dev=False, all=False, verbose=False
 ):
 
     # Automatically use an activated virtualenv.
     if PIPENV_USE_SYSTEM:
         system = True
@@ -1994,22 +1845,22 @@
 
     for package_name in package_names:
 
         click.echo(u'Un-installing {0}…'.format(
             crayons.green(package_name))
         )
 
-        cmd = '"{0}" uninstall {1} -y'
-        if verbose:
-            click.echo('$ {0}').format(cmd)
-
-        c = delegator.run(cmd.format(
+        cmd = '"{0}" uninstall {1} -y'.format(
             which_pip(allow_global=system),
             package_name
-        ))
+        )
+        if verbose:
+            click.echo('$ {0}'.format(cmd))
+
+        c = delegator.run(cmd)
 
         click.echo(crayons.blue(c.out))
 
         if pipfile_remove:
             norm_name = pep423_name(package_name)
 
             in_dev_packages = (norm_name in project._pipfile.get('dev-packages', {}))
@@ -2033,37 +1884,14 @@
             project.remove_package_from_pipfile(package_name, dev=True)
             project.remove_package_from_pipfile(package_name, dev=False)
 
     if lock:
         do_lock(system=system, pre=pre)
 
 
-@click.command(short_help="Generates Pipfile.lock.")
-@click.option('--three/--two', is_flag=True, default=None, help="Use Python 3/2 when creating virtualenv.")
-@click.option('--python', default=False, nargs=1, help="Specify which version of Python virtualenv should use.")
-@click.option('--verbose', is_flag=True, default=False, help="Verbose mode.")
-@click.option('--requirements', '-r', is_flag=True, default=False, help="Generate output compatible with requirements.txt.")
-@click.option('--dev', '-d', is_flag=True, default=False, help="Generate output compatible with requirements.txt for the development dependencies.")
-@click.option('--clear', is_flag=True, default=False, help="Clear the dependency cache.")
-@click.option('--pre', is_flag=True, default=False, help=u"Allow pre–releases.")
-def lock(three=None, python=False, verbose=False, requirements=False, dev=False, clear=False, pre=False):
-
-    # Ensure that virtualenv is available.
-    ensure_project(three=three, python=python)
-
-    # Load the --pre settings from the Pipfile.
-    if not pre:
-        pre = project.settings.get('pre')
-
-    if requirements:
-        do_init(dev=dev, requirements=requirements)
-
-    do_lock(verbose=verbose, clear=clear, pre=pre)
-
-
 def do_shell(three=None, python=False, fancy=False, shell_args=None):
 
     # Ensure that virtualenv is available.
     ensure_project(three=three, python=python, validate=False)
 
     # Set an environment variable, so we know we're in the environment.
     os.environ['PIPENV_ACTIVE'] = '1'
@@ -2157,49 +1985,14 @@
 
     # Interact with the new shell.
     c.interact(escape_character=None)
     c.close()
     sys.exit(c.exitstatus)
 
 
-@click.command(short_help="Spawns a shell within the virtualenv.", context_settings=dict(
-    ignore_unknown_options=True,
-    allow_extra_args=True
-))
-@click.option('--three/--two', is_flag=True, default=None, help="Use Python 3/2 when creating virtualenv.")
-@click.option('--python', default=False, nargs=1, help="Specify which version of Python virtualenv should use.")
-@click.option('--fancy', is_flag=True, default=False, help="Run in shell in fancy mode (for elegantly configured shells).")
-@click.option('--anyway', is_flag=True, default=False, help="Always spawn a subshell, even if one is already spawned.")
-@click.argument('shell_args', nargs=-1)
-def shell(three=None, python=False, fancy=False, shell_args=None, anyway=False):
-
-    # Prevent user from activating nested environments.
-    if 'PIPENV_ACTIVE' in os.environ:
-        # If PIPENV_ACTIVE is set, VIRTUAL_ENV should always be set too.
-        venv_name = os.environ.get('VIRTUAL_ENV', 'UNKNOWN_VIRTUAL_ENVIRONMENT')
-
-        if not anyway:
-            click.echo('{0} {1} {2}\nNo action taken to avoid nested environments.'.format(
-                crayons.normal('Shell for'),
-                crayons.green(venv_name, bold=True),
-                crayons.normal('already activated.', bold=True)
-            ), err=True)
-
-            sys.exit(1)
-
-    # Load .env file.
-    load_dot_env()
-
-    # Use fancy mode for Windows.
-    if os.name == 'nt':
-        fancy = True
-
-    do_shell(three=three, python=python, fancy=fancy, shell_args=shell_args)
-
-
 def inline_activate_virtualenv():
     try:
         activate_this = which('activate_this.py')
         with open(activate_this) as f:
             code = compile(f.read(), activate_this, 'exec')
             exec(code, dict(__file__=activate_this))
     # Catch all errors, just in case.
@@ -2207,33 +2000,24 @@
         click.echo(
             u'{0}: There was an unexpected error while activating your virtualenv. Continuing anyway…'
             ''.format(crayons.red('Warning', bold=True)),
             err=True
         )
 
 
-@click.command(
-    add_help_option=False,
-    short_help="Spawns a command installed into the virtualenv.",
-    context_settings=dict(
-        ignore_unknown_options=True,
-        allow_interspersed_args=False,
-        allow_extra_args=True
-    )
-)
-@click.argument('command')
-@click.argument('args', nargs=-1)
-@click.option('--three/--two', is_flag=True, default=None, help="Use Python 3/2 when creating virtualenv.")
-@click.option('--python', default=False, nargs=1, help="Specify which version of Python virtualenv should use.")
-def run(command, args, three=None, python=False):
+def do_run(command, args, three=None, python=False):
     # Ensure that virtualenv is available.
     ensure_project(three=three, python=python, validate=False)
 
     load_dot_env()
 
+    # Script was found…
+    if command in project.scripts:
+        command = ' '.join(project.scripts[command])
+
     # Separate out things that were passed in as a string.
     _c = list(command.split())
     command = _c.pop(0)
     if _c:
         args = list(args)
         for __c in reversed(_c):
             args.insert(0, __c)
@@ -2247,46 +2031,44 @@
         p = subprocess.Popen([command] + list(args), shell=True, universal_newlines=True)
         p.communicate()
         sys.exit(p.returncode)
     else:
         command_path = system_which(command)
         if not command_path:
             click.echo(
-                '{0}: the command {1} could not be found within {2}.'
+                '{0}: the command {1} could not be found within {2} or Pipfile\'s {3}.'
                 ''.format(
                     crayons.red('Error', bold=True),
                     crayons.red(command),
-                    crayons.normal('PATH', bold=True)
+                    crayons.normal('PATH', bold=True),
+                    crayons.normal('[scripts]', bold=True)
                 ), err=True
             )
             sys.exit(1)
 
         # Execute the command.
         os.execl(command_path, command_path, *args)
         pass
 
 
-@click.command(short_help="Checks for security vulnerabilities and against PEP 508 markers provided in Pipfile.",  context_settings=dict(
-    ignore_unknown_options=True,
-    allow_extra_args=True
-))
-@click.option('--three/--two', is_flag=True, default=None, help="Use Python 3/2 when creating virtualenv.")
-@click.option('--python', default=False, nargs=1, help="Specify which version of Python virtualenv should use.")
-@click.option('--unused', nargs=1, default=False, help="Given a code path, show potentially unused dependencies.")
-@click.option('--style', nargs=1, default=False, help="Given a code path, show Flake8 errors.")
-@click.argument('args', nargs=-1)
-def check(three=None, python=False, unused=False, style=False, args=None):
+def do_check(three=None, python=False, system=False, unused=False, style=False, args=None):
 
-    # Ensure that virtualenv is available.
-    ensure_project(three=three, python=python, validate=False, warn=False)
+    if not system:
+        # Ensure that virtualenv is available.
+        ensure_project(three=three, python=python, validate=False, warn=False)
 
     if not args:
         args = []
 
     if style:
+        click.echo(
+            '{0}: --style argument is deprecated since 9.1.0 and will be '
+            'removed in 10.0.0.'.format(crayons.red('Warning', bold=True)),
+            err=True
+        )
         sys.argv = ['magic', project.path_to(style)] + list(args)
         flake8.main.cli.main()
         exit()
 
     if unused:
         deps_required = [k for k in project.packages.keys()]
         deps_needed = import_from_code(unused)
@@ -2305,16 +2087,21 @@
         else:
             sys.exit(0)
 
     click.echo(
         crayons.normal(u'Checking PEP 508 requirements…', bold=True)
     )
 
+    if system:
+        python = system_which('python')
+    else:
+        python = which('python')
+
     # Run the PEP 508 checker in the virtualenv.
-    c = delegator.run('"{0}" {1}'.format(which('python'), shellquote(pep508checker.__file__.rstrip('cdo'))))
+    c = delegator.run('"{0}" {1}'.format(python, shellquote(pep508checker.__file__.rstrip('cdo'))))
     results = simplejson.loads(c.out)
 
     # Load the pipfile.
     p = pipfile.Pipfile.load(project.pipfile_location)
 
     failed = False
     # Assert each specified requirement.
@@ -2342,15 +2129,20 @@
     click.echo(
         crayons.normal(u'Checking installed package safety…', bold=True)
     )
 
     path = pep508checker.__file__.rstrip('cdo')
     path = os.sep.join(__file__.split(os.sep)[:-1] + ['patched', 'safety.zip'])
 
-    c = delegator.run('"{0}" {1} check --json'.format(which('python'), shellquote(path)))
+    if not system:
+        python = which('python')
+    else:
+        python = system_which('python')
+
+    c = delegator.run('"{0}" {1} check --json'.format(python, shellquote(path)))
     try:
         results = simplejson.loads(c.out)
     except ValueError:
         click.echo('An error occurred:', err=True)
         click.echo(c.err, err=True)
         sys.exit(1)
 
@@ -2369,19 +2161,15 @@
 
     if not results:
         click.echo(crayons.green('All good!'))
     else:
         sys.exit(1)
 
 
-@click.command(short_help=u"Displays currently–installed dependency graph information.")
-@click.option('--bare', is_flag=True, default=False, help="Minimal output.")
-@click.option('--json', is_flag=True, default=False, help="Output JSON.")
-@click.option('--reverse', is_flag=True, default=False, help="Reversed dependency graph.")
-def graph(bare=False, json=False, reverse=False):
+def do_graph(bare=False, json=False, reverse=False):
     try:
         python_path = which('python')
     except AttributeError:
         click.echo(
             u'{0}: {1}'.format(
                 crayons.red('Warning', bold=True),
                 u'Unable to display currently–installed dependency graph information here. '
@@ -2443,53 +2231,15 @@
     else:
         click.echo(c.out)
 
     # Return its return code.
     sys.exit(c.return_code)
 
 
-@click.command(short_help="View a given module in your editor.", name="open")
-@click.option('--three/--two', is_flag=True, default=None, help="Use Python 3/2 when creating virtualenv.")
-@click.option('--python', default=False, nargs=1, help="Specify which version of Python virtualenv should use.")
-@click.argument('module', nargs=1)
-def run_open(module, three=None, python=None):
-
-    # Ensure that virtualenv is available.
-    ensure_project(three=three, python=python, validate=False)
-
-    c = delegator.run('{0} -c "import {1}; print({1}.__file__);"'.format(which('python'), module))
-
-    try:
-        assert c.return_code == 0
-    except AssertionError:
-        click.echo(crayons.red('Module not found!'))
-        sys.exit(1)
-
-    if '__init__.py' in c.out:
-        p = os.path.dirname(c.out.strip().rstrip('cdo'))
-    else:
-        p = c.out.strip().rstrip('cdo')
-
-    click.echo(crayons.normal('Opening {0!r} in your EDITOR.'.format(p), bold=True))
-    click.edit(filename=p)
-    sys.exit(0)
-
-
-@click.command(short_help="Uninstalls all packages, and re-installs package(s) in [packages] to latest compatible versions.")
-@click.argument('package_name', default=False)
-@click.option('--verbose', '-v', is_flag=True, default=False, help="Verbose mode.")
-@click.option('--dev', '-d', is_flag=True, default=False, help="Additionally install package(s) in [dev-packages].")
-@click.option('--three/--two', is_flag=True, default=None, help="Use Python 3/2 when creating virtualenv.")
-@click.option('--python', default=False, nargs=1, help="Specify which version of Python virtualenv should use.")
-@click.option('--dry-run', is_flag=True, default=False, help="Just output outdated packages.")
-@click.option('--bare', is_flag=True, default=False, help="Minimal output.")
-@click.option('--clear', is_flag=True, default=False, help="Clear the dependency cache.")
-@click.option('--sequential', is_flag=True, default=False, help="Install dependencies one-at-a-time, instead of concurrently.")
-@click.pass_context
-def update(ctx, dev=False, three=None, python=None, dry_run=False, bare=False, dont_upgrade=False, user=False, verbose=False, clear=False, unused=False, package_name=None, sequential=False):
+def do_update(ctx, install, dev=False, three=None, python=None, dry_run=False, bare=False, dont_upgrade=False, user=False, verbose=False, clear=False, unused=False, package_name=None, sequential=False):
 
     # Ensure that virtualenv is available.
     ensure_project(three=three, python=python, validate=False)
 
     concurrent = (not sequential)
 
     # --dry-run:
@@ -2552,15 +2302,15 @@
 
         pre = project.settings.get('allow_prereleases')
 
         # Purge.
         do_purge()
 
         # Lock.
-        do_lock(pre=pre)
+        do_lock(clear=clear, pre=pre)
 
         # Install everything.
         do_init(dev=dev, verbose=verbose, concurrent=concurrent)
 
         click.echo(
             crayons.green('All dependencies are now up-to-date!')
         )
@@ -2590,26 +2340,7 @@
         else:
             click.echo(
                 '{0} was not found in your {1}!'.format(
                     crayons.green(package_name),
                     crayons.normal('Pipfile', bold=True)
                 )
             )
-
-
-# Install click commands.
-cli.add_command(graph)
-cli.add_command(install)
-cli.add_command(uninstall)
-cli.add_command(update)
-cli.add_command(lock)
-cli.add_command(check)
-cli.add_command(shell)
-cli.add_command(run)
-cli.add_command(run_open)
-
-# Only invoke the "did you mean" when an argument wasn't passed (it breaks those).
-if '-' not in ''.join(sys.argv) and len(sys.argv) > 1:
-    cli = DYMCommandCollection(sources=[cli])
-
-if __name__ == '__main__':
-    cli()
```

### Comparing `pipenv-9.0.3/pipenv/environments.py` & `pipenv-9.1.0/pipenv/environments.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/progress.py` & `pipenv-9.1.0/pipenv/progress.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/crayons.py` & `pipenv-9.1.0/pipenv/patched/crayons.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import colorama
 
 PY3 = sys.version_info[0] >= 3
 
 __all__ = (
     'red', 'green', 'yellow', 'blue',
-    'black', 'magenta', 'cyan', 'white', 'normal'
+    'black', 'magenta', 'cyan', 'white', 'normal',
     'clean', 'disable',
 )
 
 COLORS = __all__[:-2]
 
 if 'get_ipython' in dir():
     """
```

### Comparing `pipenv-9.0.3/pipenv/patched/dotenv/cli.py` & `pipenv-9.1.0/pipenv/patched/dotenv/cli.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/dotenv/main.py` & `pipenv-9.1.0/pipenv/patched/dotenv/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import sys
 import warnings
 import re
 from collections import OrderedDict
 
 __escape_decoder = codecs.getdecoder('unicode_escape')
 __posix_variable = re.compile('\$\{[^\}]*\}')
+__variable_declaration = re.compile('^\s*(\w*)\s*=\s*("[^"]*"|\'[^\']*\'|[^\s]*)\s*$',
+                                    flags=re.MULTILINE)
 
 
 def decode_escaped(escaped):
     return __escape_decoder(escaped)[0]
 
 
 def load_dotenv(dotenv_path, verbose=False, override=False):
@@ -93,15 +95,15 @@
     values = OrderedDict(parse_dotenv(dotenv_path))
     values = resolve_nested_variables(values)
     return values
 
 
 def parse_dotenv(dotenv_path):
     with open(dotenv_path) as f:
-        for k, v in re.findall('^\s*(\w*)\s*=\s*("[^"]*"|[^\s]*)\s*$', f.read(), flags=re.MULTILINE):
+        for k, v in __variable_declaration.findall(f.read()):
             if len(v) > 0:
                 quoted = v[0] == v[len(v) - 1] in ['"', "'"]
 
                 if quoted:
                     v = decode_escaped(v[1:-1])
 
             yield k, v
```

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/sync.py` & `pipenv-9.1.0/pipenv/patched/piptools/sync.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/logging.py` & `pipenv-9.1.0/pipenv/patched/piptools/logging.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/io.py` & `pipenv-9.1.0/pipenv/patched/piptools/io.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/cache.py` & `pipenv-9.1.0/pipenv/patched/piptools/cache.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/repositories/local.py` & `pipenv-9.1.0/pipenv/patched/piptools/repositories/local.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/repositories/pypi.py` & `pipenv-9.1.0/pipenv/patched/piptools/repositories/pypi.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/repositories/base.py` & `pipenv-9.1.0/pipenv/patched/piptools/repositories/base.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/utils.py` & `pipenv-9.1.0/pipenv/patched/piptools/utils.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/resolver.py` & `pipenv-9.1.0/pipenv/patched/piptools/resolver.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/scripts/sync.py` & `pipenv-9.1.0/pipenv/patched/piptools/scripts/sync.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/scripts/compile.py` & `pipenv-9.1.0/pipenv/patched/piptools/scripts/compile.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/exceptions.py` & `pipenv-9.1.0/pipenv/patched/piptools/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/writer.py` & `pipenv-9.1.0/pipenv/patched/piptools/writer.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/_compat/tempfile.py` & `pipenv-9.1.0/pipenv/patched/piptools/_compat/tempfile.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/_compat/contextlib.py` & `pipenv-9.1.0/pipenv/patched/piptools/_compat/contextlib.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/piptools/locations.py` & `pipenv-9.1.0/pipenv/patched/piptools/locations.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/lexer/test_lexer.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/lexer/test_lexer.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/lexer/__init__.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/lexer/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/util.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/util.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/__init__.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/test_util.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/test_util.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/parser/test_parser.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/parser/tokenstream.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/parser/tokenstream.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/parser/__init__.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/parser/elementsanitizer.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/parser/elementsanitizer.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/parser/recdesc.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/parser/recdesc.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/parser/parser.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/abstracttable.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/abstracttable.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_common.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_common.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/metadata.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/metadata.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_table.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_table.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_array.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_array.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_factory.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_factory.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_metadata.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/factory.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/factory.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/common.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/common.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/traversal/predicates.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/traversal/predicates.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/traversal/__init__.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/traversal/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/inlinetable.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/inlinetable.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/table.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/table.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/tableheader.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/tableheader.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/atomic.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/atomic.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/array.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/array.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_inlinetable.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_inlinetable.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/elements/test_traversal.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/elements/test_traversal.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/errors.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/errors.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/deindentanonymoustable.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/deindentanonymoustable.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/test_tableindent.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/test_tableindent.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/test_linelength.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/test_linelength.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/test_tableentrysort.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/test_tableentrysort.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/tableassignment.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/tableassignment.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/__init__.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/tableindent.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/tableindent.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/commentspace.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/commentspace.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/tableentrysort.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/tableentrysort.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/common.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/common.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/test_commentspace.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/test_commentspace.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/test_tableassignment.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/test_tableassignment.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/tablesep.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/tablesep.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/prettifier/linelength.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/prettifier/linelength.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/tokens/__init__.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/tokens/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/tokens/toml2py.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/tokens/toml2py.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/tokens/test_toml2py.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/tokens/test_toml2py.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/tokens/test_py2toml.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/tokens/test_py2toml.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/prettytoml/tokens/py2toml.py` & `pipenv-9.1.0/pipenv/patched/prettytoml/tokens/py2toml.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/baseparser.py` & `pipenv-9.1.0/pipenv/patched/pip/baseparser.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/compat/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/compat/dictconfig.py` & `pipenv-9.1.0/pipenv/patched/pip/compat/dictconfig.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/index.py` & `pipenv-9.1.0/pipenv/patched/pip/index.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/retrying.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/retrying.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/version.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/requirements.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/_structures.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/markers.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/__about__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/_compat.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/packaging/specifiers.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/ipaddress.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/ipaddress.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/webencodings/labels.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/webencodings/mklabels.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/webencodings/x_user_defined.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/webencodings/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/webencodings/tests.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/ordereddict.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/ordereddict.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/progress/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/progress/bar.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/progress/bar.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/progress/spinner.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/progress/helpers.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/progress/helpers.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/progress/counter.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/progress/counter.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/_backport/shutil.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/_backport/shutil.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/_backport/misc.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/_backport/misc.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/_backport/tarfile.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/_backport/tarfile.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/_backport/sysconfig.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/_backport/sysconfig.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/locators.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/metadata.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/version.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/compat.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/index.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/manifest.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/util.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/database.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/markers.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/resources.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/scripts.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distlib/wheel.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/colorama/win32.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/colorama/ansitowin32.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/colorama/ansi.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/colorama/winterm.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/colorama/initialise.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/lockfile/sqlitelockfile.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/lockfile/sqlitelockfile.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/lockfile/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/lockfile/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/lockfile/linklockfile.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/lockfile/linklockfile.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/lockfile/mkdirlockfile.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/lockfile/mkdirlockfile.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/lockfile/symlinklockfile.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/lockfile/symlinklockfile.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/lockfile/pidlockfile.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/lockfile/pidlockfile.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/serialize.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/controller.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/filewrapper.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/heuristics.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/adapter.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/cache.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/_cmd.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/caches/file_cache.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/cachecontrol/caches/redis_cache.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/cookies.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/auth.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/sessions.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/hooks.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/compat.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/models.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/certs.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/status_codes.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/api.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/utils.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/langhungarianmodel.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/mbcssm.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/langthaimodel.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/compat.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/langbulgarianmodel.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/euckrprober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/sjisprober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/cp949prober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/constants.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/constants.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/euctwfreq.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/langhebrewmodel.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/chardistribution.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/latin1prober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/charsetprober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/gb2312prober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/mbcharsetprober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/langcyrillicmodel.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/langcyrillicmodel.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/euctwprober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/codingstatemachine.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/escprober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/universaldetector.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/utf8prober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/gb2312freq.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/mbcsgroupprober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/chardetect.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/chardetect.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/langgreekmodel.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/eucjpprober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/jisfreq.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/escsm.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/sbcharsetprober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/big5freq.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/euckrfreq.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/big5prober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/hebrewprober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/charsetgroupprober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/sbcsgroupprober.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/chardet/jpcntx.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/filepost.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/fields.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/request.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/timeout.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/response.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/ssl_.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/retry.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/url.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/connection.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/request.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/poolmanager.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/response.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/socks.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/pyopenssl.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/appengine.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/ntlmpool.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/connection.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/_collections.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/ordered_dict.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/ordered_dict.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/six.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/exceptions.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/packages/urllib3/connectionpool.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/exceptions.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/cacert.pem` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/cacert.pem`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/structures.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/requests/adapters.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/appdirs.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/sanitizer.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/sanitizer.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/inject_meta_charset.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/inject_meta_charset.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/alphabeticalattributes.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/alphabeticalattributes.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/optionaltags.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/optionaltags.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/lint.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/lint.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/filters/whitespace.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/filters/whitespace.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treewalkers/etree_lxml.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treewalkers/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treewalkers/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treewalkers/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treewalkers/etree.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treewalkers/etree.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treewalkers/genshi.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treewalkers/genshi.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treewalkers/base.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treewalkers/base.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treewalkers/dom.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treewalkers/dom.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treebuilders/etree_lxml.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treebuilders/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treebuilders/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treebuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treebuilders/etree.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treebuilders/etree.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treebuilders/base.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treebuilders/base.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treebuilders/dom.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treebuilders/dom.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_inputstream.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_inputstream.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_ihatexml.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_ihatexml.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/constants.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/constants.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/html5parser.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/html5parser.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_trie/_base.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_trie/_base.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_trie/datrie.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_trie/datrie.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_trie/py.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_trie/py.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treeadapters/sax.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treeadapters/sax.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/treeadapters/genshi.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/treeadapters/genshi.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/serializer.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/serializer.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_tokenizer.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/html5lib/_utils.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/html5lib/_utils.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/six.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/distro.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/distro.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/pkg_resources/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/re-vendor.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/re-vendor.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/_vendor/pyparsing.py` & `pipenv-9.1.0/pipenv/patched/pip/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/cmdoptions.py` & `pipenv-9.1.0/pipenv/patched/pip/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/download.py` & `pipenv-9.1.0/pipenv/patched/pip/download.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/utils/build.py` & `pipenv-9.1.0/pipenv/patched/pip/utils/build.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/utils/logging.py` & `pipenv-9.1.0/pipenv/patched/pip/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/utils/encoding.py` & `pipenv-9.1.0/pipenv/patched/pip/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/utils/deprecation.py` & `pipenv-9.1.0/pipenv/patched/pip/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/utils/ui.py` & `pipenv-9.1.0/pipenv/patched/pip/utils/ui.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/utils/filesystem.py` & `pipenv-9.1.0/pipenv/patched/pip/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/utils/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/utils/appdirs.py` & `pipenv-9.1.0/pipenv/patched/pip/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/utils/packaging.py` & `pipenv-9.1.0/pipenv/patched/pip/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/utils/outdated.py` & `pipenv-9.1.0/pipenv/patched/pip/utils/outdated.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/utils/hashes.py` & `pipenv-9.1.0/pipenv/patched/pip/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/utils/glibc.py` & `pipenv-9.1.0/pipenv/patched/pip/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/operations/check.py` & `pipenv-9.1.0/pipenv/patched/pip/operations/check.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/operations/freeze.py` & `pipenv-9.1.0/pipenv/patched/pip/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/req/req_install.py` & `pipenv-9.1.0/pipenv/patched/pip/req/req_install.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/req/req_set.py` & `pipenv-9.1.0/pipenv/patched/pip/req/req_set.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/req/req_uninstall.py` & `pipenv-9.1.0/pipenv/patched/pip/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/req/req_file.py` & `pipenv-9.1.0/pipenv/patched/pip/req/req_file.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/vcs/git.py` & `pipenv-9.1.0/pipenv/patched/pip/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/vcs/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/vcs/mercurial.py` & `pipenv-9.1.0/pipenv/patched/pip/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/vcs/bazaar.py` & `pipenv-9.1.0/pipenv/patched/pip/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/vcs/subversion.py` & `pipenv-9.1.0/pipenv/patched/pip/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/pep425tags.py` & `pipenv-9.1.0/pipenv/patched/pip/pep425tags.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/exceptions.py` & `pipenv-9.1.0/pipenv/patched/pip/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/commands/show.py` & `pipenv-9.1.0/pipenv/patched/pip/commands/show.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/commands/list.py` & `pipenv-9.1.0/pipenv/patched/pip/commands/list.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/commands/check.py` & `pipenv-9.1.0/pipenv/patched/pip/commands/check.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/commands/completion.py` & `pipenv-9.1.0/pipenv/patched/pip/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/commands/download.py` & `pipenv-9.1.0/pipenv/patched/pip/commands/download.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/commands/__init__.py` & `pipenv-9.1.0/pipenv/patched/pip/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/commands/hash.py` & `pipenv-9.1.0/pipenv/patched/pip/commands/hash.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/commands/uninstall.py` & `pipenv-9.1.0/pipenv/patched/pip/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/commands/freeze.py` & `pipenv-9.1.0/pipenv/patched/pip/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/commands/search.py` & `pipenv-9.1.0/pipenv/patched/pip/commands/search.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/commands/install.py` & `pipenv-9.1.0/pipenv/patched/pip/commands/install.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/commands/help.py` & `pipenv-9.1.0/pipenv/patched/pip/commands/help.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/commands/wheel.py` & `pipenv-9.1.0/pipenv/patched/pip/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/basecommand.py` & `pipenv-9.1.0/pipenv/patched/pip/basecommand.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/__main__.py` & `pipenv-9.1.0/pipenv/patched/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/locations.py` & `pipenv-9.1.0/pipenv/patched/pip/locations.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/pip/wheel.py` & `pipenv-9.1.0/pipenv/patched/pip/wheel.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/safety.zip` & `pipenv-9.1.0/pipenv/patched/safety.zip`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/contoml/file/cascadedict.py` & `pipenv-9.1.0/pipenv/patched/contoml/file/cascadedict.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/contoml/file/test_structurer.py` & `pipenv-9.1.0/pipenv/patched/contoml/file/test_structurer.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/contoml/file/toplevels.py` & `pipenv-9.1.0/pipenv/patched/contoml/file/toplevels.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/contoml/file/test_cascadedict.py` & `pipenv-9.1.0/pipenv/patched/contoml/file/test_cascadedict.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/contoml/file/freshtable.py` & `pipenv-9.1.0/pipenv/patched/contoml/file/freshtable.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/contoml/file/file.py` & `pipenv-9.1.0/pipenv/patched/contoml/file/file.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/contoml/file/test_entries.py` & `pipenv-9.1.0/pipenv/patched/contoml/file/test_entries.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/contoml/file/peekableit.py` & `pipenv-9.1.0/pipenv/patched/contoml/file/peekableit.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/contoml/file/array.py` & `pipenv-9.1.0/pipenv/patched/contoml/file/array.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/contoml/file/structurer.py` & `pipenv-9.1.0/pipenv/patched/contoml/file/structurer.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/patched/contoml/__init__.py` & `pipenv-9.1.0/pipenv/patched/contoml/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/project.py` & `pipenv-9.1.0/pipenv/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # -*- coding: utf-8 -*-
 import json
 import os
 import re
 import sys
+import shlex
 import base64
 import hashlib
 
 import contoml
 import delegator
 import pipfile
 import toml
 
 from .utils import (
     mkdir_p, convert_deps_from_pip, pep423_name, recase_file,
     find_requirements, is_file, is_vcs, python_version, cleanup_toml,
-    is_installable_file, is_valid_url
+    is_installable_file, is_valid_url, normalize_drive
 )
 from .environments import PIPENV_MAX_DEPTH, PIPENV_VENV_IN_PROJECT
 from .environments import PIPENV_VIRTUALENV, PIPENV_PIPFILE
 
 if PIPENV_PIPFILE:
     if not os.path.isfile(PIPENV_PIPFILE):
         raise RuntimeError('Given PIPENV_PIPFILE is not found!')
     else:
-        PIPENV_PIPFILE = os.path.abspath(PIPENV_PIPFILE)
+        PIPENV_PIPFILE = normalize_drive(os.path.abspath(PIPENV_PIPFILE))
 
 
 class Project(object):
     """docstring for Project"""
 
     def __init__(self, chdir=True):
         super(Project, self).__init__()
@@ -220,15 +221,15 @@
             return PIPENV_PIPFILE
 
         if self._pipfile_location is None:
             try:
                 loc = pipfile.Pipfile.find(max_depth=PIPENV_MAX_DEPTH)
             except RuntimeError:
                 loc = None
-            self._pipfile_location = loc
+            self._pipfile_location = normalize_drive(loc)
 
         return self._pipfile_location
 
     @property
     def requirements_location(self):
         if self._requirements_location is None:
             try:
@@ -288,14 +289,23 @@
         return pfile
 
     @property
     def settings(self):
         """A dictionary of the settings added to the Pipfile."""
         return self.parsed_pipfile.get('pipenv', {})
 
+    @property
+    def scripts(self):
+        scripts = self.parsed_pipfile.get('scripts', {})
+        for (k, v) in scripts.items():
+            scripts[k] = shlex.split(v, posix=True)
+
+        return scripts
+
+
     def update_settings(self, d):
         settings = self.settings
 
         changed = False
         for new in d:
             if new not in settings:
                 settings[new] = d[new]
```

### Comparing `pipenv-9.0.3/pipenv/vendor/click_didyoumean/__init__.py` & `pipenv-9.1.0/pipenv/vendor/click_didyoumean/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/concurrent27/futures/_base.py` & `pipenv-9.1.0/pipenv/vendor/concurrent27/futures/_base.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/concurrent27/futures/thread.py` & `pipenv-9.1.0/pipenv/vendor/concurrent27/futures/thread.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/concurrent27/futures/__init__.py` & `pipenv-9.1.0/pipenv/vendor/concurrent27/futures/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/concurrent27/futures/process.py` & `pipenv-9.1.0/pipenv/vendor/concurrent27/futures/process.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pytoml/parser.py` & `pipenv-9.1.0/pipenv/vendor/pytoml/parser.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pytoml/writer.py` & `pipenv-9.1.0/pipenv/vendor/pytoml/writer.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/markupsafe/_constants.py` & `pipenv-9.1.0/pipenv/vendor/markupsafe/_constants.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/markupsafe/__init__.py` & `pipenv-9.1.0/pipenv/vendor/markupsafe/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/markupsafe/_native.py` & `pipenv-9.1.0/pipenv/vendor/markupsafe/_native.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/markupsafe/_compat.py` & `pipenv-9.1.0/pipenv/vendor/markupsafe/_compat.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/semver.py` & `pipenv-9.1.0/pipenv/vendor/semver.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/iso8601/iso8601.py` & `pipenv-9.1.0/pipenv/vendor/iso8601/iso8601.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/iso8601/test_iso8601.py` & `pipenv-9.1.0/pipenv/vendor/iso8601/test_iso8601.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/docopt.py` & `pipenv-9.1.0/pipenv/vendor/docopt.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/asyncsupport.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/asyncsupport.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/compiler.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/_stringdefs.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/_stringdefs.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/constants.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/loaders.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/__init__.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/idtracking.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/runtime.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/parser.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/sandbox.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/visitor.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/utils.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/debug.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/lexer.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/environment.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/optimizer.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/exceptions.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/defaults.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/_compat.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/nodes.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/tests.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/bccache.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/filters.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/ext.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/meta.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/jinja2/asyncfilters.py` & `pipenv-9.1.0/pipenv/vendor/jinja2/asyncfilters.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/blindspin/__init__.py` & `pipenv-9.1.0/pipenv/vendor/blindspin/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/colorama/win32.py` & `pipenv-9.1.0/pipenv/vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/colorama/ansitowin32.py` & `pipenv-9.1.0/pipenv/vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/colorama/ansi.py` & `pipenv-9.1.0/pipenv/vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/colorama/winterm.py` & `pipenv-9.1.0/pipenv/vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/colorama/initialise.py` & `pipenv-9.1.0/pipenv/vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/fuzzywuzzy/StringMatcher.py` & `pipenv-9.1.0/pipenv/vendor/Levenshtein/StringMatcher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,10 @@
-#!/usr/bin/env python
-# encoding: utf-8
-"""
-StringMatcher.py
-
-ported from python-Levenshtein
-[https://github.com/miohtama/python-Levenshtein]
-License available here: https://github.com/miohtama/python-Levenshtein/blob/master/COPYING
-"""
-
 from Levenshtein import *
 from warnings import warn
 
-
 class StringMatcher:
     """A SequenceMatcher-like class built on the top of Levenshtein"""
 
     def _reset_cache(self):
         self._ratio = self._distance = None
         self._opcodes = self._editops = self._matching_blocks = None
```

### Comparing `pipenv-9.0.3/pipenv/vendor/delegator.py` & `pipenv-9.1.0/pipenv/vendor/delegator.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/background.py` & `pipenv-9.1.0/pipenv/vendor/background.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/_winconsole.py` & `pipenv-9.1.0/pipenv/vendor/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/_unicodefun.py` & `pipenv-9.1.0/pipenv/vendor/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/_textwrap.py` & `pipenv-9.1.0/pipenv/vendor/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/globals.py` & `pipenv-9.1.0/pipenv/vendor/click/globals.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/__init__.py` & `pipenv-9.1.0/pipenv/vendor/click/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/core.py` & `pipenv-9.1.0/pipenv/vendor/click/core.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/types.py` & `pipenv-9.1.0/pipenv/vendor/click/types.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/formatting.py` & `pipenv-9.1.0/pipenv/vendor/click/formatting.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/parser.py` & `pipenv-9.1.0/pipenv/vendor/click/parser.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/termui.py` & `pipenv-9.1.0/pipenv/vendor/click/termui.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/utils.py` & `pipenv-9.1.0/pipenv/vendor/click/utils.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/_bashcomplete.py` & `pipenv-9.1.0/pipenv/vendor/click/_bashcomplete.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/exceptions.py` & `pipenv-9.1.0/pipenv/vendor/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/_compat.py` & `pipenv-9.1.0/pipenv/vendor/click/_compat.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/_termui_impl.py` & `pipenv-9.1.0/pipenv/vendor/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/testing.py` & `pipenv-9.1.0/pipenv/vendor/click/testing.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click/decorators.py` & `pipenv-9.1.0/pipenv/vendor/click/decorators.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/yarg/package.py` & `pipenv-9.1.0/pipenv/vendor/yarg/package.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/yarg/release.py` & `pipenv-9.1.0/pipenv/vendor/yarg/release.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/yarg/client.py` & `pipenv-9.1.0/pipenv/vendor/yarg/client.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/yarg/__init__.py` & `pipenv-9.1.0/pipenv/vendor/yarg/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/yarg/exceptions.py` & `pipenv-9.1.0/pipenv/vendor/yarg/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/yarg/parse.py` & `pipenv-9.1.0/pipenv/vendor/yarg/parse.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/requirements/requirement.py` & `pipenv-9.1.0/pipenv/vendor/requirements/requirement.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/requirements/parser.py` & `pipenv-9.1.0/pipenv/vendor/requirements/parser.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/requirements/fragment.py` & `pipenv-9.1.0/pipenv/vendor/requirements/fragment.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/shutilwhich/lib.py` & `pipenv-9.1.0/pipenv/vendor/shutilwhich/lib.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/backports/shutil_get_terminal_size/get_terminal_size.py` & `pipenv-9.1.0/pipenv/vendor/backports/shutil_get_terminal_size/get_terminal_size.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/appdirs.py` & `pipenv-9.1.0/pipenv/vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pipfile/api.py` & `pipenv-9.1.0/pipenv/vendor/pipfile/api.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pipfile/__about__.py` & `pipenv-9.1.0/pipenv/vendor/pipfile/__about__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/screen.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/screen.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/popen_spawn.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/popen_spawn.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/run.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/run.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/expect.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/expect.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/replwrap.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/replwrap.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/spawnbase.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/spawnbase.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/pxssh.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/pxssh.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/__init__.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/fdpexpect.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/fdpexpect.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/utils.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/utils.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/_async.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/_async.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/exceptions.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/ANSI.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/ANSI.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/pty_spawn.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/pty_spawn.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pexpect/FSM.py` & `pipenv-9.1.0/pipenv/vendor/pexpect/FSM.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/first.py` & `pipenv-9.1.0/pipenv/vendor/first.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pathlib2.py` & `pipenv-9.1.0/pipenv/vendor/pathlib2.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/ptyprocess/util.py` & `pipenv-9.1.0/pipenv/vendor/ptyprocess/util.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/ptyprocess/_fork_pty.py` & `pipenv-9.1.0/pipenv/vendor/ptyprocess/_fork_pty.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/ptyprocess/ptyprocess.py` & `pipenv-9.1.0/pipenv/vendor/ptyprocess/ptyprocess.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/six.py` & `pipenv-9.1.0/pipenv/vendor/six.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pipreqs/mapping` & `pipenv-9.1.0/pipenv/vendor/pipreqs/mapping`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pipreqs/pipreqs.py` & `pipenv-9.1.0/pipenv/vendor/pipreqs/pipreqs.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pipreqs/stdlib` & `pipenv-9.1.0/pipenv/vendor/pipreqs/stdlib`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/click_completion.py` & `pipenv-9.1.0/pipenv/vendor/click_completion.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/parse.py` & `pipenv-9.1.0/pipenv/vendor/parse.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/strict_rfc3339.py` & `pipenv-9.1.0/pipenv/vendor/strict_rfc3339.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/pipdeptree.py` & `pipenv-9.1.0/pipenv/vendor/pipdeptree.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/psutil/_pswindows.py` & `pipenv-9.1.0/pipenv/vendor/psutil/_pswindows.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/psutil/_common.py` & `pipenv-9.1.0/pipenv/vendor/psutil/_common.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/psutil/__init__.py` & `pipenv-9.1.0/pipenv/vendor/psutil/__init__.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/psutil/_psosx.py` & `pipenv-9.1.0/pipenv/vendor/psutil/_psosx.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/psutil/_psbsd.py` & `pipenv-9.1.0/pipenv/vendor/psutil/_psbsd.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/psutil/_pslinux.py` & `pipenv-9.1.0/pipenv/vendor/psutil/_pslinux.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/psutil/_compat.py` & `pipenv-9.1.0/pipenv/vendor/psutil/_compat.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/psutil/_psposix.py` & `pipenv-9.1.0/pipenv/vendor/psutil/_psposix.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/psutil/_pssunos.py` & `pipenv-9.1.0/pipenv/vendor/psutil/_pssunos.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv/vendor/toml.py` & `pipenv-9.1.0/pipenv/vendor/toml.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/LICENSE` & `pipenv-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/setup.py` & `pipenv-9.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/HISTORY.txt` & `pipenv-9.1.0/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+9.1.0:
+ - Add --system flag to $ pipenv check.
+ - Removal of package name suggestions.
+ - Support for [scripts] in Pipfile.
+ - Comment out invalid (to pip's hash checking mode) packages from `$ pipenv lock -r`.
+ - Updated patched version of dotenv.
+ - Do not allow `$ pipenv install --system packagename `to be used.
+ - Deprecate the usage of `$ pipenv check --style`.
+ - Show pip install logs with --verbose.
+ - Allow -v as shorthand for --verbose for all commands.
 9.0.3:
  - v9.0.1.
 9.0.2:
  - A mistake.
 9.0.1:
  - Fixed issue with specifiers being treated as paths on Windows.
  - Fixed regression causing development packages to always be installed.
```

### Comparing `pipenv-9.0.3/README.rst` & `pipenv-9.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -40,20 +40,14 @@
 Installation
 ------------
 
 ::
 
     $ pip install pipenv
 
-Or if you are on macOS, you can install Pipenv via `Homebrew <https://brew.sh/>`_ with:
-
-::
-
-    $ brew install pipenv
-
 ✨🍰✨
 
 ☤ User Testimonials
 -------------------
 
 **Jannis Leidel**, former pip maintainer—
     *Pipenv is the porcelain I always wanted to build for pip. It fits my brain and mostly replaces virtualenvwrapper and manual pip calls for me. Use it.*
```

### Comparing `pipenv-9.0.3/pipenv.egg-info/PKG-INFO` & `pipenv-9.1.0/pipenv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pipenv
-Version: 9.0.3
+Version: 9.1.0
 Summary: Python Development Workflow for Humans.
 Home-page: https://github.com/pypa/pipenv
 Author: Kenneth Reitz
 Author-email: me@kennethreitz.org
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: 
@@ -50,20 +50,14 @@
         Installation
         ------------
         
         ::
         
             $ pip install pipenv
         
-        Or if you are on macOS, you can install Pipenv via `Homebrew <https://brew.sh/>`_ with:
-        
-        ::
-        
-            $ brew install pipenv
-        
         ✨🍰✨
         
         ☤ User Testimonials
         -------------------
         
         **Jannis Leidel**, former pip maintainer—
             *Pipenv is the porcelain I always wanted to build for pip. It fits my brain and mostly replaces virtualenvwrapper and manual pip calls for me. Use it.*
```

### Comparing `pipenv-9.0.3/pipenv.egg-info/PKG-INFO 2` & `pipenv-9.1.0/pipenv.egg-info/PKG-INFO 2`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv.egg-info/SOURCES.txt` & `pipenv-9.1.0/pipenv.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 README.rst
 setup.cfg
 setup.py
 pipenv/__init__.py
 pipenv/__main__.py
 pipenv/__version__.py
 pipenv/cli.py
+pipenv/core.py
 pipenv/environments.py
 pipenv/pep508checker.py
 pipenv/pipenv.1
 pipenv/progress.py
 pipenv/project.py
 pipenv/utils.py
 pipenv.egg-info/PKG-INFO
@@ -42,16 +43,16 @@
 pipenv/patched/contoml/file/test_cascadedict.py
 pipenv/patched/contoml/file/test_entries.py
 pipenv/patched/contoml/file/test_peekableit.py
 pipenv/patched/contoml/file/test_structurer.py
 pipenv/patched/contoml/file/toplevels.py
 pipenv/patched/dotenv/__init__.py
 pipenv/patched/dotenv/cli.py
-pipenv/patched/dotenv/ipython.py
 pipenv/patched/dotenv/main.py
+pipenv/patched/dotenv/test_main.py
 pipenv/patched/pip/__init__.py
 pipenv/patched/pip/__main__.py
 pipenv/patched/pip/basecommand.py
 pipenv/patched/pip/baseparser.py
 pipenv/patched/pip/cmdoptions.py
 pipenv/patched/pip/download.py
 pipenv/patched/pip/exceptions.py
@@ -418,20 +419,14 @@
 pipenv/vendor/colorama/win32.py
 pipenv/vendor/colorama/winterm.py
 pipenv/vendor/concurrent27/__init__.py
 pipenv/vendor/concurrent27/futures/__init__.py
 pipenv/vendor/concurrent27/futures/_base.py
 pipenv/vendor/concurrent27/futures/process.py
 pipenv/vendor/concurrent27/futures/thread.py
-pipenv/vendor/fuzzywuzzy/StringMatcher.py
-pipenv/vendor/fuzzywuzzy/__init__.py
-pipenv/vendor/fuzzywuzzy/fuzz.py
-pipenv/vendor/fuzzywuzzy/process.py
-pipenv/vendor/fuzzywuzzy/string_processing.py
-pipenv/vendor/fuzzywuzzy/utils.py
 pipenv/vendor/iso8601/__init__.py
 pipenv/vendor/iso8601/iso8601.py
 pipenv/vendor/iso8601/test_iso8601.py
 pipenv/vendor/jinja2/__init__.py
 pipenv/vendor/jinja2/_compat.py
 pipenv/vendor/jinja2/_stringdefs.py
 pipenv/vendor/jinja2/asyncfilters.py
```

### Comparing `pipenv-9.0.3/pipenv.egg-info/SOURCES 2.txt` & `pipenv-9.1.0/pipenv.egg-info/SOURCES 2.txt`

 * *Files identical despite different names*

### Comparing `pipenv-9.0.3/pipenv.egg-info/SOURCES 3.txt` & `pipenv-9.1.0/pipenv.egg-info/SOURCES 3.txt`

 * *Files identical despite different names*


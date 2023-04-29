# Comparing `tmp/pycobertura-3.0.0.tar.gz` & `tmp/pycobertura-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycobertura-3.0.0.tar", last modified: Sat Oct  8 00:34:46 2022, max compression
+gzip compressed data, was "pycobertura-3.1.0.tar", last modified: Sat Apr 29 17:18:42 2023, max compression
```

## Comparing `pycobertura-3.0.0.tar` & `pycobertura-3.1.0.tar`

### file list

```diff
@@ -1,133 +1,136 @@
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.793552 pycobertura-3.0.0/
--rw-r--r--   0 alexandre   (501) staff       (20)       32 2022-10-07 08:01:13.000000 pycobertura-3.0.0/.coveragerc
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.774469 pycobertura-3.0.0/.github/
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.778239 pycobertura-3.0.0/.github/workflows/
--rw-r--r--   0 alexandre   (501) staff       (20)      642 2022-03-20 16:09:41.000000 pycobertura-3.0.0/.github/workflows/build-and-test-pycobertura.yml
--rw-r--r--   0 alexandre   (501) staff       (20)      604 2022-03-03 22:33:26.000000 pycobertura-3.0.0/.gitignore
--rw-r--r--   0 alexandre   (501) staff       (20)    15306 2022-10-07 23:52:49.000000 pycobertura-3.0.0/CHANGES.md
--rw-r--r--   0 alexandre   (501) staff       (20)     1103 2022-03-03 22:33:26.000000 pycobertura-3.0.0/LICENSE
--rw-r--r--   0 alexandre   (501) staff       (20)    23173 2022-10-08 00:34:46.793685 pycobertura-3.0.0/PKG-INFO
--rw-r--r--   0 alexandre   (501) staff       (20)    22187 2022-10-07 23:42:24.000000 pycobertura-3.0.0/README.md
--rw-r--r--   0 alexandre   (501) staff       (20)     2697 2022-01-04 01:58:44.000000 pycobertura-3.0.0/aysha-logo.svg
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.779605 pycobertura-3.0.0/images/
--rw-r--r--   0 alexandre   (501) staff       (20)    30894 2022-03-03 22:33:26.000000 pycobertura-3.0.0/images/example_csv_diff_output.png
--rw-r--r--   0 alexandre   (501) staff       (20)    61287 2022-03-03 22:33:26.000000 pycobertura-3.0.0/images/example_json_output.png
--rw-r--r--   0 alexandre   (501) staff       (20)    53710 2022-03-03 22:33:26.000000 pycobertura-3.0.0/images/example_markdown_diff_output.png
--rw-r--r--   0 alexandre   (501) staff       (20)    45822 2022-03-03 22:33:26.000000 pycobertura-3.0.0/images/example_yaml_output.png
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.780961 pycobertura-3.0.0/pycobertura/
--rw-r--r--   0 alexandre   (501) staff       (20)      119 2022-01-04 01:58:44.000000 pycobertura-3.0.0/pycobertura/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)     7962 2022-10-07 23:42:24.000000 pycobertura-3.0.0/pycobertura/cli.py
--rw-r--r--   0 alexandre   (501) staff       (20)    15355 2022-10-07 23:42:24.000000 pycobertura-3.0.0/pycobertura/cobertura.py
--rw-r--r--   0 alexandre   (501) staff       (20)     4886 2022-03-03 22:33:26.000000 pycobertura-3.0.0/pycobertura/filesystem.py
--rw-r--r--   0 alexandre   (501) staff       (20)    15454 2022-10-07 23:42:24.000000 pycobertura-3.0.0/pycobertura/reporters.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.783142 pycobertura-3.0.0/pycobertura/templates/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.0.0/pycobertura/templates/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      624 2022-10-07 08:01:13.000000 pycobertura-3.0.0/pycobertura/templates/filters.py
--rw-r--r--   0 alexandre   (501) staff       (20)     2805 2022-03-04 19:55:00.000000 pycobertura-3.0.0/pycobertura/templates/html-delta.jinja2
--rw-r--r--   0 alexandre   (501) staff       (20)     1764 2022-03-03 22:33:26.000000 pycobertura-3.0.0/pycobertura/templates/html.jinja2
--rw-r--r--   0 alexandre   (501) staff       (20)      473 2022-01-04 01:58:44.000000 pycobertura-3.0.0/pycobertura/templates/macro.source.jinja2
--rw-r--r--   0 alexandre   (501) staff       (20)     7797 2022-01-04 01:58:44.000000 pycobertura-3.0.0/pycobertura/templates/normalize.css
--rw-r--r--   0 alexandre   (501) staff       (20)    11452 2022-01-04 01:58:44.000000 pycobertura-3.0.0/pycobertura/templates/skeleton.css
--rw-r--r--   0 alexandre   (501) staff       (20)     7151 2022-10-07 23:42:24.000000 pycobertura-3.0.0/pycobertura/utils.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.782045 pycobertura-3.0.0/pycobertura.egg-info/
--rw-r--r--   0 alexandre   (501) staff       (20)    23173 2022-10-08 00:34:46.000000 pycobertura-3.0.0/pycobertura.egg-info/PKG-INFO
--rw-r--r--   0 alexandre   (501) staff       (20)     3288 2022-10-08 00:34:46.000000 pycobertura-3.0.0/pycobertura.egg-info/SOURCES.txt
--rw-r--r--   0 alexandre   (501) staff       (20)        1 2022-10-08 00:34:46.000000 pycobertura-3.0.0/pycobertura.egg-info/dependency_links.txt
--rw-r--r--   0 alexandre   (501) staff       (20)       60 2022-10-08 00:34:46.000000 pycobertura-3.0.0/pycobertura.egg-info/entry_points.txt
--rw-r--r--   0 alexandre   (501) staff       (20)        1 2022-03-04 19:49:40.000000 pycobertura-3.0.0/pycobertura.egg-info/not-zip-safe
--rw-r--r--   0 alexandre   (501) staff       (20)       44 2022-10-08 00:34:46.000000 pycobertura-3.0.0/pycobertura.egg-info/requires.txt
--rw-r--r--   0 alexandre   (501) staff       (20)       12 2022-10-08 00:34:46.000000 pycobertura-3.0.0/pycobertura.egg-info/top_level.txt
--rw-r--r--   0 alexandre   (501) staff       (20)      122 2022-03-03 22:33:26.000000 pycobertura-3.0.0/pyproject.toml
--rw-r--r--   0 alexandre   (501) staff       (20)      997 2022-10-07 08:01:13.000000 pycobertura-3.0.0/pytest.ini
--rwxr-xr-x   0 alexandre   (501) staff       (20)      688 2022-10-08 00:09:40.000000 pycobertura-3.0.0/release.sh
--rw-r--r--   0 alexandre   (501) staff       (20)     1295 2022-10-08 00:34:46.794050 pycobertura-3.0.0/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)       38 2022-03-03 22:33:26.000000 pycobertura-3.0.0/setup.py
--rw-r--r--   0 alexandre   (501) staff       (20)       82 2022-10-07 08:01:13.000000 pycobertura-3.0.0/test-requirements.txt
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.787498 pycobertura-3.0.0/tests/
--rw-r--r--   0 alexandre   (501) staff       (20)       64 2022-10-07 23:42:24.000000 pycobertura-3.0.0/tests/.testgitignore
--rw-r--r--   0 alexandre   (501) staff       (20)      748 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/README.generate-dummy-coverage-for-testing.md
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1162 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/cobertura-generated-by-istanbul-from-coffeescript.xml
--rw-r--r--   0 alexandre   (501) staff       (20)     7963 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/cobertura.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.788190 pycobertura-3.0.0/tests/dummy/
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.793389 pycobertura-3.0.0/tests/dummy/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)       41 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)       20 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy/dummy/dummy2.py
--rw-r--r--   0 alexandre   (501) staff       (20)      995 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy/dummy-with-prefix.zip
--rw-r--r--   0 alexandre   (501) staff       (20)      687 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy/dummy.zip
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      179 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.788490 pycobertura-3.0.0/tests/dummy.linestatus/
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.788624 pycobertura-3.0.0/tests/dummy.linestatus/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)       14 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.linestatus/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      623 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.linestatus/test1.xml
--rw-r--r--   0 alexandre   (501) staff       (20)      578 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.linestatus/test2.xml
--rw-r--r--   0 alexandre   (501) staff       (20)      861 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.original-better-cov.xml
--rw-r--r--   0 alexandre   (501) staff       (20)      852 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.original-full-cov.xml
--rw-r--r--   0 alexandre   (501) staff       (20)      858 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.original.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.789050 pycobertura-3.0.0/tests/dummy.source1/
--rw-r--r--   0 alexandre   (501) staff       (20)     1456 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.source1/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.789512 pycobertura-3.0.0/tests/dummy.source1/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.source1/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)       56 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.source1/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)       20 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.source1/dummy/dummy2.py
--rw-r--r--   0 alexandre   (501) staff       (20)       64 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.source1/dummy/dummy4.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.source1/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      119 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.source1/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.790000 pycobertura-3.0.0/tests/dummy.source2/
--rw-r--r--   0 alexandre   (501) staff       (20)     1423 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.source2/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.790454 pycobertura-3.0.0/tests/dummy.source2/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.source2/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)       56 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.source2/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)       44 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.source2/dummy/dummy2.py
--rw-r--r--   0 alexandre   (501) staff       (20)      209 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.source2/dummy/dummy3.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.source2/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      179 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.source2/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.790829 pycobertura-3.0.0/tests/dummy.uncovered/
--rw-r--r--   0 alexandre   (501) staff       (20)     1178 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.uncovered/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.791652 pycobertura-3.0.0/tests/dummy.uncovered/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.uncovered/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      114 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.uncovered/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.uncovered/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      178 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.uncovered/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.791255 pycobertura-3.0.0/tests/dummy.uncovered.addcode/
--rw-r--r--   0 alexandre   (501) staff       (20)     1250 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.uncovered.addcode/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.791453 pycobertura-3.0.0/tests/dummy.uncovered.addcode/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.uncovered.addcode/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      185 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.uncovered.addcode/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.uncovered.addcode/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      178 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.uncovered.addcode/test_dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1093 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.with-dummy2-better-and-worse.xml
--rw-r--r--   0 alexandre   (501) staff       (20)     1092 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.with-dummy2-better-cov.xml
--rw-r--r--   0 alexandre   (501) staff       (20)     1080 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.with-dummy2-full-cov.xml
--rw-r--r--   0 alexandre   (501) staff       (20)     1090 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.with-dummy2-no-cov.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.792029 pycobertura-3.0.0/tests/dummy.zeroexit1/
--rw-r--r--   0 alexandre   (501) staff       (20)      969 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.zeroexit1/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.792265 pycobertura-3.0.0/tests/dummy.zeroexit1/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.zeroexit1/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      108 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.zeroexit1/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.zeroexit1/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)       58 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.zeroexit1/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.792730 pycobertura-3.0.0/tests/dummy.zeroexit2/
--rw-r--r--   0 alexandre   (501) staff       (20)     1000 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.zeroexit2/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2022-10-08 00:34:46.792991 pycobertura-3.0.0/tests/dummy.zeroexit2/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.zeroexit2/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      134 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.zeroexit2/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.zeroexit2/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)       68 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/dummy.zeroexit2/test_dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)    27978 2022-10-07 23:40:05.000000 pycobertura-3.0.0/tests/test_cli.py
--rw-r--r--   0 alexandre   (501) staff       (20)     9064 2022-03-03 22:33:26.000000 pycobertura-3.0.0/tests/test_cobertura.py
--rw-r--r--   0 alexandre   (501) staff       (20)     5737 2022-10-07 08:01:13.000000 pycobertura-3.0.0/tests/test_cobertura_diff.py
--rw-r--r--   0 alexandre   (501) staff       (20)      127 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/test_colorize.py
--rw-r--r--   0 alexandre   (501) staff       (20)      429 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/test_extrapolate_coverage.py
--rw-r--r--   0 alexandre   (501) staff       (20)     6494 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/test_filesystem.py
--rw-r--r--   0 alexandre   (501) staff       (20)     6429 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/test_hunkify_coverage.py
--rw-r--r--   0 alexandre   (501) staff       (20)      187 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/test_imports.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1166 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/test_rangify.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1076 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/test_reconcile_lines.py
--rw-r--r--   0 alexandre   (501) staff       (20)      926 2022-10-07 23:42:24.000000 pycobertura-3.0.0/tests/test_regex_utils.py
--rw-r--r--   0 alexandre   (501) staff       (20)    18630 2022-10-07 08:01:13.000000 pycobertura-3.0.0/tests/test_reporters.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1175 2022-03-03 22:33:26.000000 pycobertura-3.0.0/tests/test_stringify.py
--rw-r--r--   0 alexandre   (501) staff       (20)      420 2022-01-04 01:58:44.000000 pycobertura-3.0.0/tests/utils.py
--rw-r--r--   0 alexandre   (501) staff       (20)      528 2022-10-07 08:01:13.000000 pycobertura-3.0.0/tox.ini
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.534694 pycobertura-3.1.0/
+-rw-r--r--   0 alexandre   (501) staff       (20)       32 2022-10-07 08:01:13.000000 pycobertura-3.1.0/.coveragerc
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.512155 pycobertura-3.1.0/.github/
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.516533 pycobertura-3.1.0/.github/workflows/
+-rw-r--r--   0 alexandre   (501) staff       (20)      642 2022-03-20 16:09:41.000000 pycobertura-3.1.0/.github/workflows/build-and-test-pycobertura.yml
+-rw-r--r--   0 alexandre   (501) staff       (20)      604 2022-03-03 22:33:26.000000 pycobertura-3.1.0/.gitignore
+-rw-r--r--   0 alexandre   (501) staff       (20)    15419 2023-04-29 17:17:00.000000 pycobertura-3.1.0/CHANGES.md
+-rw-r--r--   0 alexandre   (501) staff       (20)     1103 2022-03-03 22:33:26.000000 pycobertura-3.1.0/LICENSE
+-rw-r--r--   0 alexandre   (501) staff       (20)    23730 2023-04-29 17:18:42.534819 pycobertura-3.1.0/PKG-INFO
+-rw-r--r--   0 alexandre   (501) staff       (20)    22744 2023-04-29 17:12:19.000000 pycobertura-3.1.0/README.md
+-rw-r--r--   0 alexandre   (501) staff       (20)        6 2023-04-29 17:15:54.000000 pycobertura-3.1.0/__version__
+-rw-r--r--   0 alexandre   (501) staff       (20)     2697 2022-01-04 01:58:44.000000 pycobertura-3.1.0/aysha-logo.svg
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.518534 pycobertura-3.1.0/images/
+-rw-r--r--   0 alexandre   (501) staff       (20)    30894 2022-03-03 22:33:26.000000 pycobertura-3.1.0/images/example_csv_diff_output.png
+-rw-r--r--   0 alexandre   (501) staff       (20)   115395 2023-04-29 17:12:19.000000 pycobertura-3.1.0/images/example_github_annotation_show.png
+-rw-r--r--   0 alexandre   (501) staff       (20)    61287 2022-03-03 22:33:26.000000 pycobertura-3.1.0/images/example_json_output.png
+-rw-r--r--   0 alexandre   (501) staff       (20)    53710 2022-03-03 22:33:26.000000 pycobertura-3.1.0/images/example_markdown_diff_output.png
+-rw-r--r--   0 alexandre   (501) staff       (20)    45822 2022-03-03 22:33:26.000000 pycobertura-3.1.0/images/example_yaml_output.png
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.520728 pycobertura-3.1.0/pycobertura/
+-rw-r--r--   0 alexandre   (501) staff       (20)      119 2022-01-04 01:58:44.000000 pycobertura-3.1.0/pycobertura/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     8792 2023-04-29 17:12:19.000000 pycobertura-3.1.0/pycobertura/cli.py
+-rw-r--r--   0 alexandre   (501) staff       (20)    15355 2022-10-24 18:43:16.000000 pycobertura-3.1.0/pycobertura/cobertura.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     4886 2023-04-29 17:12:17.000000 pycobertura-3.1.0/pycobertura/filesystem.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      203 2023-04-05 07:16:26.000000 pycobertura-3.1.0/pycobertura/merge.py
+-rw-r--r--   0 alexandre   (501) staff       (20)    16812 2023-04-29 17:12:19.000000 pycobertura-3.1.0/pycobertura/reporters.py
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.523199 pycobertura-3.1.0/pycobertura/templates/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.1.0/pycobertura/templates/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      624 2022-10-07 08:01:13.000000 pycobertura-3.1.0/pycobertura/templates/filters.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     2805 2022-03-04 19:55:00.000000 pycobertura-3.1.0/pycobertura/templates/html-delta.jinja2
+-rw-r--r--   0 alexandre   (501) staff       (20)     1764 2022-03-03 22:33:26.000000 pycobertura-3.1.0/pycobertura/templates/html.jinja2
+-rw-r--r--   0 alexandre   (501) staff       (20)      473 2022-01-04 01:58:44.000000 pycobertura-3.1.0/pycobertura/templates/macro.source.jinja2
+-rw-r--r--   0 alexandre   (501) staff       (20)     7797 2022-01-04 01:58:44.000000 pycobertura-3.1.0/pycobertura/templates/normalize.css
+-rw-r--r--   0 alexandre   (501) staff       (20)    11452 2022-01-04 01:58:44.000000 pycobertura-3.1.0/pycobertura/templates/skeleton.css
+-rw-r--r--   0 alexandre   (501) staff       (20)     7151 2022-10-07 23:42:24.000000 pycobertura-3.1.0/pycobertura/utils.py
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.521979 pycobertura-3.1.0/pycobertura.egg-info/
+-rw-r--r--   0 alexandre   (501) staff       (20)    23730 2023-04-29 17:18:42.000000 pycobertura-3.1.0/pycobertura.egg-info/PKG-INFO
+-rw-r--r--   0 alexandre   (501) staff       (20)     3363 2023-04-29 17:18:42.000000 pycobertura-3.1.0/pycobertura.egg-info/SOURCES.txt
+-rw-r--r--   0 alexandre   (501) staff       (20)        1 2023-04-29 17:18:42.000000 pycobertura-3.1.0/pycobertura.egg-info/dependency_links.txt
+-rw-r--r--   0 alexandre   (501) staff       (20)       60 2023-04-29 17:18:42.000000 pycobertura-3.1.0/pycobertura.egg-info/entry_points.txt
+-rw-r--r--   0 alexandre   (501) staff       (20)        1 2022-03-04 19:49:40.000000 pycobertura-3.1.0/pycobertura.egg-info/not-zip-safe
+-rw-r--r--   0 alexandre   (501) staff       (20)       44 2023-04-29 17:18:42.000000 pycobertura-3.1.0/pycobertura.egg-info/requires.txt
+-rw-r--r--   0 alexandre   (501) staff       (20)       12 2023-04-29 17:18:42.000000 pycobertura-3.1.0/pycobertura.egg-info/top_level.txt
+-rw-r--r--   0 alexandre   (501) staff       (20)      122 2022-03-03 22:33:26.000000 pycobertura-3.1.0/pyproject.toml
+-rw-r--r--   0 alexandre   (501) staff       (20)      997 2022-10-07 08:01:13.000000 pycobertura-3.1.0/pytest.ini
+-rwxr-xr-x   0 alexandre   (501) staff       (20)      415 2022-10-09 09:37:38.000000 pycobertura-3.1.0/release.sh
+-rw-r--r--   0 alexandre   (501) staff       (20)     1300 2023-04-29 17:18:42.535201 pycobertura-3.1.0/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)       38 2022-03-03 22:33:26.000000 pycobertura-3.1.0/setup.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       82 2022-10-07 08:01:13.000000 pycobertura-3.1.0/test-requirements.txt
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.527942 pycobertura-3.1.0/tests/
+-rw-r--r--   0 alexandre   (501) staff       (20)       64 2022-10-07 23:42:24.000000 pycobertura-3.1.0/tests/.testgitignore
+-rw-r--r--   0 alexandre   (501) staff       (20)      748 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/README.generate-dummy-coverage-for-testing.md
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1162 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/cobertura-generated-by-istanbul-from-coffeescript.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)     7963 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/cobertura.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.528612 pycobertura-3.1.0/tests/dummy/
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.534570 pycobertura-3.1.0/tests/dummy/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       41 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy/dummy/dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       20 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy/dummy/dummy2.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      995 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy/dummy-with-prefix.zip
+-rw-r--r--   0 alexandre   (501) staff       (20)      687 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy/dummy.zip
+-rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)      179 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy/test_dummy.py
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.528904 pycobertura-3.1.0/tests/dummy.linestatus/
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.529053 pycobertura-3.1.0/tests/dummy.linestatus/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)       14 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.linestatus/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      623 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.linestatus/test1.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)      578 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.linestatus/test2.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)      861 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.original-better-cov.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)      852 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.original-full-cov.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)      858 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.original.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.529530 pycobertura-3.1.0/tests/dummy.source1/
+-rw-r--r--   0 alexandre   (501) staff       (20)     1456 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.source1/coverage.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.530105 pycobertura-3.1.0/tests/dummy.source1/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.source1/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       56 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.source1/dummy/dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       20 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.source1/dummy/dummy2.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       64 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.source1/dummy/dummy4.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.source1/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)      119 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.source1/test_dummy.py
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.530563 pycobertura-3.1.0/tests/dummy.source2/
+-rw-r--r--   0 alexandre   (501) staff       (20)     1423 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.source2/coverage.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.531062 pycobertura-3.1.0/tests/dummy.source2/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.source2/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       56 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.source2/dummy/dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       44 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.source2/dummy/dummy2.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      209 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.source2/dummy/dummy3.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.source2/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)      179 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.source2/test_dummy.py
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.531488 pycobertura-3.1.0/tests/dummy.uncovered/
+-rw-r--r--   0 alexandre   (501) staff       (20)     1178 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.uncovered/coverage.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.532431 pycobertura-3.1.0/tests/dummy.uncovered/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.uncovered/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      114 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.uncovered/dummy/dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.uncovered/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)      178 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.uncovered/test_dummy.py
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.531929 pycobertura-3.1.0/tests/dummy.uncovered.addcode/
+-rw-r--r--   0 alexandre   (501) staff       (20)     1250 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.uncovered.addcode/coverage.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.532183 pycobertura-3.1.0/tests/dummy.uncovered.addcode/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.uncovered.addcode/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      185 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.uncovered.addcode/dummy/dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.uncovered.addcode/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)      178 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.uncovered.addcode/test_dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1093 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.with-dummy2-better-and-worse.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)     1092 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.with-dummy2-better-cov.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)     1080 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.with-dummy2-full-cov.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)     1090 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.with-dummy2-no-cov.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.533163 pycobertura-3.1.0/tests/dummy.zeroexit1/
+-rw-r--r--   0 alexandre   (501) staff       (20)      969 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.zeroexit1/coverage.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.533474 pycobertura-3.1.0/tests/dummy.zeroexit1/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.zeroexit1/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      108 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.zeroexit1/dummy/dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.zeroexit1/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)       58 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.zeroexit1/test_dummy.py
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.533954 pycobertura-3.1.0/tests/dummy.zeroexit2/
+-rw-r--r--   0 alexandre   (501) staff       (20)     1000 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.zeroexit2/coverage.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-04-29 17:18:42.534205 pycobertura-3.1.0/tests/dummy.zeroexit2/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.zeroexit2/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      134 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.zeroexit2/dummy/dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.zeroexit2/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)       68 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/dummy.zeroexit2/test_dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)    29409 2023-04-29 17:12:19.000000 pycobertura-3.1.0/tests/test_cli.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     9064 2022-03-03 22:33:26.000000 pycobertura-3.1.0/tests/test_cobertura.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     5737 2022-10-07 08:01:13.000000 pycobertura-3.1.0/tests/test_cobertura_diff.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      127 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/test_colorize.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      429 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/test_extrapolate_coverage.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     6494 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/test_filesystem.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     6429 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/test_hunkify_coverage.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      187 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/test_imports.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1166 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/test_rangify.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1076 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/test_reconcile_lines.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      926 2022-10-07 23:42:24.000000 pycobertura-3.1.0/tests/test_regex_utils.py
+-rw-r--r--   0 alexandre   (501) staff       (20)    20163 2023-04-29 17:12:19.000000 pycobertura-3.1.0/tests/test_reporters.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1175 2022-03-03 22:33:26.000000 pycobertura-3.1.0/tests/test_stringify.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      420 2022-01-04 01:58:44.000000 pycobertura-3.1.0/tests/utils.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      528 2022-10-07 08:01:13.000000 pycobertura-3.1.0/tox.ini
```

### Comparing `pycobertura-3.0.0/.github/workflows/build-and-test-pycobertura.yml` & `pycobertura-3.1.0/.github/workflows/build-and-test-pycobertura.yml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/.gitignore` & `pycobertura-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/CHANGES.md` & `pycobertura-3.1.0/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Release Notes
 
 ## Unreleased
 
+## 3.1.0 (2023-04-29)
+
+* `pycobertura show` now supports output format: `github-annotation`. Thanks @goatwu1993
+
 ## 3.0.0 (2022-10-08)
 
 * BACKWARD INCOMPATIBLE:
   * Deprecate Python3.5 and 3.6, support Python 3.7 onwards (see
     python_requires, classifiers in `setup.cfg`)
   * Update tests to Python 3.7 through 3.9 (affects `tox.ini` and `.travis.yml`)
   * Migrate to `setup.cfg` and `pyproject.toml`; empty `setup.py` kept for
```

### Comparing `pycobertura-3.0.0/LICENSE` & `pycobertura-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/PKG-INFO` & `pycobertura-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycobertura
-Version: 3.0.0
+Version: 3.1.0
 Summary: "A Cobertura coverage parser that can diff reports and show coverage progress."
 Home-page: https://github.com/aconrad/pycobertura
 Author: "Alex Conrad"
 Author-email: "alexandre.conrad@gmail.com"
 Maintainer: "Alex Conrad"
 Maintainer-email: "alexandre.conrad@gmail.com"
 Keywords: "cobertura coverage diff report parser parse xml"
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pycobertura
 
-<img src="aysha-logo.svg" alt="pycobertura logo" width="100">
+![pycobertura logo](https://raw.githubusercontent.com/aconrad/pycobertura/master/aysha-logo.svg)
 
 A code coverage diff tool for Cobertura reports.
 
 ![pycobertura](https://github.com/aconrad/pycobertura/actions/workflows/build-and-test-pycobertura.yml/badge.svg)
 [![PyPI](http://img.shields.io/pypi/v/pycobertura.svg?style=flat)](https://pypi.python.org/pypi/pycobertura)
 
 - [About](#about)
@@ -220,14 +220,26 @@
   Filename: TOTAL
   Stmts: 34
   Miss: 3
   Cover: 90.00%
 
 ```
 
+The following shows how to generate GitHub annotations given a coverage file.
+
+```shell
+$ pycobertura show --format github-annotation tests/cobertura.xml
+::notice file=dummy/dummy.py,line=5,endLine=6,title=pycobertura::not covered
+::notice file=dummy/dummy4.py,line=1,endLine=6,title=pycobertura::not covered
+```
+
+If you run it in GitHub Actions/Apps, the above log generates check annotations.
+
+![Example output of github-annotation formatted pycobertura show command](images/example_github_annotation_show.png)
+
 ### Command `diff`
 
 You can also use the `diff` command to show the difference between two coverage
 files. To properly compute the `Missing` column, it is necessary to provide the
 source code that was used to generate each of the passed Cobertura reports
 ([see why](#why-do-i-need-to-provide-the-path-to-the-source-code-directory)).
 
@@ -632,8 +644,8 @@
 Python. If you see issues, please [create a
 ticket](https://github.com/SurveyMonkey/pycobertura/issues).
 
 ## Logo credit
 
 The pycobertura logo, Aysha, was graciously
 [donated](https://github.com/arasatasaygin/openlogos/issues/19) by
-[Open Logos](http://openlogos.org/). Check them out!
+[Open Logos](http://openlogos.org/). 🙇‍ Check them out!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycobertura-3.0.0/README.md` & `pycobertura-3.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pycobertura
 
-<img src="aysha-logo.svg" alt="pycobertura logo" width="100">
+![pycobertura logo](https://raw.githubusercontent.com/aconrad/pycobertura/master/aysha-logo.svg)
 
 A code coverage diff tool for Cobertura reports.
 
 ![pycobertura](https://github.com/aconrad/pycobertura/actions/workflows/build-and-test-pycobertura.yml/badge.svg)
 [![PyPI](http://img.shields.io/pypi/v/pycobertura.svg?style=flat)](https://pypi.python.org/pypi/pycobertura)
 
 - [About](#about)
@@ -196,14 +196,26 @@
   Filename: TOTAL
   Stmts: 34
   Miss: 3
   Cover: 90.00%
 
 ```
 
+The following shows how to generate GitHub annotations given a coverage file.
+
+```shell
+$ pycobertura show --format github-annotation tests/cobertura.xml
+::notice file=dummy/dummy.py,line=5,endLine=6,title=pycobertura::not covered
+::notice file=dummy/dummy4.py,line=1,endLine=6,title=pycobertura::not covered
+```
+
+If you run it in GitHub Actions/Apps, the above log generates check annotations.
+
+![Example output of github-annotation formatted pycobertura show command](images/example_github_annotation_show.png)
+
 ### Command `diff`
 
 You can also use the `diff` command to show the difference between two coverage
 files. To properly compute the `Missing` column, it is necessary to provide the
 source code that was used to generate each of the passed Cobertura reports
 ([see why](#why-do-i-need-to-provide-the-path-to-the-source-code-directory)).
 
@@ -608,8 +620,8 @@
 Python. If you see issues, please [create a
 ticket](https://github.com/SurveyMonkey/pycobertura/issues).
 
 ## Logo credit
 
 The pycobertura logo, Aysha, was graciously
 [donated](https://github.com/arasatasaygin/openlogos/issues/19) by
-[Open Logos](http://openlogos.org/). Check them out!
+[Open Logos](http://openlogos.org/). 🙇‍ Check them out!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycobertura-3.0.0/aysha-logo.svg` & `pycobertura-3.1.0/aysha-logo.svg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/images/example_csv_diff_output.png` & `pycobertura-3.1.0/images/example_csv_diff_output.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/images/example_json_output.png` & `pycobertura-3.1.0/images/example_json_output.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/images/example_markdown_diff_output.png` & `pycobertura-3.1.0/images/example_markdown_diff_output.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/images/example_yaml_output.png` & `pycobertura-3.1.0/images/example_yaml_output.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/pycobertura/cli.py` & `pycobertura-3.1.0/pycobertura/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import click
 
 from pycobertura.cobertura import Cobertura
 from pycobertura.reporters import (
+    GitHubAnnotationReporter,
     HtmlReporter,
     TextReporter,
     CsvReporter,
     MarkdownReporter,
     JsonReporter,
     YamlReporter,
     HtmlReporterDelta,
@@ -24,14 +25,15 @@
 reporters = {
     "html": HtmlReporter,
     "text": TextReporter,
     "csv": CsvReporter,
     "markdown": MarkdownReporter,
     "json": JsonReporter,
     "yaml": YamlReporter,
+    "github-annotation": GitHubAnnotationReporter,
 }
 
 
 class ExitCodes:
     OK = 0
     EXCEPTION = 1
     COVERAGE_WORSENED = 2
@@ -69,14 +71,32 @@
     "-delim",
     "--delimiter",
     default=";",
     type=str,
     help="Delimiter for csv format, e.g. ,;\n\t",
 )
 @click.option(
+    "--annotation-title",
+    default="pycobertura",
+    type=str,
+    help="annotation title for github annotation format",
+)
+@click.option(
+    "--annotation-level",
+    default="notice",
+    type=str,
+    help="annotation level for github annotation format",
+)
+@click.option(
+    "--annotation-message",
+    default="not covered",
+    type=str,
+    help="annotation message for github annotation format",
+)
+@click.option(
     "-o",
     "--output",
     metavar="<file>",
     type=click.File("wb"),
     help="Write output to <file> instead of stdout.",
 )
 @click.option(
@@ -92,15 +112,24 @@
     metavar="<dir-prefix>",
     help="For every file found in the coverage report, it will use this "
     "prefix to lookup files on disk. This is especially useful when "
     "the --source is a zip archive and the files were zipped under "
     "a directory prefix that is not part of the source.",
 )
 def show(
-    cobertura_file, ignore_regex, format, delimiter, output, source, source_prefix
+    cobertura_file,
+    ignore_regex,
+    format,
+    delimiter,
+    output,
+    source,
+    source_prefix,
+    annotation_level,
+    annotation_title,
+    annotation_message,
 ):
     """show coverage summary of a Cobertura report"""
 
     if not source:
         source = get_dir_from_file_path(cobertura_file)
 
     cobertura = Cobertura(
@@ -108,14 +137,20 @@
         filesystem=filesystem_factory(source, source_prefix=source_prefix),
     )
     Reporter = reporters[format]
     reporter = Reporter(cobertura, ignore_regex)
 
     if format == "csv":
         report = reporter.generate(delimiter)
+    elif format == "github-annotation":
+        report = reporter.generate(
+            annotation_level=annotation_level,
+            annotation_title=annotation_title,
+            annotation_message=annotation_message,
+        )
     else:
         report = reporter.generate()
 
     if not isinstance(report, bytes):
         report = report.encode("utf-8")
 
     isatty = True if output is None else output.isatty()
```

### Comparing `pycobertura-3.0.0/pycobertura/cobertura.py` & `pycobertura-3.1.0/pycobertura/cobertura.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/pycobertura/filesystem.py` & `pycobertura-3.1.0/pycobertura/filesystem.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/pycobertura/reporters.py` & `pycobertura-3.1.0/pycobertura/reporters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from jinja2 import Environment, PackageLoader
 from pycobertura.cobertura import CoberturaDiff
-from pycobertura.utils import green, red, stringify
+from pycobertura.utils import green, red, stringify, rangify
 from pycobertura.templates import filters
 from tabulate import tabulate
 from ruamel import yaml
 import json
 import io
 
 
@@ -439,7 +439,45 @@
                 differ_file_source_hunks = self.differ.file_source_hunks(filename)
                 if differ_file_source_hunks:
                     render_kwargs["sources"].append(
                         (filename, differ_file_source_hunks)
                     )
 
         return template.render(**render_kwargs)
+
+
+class GitHubAnnotationReporter(Reporter):
+    def generate(
+        self,
+        annotation_level: str,
+        annotation_title: str,
+        annotation_message: str,
+    ):
+        file_names = self.cobertura.files(ignore_regex=self.ignore_regex)
+        result_strs = []
+        for file_name in file_names:
+            for range_start, range_end in rangify(
+                self.cobertura.missed_lines(file_name)
+            ):
+                result_strs.append(
+                    self.to_github_annotation_message(
+                        file_name=file_name,
+                        start_line_num=range_start,
+                        end_line_num=range_end,
+                        annotation_level=annotation_level,
+                        annotation_title=annotation_title,
+                        annotation_message=annotation_message,
+                    )
+                )
+        result = "\n".join(result_strs)
+        return result
+
+    @staticmethod
+    def to_github_annotation_message(
+        file_name: str,
+        start_line_num: int,
+        end_line_num: int,
+        annotation_level: str,
+        annotation_title: str,
+        annotation_message: str,
+    ):
+        return f"::{annotation_level} file={file_name},line={start_line_num},endLine={end_line_num},title={annotation_title}::{annotation_message}"  # noqa
```

### Comparing `pycobertura-3.0.0/pycobertura/templates/filters.py` & `pycobertura-3.1.0/pycobertura/templates/filters.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/pycobertura/templates/html-delta.jinja2` & `pycobertura-3.1.0/pycobertura/templates/html-delta.jinja2`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/pycobertura/templates/html.jinja2` & `pycobertura-3.1.0/pycobertura/templates/html.jinja2`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/pycobertura/templates/normalize.css` & `pycobertura-3.1.0/pycobertura/templates/normalize.css`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/pycobertura/templates/skeleton.css` & `pycobertura-3.1.0/pycobertura/templates/skeleton.css`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/pycobertura/utils.py` & `pycobertura-3.1.0/pycobertura/utils.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/pycobertura.egg-info/PKG-INFO` & `pycobertura-3.1.0/pycobertura.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycobertura
-Version: 3.0.0
+Version: 3.1.0
 Summary: "A Cobertura coverage parser that can diff reports and show coverage progress."
 Home-page: https://github.com/aconrad/pycobertura
 Author: "Alex Conrad"
 Author-email: "alexandre.conrad@gmail.com"
 Maintainer: "Alex Conrad"
 Maintainer-email: "alexandre.conrad@gmail.com"
 Keywords: "cobertura coverage diff report parser parse xml"
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pycobertura
 
-<img src="aysha-logo.svg" alt="pycobertura logo" width="100">
+![pycobertura logo](https://raw.githubusercontent.com/aconrad/pycobertura/master/aysha-logo.svg)
 
 A code coverage diff tool for Cobertura reports.
 
 ![pycobertura](https://github.com/aconrad/pycobertura/actions/workflows/build-and-test-pycobertura.yml/badge.svg)
 [![PyPI](http://img.shields.io/pypi/v/pycobertura.svg?style=flat)](https://pypi.python.org/pypi/pycobertura)
 
 - [About](#about)
@@ -220,14 +220,26 @@
   Filename: TOTAL
   Stmts: 34
   Miss: 3
   Cover: 90.00%
 
 ```
 
+The following shows how to generate GitHub annotations given a coverage file.
+
+```shell
+$ pycobertura show --format github-annotation tests/cobertura.xml
+::notice file=dummy/dummy.py,line=5,endLine=6,title=pycobertura::not covered
+::notice file=dummy/dummy4.py,line=1,endLine=6,title=pycobertura::not covered
+```
+
+If you run it in GitHub Actions/Apps, the above log generates check annotations.
+
+![Example output of github-annotation formatted pycobertura show command](images/example_github_annotation_show.png)
+
 ### Command `diff`
 
 You can also use the `diff` command to show the difference between two coverage
 files. To properly compute the `Missing` column, it is necessary to provide the
 source code that was used to generate each of the passed Cobertura reports
 ([see why](#why-do-i-need-to-provide-the-path-to-the-source-code-directory)).
 
@@ -632,8 +644,8 @@
 Python. If you see issues, please [create a
 ticket](https://github.com/SurveyMonkey/pycobertura/issues).
 
 ## Logo credit
 
 The pycobertura logo, Aysha, was graciously
 [donated](https://github.com/arasatasaygin/openlogos/issues/19) by
-[Open Logos](http://openlogos.org/). Check them out!
+[Open Logos](http://openlogos.org/). 🙇‍ Check them out!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycobertura-3.0.0/pycobertura.egg-info/SOURCES.txt` & `pycobertura-3.1.0/pycobertura.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 .coveragerc
 .gitignore
 CHANGES.md
 LICENSE
 README.md
+__version__
 aysha-logo.svg
 pyproject.toml
 pytest.ini
 release.sh
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
 .github/workflows/build-and-test-pycobertura.yml
 images/example_csv_diff_output.png
+images/example_github_annotation_show.png
 images/example_json_output.png
 images/example_markdown_diff_output.png
 images/example_yaml_output.png
 pycobertura/__init__.py
 pycobertura/cli.py
 pycobertura/cobertura.py
 pycobertura/filesystem.py
+pycobertura/merge.py
 pycobertura/reporters.py
 pycobertura/utils.py
 pycobertura.egg-info/PKG-INFO
 pycobertura.egg-info/SOURCES.txt
 pycobertura.egg-info/dependency_links.txt
 pycobertura.egg-info/entry_points.txt
 pycobertura.egg-info/not-zip-safe
```

### Comparing `pycobertura-3.0.0/pytest.ini` & `pycobertura-3.1.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/setup.cfg` & `pycobertura-3.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pycobertura
-version = 3.0.0
+version = file: __version__
 description = "A Cobertura coverage parser that can diff reports and show coverage progress."
 author = "Alex Conrad"
 author_email = "alexandre.conrad@gmail.com"
 long_description = file: README.md
 long_description_content_type = text/markdown
 maintainer = "Alex Conrad"
 maintainer_email = "alexandre.conrad@gmail.com"
@@ -25,15 +25,14 @@
 
 [options]
 zip_safe = False
 python_requires = >= 3.7
 packages = find:
 setup_requires = 
 	setuptools_git
-	build
 install_requires = 
 	click>=4.0
 	jinja2
 	lxml
 	tabulate
 	ruamel.yaml
```

### Comparing `pycobertura-3.0.0/tests/README.generate-dummy-coverage-for-testing.md` & `pycobertura-3.1.0/tests/README.generate-dummy-coverage-for-testing.md`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/cobertura-generated-by-istanbul-from-coffeescript.xml` & `pycobertura-3.1.0/tests/cobertura-generated-by-istanbul-from-coffeescript.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/cobertura.xml` & `pycobertura-3.1.0/tests/cobertura.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy/dummy-with-prefix.zip` & `pycobertura-3.1.0/tests/dummy/dummy-with-prefix.zip`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy/dummy.zip` & `pycobertura-3.1.0/tests/dummy/dummy.zip`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy/setup.cfg` & `pycobertura-3.1.0/tests/dummy/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.linestatus/test1.xml` & `pycobertura-3.1.0/tests/dummy.linestatus/test1.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.linestatus/test2.xml` & `pycobertura-3.1.0/tests/dummy.linestatus/test2.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.original-better-cov.xml` & `pycobertura-3.1.0/tests/dummy.original-better-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.original-full-cov.xml` & `pycobertura-3.1.0/tests/dummy.original-full-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.original.xml` & `pycobertura-3.1.0/tests/dummy.original.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.source1/coverage.xml` & `pycobertura-3.1.0/tests/dummy.source1/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.source1/setup.cfg` & `pycobertura-3.1.0/tests/dummy.source1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.source2/coverage.xml` & `pycobertura-3.1.0/tests/dummy.source2/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.source2/setup.cfg` & `pycobertura-3.1.0/tests/dummy.source2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.uncovered/coverage.xml` & `pycobertura-3.1.0/tests/dummy.uncovered/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.uncovered/setup.cfg` & `pycobertura-3.1.0/tests/dummy.uncovered/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.uncovered.addcode/coverage.xml` & `pycobertura-3.1.0/tests/dummy.uncovered.addcode/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.uncovered.addcode/setup.cfg` & `pycobertura-3.1.0/tests/dummy.uncovered.addcode/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.with-dummy2-better-and-worse.xml` & `pycobertura-3.1.0/tests/dummy.with-dummy2-better-and-worse.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.with-dummy2-better-cov.xml` & `pycobertura-3.1.0/tests/dummy.with-dummy2-better-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.with-dummy2-full-cov.xml` & `pycobertura-3.1.0/tests/dummy.with-dummy2-full-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.with-dummy2-no-cov.xml` & `pycobertura-3.1.0/tests/dummy.with-dummy2-no-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.zeroexit1/coverage.xml` & `pycobertura-3.1.0/tests/dummy.zeroexit1/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.zeroexit1/setup.cfg` & `pycobertura-3.1.0/tests/dummy.zeroexit1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.zeroexit2/coverage.xml` & `pycobertura-3.1.0/tests/dummy.zeroexit2/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/dummy.zeroexit2/setup.cfg` & `pycobertura-3.1.0/tests/dummy.zeroexit2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/test_cli.py` & `pycobertura-3.1.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,14 +200,60 @@
   Stmts: 4
   Miss: 2
   Cover: 50.00%
 
 """
     assert result.exit_code == ExitCodes.OK
 
+def test_show__format_github_annotation():
+    from pycobertura.cli import show, ExitCodes
+
+    runner = CliRunner()
+    for opt in ("-f", "--format"):
+        result = runner.invoke(
+            show,
+            ["tests/dummy.original.xml", opt, "github-annotation"],
+            catch_exceptions=False,
+        )
+        assert (
+            result.output
+            == """\
+::notice file=dummy/dummy.py,line=2,endLine=2,title=pycobertura::not covered
+::notice file=dummy/dummy.py,line=5,endLine=5,title=pycobertura::not covered
+"""
+        )
+    assert result.exit_code == ExitCodes.OK
+
+
+def test_show__format_github_annotation_custom_annotation_input():
+    from pycobertura.cli import show, ExitCodes
+
+    runner = CliRunner()
+    for opt in ("-f", "--format"):
+        result = runner.invoke(
+            show,
+            [
+                "tests/dummy.original.xml",
+                opt,
+                "github-annotation",
+                "--annotation-title=coverage.py",
+                "--annotation-level=error",
+                "--annotation-message=missing coverage",
+            ],
+            catch_exceptions=False,
+        )
+        assert (
+            result.output
+            == """\
+::error file=dummy/dummy.py,line=2,endLine=2,title=coverage.py::missing coverage
+::error file=dummy/dummy.py,line=5,endLine=5,title=coverage.py::missing coverage
+"""
+        )
+    assert result.exit_code == ExitCodes.OK
+
 
 def test_show__output_to_file():
     from pycobertura.cli import show, ExitCodes
 
     runner = CliRunner()
     for opt in ('-o', '--output'):
         result = runner.invoke(show, [
```

### Comparing `pycobertura-3.0.0/tests/test_cobertura.py` & `pycobertura-3.1.0/tests/test_cobertura.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/test_cobertura_diff.py` & `pycobertura-3.1.0/tests/test_cobertura_diff.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/test_filesystem.py` & `pycobertura-3.1.0/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/test_hunkify_coverage.py` & `pycobertura-3.1.0/tests/test_hunkify_coverage.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/test_rangify.py` & `pycobertura-3.1.0/tests/test_rangify.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/test_reconcile_lines.py` & `pycobertura-3.1.0/tests/test_reconcile_lines.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/test_regex_utils.py` & `pycobertura-3.1.0/tests/test_regex_utils.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tests/test_reporters.py` & `pycobertura-3.1.0/tests/test_reporters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 from .utils import make_cobertura
 
 
 def remove_style_tag(html):
     style_pattern_start = '\n    <style>'
     style_pattern_stop = '\n    </style>'
     style_starts = html.find(style_pattern_start)
@@ -657,7 +659,49 @@
       </td>
     </tr>
   </tbody>
 </table>
     </div>
   </body>
 </html>"""
+
+@pytest.mark.parametrize(
+    "report, expected_default_output, expected_custom_output",
+    [
+        (
+            "tests/cobertura.xml",
+            """\
+::notice file=search/BinarySearch.java,line=24,endLine=24,title=pycobertura::not covered
+::notice file=search/LinearSearch.java,line=19,endLine=24,title=pycobertura::not covered""",
+            """\
+::error file=search/BinarySearch.java,line=24,endLine=24,title=JCov::missing coverage
+::error file=search/LinearSearch.java,line=19,endLine=24,title=JCov::missing coverage""",
+        ),
+        (
+            "tests/cobertura-generated-by-istanbul-from-coffeescript.xml",
+            "::notice file=app.coffee,line=10,endLine=10,title=pycobertura::not covered",
+            "::error file=app.coffee,line=10,endLine=10,title=JCov::missing coverage",
+        ),
+    ],
+)
+def test_github_annotation_report(
+    report, expected_default_output, expected_custom_output
+):
+    from pycobertura.reporters import GitHubAnnotationReporter
+
+    cobertura = make_cobertura(report)
+    report = GitHubAnnotationReporter(cobertura)
+    default_config = {
+        "annotation_level": "notice",
+        "annotation_title": "pycobertura",
+        "annotation_message": "not covered",
+    }
+
+    assert report.generate(**default_config) == expected_default_output
+    assert (
+        report.generate(
+            annotation_level="error",
+            annotation_title="JCov",
+            annotation_message="missing coverage",
+        )
+        == expected_custom_output
+    )
```

### Comparing `pycobertura-3.0.0/tests/test_stringify.py` & `pycobertura-3.1.0/tests/test_stringify.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.0.0/tox.ini` & `pycobertura-3.1.0/tox.ini`

 * *Files identical despite different names*


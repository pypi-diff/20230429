# Comparing `tmp/genno-1.9.1.tar.gz` & `tmp/genno-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genno-1.9.1.tar", last modified: Thu Jan 27 00:05:45 2022, max compression
+gzip compressed data, was "genno-1.9.2.tar", last modified: Thu Mar  3 13:04:30 2022, max compression
```

## Comparing `genno-1.9.1.tar` & `genno-1.9.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.418940 genno-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-01-27 00:05:37.000000 genno-1.9.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.410940 genno-1.9.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-01-27 00:05:37.000000 genno-1.9.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.410940 genno-1.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-01-27 00:05:37.000000 genno-1.9.1/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-01-27 00:05:37.000000 genno-1.9.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-01-27 00:05:37.000000 genno-1.9.1/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-01-27 00:05:37.000000 genno-1.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-01-27 00:05:37.000000 genno-1.9.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-01-27 00:05:37.000000 genno-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-01-27 00:05:45.418940 genno-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-01-27 00:05:37.000000 genno-1.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.410940 genno-1.9.1/ci/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1412 2022-01-27 00:05:37.000000 genno-1.9.1/ci/install-gams.sh
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-01-27 00:05:37.000000 genno-1.9.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.410940 genno-1.9.1/doc/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-01-27 00:05:37.000000 genno-1.9.1/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-01-27 00:05:37.000000 genno-1.9.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    10385 2022-01-27 00:05:37.000000 genno-1.9.1/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4416 2022-01-27 00:05:37.000000 genno-1.9.1/doc/cache.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-01-27 00:05:37.000000 genno-1.9.1/doc/compat-plotnine.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-01-27 00:05:37.000000 genno-1.9.1/doc/compat-pyam.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2900 2022-01-27 00:05:37.000000 genno-1.9.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     9737 2022-01-27 00:05:37.000000 genno-1.9.1/doc/config.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-01-27 00:05:37.000000 genno-1.9.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-01-27 00:05:37.000000 genno-1.9.1/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-01-27 00:05:37.000000 genno-1.9.1/doc/releasing.rst
--rw-r--r--   0 runner    (1001) docker     (121)    17122 2022-01-27 00:05:37.000000 genno-1.9.1/doc/tutorial.rst.disabled
--rw-r--r--   0 runner    (1001) docker     (121)    10068 2022-01-27 00:05:37.000000 genno-1.9.1/doc/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7803 2022-01-27 00:05:37.000000 genno-1.9.1/doc/whatsnew.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.410940 genno-1.9.1/genno/
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-01-27 00:05:37.000000 genno-1.9.1/genno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6505 2022-01-27 00:05:37.000000 genno-1.9.1/genno/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.414939 genno-1.9.1/genno/compat/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:37.000000 genno-1.9.1/genno/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-01-27 00:05:37.000000 genno-1.9.1/genno/compat/_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.414939 genno-1.9.1/genno/compat/plotnine/
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-01-27 00:05:37.000000 genno-1.9.1/genno/compat/plotnine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3265 2022-01-27 00:05:37.000000 genno-1.9.1/genno/compat/plotnine/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.414939 genno-1.9.1/genno/compat/pyam/
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-01-27 00:05:37.000000 genno-1.9.1/genno/compat/pyam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3402 2022-01-27 00:05:37.000000 genno-1.9.1/genno/compat/pyam/computations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2519 2022-01-27 00:05:37.000000 genno-1.9.1/genno/compat/pyam/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    17036 2022-01-27 00:05:37.000000 genno-1.9.1/genno/computations.py
--rw-r--r--   0 runner    (1001) docker     (121)     8675 2022-01-27 00:05:37.000000 genno-1.9.1/genno/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.414939 genno-1.9.1/genno/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:37.000000 genno-1.9.1/genno/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18585 2022-01-27 00:05:37.000000 genno-1.9.1/genno/core/attrseries.py
--rw-r--r--   0 runner    (1001) docker     (121)    29707 2022-01-27 00:05:37.000000 genno-1.9.1/genno/core/computer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-01-27 00:05:37.000000 genno-1.9.1/genno/core/describe.py
--rw-r--r--   0 runner    (1001) docker     (121)     4217 2022-01-27 00:05:37.000000 genno-1.9.1/genno/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7499 2022-01-27 00:05:37.000000 genno-1.9.1/genno/core/key.py
--rw-r--r--   0 runner    (1001) docker     (121)     6010 2022-01-27 00:05:37.000000 genno-1.9.1/genno/core/quantity.py
--rw-r--r--   0 runner    (1001) docker     (121)     7942 2022-01-27 00:05:37.000000 genno-1.9.1/genno/core/sparsedataarray.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:37.000000 genno-1.9.1/genno/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    11590 2022-01-27 00:05:37.000000 genno-1.9.1/genno/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.414939 genno-1.9.1/genno/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.414939 genno-1.9.1/genno/tests/compat/
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/compat/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2973 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/compat/test_plotnine.py
--rw-r--r--   0 runner    (1001) docker     (121)     9557 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/compat/test_pyam.py
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.414939 genno-1.9.1/genno/tests/core/
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/core/test_attrseries.py
--rw-r--r--   0 runner    (1001) docker     (121)    20976 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/core/test_computer.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/core/test_describe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/core/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2784 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/core/test_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     9499 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/core/test_quantity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/core/test_sparsedataarray.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.418940 genno-1.9.1/genno/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/config-0.json
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/config-0.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/config-aggregate.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/config-combine.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/config-general0.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/config-general1.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/config-global.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/config-pyam.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/config-report.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/config-units.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/dantzig-ACT.csv
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/dantzig-var_cost.csv
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/dantzig-vom.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/describe.txt
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/exceptions.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/input0.csv
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/input1.csv
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/load_file-invalid.csv
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/data/pyam-write.csv
--rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (121)    11556 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/test_computations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-01-27 00:05:37.000000 genno-1.9.1/genno/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     5142 2022-01-27 00:05:37.000000 genno-1.9.1/genno/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 00:05:45.414939 genno-1.9.1/genno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-01-27 00:05:45.000000 genno-1.9.1/genno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2324 2022-01-27 00:05:45.000000 genno-1.9.1/genno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-27 00:05:45.000000 genno-1.9.1/genno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-01-27 00:05:45.000000 genno-1.9.1/genno.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-27 00:05:45.000000 genno-1.9.1/genno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-01-27 00:05:45.418940 genno-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-01-27 00:05:37.000000 genno-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.454183 genno-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-03-03 13:04:16.000000 genno-1.9.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.442182 genno-1.9.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-03-03 13:04:16.000000 genno-1.9.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.442182 genno-1.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-03-03 13:04:16.000000 genno-1.9.2/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-03-03 13:04:16.000000 genno-1.9.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-03-03 13:04:16.000000 genno-1.9.2/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-03-03 13:04:16.000000 genno-1.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-03-03 13:04:16.000000 genno-1.9.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-03-03 13:04:16.000000 genno-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-03-03 13:04:30.454183 genno-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-03-03 13:04:16.000000 genno-1.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.442182 genno-1.9.2/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1412 2022-03-03 13:04:16.000000 genno-1.9.2/ci/install-gams.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-03-03 13:04:16.000000 genno-1.9.2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.446183 genno-1.9.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-03-03 13:04:16.000000 genno-1.9.2/doc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-03-03 13:04:16.000000 genno-1.9.2/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)    10385 2022-03-03 13:04:16.000000 genno-1.9.2/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4416 2022-03-03 13:04:16.000000 genno-1.9.2/doc/cache.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-03-03 13:04:16.000000 genno-1.9.2/doc/compat-plotnine.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-03-03 13:04:16.000000 genno-1.9.2/doc/compat-pyam.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2900 2022-03-03 13:04:16.000000 genno-1.9.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9737 2022-03-03 13:04:16.000000 genno-1.9.2/doc/config.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-03-03 13:04:16.000000 genno-1.9.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2022-03-03 13:04:16.000000 genno-1.9.2/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-03-03 13:04:16.000000 genno-1.9.2/doc/releasing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    17122 2022-03-03 13:04:16.000000 genno-1.9.2/doc/tutorial.rst.disabled
+-rw-r--r--   0 runner    (1001) docker     (121)    10068 2022-03-03 13:04:16.000000 genno-1.9.2/doc/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8198 2022-03-03 13:04:16.000000 genno-1.9.2/doc/whatsnew.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.446183 genno-1.9.2/genno/
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2022-03-03 13:04:16.000000 genno-1.9.2/genno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6505 2022-03-03 13:04:16.000000 genno-1.9.2/genno/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.446183 genno-1.9.2/genno/compat/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:16.000000 genno-1.9.2/genno/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-03 13:04:16.000000 genno-1.9.2/genno/compat/_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.446183 genno-1.9.2/genno/compat/plotnine/
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2022-03-03 13:04:16.000000 genno-1.9.2/genno/compat/plotnine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3265 2022-03-03 13:04:16.000000 genno-1.9.2/genno/compat/plotnine/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.446183 genno-1.9.2/genno/compat/pyam/
+-rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-03-03 13:04:16.000000 genno-1.9.2/genno/compat/pyam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3402 2022-03-03 13:04:16.000000 genno-1.9.2/genno/compat/pyam/computations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2519 2022-03-03 13:04:16.000000 genno-1.9.2/genno/compat/pyam/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17034 2022-03-03 13:04:16.000000 genno-1.9.2/genno/computations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8675 2022-03-03 13:04:16.000000 genno-1.9.2/genno/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.450183 genno-1.9.2/genno/core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:16.000000 genno-1.9.2/genno/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19258 2022-03-03 13:04:16.000000 genno-1.9.2/genno/core/attrseries.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29707 2022-03-03 13:04:16.000000 genno-1.9.2/genno/core/computer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-03-03 13:04:16.000000 genno-1.9.2/genno/core/describe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4217 2022-03-03 13:04:16.000000 genno-1.9.2/genno/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7499 2022-03-03 13:04:16.000000 genno-1.9.2/genno/core/key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6495 2022-03-03 13:04:16.000000 genno-1.9.2/genno/core/quantity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8155 2022-03-03 13:04:16.000000 genno-1.9.2/genno/core/sparsedataarray.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:16.000000 genno-1.9.2/genno/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    11590 2022-03-03 13:04:16.000000 genno-1.9.2/genno/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.450183 genno-1.9.2/genno/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.450183 genno-1.9.2/genno/tests/compat/
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/compat/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2973 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/compat/test_plotnine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9557 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/compat/test_pyam.py
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.450183 genno-1.9.2/genno/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/core/test_attrseries.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20974 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/core/test_computer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/core/test_describe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/core/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2784 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/core/test_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10309 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/core/test_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/core/test_sparsedataarray.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.454183 genno-1.9.2/genno/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/config-0.json
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/config-0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/config-aggregate.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/config-combine.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/config-general0.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/config-general1.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/config-global.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/config-pyam.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/config-report.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/config-units.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/dantzig-ACT.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/dantzig-var_cost.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/dantzig-vom.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     1690 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/describe.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/exceptions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/input0.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/input1.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/load_file-invalid.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/data/pyam-write.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11550 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/test_computations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-03-03 13:04:16.000000 genno-1.9.2/genno/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5146 2022-03-03 13:04:16.000000 genno-1.9.2/genno/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 13:04:30.446183 genno-1.9.2/genno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-03-03 13:04:30.000000 genno-1.9.2/genno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2324 2022-03-03 13:04:30.000000 genno-1.9.2/genno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-03 13:04:30.000000 genno-1.9.2/genno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-03-03 13:04:30.000000 genno-1.9.2/genno.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-03 13:04:30.000000 genno-1.9.2/genno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-03-03 13:04:30.454183 genno-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-03-03 13:04:16.000000 genno-1.9.2/setup.py
```

### Comparing `genno-1.9.1/.github/workflows/lint.yaml` & `genno-1.9.2/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/.github/workflows/publish.yaml` & `genno-1.9.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/.github/workflows/pytest.yaml` & `genno-1.9.2/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/LICENSE` & `genno-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/PKG-INFO` & `genno-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genno
-Version: 1.9.1
+Version: 1.9.2
 Summary: Efficient, transparent calculation on N-D data
 Home-page: https://github.com/khaeru/genno
 Author: genno contributors
 Author-email: mail@paul.kishimoto.name
 Maintainer: Paul Natsuo Kishimoto
 Maintainer-email: mail@paul.kishimoto.name
 License: GPLv3
```

### Comparing `genno-1.9.1/README.rst` & `genno-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/ci/install-gams.sh` & `genno-1.9.2/ci/install-gams.sh`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/doc/Makefile` & `genno-1.9.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/doc/api.rst` & `genno-1.9.2/doc/api.rst`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/doc/cache.rst` & `genno-1.9.2/doc/cache.rst`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/doc/compat-plotnine.rst` & `genno-1.9.2/doc/compat-plotnine.rst`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/doc/compat-pyam.rst` & `genno-1.9.2/doc/compat-pyam.rst`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/doc/conf.py` & `genno-1.9.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/doc/config.rst` & `genno-1.9.2/doc/config.rst`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/doc/index.rst` & `genno-1.9.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/doc/make.bat` & `genno-1.9.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/doc/releasing.rst` & `genno-1.9.2/doc/releasing.rst`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/doc/tutorial.rst.disabled` & `genno-1.9.2/doc/tutorial.rst.disabled`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/doc/usage.rst` & `genno-1.9.2/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/doc/whatsnew.rst` & `genno-1.9.2/doc/whatsnew.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,21 @@
    :local:
    :backlinks: none
    :depth: 1
 
 .. Next release
 .. ============
 
+v1.9.2 (2022-03-03)
+===================
+
+- Silence :func:`collect_units` when units are explicitly `""`, rather than :obj:`None` (:pull:`56`).
+- Add explicit implementations of :meth:`~.object.__radd__`, :meth:`~.object.__rmul__`, :meth:`~.object.__rsub__` and :meth:`~.object.__rtruediv__` for e.g. ``4.2 * Quantity(...)`` (:pull:`55`)
+- Improve typing of :meth:`.Quantity.shift` (:pull:`55`)
+
 v1.9.1 (2022-01-27)
 ===================
 
 Note that installing ``genno[pyam]`` (including via ``genno[compat]``) currently forces the installation of an old version of :mod:`pint`; version 0.17 or earlier.
 Users wishing to use :mod:`genno.compat.pyam` should first install ``genno[pyam]``, then ``pip install --upgrade pint`` to restore a recent version of pint (0.18 or newer) that is usable with genno.
 
 - :func:`computations.concat` works with :class:`.AttrSeries` with misaligned dimensions (:pull:`53`).
```

### Comparing `genno-1.9.1/genno/__init__.py` & `genno-1.9.2/genno/__init__.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/caching.py` & `genno-1.9.2/genno/caching.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/compat/plotnine/plot.py` & `genno-1.9.2/genno/compat/plotnine/plot.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/compat/pyam/__init__.py` & `genno-1.9.2/genno/compat/pyam/__init__.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/compat/pyam/computations.py` & `genno-1.9.2/genno/compat/pyam/computations.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/compat/pyam/util.py` & `genno-1.9.2/genno/compat/pyam/util.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/computations.py` & `genno-1.9.2/genno/computations.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,15 +419,15 @@
 
     if not u_b.dimensionless:
         raise ValueError(f"Cannot raise to a power with units ({u_b:~})")
 
     if isinstance(a, AttrSeries):
         result = a ** b.align_levels(a)
     else:
-        result = a ** b
+        result = a**b
 
     result.attrs["_unit"] = (
         a.attrs["_unit"] ** unit_exponent
         if unit_exponent
         else pint.get_application_registry().dimensionless
     )
```

### Comparing `genno-1.9.1/genno/config.py` & `genno-1.9.2/genno/config.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/core/attrseries.py` & `genno-1.9.2/genno/core/attrseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
+import warnings
 from functools import partial
-from typing import Any, Hashable, Iterable, Mapping, Union
+from typing import Any, Hashable, Iterable, List, Mapping, Union
 
 import numpy as np
 import pandas as pd
 import pandas.core.indexes.base as ibase
 import xarray as xr
 from xarray.core.utils import either_dict_or_kwargs
 
@@ -362,16 +363,24 @@
 
                 if np.isscalar(i) and drop:
                     to_drop.add(dim)
 
                 # Maybe unpack an xarray DataArray indexers, for pandas
                 idx.append(i.data if isinstance(i, xr.DataArray) else i)
 
-            # Select
-            data = self.loc[tuple(idx)]
+            # Silence a warning from pandas ≥1.4 that may be spurious
+            # FIXME investigate, adjust the code, remove the filter
+            with warnings.catch_warnings():
+                warnings.filterwarnings(
+                    "ignore",
+                    ".*indexing on a MultiIndex with a nested sequence.*",
+                    FutureWarning,
+                )
+                # Select
+                data = self.loc[tuple(idx)]
 
             # Only drop if not returning a scalar value
             if not np.isscalar(data):
                 # Drop levels where a single value was selected
                 data = data.droplevel(list(to_drop & set(data.index.names)))
 
         # Return
@@ -457,16 +466,22 @@
 
         return self.droplevel(to_drop)
 
     def transpose(self, *dims):
         """Like :meth:`xarray.DataArray.transpose`."""
         return self.reorder_levels(dims)
 
-    def to_dataframe(self):
+    def to_dataframe(
+        self, name: Hashable = None, dim_order: List[Hashable] = None
+    ) -> pd.DataFrame:
         """Like :meth:`xarray.DataArray.to_dataframe`."""
+        if dim_order is not None:
+            raise NotImplementedError("dim_order arg to to_dataframe()")
+
+        self.name = name or self.name or "value"  # type: ignore
         return self.to_frame()
 
     def to_series(self):
         """Like :meth:`xarray.DataArray.to_series`."""
         return self
 
     # Internal methods
```

### Comparing `genno-1.9.1/genno/core/computer.py` & `genno-1.9.2/genno/core/computer.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/core/describe.py` & `genno-1.9.2/genno/core/describe.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/core/exceptions.py` & `genno-1.9.2/genno/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/core/key.py` & `genno-1.9.2/genno/core/key.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/core/quantity.py` & `genno-1.9.2/genno/core/quantity.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,14 +62,26 @@
     def units(self, value):
         self.attrs["_unit"] = pint.get_application_registry().Unit(value)
 
     # Type hints for mypy in downstream applications
     def __len__(self) -> int:
         ...  # pragma: no cover
 
+    def __radd__(self, other):
+        ...  # pragma: no cover
+
+    def __rmul__(self, other):
+        ...  # pragma: no cover
+
+    def __rsub__(self, other):
+        ...  # pragma: no cover
+
+    def __rtruediv__(self, other):
+        ...  # pragma: no cover
+
     def __truediv__(self, other) -> "Quantity":
         ...  # pragma: no cover
 
     @property
     def attrs(self) -> Dict[Any, Any]:
         ...  # pragma: no cover
 
@@ -103,14 +115,22 @@
         method: str = None,
         tolerance=None,
         drop: bool = False,
         **indexers_kwargs: Any,
     ) -> "Quantity":
         ...  # pragma: no cover
 
+    def shift(
+        self,
+        shifts: Mapping[Hashable, int] = None,
+        fill_value: Any = None,
+        **shifts_kwargs: int,
+    ):  # NB "Quantity" here offends mypy
+        ...  # pragma: no cover
+
     def to_numpy(self) -> np.ndarray:
         ...  # pragma: no cover
 
     # Internal methods
 
     @staticmethod
     def _get_class(cls=None):
@@ -152,15 +172,15 @@
         new_attrs = getattr(data, "attrs", dict()).copy()
 
         # Overwrite with values from an explicit attrs argument
         new_attrs.update(attrs_arg or dict())
 
         # Store the "units" keyword argument as an attr
         units = kwargs.pop("units", None)
-        if units:
+        if units is not None:
             new_attrs["_unit"] = pint.Unit(units)
 
         return new_attrs
 
 
 def assert_quantity(*args):
     """Assert that each of `args` is a Quantity object.
```

### Comparing `genno-1.9.1/genno/core/sparsedataarray.py` & `genno-1.9.2/genno/core/sparsedataarray.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Hashable, Mapping, Sequence, Tuple, Union
+from typing import Any, Dict, Hashable, List, Mapping, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import sparse
 import xarray as xr
 from xarray.core import dtypes
 from xarray.core.utils import either_dict_or_kwargs
@@ -196,20 +196,24 @@
         else:
             return (
                 super()
                 .sel(indexers=indexers, method=method, tolerance=tolerance, drop=drop)
                 ._sda.convert()
             )
 
-    def to_dataframe(self, name=None):
+    def to_dataframe(
+        self, name: Hashable = None, dim_order: List[Hashable] = None
+    ) -> pd.DataFrame:
         """Convert this array and its coords into a :class:`~xarray.DataFrame`.
 
         Overrides :meth:`~xarray.DataArray.to_dataframe`.
         """
-        return self.to_series().to_frame(name)
+        if dim_order is not None:
+            raise NotImplementedError("dim_order arg to to_dataframe()")
+        return self.to_series().to_frame(name or self.name or "value")
 
     def to_series(self) -> pd.Series:
         """Convert this array into a :class:`~pandas.Series`.
 
         Overrides :meth:`~xarray.DataArray.to_series` to create the series without
         first converting to a potentially very large :class:`numpy.ndarray`.
         """
```

### Comparing `genno-1.9.1/genno/testing.py` & `genno-1.9.2/genno/testing.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/tests/compat/test_plotnine.py` & `genno-1.9.2/genno/tests/compat/test_plotnine.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/tests/compat/test_pyam.py` & `genno-1.9.2/genno/tests/compat/test_pyam.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/tests/core/test_attrseries.py` & `genno-1.9.2/genno/tests/core/test_attrseries.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/tests/core/test_computer.py` & `genno-1.9.2/genno/tests/core/test_computer.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,15 +390,15 @@
     # add_product() works
     key = c.add_product("x squared", "x", "x", sums=True)
 
     # Product has the expected dimensions
     assert key == "x squared:t-y"
 
     # Product has the expected value
-    assert_qty_equal(Quantity(x * x, units=ureg.kilogram ** 2), c.get(key))
+    assert_qty_equal(Quantity(x * x, units=ureg.kilogram**2), c.get(key))
 
     # add('product', ...) works
     key = c.add("product", "x_squared", "x", "x", sums=True)
 
 
 def test_aggregate():
     c = Computer()
```

### Comparing `genno-1.9.1/genno/tests/core/test_exceptions.py` & `genno-1.9.2/genno/tests/core/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/tests/core/test_key.py` & `genno-1.9.2/genno/tests/core/test_key.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/tests/core/test_quantity.py` & `genno-1.9.2/genno/tests/core/test_quantity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Tests for genno.quantity."""
 import logging
+import operator
 import re
 
 import pandas as pd
 import pint
 import pytest
 import xarray as xr
 from numpy import nan
+from pytest import param
 
 from genno import Computer, Quantity, computations
 from genno.core.attrseries import AttrSeries
 from genno.core.quantity import assert_quantity
 from genno.core.sparsedataarray import SparseDataArray
 from genno.testing import add_large_data, assert_qty_allclose, assert_qty_equal
 
@@ -266,15 +268,26 @@
         result = c.get("bigmem")
 
         # Result can be converted to pd.Series
         result.to_series()
 
     def test_to_dataframe(self, a):
         """Test Quantity.to_dataframe()."""
-        assert isinstance(a.to_dataframe(), pd.DataFrame)
+        # Returns pd.DataFrame
+        result = a.to_dataframe()
+        assert isinstance(result, pd.DataFrame)
+
+        # "value" is used as a column name
+        assert ["value"] == result.columns
+
+        # Explicitly passed name produces a named column
+        assert ["foo"] == a.to_dataframe("foo").columns
+
+        with pytest.raises(NotImplementedError):
+            a.to_dataframe(dim_order=["foo", "bar"])
 
     def test_to_series(self, a):
         """Test .to_series() on child classes, and Quantity.from_series."""
         s = a.to_series()
         assert isinstance(s, pd.Series)
 
         Quantity.from_series(s)
@@ -286,7 +299,18 @@
         # Set with a string results in a pint.Unit instance
         a.units = "kg"
         assert pint.Unit("kg") == a.units
 
         # Can be set to dimensionless
         a.units = ""
         assert a.units.dimensionless
+
+    @pytest.mark.parametrize(
+        "op", [operator.add, operator.mul, operator.sub, operator.truediv]
+    )
+    @pytest.mark.parametrize("type_", [int, float, param(str, marks=pytest.mark.xfail)])
+    def test_arithmetic(self, op, type_, a):
+        """Quantity can be added to int or float."""
+        result = op(type_(4.2), a)
+
+        assert (2,) == result.shape
+        assert a.dtype == result.dtype
```

### Comparing `genno-1.9.1/genno/tests/core/test_sparsedataarray.py` & `genno-1.9.2/genno/tests/core/test_sparsedataarray.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/tests/data/dantzig-ACT.csv` & `genno-1.9.2/genno/tests/data/dantzig-ACT.csv`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/tests/data/describe.txt` & `genno-1.9.2/genno/tests/data/describe.txt`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/tests/data/exceptions.ipynb` & `genno-1.9.2/genno/tests/data/exceptions.ipynb`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/tests/data/pyam-write.csv` & `genno-1.9.2/genno/tests/data/pyam-write.csv`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/tests/test_caching.py` & `genno-1.9.2/genno/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/tests/test_computations.py` & `genno-1.9.2/genno/tests/test_computations.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
     assert_qty_equal(A.sel(x="x1", y="y1") ** 2, result.sel(x="x1", y="y1"))
 
     # 2D with units ** int
     A = random_qty(dict(x=3, y=3), units="kg")
     result = computations.pow(A, 2)
 
     # Expected units
-    assert ureg.kg ** 2 == result.attrs["_unit"]
+    assert ureg.kg**2 == result.attrs["_unit"]
 
     # 2D ** 1D
     B = random_qty(dict(y=3))
 
     result = computations.pow(A, B)
 
     # Expected values
@@ -343,17 +343,17 @@
     computations.product(exp, B)
 
 
 @pytest.mark.parametrize(
     "dims, exp_size",
     (
         # Some overlapping dimensions
-        ((dict(a=2, b=2, c=2, d=2), dict(b=2, c=2, d=2, e=2, f=2)), 2 ** 6),
+        ((dict(a=2, b=2, c=2, d=2), dict(b=2, c=2, d=2, e=2, f=2)), 2**6),
         # 1D with disjoint dimensions ** 3 = 3D
-        ((dict(a=2), dict(b=2), dict(c=2)), 2 ** 3),
+        ((dict(a=2), dict(b=2), dict(c=2)), 2**3),
         # 2D × scalar × scalar = 2D
         ((dict(a=2, b=2), dict(), dict()), 4),
         # scalar × 1D × scalar = 1D
         # XFAIL for AttrSeries, not SparseDataArray
         pytest.param((dict(), dict(a=2), dict()), 2, marks=pytest.mark.xfail),
     ),
 )
```

### Comparing `genno-1.9.1/genno/tests/test_config.py` & `genno-1.9.2/genno/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/tests/test_testing.py` & `genno-1.9.2/genno/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/tests/test_util.py` & `genno-1.9.2/genno/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/genno/util.py` & `genno-1.9.2/genno/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 def collect_units(*args):
     """Return the "_unit" attributes of the `args`."""
     registry = pint.get_application_registry()
 
     for arg in args:
         unit = arg.attrs.get("_unit")
-        if not unit:
+        if unit is None:
             log.debug(f"{arg} lacks units; assume dimensionless")
             unit = registry.dimensionless
 
         arg.attrs["_unit"] = registry.Unit(unit)
 
     return tuple(arg.attrs["_unit"] for arg in args)
```

### Comparing `genno-1.9.1/genno.egg-info/PKG-INFO` & `genno-1.9.2/genno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genno
-Version: 1.9.1
+Version: 1.9.2
 Summary: Efficient, transparent calculation on N-D data
 Home-page: https://github.com/khaeru/genno
 Author: genno contributors
 Author-email: mail@paul.kishimoto.name
 Maintainer: Paul Natsuo Kishimoto
 Maintainer-email: mail@paul.kishimoto.name
 License: GPLv3
```

### Comparing `genno-1.9.1/genno.egg-info/SOURCES.txt` & `genno-1.9.2/genno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genno-1.9.1/setup.cfg` & `genno-1.9.2/setup.cfg`

 * *Files identical despite different names*


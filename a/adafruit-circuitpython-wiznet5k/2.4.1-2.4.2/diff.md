# Comparing `tmp/adafruit-circuitpython-wiznet5k-2.4.1.tar.gz` & `tmp/adafruit-circuitpython-wiznet5k-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-wiznet5k-2.4.1.tar", last modified: Wed Apr 19 17:52:22 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-wiznet5k-2.4.2.tar", last modified: Sat Apr 29 15:33:20 2023, max compression
```

## Comparing `adafruit-circuitpython-wiznet5k-2.4.1.tar` & `adafruit-circuitpython-wiznet5k-2.4.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.909604 adafruit-circuitpython-wiznet5k-2.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.909604 adafruit-circuitpython-wiznet5k-2.4.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.909604 adafruit-circuitpython-wiznet5k-2.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.909604 adafruit-circuitpython-wiznet5k-2.4.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.909604 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-19 17:52:22.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-19 17:52:22.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:52:22.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 17:52:22.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 17:52:22.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44913 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    19550 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py
--rw-r--r--   0 runner    (1001) docker     (123)    27026 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_aio_post.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_cheerlights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_cpython_client_for_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_simpletest_manual_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_wsgiserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-19 17:52:05.000000 adafruit-circuitpython-wiznet5k-2.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:22.913604 adafruit-circuitpython-wiznet5k-2.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/tests/extract_unique_dns_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)    22772 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/tests/test_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/tests/test_dns_server_nonbreaking_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-19 17:52:15.000000 adafruit-circuitpython-wiznet5k-2.4.1/tests/test_parse_dns_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:33:20.959564 adafruit-circuitpython-wiznet5k-2.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:33:20.951563 adafruit-circuitpython-wiznet5k-2.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:33:20.951563 adafruit-circuitpython-wiznet5k-2.4.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:33:20.955564 adafruit-circuitpython-wiznet5k-2.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:33:20.955564 adafruit-circuitpython-wiznet5k-2.4.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-29 15:33:20.959564 adafruit-circuitpython-wiznet5k-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:33:20.955564 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_circuitpython_wiznet5k.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-29 15:33:20.000000 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-29 15:33:20.000000 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:33:20.000000 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 15:33:20.000000 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-29 15:33:20.000000 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:33:20.955564 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45047 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/adafruit_wiznet5k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19550 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27026 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:33:20.955564 adafruit-circuitpython-wiznet5k-2.4.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:33:20.955564 adafruit-circuitpython-wiznet5k-2.4.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:33:20.959564 adafruit-circuitpython-wiznet5k-2.4.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/examples/wiznet5k_aio_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/examples/wiznet5k_cheerlights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/examples/wiznet5k_cpython_client_for_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/examples/wiznet5k_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/examples/wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/examples/wiznet5k_simpletest_manual_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/examples/wiznet5k_wsgiserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-29 15:33:04.000000 adafruit-circuitpython-wiznet5k-2.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:33:20.959564 adafruit-circuitpython-wiznet5k-2.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:33:20.959564 adafruit-circuitpython-wiznet5k-2.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/tests/extract_unique_dns_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22772 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/tests/test_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/tests/test_dns_server_nonbreaking_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-29 15:33:13.000000 adafruit-circuitpython-wiznet5k-2.4.2/tests/test_parse_dns_function.py
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-wiznet5k-2.4.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/.gitignore` & `adafruit-circuitpython-wiznet5k-2.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/.pre-commit-config.yaml` & `adafruit-circuitpython-wiznet5k-2.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/.pylintrc` & `adafruit-circuitpython-wiznet5k-2.4.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-wiznet5k-2.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/LICENSE` & `adafruit-circuitpython-wiznet5k-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-wiznet5k-2.4.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/LICENSES/MIT.txt` & `adafruit-circuitpython-wiznet5k-2.4.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-wiznet5k-2.4.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/PKG-INFO` & `adafruit-circuitpython-wiznet5k-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 2.4.1
+Version: 2.4.2
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/README.rst` & `adafruit-circuitpython-wiznet5k-2.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO` & `adafruit-circuitpython-wiznet5k-2.4.2/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 2.4.1
+Version: 2.4.2
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt` & `adafruit-circuitpython-wiznet5k-2.4.2/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k.py` & `adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/adafruit_wiznet5k.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     if TYPE_CHECKING:
         from circuitpython_typing import WriteableBuffer
         import busio
         import digitalio
 except ImportError:
     pass
 
-__version__ = "2.4.1"
+__version__ = "2.4.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k.git"
 
 from random import randint
 import time
 import gc
 from micropython import const
 
@@ -477,14 +477,19 @@
             Detect and reset a W5500 chip. Called at startup to initialize the
             interface hardware.
 
             :return bool: True if a W5500 chip is detected, False if not.
             """
             self._chip_type = "w5500"
             # assert self.sw_reset() == 0, "Chip not reset properly!"
+            self._write_mr(0x80)
+            time.sleep(0.05)
+            if self._read_mr()[0] & 0x80:
+                return False
+
             self._write_mr(0x08)
             # assert self._read_mr()[0] == 0x08, "Expected 0x08."
             if self._read_mr()[0] != 0x08:
                 return False
 
             self._write_mr(0x10)
             # assert self._read_mr()[0] == 0x10, "Expected 0x10."
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_debug.py` & `adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/adafruit_wiznet5k_debug.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py` & `adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_dns.py` & `adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/adafruit_wiznet5k_dns.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py` & `adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     if TYPE_CHECKING:
         from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
 except ImportError:
     pass
 import time
 import adafruit_wiznet5k.adafruit_wiznet5k_socket as socket
 
-# __version__ = "2.4.1"
+# __version__ = "2.4.2"
 # __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_NTP.git"
 
 
 class NTP:
     """Wiznet5k NTP Client."""
 
     def __init__(
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_socket.py` & `adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/adafruit_wiznet5k_socket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py` & `adafruit-circuitpython-wiznet5k-2.4.2/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/docs/_static/favicon.ico` & `adafruit-circuitpython-wiznet5k-2.4.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/docs/api.rst` & `adafruit-circuitpython-wiznet5k-2.4.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/docs/conf.py` & `adafruit-circuitpython-wiznet5k-2.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/docs/index.rst` & `adafruit-circuitpython-wiznet5k-2.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_aio_post.py` & `adafruit-circuitpython-wiznet5k-2.4.2/examples/wiznet5k_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_cheerlights.py` & `adafruit-circuitpython-wiznet5k-2.4.2/examples/wiznet5k_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_cpython_client_for_simpleserver.py` & `adafruit-circuitpython-wiznet5k-2.4.2/examples/wiznet5k_cpython_client_for_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_simpleserver.py` & `adafruit-circuitpython-wiznet5k-2.4.2/examples/wiznet5k_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_simpletest.py` & `adafruit-circuitpython-wiznet5k-2.4.2/examples/wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_simpletest_manual_network.py` & `adafruit-circuitpython-wiznet5k-2.4.2/examples/wiznet5k_simpletest_manual_network.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/examples/wiznet5k_wsgiserver.py` & `adafruit-circuitpython-wiznet5k-2.4.2/examples/wiznet5k_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/pyproject.toml` & `adafruit-circuitpython-wiznet5k-2.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-wiznet5k"
 description = "Pure-Python interface for WIZNET 5k ethernet modules."
-version = "2.4.1"
+version = "2.4.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/tests/extract_unique_dns_responses.py` & `adafruit-circuitpython-wiznet5k-2.4.2/tests/extract_unique_dns_responses.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/tests/test_dhcp.py` & `adafruit-circuitpython-wiznet5k-2.4.2/tests/test_dhcp.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/tests/test_dns_server_nonbreaking_changes.py` & `adafruit-circuitpython-wiznet5k-2.4.2/tests/test_dns_server_nonbreaking_changes.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-2.4.1/tests/test_parse_dns_function.py` & `adafruit-circuitpython-wiznet5k-2.4.2/tests/test_parse_dns_function.py`

 * *Files identical despite different names*


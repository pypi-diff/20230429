# Comparing `tmp/invenio-alma-0.7.6.tar.gz` & `tmp/invenio-alma-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-alma-0.7.6.tar", last modified: Wed Apr 26 16:24:09 2023, max compression
+gzip compressed data, was "invenio-alma-0.8.0.tar", last modified: Sat Apr 29 20:29:04 2023, max compression
```

## Comparing `invenio-alma-0.7.6.tar` & `invenio-alma-0.8.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:24:09.905268 invenio-alma-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-26 16:24:09.905268 invenio-alma-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:24:09.901268 invenio-alma-0.7.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:24:09.901268 invenio-alma-0.7.6/invenio_alma/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/click_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:24:09.901268 invenio-alma-0.7.6/invenio_alma/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:24:09.901268 invenio-alma-0.7.6/invenio_alma/services/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/services/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/services/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/services/sru.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/services/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/invenio_alma/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:24:09.901268 invenio-alma-0.7.6/invenio_alma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-26 16:24:09.000000 invenio-alma-0.7.6/invenio_alma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-26 16:24:09.000000 invenio-alma-0.7.6/invenio_alma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:24:09.000000 invenio-alma-0.7.6/invenio_alma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-26 16:24:09.000000 invenio-alma-0.7.6/invenio_alma.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:24:09.000000 invenio-alma-0.7.6/invenio_alma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-26 16:24:09.000000 invenio-alma-0.7.6/invenio_alma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 16:24:09.000000 invenio-alma-0.7.6/invenio_alma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      550 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-26 16:24:09.905268 invenio-alma-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:24:09.901268 invenio-alma-0.7.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/tests/test_invenio_alma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-26 16:23:58.000000 invenio-alma-0.7.6/tests/test_invenio_alma_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:29:04.978420 invenio-alma-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-29 20:29:04.978420 invenio-alma-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:29:04.974420 invenio-alma-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:29:04.974420 invenio-alma-0.8.0/invenio_alma/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/click_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:29:04.978420 invenio-alma-0.8.0/invenio_alma/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:29:04.978420 invenio-alma-0.8.0/invenio_alma/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/services/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/services/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/services/sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:29:04.978420 invenio-alma-0.8.0/invenio_alma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-29 20:29:04.000000 invenio-alma-0.8.0/invenio_alma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-29 20:29:04.000000 invenio-alma-0.8.0/invenio_alma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 20:29:04.000000 invenio-alma-0.8.0/invenio_alma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-29 20:29:04.000000 invenio-alma-0.8.0/invenio_alma.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 20:29:04.000000 invenio-alma-0.8.0/invenio_alma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-29 20:29:04.000000 invenio-alma-0.8.0/invenio_alma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 20:29:04.000000 invenio-alma-0.8.0/invenio_alma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-29 20:29:04.978420 invenio-alma-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:29:04.978420 invenio-alma-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/tests/test_invenio_alma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/tests/test_invenio_alma_service.py
```

### Comparing `invenio-alma-0.7.6/.editorconfig` & `invenio-alma-0.8.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.6/CHANGES.rst` & `invenio-alma-0.8.0/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,23 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.0 (release 2023-04-29)
+
+- ext: add existence check before resource creation
+- global: use ruff instead of pylint
+- global: add services to export
+- tasks: add option to use update func
+- sru: add search_key on the search
+
+
 Version v0.7.6 (release 2023-04-26)
 
 - fix: remove variable check
 
 
 Version v0.7.5 (release 2023-04-26)
```

### Comparing `invenio-alma-0.7.6/CONTRIBUTING.rst` & `invenio-alma-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.6/LICENSE` & `invenio-alma-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.6/MANIFEST.in` & `invenio-alma-0.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.6/PKG-INFO` & `invenio-alma-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-alma
-Version: 0.7.6
+Version: 0.8.0
 Summary: "Provides API for Alma."
 Home-page: https://github.com/tu-graz-library/invenio-alma
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,23 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.0 (release 2023-04-29)
+
+- ext: add existence check before resource creation
+- global: use ruff instead of pylint
+- global: add services to export
+- tasks: add option to use update func
+- sru: add search_key on the search
+
+
 Version v0.7.6 (release 2023-04-26)
 
 - fix: remove variable check
 
 
 Version v0.7.5 (release 2023-04-26)
```

### Comparing `invenio-alma-0.7.6/README.rst` & `invenio-alma-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.6/docs/Makefile` & `invenio-alma-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.6/docs/conf.py` & `invenio-alma-0.8.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 # Copyright (C) 2021-2022 Graz University of Technology.
 #
 # invenio-alma is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Sphinx configuration."""
 
-import os
-
 from invenio_alma import __version__
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
+nitpick_ignore = [("py:class", "Flask")]
+
+
 # Do not warn on external images.
 suppress_warnings = ["image.nonlocal_uri"]
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `invenio-alma-0.7.6/docs/index.rst` & `invenio-alma-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.6/docs/make.bat` & `invenio-alma-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.6/invenio_alma/api.py` & `invenio-alma-0.8.0/invenio_alma/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 from invenio_search.engine import dsl
 from marshmallow.exceptions import ValidationError
 from sqlalchemy.orm.exc import StaleDataError
 
 from .services import AlmaRESTError, AlmaRESTService, AlmaSRUService
 from .utils import is_duplicate_in_alma
 
+MAX_RETRY_COUNT = 3
+"""There could be problems with opensearch connections. This is the retry counter."""
+
 
 def create_alma_record(
     records_service: Marc21RecordService,
     alma_service: AlmaRESTService,
     identity: Identity,
     marc_id: str,
     cms_id: str = "",
@@ -51,15 +54,15 @@
         return
 
     try:
         response = alma_service.create_record(marc21_record_etree)
         current_app.logger.info(response)
     except AlmaRESTError as rest_error:
         current_app.logger.warning(rest_error)
-        raise rest_error
+        raise
 
 
 def update_repository_record(
     records_service: Marc21RecordService,
     alma_service: AlmaSRUService,
     marc_id: str,
     identity: Identity,
@@ -67,27 +70,29 @@
 ) -> None:
     """Update repository record fetched from alma."""
     marc21_etree = alma_service.get_record(alma_thesis_id)
     marc21_record_from_alma = Marc21Metadata(metadata=marc21_etree)
 
     records_service.edit(id_=marc_id, identity=identity)
     records_service.update_draft(
-        id_=marc_id, identity=identity, metadata=marc21_record_from_alma
+        id_=marc_id,
+        identity=identity,
+        metadata=marc21_record_from_alma,
     )
     records_service.publish(id_=marc_id, identity=identity)
 
 
 def import_record(
     alma_service: AlmaSRUService,
     ac_number: str,
     file_path: str,
     identity: Identity,
     marcid: str = None,
-    **_,
-):
+    **_: any,
+) -> None:
     """Process a single import of a alma record by ac number."""
     if marcid:
         MarcDraftProvider.predefined_pid_value = marcid
 
     service = current_records_marc21.records_service
 
     retry_counter = 0
@@ -113,30 +118,30 @@
         except ValidationError:
             current_app.logger.info(f"ValidationError   search_value: {ac_number}")
             run = False
         except dsl.RequestError:
             current_app.logger.info(f"RequestError      search_value: {ac_number}")
             run = False
         except dsl.ConnectionTimeout:
-            msg = f"ConnectionTimeout search_value: {ac_number}, retry_counter: {retry_counter}"
+            msg = f"ConnectionTimeout search_value: {ac_number}, retry_counter: {retry_counter}"  # noqa: E501
             current_app.logger.info(msg)
 
             # cool down the opensearch indexing process. necessary for
             # multiple imports in a short timeframe
             sleep(100)
 
-            # don't overestimate the problem. if three rounds doesn't help go to
-            # the next ac number
-            if retry_counter > 3:
+            if retry_counter > MAX_RETRY_COUNT:
                 run = False
             retry_counter += 1
 
 
 def import_list_of_records(
-    alma_service: AlmaSRUService, csv_file: DictReader, identity: Identity
-):
+    alma_service: AlmaSRUService,
+    csv_file: DictReader,
+    identity: Identity,
+) -> None:
     """Process csv file."""
     for row in csv_file:
         if len(row["ac_number"]) == 0:
             continue
 
         import_record(alma_service, **row, identity=identity)
```

### Comparing `invenio-alma-0.7.6/invenio_alma/cli.py` & `invenio-alma-0.8.0/invenio_alma/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .click_param_type import CSV
 from .proxies import current_alma
 from .services import AlmaSRUService
 from .utils import preliminaries
 
 
 @click.group()
-def alma():
+def alma() -> None:
     """Alma CLI."""
 
 
 @alma.command()
 @with_appcontext
 @optgroup.group("Request Configuration", help="The Configuration for the request")
 @optgroup.option("--search-key", type=click.STRING, required=True)
@@ -39,143 +39,166 @@
 @optgroup.option("--ac-number", type=click.STRING)
 @optgroup.option("--filename", type=click.STRING)
 @optgroup.option("--user-email", type=click.STRING, default="alma@tugraz.at")
 @optgroup.option("--marcid", type=click.STRING, default="")
 @optgroup.group("Import by file list")
 @optgroup.option("--csv-file", type=CSV())
 def sru(
-    search_key,
-    domain,
-    institution_code,
-    ac_number,
-    filename,
-    user_email,
-    marcid,
-    csv_file,
-):
+    search_key: str,
+    domain: str,
+    institution_code: str,
+    ac_number: str,
+    filename: str,
+    user_email: str,
+    marcid: str,
+    csv_file: CSV,
+) -> None:
     """Search on the SRU service of alma."""
     identity = get_identity_from_user_by_email(email=user_email)
     alma_sru_service = AlmaSRUService.build(search_key, domain, institution_code)
 
     if csv_file:
         import_list_of_records(alma_sru_service, csv_file, identity)
     else:
         import_record(alma_sru_service, ac_number, filename, identity, marcid)
 
 
 @alma.group()
-def create():
+def create() -> None:
     """Alma Create group."""
 
 
 @create.command("alma-record")
 @with_appcontext
 @click.option("--marc-id", type=click.STRING, required=True)
 @click.option("--user-email", type=click.STRING, default="alma@tugraz.at")
 @click.option("--api-key", type=click.STRING, required=True)
 @click.option("--cms-id", type=click.STRING, required=True)
-def cli_create_alma_record(marc_id, user_email, api_key, cms_id):
+def cli_create_alma_record(
+    marc_id: str,
+    user_email: str,
+    api_key: str,
+    cms_id: str,
+) -> None:
     """Create alma record."""
     records_service, alma_service, identity = preliminaries(user_email, use_rest=True)
 
     alma_service.config.api_key = api_key
 
     create_alma_record(records_service, alma_service, identity, marc_id, cms_id)
 
 
 @create.command("repository-record")
 @click.option("--mms-id", type=click.STRING, required=True)
-def create_repository_record(mms_id):  # pylint: disable=unused-argument
+def create_repository_record(mms_id: str) -> None:  # noqa: ARG001
     """Create repository record."""
-    print("not yet implemented")
+    print("not yet implemented")  # noqa: T201
     # TODO:
     # create a record within the repository from an existing alma record
     # with mms_id=[MMS_ID]
     # use service provided by invenio-records-marc21 to create the record
 
     # SKETCH
-    # record = current_alma.record_service.get_record(mms_id)
+    # record = current_alma.record_service.get_record(mms_id) # noqa: ERA001
 
     # TODO:
     # massage data to move 001 mms-id to 035__a (tugraz)mms-id
 
-    # current_records_marc21.record_service.create_record()
+    # current_records_marc21.record_service.create_record() # noqa: ERA001
 
 
 @alma.group()
-def update():
+def update() -> None:
     """Alma update group."""
 
 
 @update.command("repository-record")
 @with_appcontext
 @click.option("--marc-id", type=click.STRING, required=True)
 @click.option("--user-email", type=click.STRING, default="alma@tugraz.at")
 @click.option("--api-key", type=click.STRING, required=True)
 @optgroup.group("Alma identifier", cls=RequiredMutuallyExclusiveOptionGroup)
 @optgroup.option("--mms-id", type=click.STRING, help="mms-id", default=None)
 @optgroup.option("--thesis-id", type=click.STRING, help="thesis-id", default=None)
-def cli_update_repository_record(marc_id, user_email, api_key, mms_id, thesis_id):
+def cli_update_repository_record(
+    marc_id: str,
+    user_email: str,
+    api_key: str,
+    mms_id: str,
+    thesis_id: str,
+) -> None:
     """Update Repository record."""
     if mms_id:
         use_rest = True
         alma_thesis_id = mms_id
     elif thesis_id:
         use_sru = True
         alma_thesis_id = thesis_id
     else:
-        raise RuntimeError("Neither of mms_id and thesis_id were given.")
+        msg = "Neither of mms_id and thesis_id were given."
+        raise RuntimeError(msg)
 
     records_service, alma_service, identity = preliminaries(
-        user_email, use_rest=use_rest, use_sru=use_sru
+        user_email,
+        use_rest=use_rest,
+        use_sru=use_sru,
     )
 
     alma_service.config.api_key = api_key
 
     update_repository_record(
-        records_service, alma_service, marc_id, identity, alma_thesis_id
+        records_service,
+        alma_service,
+        marc_id,
+        identity,
+        alma_thesis_id,
     )
 
 
 @update.command("url-in-alma")
 @with_appcontext
 @click.option(
     "--csv-file",
     type=CSV(header="mms_id,new_url"),
     required=True,
     help="two columns: mms_id and new_url",
 )
-def update_url_in_alma(csv_file):
+def update_url_in_alma(csv_file: CSV) -> None:
     """Update url in remote repository records.
 
     :params csv_file (file) with two columns mms_id and new_url
     """
-    for row in csv_file:
-        current_alma.alma_rest_service.update_field(
-            row["mms_id"], "856.4._.u", row["new_url"]
-        )
+    for mms_id, new_url in csv_file:
+        current_alma.alma_rest_service.update_field(mms_id, "856.4._.u", new_url)
 
 
 @update.command("field")
 @with_appcontext
 @click.option("--mms-id", type=click.STRING, required=True)
 @click.option(
-    "--field-json-path", type=click.STRING, required=True, help="e.g. 100.1._.u"
+    "--field-json-path",
+    type=click.STRING,
+    required=True,
+    help="e.g. 100.1._.u",
 )
 @click.option("--subfield-value", type=click.STRING, default="")
 @click.option("--new-subfield-value", type=click.STRING, required=True)
 @click.option(
     "--new-subfield-template",
     type=click.STRING,
     help="the template is given as json path 100.2.1.u",
     default="",
 )
 def update_field(
-    mms_id, field_json_path, subfield_value, new_subfield_value, new_subfield_template
-):
+    mms_id: str,
+    field_json_path: str,
+    subfield_value: str,
+    new_subfield_value: str,
+    new_subfield_template: str,
+) -> None:
     """Update field."""
     current_alma.alma_rest_service.update_field(
         mms_id,
         field_json_path,
         new_subfield_value,
         subfield_value,
         new_subfield_template,
```

### Comparing `invenio-alma-0.7.6/invenio_alma/click_param_type.py` & `invenio-alma-0.8.0/invenio_alma/click_param_type.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,54 +2,65 @@
 #
 # Copyright (C) 2022 Graz University of Technology.
 #
 # invenio-alma is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Click param types."""
+from __future__ import annotations
 
 import sys
+import typing as t
 from csv import DictReader
-from os.path import isfile
+from pathlib import Path
+from typing import Any
 
 from click import ParamType, secho
 
+if t.TYPE_CHECKING:
+    from io import TextIOWrapper
+
 
 class CSV(ParamType):
     """CSV provides the ability to load a csv from a file."""
 
     name = "CSV"
 
-    def __init__(self, header=None):
-        """Constructor of CSV type."""
+    def __init__(self, header: str = None) -> None:
+        """Create type CSV."""
         super().__init__()
         self.header = header
         self.check_header = header is not None
 
     @property
-    def headers(self):
+    def headers(self) -> list[str]:
         """Headers."""
         return self.header.split(",")
 
-    def is_header_as_expected(self, csv_file):
+    def is_header_as_expected(self, csv_file: TextIOWrapper) -> bool:
         """Check if the header is as expected."""
         reader = DictReader(csv_file)
         first_row = next(reader)
         # because iterator has no previous method
         csv_file.seek(0)
 
         return all(name in first_row for name in self.headers)
 
-    def convert(self, value, param, ctx) -> DictReader:
-        """This method opens the files as a DictReader object."""
-        if not isfile(value):
+    def convert(
+        self,
+        value: Any,  # noqa: ANN401
+        param: Any,  # noqa: ANN401, ARG002
+        ctx: Any,  # noqa: ANN401, ARG002
+    ) -> DictReader:
+        """Convert filename in value to an DictReader object."""
+        if not Path(value).is_file():
             secho("ERROR - please look up if the file path is correct.", fg="red")
             sys.exit()
 
-        csv_file = open(value, mode="r", encoding="utf-8")
+        csv_file = Path(value).open(mode="r", encoding="utf-8")
         reader = DictReader(csv_file)
 
         if self.check_header and not self.is_header_as_expected(csv_file):
             msg = f"ERROR - the header should have the form: {self.header}."
             secho(msg, fg="red")
             sys.exit()
```

### Comparing `invenio-alma-0.7.6/invenio_alma/config.py` & `invenio-alma-0.8.0/invenio_alma/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,18 @@
 This value should be set on a place which is not under DVCS control.
 """
 
 ALMA_ALMA_RECORDS_CREATE_AGGREGATORS = []
 """List of aggregators with following signature: aggregator() -> list[marc_id]."""
 
 ALMA_REPOSITORY_RECORDS_UPDATE_AGGREGATORS = []
-"""List of aggregators with following signature: aggregator() -> list[tuple[marc_id, alma_id]]."""
+"""List of aggregators with following signature: aggregator() -> list[tuple[marc_id, alma_id]]."""  # noqa: E501
+
+ALMA_REPOSITORY_RECORDS_UPDATE_FUNC = None
+"""This is a callable to make the update process dependend on the workflow."""
 
 ALMA_USER_EMAIL = ""
 """This is the email adress of the alma user in the repository."""
 
 ALMA_ERROR_MAIL_SENDER = ""
 """This is the error mail sender."""
```

### Comparing `invenio-alma-0.7.6/invenio_alma/ext.py` & `invenio-alma-0.8.0/invenio_alma/ext.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,41 +3,50 @@
 # Copyright (C) 2021-2023 Graz University of Technology.
 #
 # invenio-alma is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio module to connect InvenioRDM to Alma."""
 
+from __future__ import annotations
+
+import typing as t
+
+if t.TYPE_CHECKING:
+    from flask import Flask
+
 from .resources import AlmaResource, AlmaResourceConfig
 from .services import AlmaRESTService, AlmaSRUService
 
 
 class InvenioAlma:
     """invenio-alma extension."""
 
-    def __init__(self, app=None):
+    def __init__(self, app: Flask = None) -> None:
         """Extension initialization."""
         if app:
             self.init_app(app)
 
-    def init_app(self, app):
+    def init_app(self, app: Flask) -> None:
         """Flask application initialization."""
         self.init_services(app)
         self.init_resources(app)
         app.extensions["invenio-alma"] = self
 
-    def init_services(self, app):
+    def init_services(self, app: Flask) -> None:
         """Initialize service."""
         api_key = app.config.get("ALMA_API_KEY", "")
         api_host = app.config.get("ALMA_API_HOST", "")
 
-        self.alma_rest_service = AlmaRESTService.build(api_key, api_host)
+        if api_key and api_host:
+            self.alma_rest_service = AlmaRESTService.build(api_key, api_host)
 
-    def init_resources(self, app):
+    def init_resources(self, app: Flask) -> None:
         """Initialize resources."""
         search_key = "local_control_field_009"  # ac_number
         domain = app.config.get("ALMA_SRU_DOMAIN")
         institution_code = app.config.get("ALMA_SRU_INSTITUTION_CODE")
-        self.alma_resource = AlmaResource(
-            service=AlmaSRUService.build(search_key, domain, institution_code),
-            config=AlmaResourceConfig,
-        )
+        if domain and institution_code:
+            self.alma_resource = AlmaResource(
+                service=AlmaSRUService.build(search_key, domain, institution_code),
+                config=AlmaResourceConfig,
+            )
```

### Comparing `invenio-alma-0.7.6/invenio_alma/resources/config.py` & `invenio-alma-0.8.0/invenio_alma/resources/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         "item": "/<any({types}):type>/<record_id>",
     }
 
     response_handlers = {
         "application/json": ResponseHandler(Marc21JSONSerializer()),
         "application/marcxml": ResponseHandler(Marc21XMLSerializer()),
         "application/vnd.inveniomarc21.v1+marcxml": ResponseHandler(
-            Marc21UIXMLSerializer()
+            Marc21UIXMLSerializer(),
         ),
     }
 
     record_id_search_key = {
         "ac_number": "local_control_field_009",
         "mmsid": "mms_id",
     }
```

### Comparing `invenio-alma-0.7.6/invenio_alma/resources/resources.py` & `invenio-alma-0.8.0/invenio_alma/resources/resources.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     request_parser,
     resource_requestctx,
     response_handler,
     route,
 )
 from invenio_records_marc21 import Marc21Metadata
 
-from ..services.errors import AlmaAPIError
+from ..services.errors import AlmaAPIError  # noqa: TID252
 from .config import AlmaResourceConfig
 
 request_view_args = request_parser(from_conf("request_view_args"), location="view_args")
 request_read_args = request_parser(from_conf("request_read_args"), location="args")
 
 request_data = request_body_parser(
     parsers=from_conf("request_body_parsers"),
@@ -36,33 +36,33 @@
 
 class AlmaResource(Resource):
     """Bibliographic record resource."""
 
     config_name = "ALMA_RESOURCES_CONFIG"
     default_config = AlmaResourceConfig
 
-    def __init__(self, service, config=default_config):
+    def __init__(self, service, config=default_config) -> None:  # noqa: ANN001
         """Initialize the alma resource."""
         super().__init__(config=config)
         self.service = service
 
-    def create_url_rules(self):
+    def create_url_rules(self) -> list[dict]:
         """Create the URL rules for the record resource."""
         routes = self.config.routes
         types = ",".join(self.config.record_id_search_key.keys())
         rules = [
             route("GET", routes["item"].format(types=types), self.read),
         ]
 
         return rules
 
     @request_read_args
     @request_view_args
     @response_handler()
-    def read(self):
+    def read(self) -> dict[dict, int]:
         """Read an item."""
         record_id = resource_requestctx.view_args["record_id"]
         type_id = resource_requestctx.view_args["type"]
 
         self.service.config.search_key = self.config.record_id_search_key[type_id]
         try:
             metadata = Marc21Metadata(metadata=self.service.get_record(record_id))
```

### Comparing `invenio-alma-0.7.6/invenio_alma/services/base.py` & `invenio-alma-0.8.0/invenio_alma/services/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 # Copyright (C) 2022 Graz University of Technology.
 #
 # invenio-alma is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 
 """Alma Base Service."""
+from http import HTTPStatus
 from xml.etree.ElementTree import Element, fromstring
 
 from requests import ReadTimeout, get
 
 from .errors import AlmaAPIError
 
 
 class AlmaAPIBase:
     """Alma remote base service."""
 
-    def __init__(self, xpath_to_records, namespaces=None):
-        """Constructor alma api base service."""
+    def __init__(self, xpath_to_records: str, namespaces: str = None) -> None:
+        """Create alma api base service."""
         self.xpath_to_records = xpath_to_records
         self.namespaces = namespaces if namespaces else {}
 
     @property
     def headers(self) -> dict:
         """Headers."""
         return {
@@ -31,15 +32,15 @@
         }
 
     @staticmethod
     def parse_alma_record(data: str) -> Element:
         """Parse Alma record."""
         data = data.encode("utf-8")
 
-        return fromstring(data)
+        return fromstring(data)  # noqa: S314
 
     def extract_alma_records(self, data: str) -> list[Element]:
         """Extract record from request.
 
         :param data (str): result list
 
         :return lxml.Element: extracted record
@@ -47,27 +48,32 @@
         record = self.parse_alma_record(data)
 
         # extract single record
         bibs = list(record.iterfind(self.xpath_to_records, namespaces=self.namespaces))
 
         if len(bibs) == 0:
             msg = f"xpath: {self.xpath_to_records} does not find records."
-            raise AlmaAPIError(code="500", msg=msg)
+            raise AlmaAPIError(code=HTTPStatus.INTERNAL_SERVER_ERROR, msg=msg)
 
         return bibs
 
     def get(self, url: str) -> list[Element]:
         """Alma base api get request.
 
         :param url (str): url to api
 
         :raises AlmaRESTError if request was not successful
 
         :return str: response content
         """
         try:
             response = get(url, headers=self.headers, timeout=10)
-            if response.status_code >= 400:
-                raise AlmaAPIError(code=response.status_code, msg=response.text)
-            return self.extract_alma_records(response.text)
         except ReadTimeout as exc:
-            raise AlmaAPIError(code=500, msg="readtimeout") from exc
+            raise AlmaAPIError(
+                code=HTTPStatus.INTERNAL_SERVER_ERROR,
+                msg="readtimeout",
+            ) from exc
+
+        if response.status_code >= HTTPStatus.BAD_REQUEST:
+            raise AlmaAPIError(code=response.status_code, msg=response.text)
+
+        return self.extract_alma_records(response.text)
```

### Comparing `invenio-alma-0.7.6/invenio_alma/services/config.py` & `invenio-alma-0.8.0/invenio_alma/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.6/invenio_alma/services/rest.py` & `invenio-alma-0.8.0/invenio_alma/services/rest.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 # Copyright (C) 2022 Graz University of Technology.
 #
 # invenio-alma is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 
 """Alma REST Service."""
+from http import HTTPStatus
 from xml.etree.ElementTree import Element, tostring
 
 from requests import ReadTimeout, post, put
 
 from .base import AlmaAPIBase
 from .config import AlmaRESTConfig
 from .errors import AlmaRESTError
 from .utils import jpath_to_xpath
 
 
 class AlmaRESTUrls:
     """Alma REST urls."""
 
-    def __init__(self, config: AlmaRESTConfig):
-        """Constructor Alma REST Urls."""
+    def __init__(self, config: AlmaRESTConfig) -> None:
+        """Create object AlmaRESTUrls."""
         self.config = config
 
     @property
     def base_url(self) -> str:
         """Base url."""
         return f"https://{self.config.api_host}/almaws/v1/bibs"
 
@@ -54,66 +55,77 @@
         """
         return f"{self.base_url}?apikey={self.config.api_key}"
 
 
 class AlmaREST(AlmaAPIBase):
     """Alma REST service class."""
 
-    def __init__(self):
-        """Constructor alma rest service."""
+    def __init__(self) -> None:
+        """Create object AlmaREST."""
         super().__init__(".//bib/record")
 
-    def put(self, url: str, data: str):
+    def put(self, url: str, data: str) -> str:
         """Alma rest api put request.
 
         :param url (str): url to api
         :param data (str): payload
 
         :raises AlmaRESTError if request was not successful
 
         :return str: response content
         """
         try:
             response = put(url, data, headers=self.headers, timeout=10)
-            if response.status_code >= 400:
-                raise AlmaRESTError(code=response.status_code, msg=response.text)
-            return response.text
         except ReadTimeout as exc:
             raise AlmaRESTError(code=500, msg="readtimeout") from exc
 
-    def post(self, url: str, data: str):
+        if response.status_code >= HTTPStatus.BAD_REQUEST:
+            raise AlmaRESTError(code=response.status_code, msg=response.text)
+        return response.text
+
+    def post(self, url: str, data: str) -> None:
         """Alma rest api post request.
 
         :param url (str): url to api_host
         :param data (str): payload
 
         :raises AlmaRESTError if request was not successful
 
         :return str: response content
         """
         try:
             response = post(url, data, headers=self.headers, timeout=10)
-            if response.status_code >= 400:
-                raise AlmaRESTError(code=response.status_code, msg=response.text)
-            return response.text
         except ReadTimeout as exc:
-            raise AlmaRESTError(code=500, msg="readtimeout") from exc
+            raise AlmaRESTError(
+                code=HTTPStatus.INTERNAL_SERVER_ERROR,
+                msg="readtimeout",
+            ) from exc
+
+        if response.status_code >= HTTPStatus.BAD_REQUEST:
+            raise AlmaRESTError(code=response.status_code, msg=response.text)
+
+        return response.text
 
 
 class AlmaRESTService:
     """Alma service class."""
 
-    def __init__(self, config: AlmaRESTConfig, urls: AlmaRESTUrls, service: AlmaREST):
-        """Constructor for AlmaService."""
+    def __init__(
+        self,
+        config: AlmaRESTConfig,
+        urls: AlmaRESTUrls,
+        service: AlmaREST,
+    ) -> None:
+        """Create object from AlmaRESTService."""
         self.config = config
         self.urls = urls
         self.service = service
 
     @classmethod
-    def build(
+    def build(  # noqa: ANN206
         cls,
         api_key: str,
         api_host: str,
         config: AlmaRESTConfig = None,
         urls: AlmaRESTUrls = None,
         service: AlmaREST = None,
     ):  # -> Self >=python3.11 necessary
@@ -129,15 +141,15 @@
         return self.service.get(api_url)  # return etree
 
     @staticmethod
     # pylint: disable-next=unused-argument
     def get_field(
         record: Element,
         field_json_path: str,
-        subfield_value: str = "",  # pylint: disable=unused-argument
+        subfield_value: str = "",  # noqa: ARG004
     ) -> Element:
         """Get field by json path and subfield value if it is set."""
         xpath = jpath_to_xpath(field_json_path)
         field = record.xpath(xpath)
 
         # TODO check about multiple results
         # allowed only one field, otherwise we have a problem and should sys.exit()
@@ -145,15 +157,15 @@
         return field
 
     @staticmethod
     # pylint: disable-next=unused-argument
     def replace_field(
         field: Element,
         new_subfield_value: str,
-        new_subfield_template: str = "",  # pylint: disable=unused-argument
+        new_subfield_template: str = "",  # noqa: ARG004
     ) -> None:
         """Replace in-inplace the subfield value with the new subfield value.
 
         Replace also the metametadata of the field if the template is set.
         """
         # TODO: implement new_subfield_template != ""
```

### Comparing `invenio-alma-0.7.6/invenio_alma/services/sru.py` & `invenio-alma-0.8.0/invenio_alma/services/sru.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,63 +12,71 @@
 from .base import AlmaAPIBase
 from .config import AlmaSRUConfig
 
 
 class AlmaSRUUrls:
     """Alma SRU urls."""
 
-    def __init__(self, config: AlmaSRUConfig):
-        """Constructor for Alma SRU urls."""
+    def __init__(self, config: AlmaSRUConfig) -> None:
+        """Create object AlmaSRUUrls."""
         self.config = config
+        self.search_key = config.search_key
         self.search_value = ""
 
     @property
     def base_url(self) -> str:
         """Base url."""
         return f"https://{self.config.domain}/view/sru/{self.config.institution_code}"
 
     @property
     def query(self) -> str:
         """Query."""
-        return f"query=alma.{self.config.search_key}={self.search_value}"
+        return f"query=alma.{self.search_key}={self.search_value}"
 
     @property
     def parameters(self) -> str:
         """Parameters."""
         return f"version=1.2&operation=searchRetrieve&{self.query}"
 
-    def url(self, search_value: str) -> str:
+    def url(self, search_value: str, search_key: str = None) -> str:
         """Alma sru url to retrieve record by search value."""
         self.search_value = search_value
+        if search_key:
+            self.search_key = search_key
         return f"{self.base_url}?{self.parameters}"
 
 
 class AlmaSRU(AlmaAPIBase):
     """Alma SRU Service class."""
 
-    def __init__(self):
-        """Constructor alma sru service."""
+    def __init__(self) -> None:
+        """Create object AlmaSRU."""
         namespaces = {
             "srw": "http://www.loc.gov/zing/srw/",
             "slim": "http://www.loc.gov/MARC21/slim",
         }
         super().__init__(".//srw:recordData/slim:record", namespaces)
 
 
 class AlmaSRUService:
     """AlmaSRUService."""
 
-    def __init__(self, config: AlmaSRUConfig, urls: AlmaSRUUrls, service: AlmaSRU):
-        """Constructor for AlmaService."""
+    def __init__(
+        self,
+        config: AlmaSRUConfig,
+        urls: AlmaSRUUrls,
+        service: AlmaSRU,
+    ) -> None:
+        """Create object AlmaSRUService."""
         self.config = config
         self.urls = urls
         self.service = service
 
     @classmethod
-    def build(
+    def build(  # noqa: ANN206
         cls,
         search_key: str,
         domain: str,
         institution_code: str,
         config: AlmaSRUConfig = None,
         urls: AlmaSRUUrls = None,
         service: AlmaSRU = None,
@@ -77,11 +85,11 @@
         config = (
             config if config else AlmaSRUConfig(search_key, domain, institution_code)
         )
         urls = urls if urls else AlmaSRUUrls(config)
         service = service if service else AlmaSRU()
         return cls(config, urls, service)
 
-    def get_record(self, ac_number: str) -> list[Element]:
+    def get_record(self, ac_number: str, search_key: str = None) -> list[Element]:
         """Get the record."""
-        url = self.urls.url(ac_number)
+        url = self.urls.url(ac_number, search_key)
         return self.service.get(url)
```

### Comparing `invenio-alma-0.7.6/invenio_alma/tasks.py` & `invenio-alma-0.8.0/invenio_alma/tasks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,70 +1,78 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021-2022 Graz University of Technology.
+# Copyright (C) 2021-2023 Graz University of Technology.
 #
 # invenio-alma is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Celery Tasks for invenio-alma."""
 
 from celery import shared_task
 from flask import current_app
 from flask_mail import Message
 
 from .api import create_alma_record, update_repository_record
 from .utils import apply_aggregators, preliminaries
 
 
-def config_variables():
-    """Configuration variables."""
+def config_variables() -> tuple:
+    """Config variables."""
     user_email = current_app.config["ALMA_USER_EMAIL"]
     sender = current_app.config["ALMA_ERROR_MAIL_SENDER"]
     recipients = ",".join(current_app.config["ALMA_ERROR_MAIL_RECIPIENTS"])
 
     return user_email, sender, recipients
 
 
 @shared_task(ignore_result=True)
-def create_alma_records():
+def create_alma_records() -> None:
     """Create records within alma from repository records."""
     user_email, sender, recipients = config_variables()
     aggregators = current_app.config["ALMA_ALMA_RECORDS_CREATE_AGGREGATORS"]
 
     marc_ids = apply_aggregators(aggregators)
     records_service, alma_service, identity = preliminaries(user_email, use_rest=True)
 
     for marc_id, cms_id in marc_ids:
         try:
             create_alma_record(records_service, alma_service, identity, marc_id, cms_id)
-        except Exception as error:
+        except Exception as error:  # noqa: BLE001
             msg = Message(
                 "ERROR: creating record in alma.",
                 sender=sender,
                 recipients=recipients,
                 body=f"e: {error}, marc_id: {marc_id}",
             )
             current_app.extensions["mail"].send(msg)
 
 
 @shared_task(ignore_result=True)
-def update_repository_records():
+def update_repository_records() -> None:
     """Update records within the repository from alma records."""
     user_email, sender, recipients = config_variables()
     aggregators = current_app.config["ALMA_REPOSITORY_RECORDS_UPDATE_AGGREGATORS"]
+    update_func = current_app.config["ALMA_REPOSITORY_RECORDS_UPDATE_FUNC"]
 
     records = apply_aggregators(aggregators)
     records_service, alma_service, identity = preliminaries(user_email, use_sru=True)
 
     for marc_id, alma_id in records:
         try:
-            update_repository_record(
-                records_service, alma_service, marc_id, identity, alma_id
-            )
-        except Exception as error:
+            if update_func:
+                update_func(records_service, alma_service, marc_id, alma_id, identity)
+            else:
+                update_repository_record(
+                    records_service,
+                    alma_service,
+                    marc_id,
+                    identity,
+                    alma_id,
+                )
+        except Exception as error:  # noqa: BLE001
             msg = Message(
                 "ERROR: updating records within the repository.",
                 sender=sender,
                 recipients=recipients,
                 body=f"e: {error}, marc21_id: {marc_id}, alma_id: {alma_id}",
             )
             current_app.extensions["mail"].send(msg)
```

### Comparing `invenio-alma-0.7.6/invenio_alma/utils.py` & `invenio-alma-0.8.0/invenio_alma/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,58 +3,69 @@
 # Copyright (C) 2021-2022 Graz University of Technology.
 #
 # invenio-alma is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Utils."""
 
+from __future__ import annotations
+
 import functools
-from typing import Callable
+import typing as t
 
 from flask import current_app
 from invenio_config_tugraz import get_identity_from_user_by_email
 from invenio_records_marc21 import current_records_marc21
 
 from .proxies import current_alma
 from .services.errors import AlmaAPIError
 from .services.sru import AlmaSRUService
 
+if t.TYPE_CHECKING:
+    from collections.abc import Callable
+
 
-def is_duplicate_in_alma(cms_id: str):
+def is_duplicate_in_alma(cms_id: str) -> None:
     """Check if there is already a record in alma."""
     search_key = "local_field_995"
     domain = current_app.config["ALMA_SRU_DOMAIN"]
     institution_code = current_app.config["ALMA_SRU_INSTITUTION_CODE"]
     sru_service = AlmaSRUService.build(search_key, domain, institution_code)
 
     try:
         record = sru_service.get_record(cms_id)
         return len(record) > 0
     except AlmaAPIError:
         return False
 
 
-def preliminaries(user_email: str, *, use_rest=False, use_sru=False):
+def preliminaries(
+    user_email: str,
+    *,
+    use_rest: bool = False,
+    use_sru: bool = False,
+) -> tuple:
     """Preliminaries to interact with the repository."""
     records_service = current_records_marc21.records_service
     if use_rest:
         alma_service = current_alma.alma_rest_service
     elif use_sru:
         search_key = "local_field_995"
         domain = current_app.config["ALMA_SRU_DOMAIN"]
         institution_code = current_app.config["ALMA_SRU_INSTITUTION_CODE"]
         alma_service = AlmaSRUService(search_key, domain, institution_code)
     else:
-        raise RuntimeError("choose between using rest or sru.")
+        msg = "choose between using rest or sru."
+        raise RuntimeError(msg)
 
     identity = get_identity_from_user_by_email(email=user_email)
 
     return records_service, alma_service, identity
 
 
 def apply_aggregators(aggregators: list[Callable[[], list]]) -> list:
     """Apply aggregators."""
 
-    def func(accumulator, aggregator):
+    def func(accumulator: list, aggregator: Callable) -> list:
         return accumulator + aggregator()
 
     return functools.reduce(func, aggregators, [])
```

### Comparing `invenio-alma-0.7.6/invenio_alma.egg-info/PKG-INFO` & `invenio-alma-0.8.0/invenio_alma.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-alma
-Version: 0.7.6
+Version: 0.8.0
 Summary: "Provides API for Alma."
 Home-page: https://github.com/tu-graz-library/invenio-alma
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,23 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.0 (release 2023-04-29)
+
+- ext: add existence check before resource creation
+- global: use ruff instead of pylint
+- global: add services to export
+- tasks: add option to use update func
+- sru: add search_key on the search
+
+
 Version v0.7.6 (release 2023-04-26)
 
 - fix: remove variable check
 
 
 Version v0.7.5 (release 2023-04-26)
```

### Comparing `invenio-alma-0.7.6/invenio_alma.egg-info/SOURCES.txt` & `invenio-alma-0.8.0/invenio_alma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.7.6/run-tests.sh` & `invenio-alma-0.8.0/run-tests.sh`

 * *Files 24% similar despite different names*

```diff
@@ -12,10 +12,12 @@
 
 # Quit on errors
 set -o errexit
 
 # Quit on unbound symbols
 set -o nounset
 
-python -m check_manifest --ignore ".*-requirements.txt"
+ruff .
+
+python -m check_manifest
 python -m sphinx.cmd.build -qnNW docs docs/_build/html
 python -m pytest -s
```

### Comparing `invenio-alma-0.7.6/setup.cfg` & `invenio-alma-0.8.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -24,24 +24,19 @@
 	click-option-group>=0.5.3
 	invenio-records-marc21>=0.4.0
 	invenio-config-tugraz>=0.10.0
 	requests>=2.0.0
 
 [options.extras_require]
 tests = 
-	wheel
 	invenio-cache>=1.1.0
 	invenio-search[opensearch2]>=2.1.0
 	pytest-invenio>=1.4.3
-	pytest-flake8>=1.0.0
-	pytest-black>=0.3.0,<0.3.10
-	pytest-isort>=3.0.0
-	pytest-pylint>=0.18.0
-	pytest-bandit>=0.6.1
-	pytest-pydocstyle>=2.2.0
+	pytest-black>=0.3.0
+	ruff>=0.0.263
 	Sphinx>=4.2.0
 
 [options.entry_points]
 flask.commands = 
 	alma = invenio_alma.cli:alma
 console_scripts = 
 	alma = invenio_alma.cli:alma
@@ -61,35 +56,20 @@
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
 
 [bdist_wheel]
 universal = 1
 
-[pydocstyle]
-add_ignore = D401
-
-[pycodestyle]
-exclude = docs/conf.py
-ignore = E203,E501
-
-[flake8]
-max-line-length = 88
-extend-ignore = E203
-select = C,E,F,W,B,B950
-ignore = E501, W503
-
-[pylint.messages_control]
-disable = consider-using-with, fixme, too-many-arguments, attribute-defined-outside-init, no-name-in-module, too-many-function-args, broad-except
-
-[tool:isort]
-profile = black
+[check-manifest]
+ignore = 
+	*-requirements.txt
 
 [tool:pytest]
-addopts = --isort --pylint --bandit --pydocstyle --black --doctest-glob="*.rst" --doctest-modules --cov=invenio_alma --cov-report=term-missing
+addopts = --black --doctest-glob="*.rst" --doctest-modules --cov=invenio_alma --cov-report=term-missing
 testpaths = tests invenio_alma
 live_server_scope = module
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `invenio-alma-0.7.6/tests/conftest.py` & `invenio-alma-0.8.0/tests/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,26 +6,32 @@
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Pytest configuration.
 
 See https://pytest-invenio.readthedocs.io/ for documentation on which test
 fixtures are available.
 """
+from __future__ import annotations
+
+import typing as t
 
 import pytest
 from flask import Flask
 
 from invenio_alma import InvenioAlma
 
+if t.TYPE_CHECKING:
+    from collections.abs import Callable
+
 
 @pytest.fixture(scope="module")
-def create_app(instance_path):
+def create_app(instance_path: str) -> Callable:
     """Application factory fixture."""
 
-    def factory(**config):
+    def factory(**config: dict) -> InvenioAlma:
         app = Flask("testapp", instance_path=instance_path)
         app.config.update(**config)
         app.config["ALMA_API_KEY"] = "test-token"
         app.config["ALMA_API_HOST"] = "test-host"
         InvenioAlma(app)
         return app
```

### Comparing `invenio-alma-0.7.6/tests/test_invenio_alma.py` & `invenio-alma-0.8.0/tests/test_invenio_alma.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 """Module tests."""
 
 from flask import Flask
 
 from invenio_alma import InvenioAlma, __version__
 
 
-def test_version():
+def test_version() -> None:
     """Test version import."""
     assert __version__
 
 
-def test_init():
+def test_init() -> None:
     """Test extension initialization."""
     app = Flask("testapp")
     app.config["ALMA_API_KEY"] = "test-token"
     app.config["ALMA_API_HOST"] = "test-host"
 
     ext = InvenioAlma(app)
     assert "invenio-alma" in app.extensions
```

### Comparing `invenio-alma-0.7.6/tests/test_invenio_alma_service.py` & `invenio-alma-0.8.0/tests/test_invenio_alma_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,33 +7,31 @@
 
 """Test Alma Services."""
 
 from invenio_alma.services.rest import AlmaRESTConfig, AlmaRESTUrls
 from invenio_alma.services.sru import AlmaSRUConfig, AlmaSRUUrls
 
 
-def test_alma_rest_urls():
+def test_alma_rest_urls() -> None:
     """Test rest urls."""
-
     mms_id = "12345-12345"
     api_key = "api_key"
     api_host = "api_host"
     config = AlmaRESTConfig(api_key, api_host)
     urls = AlmaRESTUrls(config)
 
     expected = f"https://{api_host}/almaws/v1/bibs?mms_id={mms_id}&apikey={api_key}"
     assert urls.url_get(mms_id) == expected
 
     expected = f"https://{api_host}/almaws/v1/bibs/{mms_id}?apikey={api_key}"
     assert urls.url_put(mms_id) == expected
 
 
-def test_alma_sru_urls():
+def test_alma_sru_urls() -> None:
     """Test sru urls."""
-
     search_key = ""
     domain = ""
     institution_code = ""
     search_value = ""
     config = AlmaSRUConfig(search_key, domain, institution_code)
     urls = AlmaSRUUrls(config)
```


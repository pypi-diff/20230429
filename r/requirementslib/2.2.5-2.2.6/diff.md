# Comparing `tmp/requirementslib-2.2.5.tar.gz` & `tmp/requirementslib-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requirementslib-2.2.5.tar", last modified: Wed Apr 19 10:36:01 2023, max compression
+gzip compressed data, was "requirementslib-2.2.6.tar", last modified: Sat Apr 29 03:39:29 2023, max compression
```

## Comparing `requirementslib-2.2.5.tar` & `requirementslib-2.2.6.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.765479 requirementslib-2.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35440 2023-04-19 10:35:19.000000 requirementslib-2.2.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-19 10:35:19.000000 requirementslib-2.2.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-19 10:35:19.000000 requirementslib-2.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-19 10:35:19.000000 requirementslib-2.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-04-19 10:36:01.765479 requirementslib-2.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-19 10:35:19.000000 requirementslib-2.2.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.761479 requirementslib-2.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.environment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.cache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.lockfile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.markers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.pipfile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.project.rst
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.resolvers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.setup_info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.models.vcs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-19 10:35:19.000000 requirementslib-2.2.5/docs/requirementslib.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-19 10:35:19.000000 requirementslib-2.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-19 10:36:01.765479 requirementslib-2.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-19 10:35:19.000000 requirementslib-2.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.753478 requirementslib-2.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.761479 requirementslib-2.2.5/src/requirementslib/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/funktools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.765479 requirementslib-2.2.5/src/requirementslib/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    26629 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/lockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    26367 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)    44137 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/old_pip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/pipfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)   119687 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    55679 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/setup_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    34664 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/models/vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25755 2023-04-19 10:35:19.000000 requirementslib-2.2.5/src/requirementslib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.761479 requirementslib-2.2.5/src/requirementslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-04-19 10:36:01.000000 requirementslib-2.2.5/src/requirementslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-19 10:36:01.000000 requirementslib-2.2.5/src/requirementslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:36:01.000000 requirementslib-2.2.5/src/requirementslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-19 10:36:01.000000 requirementslib-2.2.5/src/requirementslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 10:36:01.000000 requirementslib-2.2.5/src/requirementslib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:35:24.000000 requirementslib-2.2.5/src/requirementslib.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:39:29.505782 requirementslib-2.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35667 2023-04-29 03:38:55.000000 requirementslib-2.2.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-29 03:38:55.000000 requirementslib-2.2.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-29 03:38:55.000000 requirementslib-2.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-29 03:38:55.000000 requirementslib-2.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-04-29 03:39:29.505782 requirementslib-2.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-29 03:38:55.000000 requirementslib-2.2.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:39:29.501783 requirementslib-2.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.environment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.models.cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.models.dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.models.lockfile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.models.markers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.models.metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.models.pipfile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.models.project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.models.requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.models.resolvers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.models.setup_info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.models.url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.models.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.models.vcs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-29 03:38:55.000000 requirementslib-2.2.6/docs/requirementslib.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-29 03:38:55.000000 requirementslib-2.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-29 03:39:29.509783 requirementslib-2.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-29 03:38:55.000000 requirementslib-2.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:39:29.497782 requirementslib-2.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:39:29.501783 requirementslib-2.2.6/src/requirementslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/funktools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:39:29.505782 requirementslib-2.2.6/src/requirementslib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26616 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26367 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44134 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/old_pip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/pipfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119684 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66148 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/setup_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34664 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/models/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27937 2023-04-29 03:38:55.000000 requirementslib-2.2.6/src/requirementslib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:39:29.505782 requirementslib-2.2.6/src/requirementslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-04-29 03:39:29.000000 requirementslib-2.2.6/src/requirementslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-29 03:39:29.000000 requirementslib-2.2.6/src/requirementslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 03:39:29.000000 requirementslib-2.2.6/src/requirementslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-29 03:39:29.000000 requirementslib-2.2.6/src/requirementslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 03:39:29.000000 requirementslib-2.2.6/src/requirementslib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 03:38:59.000000 requirementslib-2.2.6/src/requirementslib.egg-info/zip-safe
```

### Comparing `requirementslib-2.2.5/CHANGELOG.rst` & `requirementslib-2.2.6/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Requirementslib 2.2.6 (2023-04-28)
+==================================
+
+
+Bug Fixes
+---------
+
+- Fix an error when parsing a setup.py file that has a UTF-8 BOM.  `#364 <https://github.com/sarugaku/requirementslib/issues/364>`_
+
+
 Requirementslib 2.2.5 (2023-04-19)
 ==================================
 
 
 Vendored Libraries
 ------------------
```

### Comparing `requirementslib-2.2.5/CONTRIBUTING.rst` & `requirementslib-2.2.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/LICENSE` & `requirementslib-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/MANIFEST.in` & `requirementslib-2.2.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/PKG-INFO` & `requirementslib-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirementslib
-Version: 2.2.5
+Version: 2.2.6
 Summary: A tool for converting between pip-style and pipfile requirements.
 Home-page: https://github.com/sarugaku/requirementslib
 Author: Dan Ryan
 Author-email: dan@danryan.co
 Maintainer: Frost Ming
 Maintainer-email: mianghong@gmail.com
 License: MIT
```

### Comparing `requirementslib-2.2.5/README.rst` & `requirementslib-2.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/docs/Makefile` & `requirementslib-2.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/docs/conf.py` & `requirementslib-2.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/docs/make.bat` & `requirementslib-2.2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/docs/requirementslib.models.rst` & `requirementslib-2.2.6/docs/requirementslib.models.rst`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/pyproject.toml` & `requirementslib-2.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 skip_glob = ["tests/artifacts/*", "tests/fixtures/*"]
 profile = "black"
 atomic = true
 line_length = 90
 filter_files = true
 known_third_party = [
   "attr",
-  "cached_property",
   "chardet",
   "distlib",
   "environ",
   "hypothesis",
   "invoke",
   "packaging",
   "parver",
@@ -83,13 +82,12 @@
   "pytest",
   "requests",
   "setuptools",
   "six",
   "tomlkit",
   "towncrier",
   "urllib3",
-  "vistir"
 ]
 known_first_party = [
   "requirementslib",
   "tests"
 ]
```

### Comparing `requirementslib-2.2.5/setup.cfg` & `requirementslib-2.2.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -38,24 +38,22 @@
 	Topic :: Utilities
 
 [options]
 zip_safe = true
 python_requires = >=3.7
 install_requires = 
 	attrs>=19.2
-	cached_property
 	distlib>=0.2.8
 	pep517>=0.5.0
 	pip>=23.1
 	platformdirs
 	plette[validation]
 	requests
 	setuptools>=40.8
 	tomlkit>=0.5.3
-	vistir==0.8.0
 
 [options.extras_require]
 tests = 
 	pytest
 	readme-renderer[md]
 	pytest-xdist
 	pytest-cov
```

### Comparing `requirementslib-2.2.5/setup.py` & `requirementslib-2.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/src/requirementslib/exceptions.py` & `requirementslib-2.2.6/src/requirementslib/exceptions.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/src/requirementslib/funktools.py` & `requirementslib-2.2.6/src/requirementslib/funktools.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/src/requirementslib/models/cache.py` & `requirementslib-2.2.6/src/requirementslib/models/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import atexit
 import copy
 import hashlib
 import json
 import os
 
-import vistir
 from pip._internal.utils.hashes import FAVORITE_HASH
 from pip._internal.vcs.versioncontrol import VcsSupport
 from pip._vendor.cachecontrol.cache import DictCache
 from pip._vendor.packaging.requirements import Requirement
 from platformdirs import user_cache_dir
 
+from ..fileutils import open_file
 from .utils import as_tuple, get_pinned_version, key_from_req, lookup_table
 
 CACHE_DIR = os.environ.get("PIPENV_CACHE_DIR", user_cache_dir("pipenv"))
 
 
 class DependencyCache(object):
     """Creates a new in memory dependency cache for the current Python
@@ -26,15 +26,16 @@
     def as_cache_key(self, ireq):
         """Given a requirement, return its cache key. This behavior is a little
         weird in order to allow backwards compatibility with cache files. For a
         requirement without extras, this will return, for example:
 
         ("ipython", "2.1.0")
 
-        For a requirement with extras, the extras will be comma-separated and appended to the version, inside brackets,
+        For a requirement with extras, the extras will be comma-separated and appended to the
+        version, inside brackets,
         like so:
 
         ("ipython", "2.1.0[nbconvert,notebook]")
         """
         name, version, extras = as_tuple(ireq)
         if not extras:
             extras_string = ""
@@ -156,11 +157,11 @@
             hash_value = hash_value.encode("utf8")
         if can_hash:
             self.set(new_location.url, hash_value)
         return hash_value.decode("utf8")
 
     def _get_file_hash(self, location):
         h = hashlib.new(FAVORITE_HASH)
-        with vistir.contextmanagers.open_file(location, self.session) as fp:
+        with open_file(location, self.session) as fp:
             for chunk in iter(lambda: fp.read(8096), b""):
                 h.update(chunk)
         return ":".join([FAVORITE_HASH, h.hexdigest()])
```

### Comparing `requirementslib-2.2.5/src/requirementslib/models/dependencies.py` & `requirementslib-2.2.6/src/requirementslib/models/dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,23 @@
 from pip._internal.req.constructors import install_req_from_line
 from pip._internal.req.req_install import InstallRequirement
 from pip._internal.req.req_set import RequirementSet
 from pip._internal.utils.temp_dir import TempDirectory, global_tempdir_manager
 from pip._vendor.packaging.markers import Marker
 from pip._vendor.packaging.utils import canonicalize_name
 from pip._vendor.packaging.version import parse
-from vistir.contextmanagers import temp_environ
-from vistir.path import create_tracked_tempdir
 
 from ..environment import MYPY_RUNNING
-from ..utils import get_package_finder, get_pip_command, prepare_pip_source_args
+from ..fileutils import create_tracked_tempdir
+from ..utils import (
+    get_package_finder,
+    get_pip_command,
+    prepare_pip_source_args,
+    temp_environ,
+)
 from .cache import CACHE_DIR, DependencyCache
 from .setup_info import SetupInfo
 from .utils import (
     clean_requires_python,
     format_requirement,
     full_groupby,
     is_pinned_requirement,
```

### Comparing `requirementslib-2.2.5/src/requirementslib/models/lockfile.py` & `requirementslib-2.2.6/src/requirementslib/models/lockfile.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/src/requirementslib/models/markers.py` & `requirementslib-2.2.6/src/requirementslib/models/markers.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/src/requirementslib/models/metadata.py` & `requirementslib-2.2.6/src/requirementslib/models/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 import zipfile
 from collections import defaultdict
 from functools import reduce
 from typing import Sequence
 
 import attr
 import requests
-import vistir
 from distlib import wheel
 from distlib.metadata import Metadata
 from pip._vendor.packaging.markers import Marker
 from pip._vendor.packaging.requirements import Requirement as PackagingRequirement
 from pip._vendor.packaging.specifiers import Specifier, SpecifierSet
 from pip._vendor.packaging.tags import Tag
 from pip._vendor.packaging.version import _BaseVersion, parse
 
 from ..environment import MYPY_RUNNING
+from ..fileutils import open_file
 from .markers import (
     get_contained_extras,
     get_contained_pyversions,
     get_without_extra,
     get_without_pyversion,
     marker_from_specifier,
     merge_markers,
@@ -162,15 +162,15 @@
         return req.line_instance.setup_info
 
 
 def get_remote_wheel_metadata(whl_file):
     # type: (str) -> Optional[Metadata]
     parsed_metadata = None
     data = io.BytesIO()
-    with vistir.contextmanagers.open_file(whl_file) as fp:
+    with open_file(whl_file) as fp:
         for chunk in iter(lambda: fp.read(8096), b""):
             data.write(chunk)
     with zipfile.ZipFile(data, mode="r", compression=zipfile.ZIP_DEFLATED) as zf:
         metadata = None
         for fn in zf.namelist():
             if os.path.basename(fn) == "METADATA":
                 metadata = fn
```

### Comparing `requirementslib-2.2.5/src/requirementslib/models/old_pip_utils.py` & `requirementslib-2.2.6/src/requirementslib/models/old_pip_utils.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/src/requirementslib/models/pipfile.py` & `requirementslib-2.2.6/src/requirementslib/models/pipfile.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/src/requirementslib/models/project.py` & `requirementslib-2.2.6/src/requirementslib/models/project.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/src/requirementslib/models/requirements.py` & `requirementslib-2.2.6/src/requirementslib/models/requirements.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,46 +6,46 @@
 from functools import lru_cache
 from pathlib import Path
 from sysconfig import get_path
 from urllib import parse as urllib_parse
 from urllib.parse import unquote
 
 import attr
-from cached_property import cached_property
 from pip._internal.models.link import Link
 from pip._internal.models.wheel import Wheel
 from pip._internal.req.constructors import (
     _strip_extras,
     install_req_from_editable,
     install_req_from_line,
 )
 from pip._internal.req.req_install import InstallRequirement
 from pip._internal.utils.temp_dir import global_tempdir_manager
 from pip._internal.utils.urls import path_to_url, url_to_path
+from pip._vendor.distlib.util import cached_property
 from pip._vendor.packaging.markers import Marker
 from pip._vendor.packaging.requirements import Requirement as PackagingRequirement
 from pip._vendor.packaging.specifiers import (
     InvalidSpecifier,
     LegacySpecifier,
     Specifier,
     SpecifierSet,
 )
 from pip._vendor.packaging.utils import canonicalize_name
 from pip._vendor.packaging.version import parse
-from vistir.contextmanagers import temp_path
-from vistir.path import (
+
+from ..environment import MYPY_RUNNING
+from ..exceptions import RequirementError
+from ..fileutils import (
     create_tracked_tempdir,
     get_converted_relative_path,
     is_file_url,
     is_valid_url,
     normalize_path,
+    temp_path,
 )
-
-from ..environment import MYPY_RUNNING
-from ..exceptions import RequirementError
 from ..funktools import dedup
 from ..utils import (
     VCS_LIST,
     add_ssh_scheme_to_git_uri,
     get_setup_paths,
     is_installable_dir,
     is_installable_file,
@@ -91,14 +91,15 @@
 if MYPY_RUNNING:
     from typing import (
         Any,
         AnyStr,
         Dict,
         FrozenSet,
         Generator,
+        Iterator,
         List,
         Optional,
         Sequence,
         Set,
         Text,
         Tuple,
         TypeVar,
```

### Comparing `requirementslib-2.2.5/src/requirementslib/models/resolvers.py` & `requirementslib-2.2.6/src/requirementslib/models/resolvers.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/src/requirementslib/models/setup_info.py` & `requirementslib-2.2.6/src/requirementslib/models/setup_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import ast
 import atexit
 import configparser
 import contextlib
+import errno
+import locale
 import os
 import shutil
+import stat
 import subprocess as sp
 import sys
+import time
+import warnings
 from collections.abc import Iterable, Mapping
 from contextlib import ExitStack
 from functools import lru_cache
+from itertools import count
 from os import scandir
 from pathlib import Path
+from typing import Callable, Optional
 from urllib.parse import parse_qs, urlparse, urlunparse
 from weakref import finalize
 
 import attr
 from distlib.wheel import Wheel
 from pep517 import envbuild, wrappers
 from pip._internal.network.download import Downloader
@@ -27,19 +34,18 @@
 from pip._vendor.pkg_resources import (
     PathMetadata,
     Requirement,
     distributions_from_metadata,
     find_distributions,
 )
 from platformdirs import user_cache_dir
-from vistir.contextmanagers import cd, temp_path
-from vistir.path import create_tracked_tempdir, rmtree
 
 from ..environment import MYPY_RUNNING
 from ..exceptions import RequirementError
+from ..fileutils import cd, create_tracked_tempdir, temp_path
 from ..utils import get_pip_command
 from .old_pip_utils import _copy_source_tree
 from .utils import (
     get_default_pyproject_backend,
     get_name_variants,
     get_pyproject,
     init_requirement,
@@ -50,15 +56,14 @@
 if MYPY_RUNNING:
     from typing import (
         Any,
         AnyStr,
         Dict,
         Generator,
         List,
-        Optional,
         Sequence,
         Set,
         Text,
         Tuple,
         TypeVar,
         Union,
     )
@@ -122,14 +127,237 @@
         if backend_path:
             backend_path = [
                 wrappers.norm_and_check(self.source_dir, p) for p in backend_path
             ]
         self.backend_path = backend_path
 
 
+def get_value_from_tuple(value, value_type):
+    try:
+        import winreg
+    except ImportError:
+        import _winreg as winreg
+    if value_type in (winreg.REG_SZ, winreg.REG_EXPAND_SZ):
+        if "\0" in value:
+            return value[: value.index("\0")]
+        return value
+    return None
+
+
+def is_readonly_path(fn: os.PathLike) -> bool:
+    """check if a provided path exists and is readonly.
+
+    permissions check is `bool(path.stat & stat.s_iread)` or `not
+    os.access(path, os.w_ok)`
+    """
+    if os.path.exists(fn):
+        file_stat = os.stat(fn).st_mode
+        return not bool(file_stat & stat.s_iwrite) or not os.access(fn, os.w_ok)
+    return False
+
+
+def query_registry_value(root, key_name, value):
+    try:
+        import winreg
+    except ImportError:
+        import _winreg as winreg
+    try:
+        with winreg.OpenKeyEx(root, key_name, 0, winreg.KEY_READ) as key:
+            return get_value_from_tuple(*winreg.QueryValueEx(key, value))
+    except OSError:
+        return None
+
+
+def _find_icacls_exe():
+    if os.name == "nt":
+        paths = [
+            os.path.expandvars(r"%windir%\{0}").format(subdir)
+            for subdir in ("system32", "SysWOW64")
+        ]
+        for path in paths:
+            icacls_path = next(
+                iter(fn for fn in os.listdir(path) if fn.lower() == "icacls.exe"), None
+            )
+            if icacls_path is not None:
+                icacls_path = os.path.join(path, icacls_path)
+                return icacls_path
+    return None
+
+
+def _walk_for_powershell(directory):
+    for _, dirs, files in os.walk(directory):
+        powershell = next(
+            iter(fn for fn in files if fn.lower() == "powershell.exe"), None
+        )
+        if powershell is not None:
+            return os.path.join(directory, powershell)
+        for subdir in dirs:
+            powershell = _walk_for_powershell(os.path.join(directory, subdir))
+            if powershell:
+                return powershell
+    return None
+
+
+def _get_powershell_path():
+    paths = [
+        os.path.expandvars(r"%windir%\{0}\WindowsPowerShell").format(subdir)
+        for subdir in ("SysWOW64", "system32")
+    ]
+    powershell_path = next(iter(_walk_for_powershell(pth) for pth in paths), None)
+    if not powershell_path:
+        powershell_path = sp.run(["where", "powershell"])
+    if powershell_path.stdout:
+        return powershell_path.stdout.strip()
+
+
+def _get_sid_with_powershell():
+    powershell_path = _get_powershell_path()
+    if not powershell_path:
+        return None
+    args = [
+        powershell_path,
+        "-ExecutionPolicy",
+        "Bypass",
+        "-Command",
+        "Invoke-Expression '[System.Security.Principal.WindowsIdentity]::GetCurrent().user | Write-Host'",
+    ]
+    sid = sp.run(args, capture_output=True)
+    return sid.stdout.strip()
+
+
+def _get_sid_from_registry():
+    try:
+        import winreg
+    except ImportError:
+        import _winreg as winreg
+    var_names = ("%USERPROFILE%", "%HOME%")
+    current_user_home = next(iter(os.path.expandvars(v) for v in var_names if v), None)
+    root, subkey = (
+        winreg.HKEY_LOCAL_MACHINE,
+        r"Software\Microsoft\Windows NT\CurrentVersion\ProfileList",
+    )
+    subkey_names = []
+    value = None
+    matching_key = None
+    try:
+        with winreg.OpenKeyEx(root, subkey, 0, winreg.KEY_READ) as key:
+            for i in count():
+                key_name = winreg.EnumKey(key, i)
+                subkey_names.append(key_name)
+                value = query_registry_value(
+                    root, r"{0}\{1}".format(subkey, key_name), "ProfileImagePath"
+                )
+                if value and value.lower() == current_user_home.lower():
+                    matching_key = key_name
+                    break
+    except OSError:
+        pass
+    if matching_key is not None:
+        return matching_key
+
+
+def _get_current_user():
+    fns = (_get_sid_from_registry, _get_sid_with_powershell)
+    for fn in fns:
+        result = fn()
+        if result:
+            return result
+    return None
+
+
+def _wait_for_files(path):  # pragma: no cover
+    """Retry with backoff up to 1 second to delete files from a directory.
+
+    :param str path: The path to crawl to delete files from
+    :return: A list of remaining paths or None
+    :rtype: Optional[List[str]]
+    """
+    timeout = 0.001
+    remaining = []
+    while timeout < 1.0:
+        remaining = []
+        if os.path.isdir(path):
+            L = os.listdir(path)
+            for target in L:
+                _remaining = _wait_for_files(target)
+                if _remaining:
+                    remaining.extend(_remaining)
+            continue
+        try:
+            os.unlink(path)
+        except FileNotFoundError as e:
+            if e.errno == errno.ENOENT:
+                return
+        except (OSError, IOError, PermissionError):  # noqa:B014
+            time.sleep(timeout)
+            timeout *= 2
+            remaining.append(path)
+        else:
+            return
+    return remaining
+
+
+def set_write_bit(fn: str) -> None:
+    """Set read-write permissions for the current user on the target path. Fail
+    silently if the path doesn't exist.
+
+    :param str fn: The target filename or path
+    :return: None
+    """
+    if not os.path.exists(fn):
+        return
+    file_stat = os.stat(fn).st_mode
+    os.chmod(fn, file_stat | stat.S_IRWXU | stat.S_IRWXG | stat.S_IRWXO)
+    if os.name == "nt":
+        user_sid = _get_current_user()
+        icacls_exe = _find_icacls_exe() or "icacls"
+
+        if user_sid:
+            c = sp.run(
+                [
+                    icacls_exe,
+                    "''{}''".format(fn),
+                    "/grant",
+                    "{}:WD".format(user_sid),
+                    "/T",
+                    "/C",
+                    "/Q",
+                ],
+                capture_output=True,
+                # 2020-06-12 Yukihiko Shinoda
+                # There are 3 way to get system default encoding in Stack Overflow.
+                # see: https://stackoverflow.com/questions/37506535/how-to-get-the-system-default-encoding-in-python-2-x
+                # I investigated these way by using Shift-JIS Windows.
+                # >>> import locale
+                # >>> locale.getpreferredencoding()
+                # "cp932" (Shift-JIS)
+                # >>> import sys
+                # >>> sys.getdefaultencoding()
+                # "utf-8"
+                # >>> sys.stdout.encoding
+                # "UTF8"
+                encoding=locale.getpreferredencoding(),
+            )
+            if not c.err and c.returncode == 0:
+                return
+
+    if not os.path.isdir(fn):
+        for path in [fn, os.path.dirname(fn)]:
+            try:
+                os.chflags(path, 0)
+            except AttributeError:
+                pass
+        return None
+    for root, dirs, files in os.walk(fn, topdown=False):
+        for dir_ in [os.path.join(root, d) for d in dirs]:
+            set_write_bit(dir_)
+        for file_ in [os.path.join(root, f) for f in files]:
+            set_write_bit(file_)
+
+
 def make_base_requirements(reqs):
     # type: (Sequence[STRING_TYPE]) -> Set[BaseRequirement]
     requirements = set()
     if not isinstance(reqs, (list, tuple, set)):
         reqs = [reqs]
     for req in reqs:
         if isinstance(req, BaseRequirement):
@@ -137,14 +365,104 @@
         elif isinstance(req, Requirement):
             requirements.add(BaseRequirement.from_req(req))
         elif req and isinstance(req, str) and not req.startswith("#"):
             requirements.add(BaseRequirement.from_string(req))
     return requirements
 
 
+def handle_remove_readonly(func, path, exc):
+    """Error handler for shutil.rmtree.
+
+    Windows source repo folders are read-only by default, so this error handler
+    attempts to set them as writeable and then proceed with deletion.
+
+    :param function func: The caller function
+    :param str path: The target path for removal
+    :param Exception exc: The raised exception
+
+    This function will call check :func:`is_readonly_path` before attempting to call
+    :func:`set_write_bit` on the target path and try again.
+    """
+
+    PERM_ERRORS = (errno.EACCES, errno.EPERM, errno.ENOENT)
+    default_warning_message = "Unable to remove file due to permissions restriction: {!r}"
+    # split the initial exception out into its type, exception, and traceback
+    exc_type, exc_exception, exc_tb = exc
+    if is_readonly_path(path):
+        # Apply write permission and call original function
+        set_write_bit(path)
+        try:
+            func(path)
+        except (  # noqa:B014
+            OSError,
+            IOError,
+            FileNotFoundError,
+            PermissionError,
+        ) as e:  # pragma: no cover
+            if e.errno in PERM_ERRORS:
+                if e.errno == errno.ENOENT:
+                    return
+                remaining = None
+                if os.path.isdir(path):
+                    remaining = _wait_for_files(path)
+                if remaining:
+                    warnings.warn(
+                        default_warning_message.format(path),
+                        ResourceWarning,
+                        stacklevel=2,
+                    )
+                else:
+                    func(path, ignore_errors=True)
+                return
+
+    if exc_exception.errno in PERM_ERRORS:
+        set_write_bit(path)
+        remaining = _wait_for_files(path)
+        try:
+            func(path)
+        except (OSError, IOError, FileNotFoundError, PermissionError) as e:  # noqa:B014
+            if e.errno in PERM_ERRORS:
+                if e.errno != errno.ENOENT:  # File still exists
+                    warnings.warn(
+                        default_warning_message.format(path),
+                        ResourceWarning,
+                        stacklevel=2,
+                    )
+            return
+    else:
+        raise exc_exception
+
+
+def rmtree(
+    directory: str, ignore_errors: bool = False, onerror: Optional[Callable] = None
+) -> None:
+    """Stand-in for :func:`~shutil.rmtree` with additional error-handling.
+
+    This version of `rmtree` handles read-only paths, especially in the case of index
+    files written by certain source control systems.
+
+    :param str directory: The target directory to remove
+    :param bool ignore_errors: Whether to ignore errors, defaults to False
+    :param func onerror: An error handling function, defaults to :func:`handle_remove_readonly`
+
+    .. note::
+
+       Setting `ignore_errors=True` may cause this to silently fail to delete the path
+    """
+
+    if onerror is None:
+        onerror = handle_remove_readonly
+    try:
+        shutil.rmtree(directory, ignore_errors=ignore_errors, onerror=onerror)
+    except (IOError, OSError, FileNotFoundError, PermissionError) as exc:  # noqa:B014
+        # Ignore removal failures where the file doesn't exist
+        if exc.errno != errno.ENOENT:
+            raise
+
+
 def suppress_unparsable(func, *args, **kwargs):
     try:
         return func(*args, **kwargs)
     except Unparsable:
         return None
 
 
@@ -154,15 +472,15 @@
 
 class SetupReader:
     """Class that reads a setup.py file without executing it."""
 
     @classmethod
     def read_setup_py(cls, file: Path, raising: bool = True) -> "Dict[str, Any]":
 
-        with file.open(encoding="utf-8") as f:
+        with file.open(encoding="utf-8-sig") as f:
             content = f.read()
 
         body = ast.parse(content).body
 
         setup_call, body = cls._find_setup_call(body)
         if not setup_call:
             return {}
```

### Comparing `requirementslib-2.2.5/src/requirementslib/models/url.py` & `requirementslib-2.2.6/src/requirementslib/models/url.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/src/requirementslib/models/utils.py` & `requirementslib-2.2.6/src/requirementslib/models/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from pip._vendor.packaging.version import parse as parse_version
 from pip._vendor.pkg_resources import Requirement, get_distribution, safe_name
 from plette.models import Package, PackageCollection
 from tomlkit.container import Container
 from tomlkit.items import AoT, Array, Bool, InlineTable, Item, String, Table
 from urllib3 import util as urllib3_util
 from urllib3.util import parse_url as urllib3_parse
-from vistir.path import is_valid_url
 
 from ..environment import MYPY_RUNNING
+from ..fileutils import is_valid_url
 from ..utils import SCHEME_LIST, VCS_LIST, is_star
 
 if MYPY_RUNNING:
     from typing import Iterable  # noqa
     from typing import (
         Any,
         AnyStr,
```

### Comparing `requirementslib-2.2.5/src/requirementslib/models/vcs.py` & `requirementslib-2.2.6/src/requirementslib/models/vcs.py`

 * *Files identical despite different names*

### Comparing `requirementslib-2.2.5/src/requirementslib/utils.py` & `requirementslib-2.2.6/src/requirementslib/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,58 @@
+# This Module is taken in part from the click project and expanded
+# see https://github.com/pallets/click/blob/6cafd32/click/_winconsole.py
+# Copyright © 2014 by the Pallets team.
+
+# Some rights reserved.
+
+# Redistribution and use in source and binary forms of the software as well as
+# documentation, with or without modification, are permitted provided that the
+# following conditions are met:
+#     Redistributions of source code must retain the above copyright notice,
+#           this list of conditions and the following disclaimer.
+#     Redistributions in binary form must reproduce the above copyright notice,
+#           this list of conditions and the following disclaimer in the
+#           documentation and/or other materials provided with the distribution.
+#     Neither the name of the copyright holder nor the names of its contributors
+#           may be used to endorse or promote products derived from this
+#           software without specific prior written permission.
+
+# THIS SOFTWARE AND DOCUMENTATION IS PROVIDED BY THE COPYRIGHT HOLDERS AND
+# CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT
+# NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
+# PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
+# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
+# EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
+# PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
+# OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
+# WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
+# OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE AND
+# DOCUMENTATION, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+
 import logging
 import os
 import sys
 from collections.abc import ItemsView, Mapping, Sequence, Set
+from contextlib import contextmanager
 from pathlib import Path
 from urllib.parse import urlparse, urlsplit, urlunparse
 
 import tomlkit
-import vistir
 from pip._internal.commands.install import InstallCommand
 from pip._internal.models.target_python import TargetPython
 from pip._internal.utils.filetypes import is_archive_file
 from pip._internal.utils.misc import is_installable_dir
 from pip._vendor.packaging import specifiers
-from vistir.path import is_valid_url
 
 from .environment import MYPY_RUNNING
+from .fileutils import is_valid_url, normalize_path, url_to_path
 
 if MYPY_RUNNING:
-    from typing import Dict, List, Optional, Text, Tuple, TypeVar, Union
+    from typing import Dict, Iterator, List, Optional, Text, Tuple, TypeVar, Union
 
     STRING_TYPE = Union[bytes, str, Text]
     S = TypeVar("S", bytes, str, Text)
     PipfileEntryType = Union[STRING_TYPE, bool, Tuple[STRING_TYPE], List[STRING_TYPE]]
     PipfileType = Union[STRING_TYPE, Dict[STRING_TYPE, PipfileEntryType]]
 
 
@@ -141,15 +172,15 @@
     if not isinstance(path, Mapping):
         raise TypeError("expecting a mapping, received {0!r}".format(path))
 
     if not any(key in path for key in ["file", "path"]):
         raise ValueError("missing path-like entry in supplied mapping {0!r}".format(path))
 
     if "file" in path:
-        path = vistir.path.url_to_path(path["file"])
+        path = url_to_path(path["file"])
 
     elif "path" in path:
         path = path["path"]
     if not os.name == "nt":
         return os.fsdecode(path)
     return Path(os.fsdecode(path)).as_posix()
 
@@ -175,16 +206,16 @@
     parsed = urlparse(path)
     is_local = (
         not parsed.scheme
         or parsed.scheme == "file"
         or (len(parsed.scheme) == 1 and os.name == "nt")
     )
     if parsed.scheme and parsed.scheme == "file":
-        path = os.fsdecode(vistir.path.url_to_path(path))
-    normalized_path = vistir.path.normalize_path(path)
+        path = os.fsdecode(url_to_path(path))
+    normalized_path = normalize_path(path)
     if is_local and not os.path.exists(normalized_path):
         return False
 
     is_archive = is_archive_file(normalized_path)
     is_local_project = os.path.isdir(normalized_path) and is_installable_dir(
         normalized_path
     )
@@ -669,7 +700,21 @@
     # Use pip's parser for pip.conf management and defaults.
     # General options (find_links, index_url, extra_index_url, trusted_host,
     # and pre) are deferred to pip.
     pip_command = InstallCommand(
         name="InstallCommand", summary="requirementslib pip Install command."
     )
     return pip_command
+
+
+# Borrowed from Pew.
+# See https://github.com/berdario/pew/blob/master/pew/_utils.py#L82
+@contextmanager
+def temp_environ():
+    # type: () -> Iterator[None]
+    """Allow the ability to set os.environ temporarily."""
+    environ = dict(os.environ)
+    try:
+        yield
+    finally:
+        os.environ.clear()
+        os.environ.update(environ)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `requirementslib-2.2.5/src/requirementslib.egg-info/PKG-INFO` & `requirementslib-2.2.6/src/requirementslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirementslib
-Version: 2.2.5
+Version: 2.2.6
 Summary: A tool for converting between pip-style and pipfile requirements.
 Home-page: https://github.com/sarugaku/requirementslib
 Author: Dan Ryan
 Author-email: dan@danryan.co
 Maintainer: Frost Ming
 Maintainer-email: mianghong@gmail.com
 License: MIT
```

### Comparing `requirementslib-2.2.5/src/requirementslib.egg-info/SOURCES.txt` & `requirementslib-2.2.6/src/requirementslib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 docs/requirementslib.models.utils.rst
 docs/requirementslib.models.vcs.rst
 docs/requirementslib.rst
 docs/requirementslib.utils.rst
 src/requirementslib/__init__.py
 src/requirementslib/environment.py
 src/requirementslib/exceptions.py
+src/requirementslib/fileutils.py
 src/requirementslib/funktools.py
 src/requirementslib/utils.py
 src/requirementslib.egg-info/PKG-INFO
 src/requirementslib.egg-info/SOURCES.txt
 src/requirementslib.egg-info/dependency_links.txt
 src/requirementslib.egg-info/requires.txt
 src/requirementslib.egg-info/top_level.txt
```


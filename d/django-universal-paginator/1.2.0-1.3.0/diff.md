# Comparing `tmp/django_universal_paginator-1.2.0.tar.gz` & `tmp/django_universal_paginator-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_universal_paginator-1.2.0.tar", last modified: Sun Apr 16 06:41:13 2023, max compression
+gzip compressed data, was "django_universal_paginator-1.3.0.tar", last modified: Sat Apr 29 04:47:42 2023, max compression
```

## Comparing `django_universal_paginator-1.2.0.tar` & `django_universal_paginator-1.3.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.292059 django_universal_paginator-1.2.0/
--rw-r--r--   0 mirec     (1000) mirec     (1000)       97 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/.editorconfig
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.288059 django_universal_paginator-1.2.0/.github/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.290059 django_universal_paginator-1.2.0/.github/workflows/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1027 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/.github/workflows/python-package.yml
--rw-r--r--   0 mirec     (1000) mirec     (1000)      142 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/.gitignore
--rw-r--r--   0 mirec     (1000) mirec     (1000)      197 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 mirec     (1000) mirec     (1000)    17720 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/.pylintrc
--rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/AUTHORS
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2444 2023-04-16 06:41:05.000000 django_universal_paginator-1.2.0/CHANGELOG.md
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1073 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/LICENSE
--rw-r--r--   0 mirec     (1000) mirec     (1000)       92 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/MANIFEST.in
--rw-r--r--   0 mirec     (1000) mirec     (1000)     5196 2023-04-16 06:41:13.292059 django_universal_paginator-1.2.0/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)     4439 2022-12-26 12:18:20.000000 django_universal_paginator-1.2.0/README.rst
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.290059 django_universal_paginator-1.2.0/django_universal_paginator/
--rw-r--r--   0 mirec     (1000) mirec     (1000)       24 2022-12-18 18:48:06.000000 django_universal_paginator-1.2.0/django_universal_paginator/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)       96 2023-02-11 17:12:19.000000 django_universal_paginator-1.2.0/django_universal_paginator/constants.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      664 2023-02-11 17:23:37.000000 django_universal_paginator-1.2.0/django_universal_paginator/converter.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     4628 2023-04-16 06:40:59.000000 django_universal_paginator-1.2.0/django_universal_paginator/cursor.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      291 2022-12-18 18:48:06.000000 django_universal_paginator-1.2.0/django_universal_paginator/settings.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.288059 django_universal_paginator-1.2.0/django_universal_paginator/templates/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.290059 django_universal_paginator-1.2.0/django_universal_paginator/templates/paginator/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      738 2022-12-18 18:48:06.000000 django_universal_paginator-1.2.0/django_universal_paginator/templates/paginator/paginator.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.290059 django_universal_paginator-1.2.0/django_universal_paginator/templatetags/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 18:48:06.000000 django_universal_paginator-1.2.0/django_universal_paginator/templatetags/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     3440 2022-12-18 18:48:06.000000 django_universal_paginator-1.2.0/django_universal_paginator/templatetags/paginator_tags.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)    13899 2023-04-16 06:40:59.000000 django_universal_paginator-1.2.0/django_universal_paginator/utils.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.290059 django_universal_paginator-1.2.0/django_universal_paginator.egg-info/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     5196 2023-04-16 06:41:13.000000 django_universal_paginator-1.2.0/django_universal_paginator.egg-info/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1685 2023-04-16 06:41:13.000000 django_universal_paginator-1.2.0/django_universal_paginator.egg-info/SOURCES.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-04-16 06:41:13.000000 django_universal_paginator-1.2.0/django_universal_paginator.egg-info/dependency_links.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       73 2023-04-16 06:41:13.000000 django_universal_paginator-1.2.0/django_universal_paginator.egg-info/requires.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       27 2023-04-16 06:41:13.000000 django_universal_paginator-1.2.0/django_universal_paginator.egg-info/top_level.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1258 2023-04-16 06:41:05.000000 django_universal_paginator-1.2.0/pyproject.toml
--rw-r--r--   0 mirec     (1000) mirec     (1000)      395 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/run_tests.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.290059 django_universal_paginator-1.2.0/sample_project/
--rwxr-xr-x   0 mirec     (1000) mirec     (1000)      749 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/manage.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.289059 django_universal_paginator-1.2.0/sample_project/static/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.290059 django_universal_paginator-1.2.0/sample_project/static/css/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1560 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/static/css/style.css
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.291059 django_universal_paginator-1.2.0/sample_project/templates/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      594 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/sample_project/templates/base.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      375 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/templates/custom_template.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      592 2023-04-16 06:40:59.000000 django_universal_paginator-1.2.0/sample_project/templates/default.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      575 2023-04-16 06:40:59.000000 django_universal_paginator-1.2.0/sample_project/templates/home.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      313 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/templates/large.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.291059 django_universal_paginator-1.2.0/sample_project/templates/paginator/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      438 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/templates/paginator/custom.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      630 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/templates/paginator/paginator.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.291059 django_universal_paginator-1.2.0/sample_project/web/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/web/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      145 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/sample_project/web/apps.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.291059 django_universal_paginator-1.2.0/sample_project/web/migrations/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      890 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/sample_project/web/migrations/0001_initial.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/sample_project/web/migrations/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      198 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/sample_project/web/models.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1757 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/sample_project/web/settings.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)       90 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/sample_project/web/settings_local.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      785 2023-04-16 06:40:59.000000 django_universal_paginator-1.2.0/sample_project/web/urls.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1157 2023-04-16 06:40:59.000000 django_universal_paginator-1.2.0/sample_project/web/views.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      384 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/web/wsgi.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-04-16 06:41:13.292059 django_universal_paginator-1.2.0/setup.cfg
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/setup.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.291059 django_universal_paginator-1.2.0/tests/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/tests/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      762 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/tests/models.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      813 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/tests/settings.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.289059 django_universal_paginator-1.2.0/tests/templates/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.291059 django_universal_paginator-1.2.0/tests/templates/django/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      112 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/tests/templates/django/example.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.291059 django_universal_paginator-1.2.0/tests/templates/jinja/
--rw-r--r--   0 mirec     (1000) mirec     (1000)       19 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/tests/templates/jinja/example.jinja
--rw-r--r--   0 mirec     (1000) mirec     (1000)    18167 2023-04-16 06:40:59.000000 django_universal_paginator-1.2.0/tests/tests.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      522 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/tests/urls.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      577 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/tests/views.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      442 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/tox.ini
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.237296 django_universal_paginator-1.3.0/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       97 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/.editorconfig
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.232296 django_universal_paginator-1.3.0/.github/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.235296 django_universal_paginator-1.3.0/.github/workflows/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1027 2022-12-18 18:41:54.000000 django_universal_paginator-1.3.0/.github/workflows/python-package.yml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      142 2022-12-18 18:41:54.000000 django_universal_paginator-1.3.0/.gitignore
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      197 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    17720 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/.pylintrc
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/AUTHORS
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2595 2023-04-29 04:47:32.000000 django_universal_paginator-1.3.0/CHANGELOG.md
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1073 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/LICENSE
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       92 2022-12-18 18:41:54.000000 django_universal_paginator-1.3.0/MANIFEST.in
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     5196 2023-04-29 04:47:42.237296 django_universal_paginator-1.3.0/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     4439 2022-12-26 12:18:20.000000 django_universal_paginator-1.3.0/README.rst
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.235296 django_universal_paginator-1.3.0/django_universal_paginator/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       24 2022-12-18 18:48:06.000000 django_universal_paginator-1.3.0/django_universal_paginator/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       54 2023-04-29 04:47:25.000000 django_universal_paginator-1.3.0/django_universal_paginator/constants.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      664 2023-02-11 17:23:37.000000 django_universal_paginator-1.3.0/django_universal_paginator/converter.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     4374 2023-04-29 04:47:25.000000 django_universal_paginator-1.3.0/django_universal_paginator/cursor.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      291 2022-12-18 18:48:06.000000 django_universal_paginator-1.3.0/django_universal_paginator/settings.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.233296 django_universal_paginator-1.3.0/django_universal_paginator/templates/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.235296 django_universal_paginator-1.3.0/django_universal_paginator/templates/paginator/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      738 2022-12-18 18:48:06.000000 django_universal_paginator-1.3.0/django_universal_paginator/templates/paginator/paginator.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.235296 django_universal_paginator-1.3.0/django_universal_paginator/templatetags/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 18:48:06.000000 django_universal_paginator-1.3.0/django_universal_paginator/templatetags/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     3440 2022-12-18 18:48:06.000000 django_universal_paginator-1.3.0/django_universal_paginator/templatetags/paginator_tags.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    13282 2023-04-29 04:47:25.000000 django_universal_paginator-1.3.0/django_universal_paginator/utils.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.235296 django_universal_paginator-1.3.0/django_universal_paginator.egg-info/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     5196 2023-04-29 04:47:42.000000 django_universal_paginator-1.3.0/django_universal_paginator.egg-info/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1685 2023-04-29 04:47:42.000000 django_universal_paginator-1.3.0/django_universal_paginator.egg-info/SOURCES.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-04-29 04:47:42.000000 django_universal_paginator-1.3.0/django_universal_paginator.egg-info/dependency_links.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       73 2023-04-29 04:47:42.000000 django_universal_paginator-1.3.0/django_universal_paginator.egg-info/requires.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       27 2023-04-29 04:47:42.000000 django_universal_paginator-1.3.0/django_universal_paginator.egg-info/top_level.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1258 2023-04-29 04:47:32.000000 django_universal_paginator-1.3.0/pyproject.toml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      395 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/run_tests.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.236296 django_universal_paginator-1.3.0/sample_project/
+-rwxr-xr-x   0 mirec     (1000) mirec     (1000)      749 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/sample_project/manage.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.233296 django_universal_paginator-1.3.0/sample_project/static/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.236296 django_universal_paginator-1.3.0/sample_project/static/css/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1560 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/sample_project/static/css/style.css
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.236296 django_universal_paginator-1.3.0/sample_project/templates/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      594 2022-12-18 18:41:54.000000 django_universal_paginator-1.3.0/sample_project/templates/base.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      375 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/sample_project/templates/custom_template.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      638 2023-04-29 04:47:25.000000 django_universal_paginator-1.3.0/sample_project/templates/default.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      575 2023-04-16 06:40:59.000000 django_universal_paginator-1.3.0/sample_project/templates/home.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      313 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/sample_project/templates/large.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.236296 django_universal_paginator-1.3.0/sample_project/templates/paginator/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      438 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/sample_project/templates/paginator/custom.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      630 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/sample_project/templates/paginator/paginator.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.236296 django_universal_paginator-1.3.0/sample_project/web/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/sample_project/web/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      145 2022-12-18 18:41:54.000000 django_universal_paginator-1.3.0/sample_project/web/apps.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.236296 django_universal_paginator-1.3.0/sample_project/web/migrations/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      890 2022-12-18 18:41:54.000000 django_universal_paginator-1.3.0/sample_project/web/migrations/0001_initial.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 18:41:54.000000 django_universal_paginator-1.3.0/sample_project/web/migrations/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      198 2022-12-18 18:41:54.000000 django_universal_paginator-1.3.0/sample_project/web/models.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1757 2022-12-18 18:41:54.000000 django_universal_paginator-1.3.0/sample_project/web/settings.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       90 2022-12-18 18:41:54.000000 django_universal_paginator-1.3.0/sample_project/web/settings_local.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      785 2023-04-16 06:40:59.000000 django_universal_paginator-1.3.0/sample_project/web/urls.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1157 2023-04-16 06:40:59.000000 django_universal_paginator-1.3.0/sample_project/web/views.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      384 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/sample_project/web/wsgi.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-04-29 04:47:42.237296 django_universal_paginator-1.3.0/setup.cfg
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/setup.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.237296 django_universal_paginator-1.3.0/tests/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/tests/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      762 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/tests/models.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      813 2022-12-18 18:41:54.000000 django_universal_paginator-1.3.0/tests/settings.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.234296 django_universal_paginator-1.3.0/tests/templates/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.237296 django_universal_paginator-1.3.0/tests/templates/django/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      112 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/tests/templates/django/example.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 04:47:42.237296 django_universal_paginator-1.3.0/tests/templates/jinja/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       19 2022-12-18 17:51:41.000000 django_universal_paginator-1.3.0/tests/templates/jinja/example.jinja
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    18171 2023-04-29 04:47:25.000000 django_universal_paginator-1.3.0/tests/tests.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      522 2022-12-18 18:41:54.000000 django_universal_paginator-1.3.0/tests/urls.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      577 2022-12-18 18:41:54.000000 django_universal_paginator-1.3.0/tests/views.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      442 2022-12-18 18:41:54.000000 django_universal_paginator-1.3.0/tox.ini
```

### Comparing `django_universal_paginator-1.2.0/.github/workflows/python-package.yml` & `django_universal_paginator-1.3.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/.pylintrc` & `django_universal_paginator-1.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/CHANGELOG.md` & `django_universal_paginator-1.3.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+## 1.3.0 (2023-04-29)
+
+### Feat
+
+- Added row numbers to example list
+
+### Refactor
+
+- Removed unused code
+- Removed first item check, it's not needed
+
 ## 1.2.0 (2023-04-16)
 
 ### Feat
 
 - Added example with values_list
 - Added pagination using values_list
```

### Comparing `django_universal_paginator-1.2.0/LICENSE` & `django_universal_paginator-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/PKG-INFO` & `django_universal_paginator-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_universal_paginator
-Version: 1.2.0
+Version: 1.3.0
 Summary: Simple pagination for django
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/django-universal-paginator
 Project-URL: documentation, https://github.com/mireq/django-universal-paginator
 Project-URL: repository, https://github.com/mireq/django-universal-paginator
 Project-URL: changelog, https://github.com/mireq/django-universal-paginator/blob/master/CHANGELOG.md
```

### Comparing `django_universal_paginator-1.2.0/README.rst` & `django_universal_paginator-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/django_universal_paginator/converter.py` & `django_universal_paginator-1.3.0/django_universal_paginator/converter.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/django_universal_paginator/cursor.py` & `django_universal_paginator-1.3.0/django_universal_paginator/cursor.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 from . import constants, utils
 
 
 OrderKeyFilter = namedtuple('OrderKeyFilter', ['direction', 'values'])
 
 
 class CursorPage(Page):
-	next_page_item = None
-	prev_page_item = None
+	next_page_item = False
+	prev_page_item = False
 	first_item = None
 	last_item = None
 
 	def has_next(self):
-		return self.next_page_item is not None and self.last_item is not None
+		return self.next_page_item and self.last_item is not None
 
 	def has_previous(self):
-		return self.prev_page_item is not None and self.first_item is not None
+		return self.prev_page_item and self.first_item is not None
 
 	def next_page_number(self):
 		page_desc = self.url_encode_order_key(self.paginator.get_order_key(self.last_item))
 		return constants.KEY_NEXT + page_desc
 
 	def previous_page_number(self):
 		page_desc = self.url_encode_order_key(self.paginator.get_order_key(self.first_item))
@@ -39,37 +39,32 @@
 
 class IteratorWrapper(object):
 	def __init__(self, iterator_class, paginator, page, *args, **kwargs):
 		self.iterator = iterator_class(*args, **kwargs)
 		self.paginator = paginator
 		self.page = page
 
-	def _get_sentinel(self, obj):
-		if isinstance(obj, dict):
-			return obj[constants.SENTINEL_NAME]
-		else:
-			return getattr(obj, constants.SENTINEL_NAME)
-
 	@cached_property
 	def _result_cache(self):
 		cache = list(self.iterator)
 		start_key = self.paginator.get_start_order_key(self.page.number)
 
-		if self.page.number is not None and cache and self._get_sentinel(cache[0]):
+		if self.page.number is not None and cache:
 			if start_key.direction == constants.KEY_BACK:
-				self.page.next_page_item = cache.pop(0)
+				self.page.next_page_item = True
 			else:
-				self.page.prev_page_item = cache.pop(0)
+				self.page.prev_page_item = True
 
 		# last item handling (used to check previous page existence)
 		if len(cache) > self.paginator.per_page:
+			cache.pop()
 			if start_key is not None and start_key.direction == constants.KEY_BACK:
-				self.page.prev_page_item = cache.pop()
+				self.page.prev_page_item = True
 			else:
-				self.page.next_page_item = cache.pop()
+				self.page.next_page_item = True
 
 		# revert backwards iterated queryset
 		if start_key is not None and start_key.direction == constants.KEY_BACK:
 			cache = cache[::-1]
 
 		# set first and last items of page
 		if cache:
@@ -100,15 +95,15 @@
 
 	def raise_invalid_page_format(self):
 		raise InvalidPage(gettext("Invalid page format"))
 
 	def page(self, number):
 		order_key_filter = self.validate_number(number)
 		page = CursorPage(None, order_key_filter, self)
-		count = self.per_page + (2 if order_key_filter else 1) # load one more item before and after list
+		count = self.per_page + 1 # load one more item before and after list
 		qs = self.object_list
 		if order_key_filter:
 			qs = utils.filter_by_order_key(qs, order_key_filter.direction, order_key_filter.values)
 		qs = qs[:count]
 		qs._iterable_class = partial(IteratorWrapper, qs._iterable_class, self, page)
 		page.object_list = qs
 		# force initialization
```

### Comparing `django_universal_paginator-1.2.0/django_universal_paginator/templates/paginator/paginator.html` & `django_universal_paginator-1.3.0/django_universal_paginator/templates/paginator/paginator.html`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/django_universal_paginator/templatetags/paginator_tags.py` & `django_universal_paginator-1.3.0/django_universal_paginator/templatetags/paginator_tags.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/django_universal_paginator/utils.py` & `django_universal_paginator-1.3.0/django_universal_paginator/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import struct
 from copy import deepcopy
 from datetime import time, date, datetime, timezone
 from decimal import Decimal as D
 from typing import Union
 
 from django.core.paginator import InvalidPage, Paginator
-from django.db.models import Case, When, Value as V, Q, F
+from django.db.models import Q, F
 from django.db.models.constants import LOOKUP_SEP
 from django.db.models.expressions import OrderBy
 from django.http import Http404
 from django.utils.http import urlsafe_base64_encode, urlsafe_base64_decode
 from django.utils.translation import gettext_lazy as _
 
 from . import constants
@@ -396,21 +396,15 @@
 		qs = qs.order_by(*order_by)
 
 	filter_combinations = {}
 	q = Q() # final filter
 
 	# create chain of rule rule for example for name="x" parent=1, id=2 will be following:
 	# name > 'x' OR name = 'x' AND parent > 1 OR name = 'x' AND parent = 1 AND id >= 2
-	for i, value in enumerate(zip(order_by, start_position)):
-		# unpack values
-		order_expression, value = value
-
-		# last tieration
-		is_last = i == len(order_by) - 1
-
+	for order_expression, value in zip(order_by, start_position):
 		# filter by
 		field_name = order_expression.expression.name
 
 		field_lookup = ''
 
 		# Value  Order (NULL)  First condition    Next condition
 		# ------------------------------------------------------
@@ -430,16 +424,14 @@
 				filter_combinations[f'{field_name}__isnull'] = True
 				continue
 			else:
 				logger.warning("No nulls_first / nulls_last specified")
 		else:
 			# smaller or greater
 			direction = 'lt' if order_expression.descending else 'gt'
-			if is_last: # change > to >= and < to <= on last iteration
-				direction = f'{direction}e'
 
 			# construct field lookup
 			field_lookup = f'{field_name}__{direction}'
 
 			# set lookup to current combination
 			if order_expression.nulls_last:
 				filter_combination = (
@@ -460,26 +452,11 @@
 		filter_combinations.pop(field_lookup, None)
 		filter_combinations[field_name] = value
 
 	# apply filter
 	if q:
 		try:
 			qs = qs.filter(q)
-
-			# mark item which matches start position
-			sentinel_query = {
-				order_expression.expression.name: start
-				for order_expression, start
-				in zip(order_by, start_position)
-			}
-			is_sentinel = Case(
-				When(Q(**sentinel_query), then=V(True)),
-				default=V(False)
-			)
-			sentinel_annotation = {
-				constants.SENTINEL_NAME: is_sentinel
-			}
-			qs = qs.annotate(**sentinel_annotation)
 		except Exception:
 			raise InvalidPage()
 
 	return qs
```

### Comparing `django_universal_paginator-1.2.0/django_universal_paginator.egg-info/PKG-INFO` & `django_universal_paginator-1.3.0/django_universal_paginator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-universal-paginator
-Version: 1.2.0
+Version: 1.3.0
 Summary: Simple pagination for django
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/django-universal-paginator
 Project-URL: documentation, https://github.com/mireq/django-universal-paginator
 Project-URL: repository, https://github.com/mireq/django-universal-paginator
 Project-URL: changelog, https://github.com/mireq/django-universal-paginator/blob/master/CHANGELOG.md
```

### Comparing `django_universal_paginator-1.2.0/django_universal_paginator.egg-info/SOURCES.txt` & `django_universal_paginator-1.3.0/django_universal_paginator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/pyproject.toml` & `django_universal_paginator-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -39,9 +39,9 @@
 [tool.setuptools]
 packages = ["django_universal_paginator", "django_universal_paginator.templates.paginator", "django_universal_paginator.templatetags"]
 
 [tool.setuptools_scm]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.2.0"
+version = "1.3.0"
 tag_format = "$version"
```

### Comparing `django_universal_paginator-1.2.0/sample_project/manage.py` & `django_universal_paginator-1.3.0/sample_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/sample_project/static/css/style.css` & `django_universal_paginator-1.3.0/sample_project/static/css/style.css`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/sample_project/templates/base.html` & `django_universal_paginator-1.3.0/sample_project/templates/base.html`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/sample_project/templates/default.html` & `django_universal_paginator-1.3.0/sample_project/templates/default.html`

 * *Files 8% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 {% block head_title %}Default paginator{% endblock %}
 
 {% block content %}
 	<div class="paginated-list">
 		<div class="pagination top">{% block pagination_top %}{% pagination %}{% endblock %}</div>
 		<ul class="items">
 			{% for object in object_list %}
-				<li>{% if object.name %}{{ object.name }}{% else %}{{ object }}{% endif %}</li>
+				<li>{% if object.id %}{{ object.id }}. {% endif %}{% if object.name %}{{ object.name }}{% else %}{{ object }}{% endif %}</li>
 			{% endfor %}
 		</ul>
 		<div class="pagination bottom">{% block pagination_bottom %}{% pagination %}{% endblock %}</div>
 	</div>
 {% endblock %}
```

### Comparing `django_universal_paginator-1.2.0/sample_project/templates/home.html` & `django_universal_paginator-1.3.0/sample_project/templates/home.html`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/sample_project/templates/paginator/paginator.html` & `django_universal_paginator-1.3.0/sample_project/templates/paginator/paginator.html`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/sample_project/web/migrations/0001_initial.py` & `django_universal_paginator-1.3.0/sample_project/web/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/sample_project/web/settings.py` & `django_universal_paginator-1.3.0/sample_project/web/settings.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/sample_project/web/urls.py` & `django_universal_paginator-1.3.0/sample_project/web/urls.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/sample_project/web/views.py` & `django_universal_paginator-1.3.0/sample_project/web/views.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/tests/models.py` & `django_universal_paginator-1.3.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/tests/settings.py` & `django_universal_paginator-1.3.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/tests/tests.py` & `django_universal_paginator-1.3.0/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,27 +212,27 @@
 		self.assertEqual([1, 2, 3, 4, 5], books)
 
 		def check_filter(order_by, backwards=False):
 			books = list(Book.objects.order_by(*order_by))
 			if backwards:
 				books.reverse()
 			ids = list(book.pk for book in books)
-			expect_ids = ids
+			expect_ids = ids[1:]
 			next_book = ids[0]
 			debug_books = '\n'.join(str(book) for book in books)
 
 			while True:
 				book = book_list[next_book]
 				order_key = get_order_key(book, order_by)
 				ids = get_books(order_by, order_key, backwards=backwards)
 				self.assertEqual(expect_ids, ids, msg=f'Wrong rows returned, requested order: {order_by}, order_key: {order_key}, books:\n{debug_books}')
 				expect_ids = ids[1:]
 				if len(ids) < 2:
 					break
-				next_book = ids[1]
+				next_book = ids[0]
 
 		def check_filters(order_by):
 			check_filter(order_by)
 			check_filter(order_by, backwards=True)
 
 		check_filters(['pk'])
 		check_filters(['-pk'])
```

### Comparing `django_universal_paginator-1.2.0/tests/urls.py` & `django_universal_paginator-1.3.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.2.0/tests/views.py` & `django_universal_paginator-1.3.0/tests/views.py`

 * *Files identical despite different names*


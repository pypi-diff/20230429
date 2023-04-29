# Comparing `tmp/django-sample-data-generator-1.0.3.tar.gz` & `tmp/django-sample-data-generator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sample-data-generator-1.0.3.tar", last modified: Thu Mar 30 07:18:30 2023, max compression
+gzip compressed data, was "django-sample-data-generator-1.0.4.tar", last modified: Sat Apr 29 10:57:10 2023, max compression
```

## Comparing `django-sample-data-generator-1.0.3.tar` & `django-sample-data-generator-1.0.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:18:30.194520 django-sample-data-generator-1.0.3/
--rw-r--r--   0 mirec     (1000) mirec     (1000)       53 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/.coveragerc
--rw-r--r--   0 mirec     (1000) mirec     (1000)       97 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.3/.editorconfig
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:18:30.191520 django-sample-data-generator-1.0.3/.github/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:18:30.192520 django-sample-data-generator-1.0.3/.github/workflows/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1029 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/.github/workflows/python-package.yml
--rw-r--r--   0 mirec     (1000) mirec     (1000)      119 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/.gitignore
--rw-r--r--   0 mirec     (1000) mirec     (1000)    17720 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/.pylintrc
--rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.3/AUTHORS
--rw-r--r--   0 mirec     (1000) mirec     (1000)      919 2023-03-30 07:18:20.000000 django-sample-data-generator-1.0.3/CHANGELOG.md
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1560 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.3/LICENSE
--rw-r--r--   0 mirec     (1000) mirec     (1000)      157 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.3/MANIFEST.in
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2066 2023-03-30 07:18:30.193520 django-sample-data-generator-1.0.3/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1320 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/README.rst
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:18:30.192520 django-sample-data-generator-1.0.3/django_sample_data_generator.egg-info/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2066 2023-03-30 07:18:30.000000 django-sample-data-generator-1.0.3/django_sample_data_generator.egg-info/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1556 2023-03-30 07:18:30.000000 django-sample-data-generator-1.0.3/django_sample_data_generator.egg-info/SOURCES.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-03-30 07:18:30.000000 django-sample-data-generator-1.0.3/django_sample_data_generator.egg-info/dependency_links.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       60 2023-03-30 07:18:30.000000 django-sample-data-generator-1.0.3/django_sample_data_generator.egg-info/requires.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       24 2023-03-30 07:18:30.000000 django-sample-data-generator-1.0.3/django_sample_data_generator.egg-info/top_level.txt
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:18:30.192520 django-sample-data-generator-1.0.3/django_sample_generator/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.3/django_sample_generator/__init__.py
--rwxr-xr-x   0 mirec     (1000) mirec     (1000)     1233 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.3/django_sample_generator/__main__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      152 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.3/django_sample_generator/constants.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     5515 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.3/django_sample_generator/fields.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     4388 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.3/django_sample_generator/functions.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     4286 2023-03-30 07:18:13.000000 django-sample-data-generator-1.0.3/django_sample_generator/generator.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:18:30.192520 django-sample-data-generator-1.0.3/django_sample_generator/management/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.3/django_sample_generator/management/__init__.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:18:30.193520 django-sample-data-generator-1.0.3/django_sample_generator/management/commands/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.3/django_sample_generator/management/commands/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      703 2021-04-09 16:21:16.000000 django-sample-data-generator-1.0.3/django_sample_generator/management/commands/create_sample_data.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)       67 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.3/django_sample_generator/mock.png
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.3/django_sample_generator/mock.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)      451 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.3/django_sample_generator/register.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)   180272 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.3/django_sample_generator/text_db
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2672 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.3/django_sample_generator/text_generator.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1154 2023-03-30 07:18:20.000000 django-sample-data-generator-1.0.3/pyproject.toml
--rw-r--r--   0 mirec     (1000) mirec     (1000)      395 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/run_tests.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:18:30.193520 django-sample-data-generator-1.0.3/sample_project/
--rw-r--r--   0 mirec     (1000) mirec     (1000)       17 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.3/sample_project/.gitignore
--rwxr-xr-x   0 mirec     (1000) mirec     (1000)      749 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.3/sample_project/manage.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:18:30.193520 django-sample-data-generator-1.0.3/sample_project/web/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.3/sample_project/web/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      887 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/sample_project/web/generators.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:18:30.193520 django-sample-data-generator-1.0.3/sample_project/web/migrations/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2318 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/sample_project/web/migrations/0001_initial.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.3/sample_project/web/migrations/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1560 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/sample_project/web/models.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      765 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/sample_project/web/settings.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)       42 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/sample_project/web/urls.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      384 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.3/sample_project/web/wsgi.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-03-30 07:18:30.194520 django-sample-data-generator-1.0.3/setup.cfg
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/setup.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:18:30.193520 django-sample-data-generator-1.0.3/tests/
--rw-r--r--   0 mirec     (1000) mirec     (1000)       17 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/tests/.gitignore
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/tests/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      884 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/tests/generators.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1430 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/tests/generators_functions.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      880 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/tests/generators_manually_defined.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      242 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/tests/generators_not_registered.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      783 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/tests/generators_unique_fail.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2295 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/tests/models.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      410 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/tests/settings.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     6480 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/tests/tests.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      445 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.3/tox.ini
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 10:57:10.424862 django-sample-data-generator-1.0.4/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       53 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/.coveragerc
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       97 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.4/.editorconfig
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 10:57:10.419862 django-sample-data-generator-1.0.4/.github/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 10:57:10.420862 django-sample-data-generator-1.0.4/.github/workflows/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1029 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/.github/workflows/python-package.yml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      119 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/.gitignore
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    17720 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/.pylintrc
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.4/AUTHORS
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      982 2023-04-29 10:57:00.000000 django-sample-data-generator-1.0.4/CHANGELOG.md
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1560 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.4/LICENSE
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      157 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.4/MANIFEST.in
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2066 2023-04-29 10:57:10.424862 django-sample-data-generator-1.0.4/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1320 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/README.rst
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 10:57:10.421862 django-sample-data-generator-1.0.4/django_sample_data_generator.egg-info/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2066 2023-04-29 10:57:10.000000 django-sample-data-generator-1.0.4/django_sample_data_generator.egg-info/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1556 2023-04-29 10:57:10.000000 django-sample-data-generator-1.0.4/django_sample_data_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-04-29 10:57:10.000000 django-sample-data-generator-1.0.4/django_sample_data_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       60 2023-04-29 10:57:10.000000 django-sample-data-generator-1.0.4/django_sample_data_generator.egg-info/requires.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       24 2023-04-29 10:57:10.000000 django-sample-data-generator-1.0.4/django_sample_data_generator.egg-info/top_level.txt
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 10:57:10.421862 django-sample-data-generator-1.0.4/django_sample_generator/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.4/django_sample_generator/__init__.py
+-rwxr-xr-x   0 mirec     (1000) mirec     (1000)     1233 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.4/django_sample_generator/__main__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      152 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.4/django_sample_generator/constants.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     5515 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.4/django_sample_generator/fields.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     4388 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.4/django_sample_generator/functions.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     4286 2023-04-29 10:55:53.000000 django-sample-data-generator-1.0.4/django_sample_generator/generator.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 10:57:10.421862 django-sample-data-generator-1.0.4/django_sample_generator/management/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.4/django_sample_generator/management/__init__.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 10:57:10.421862 django-sample-data-generator-1.0.4/django_sample_generator/management/commands/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.4/django_sample_generator/management/commands/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      703 2021-04-09 16:21:16.000000 django-sample-data-generator-1.0.4/django_sample_generator/management/commands/create_sample_data.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       67 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.4/django_sample_generator/mock.png
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.4/django_sample_generator/mock.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      451 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.4/django_sample_generator/register.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)   180272 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.4/django_sample_generator/text_db
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2672 2023-03-30 07:17:14.000000 django-sample-data-generator-1.0.4/django_sample_generator/text_generator.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1154 2023-04-29 10:57:00.000000 django-sample-data-generator-1.0.4/pyproject.toml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      395 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/run_tests.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 10:57:10.422862 django-sample-data-generator-1.0.4/sample_project/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       17 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.4/sample_project/.gitignore
+-rwxr-xr-x   0 mirec     (1000) mirec     (1000)      749 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.4/sample_project/manage.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 10:57:10.423862 django-sample-data-generator-1.0.4/sample_project/web/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.4/sample_project/web/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      887 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/sample_project/web/generators.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 10:57:10.423862 django-sample-data-generator-1.0.4/sample_project/web/migrations/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2318 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/sample_project/web/migrations/0001_initial.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.4/sample_project/web/migrations/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1560 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/sample_project/web/models.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      765 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/sample_project/web/settings.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       42 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/sample_project/web/urls.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      384 2017-06-10 15:40:04.000000 django-sample-data-generator-1.0.4/sample_project/web/wsgi.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-04-29 10:57:10.424862 django-sample-data-generator-1.0.4/setup.cfg
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/setup.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-29 10:57:10.424862 django-sample-data-generator-1.0.4/tests/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       17 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/tests/.gitignore
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/tests/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      884 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/tests/generators.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1430 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/tests/generators_functions.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      880 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/tests/generators_manually_defined.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      242 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/tests/generators_not_registered.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      783 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/tests/generators_unique_fail.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2295 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/tests/models.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      410 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/tests/settings.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     6480 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/tests/tests.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      445 2022-12-31 16:38:58.000000 django-sample-data-generator-1.0.4/tox.ini
```

### Comparing `django-sample-data-generator-1.0.3/.github/workflows/python-package.yml` & `django-sample-data-generator-1.0.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/.pylintrc` & `django-sample-data-generator-1.0.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/CHANGELOG.md` & `django-sample-data-generator-1.0.4/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.0.4 (2023-04-29)
+
+### Fix
+
+- Unique check should be list
+
 ## 1.0.3 (2023-03-30)
 
 ### Feat
 
 - Allow modify instance before unique checks
 
 ## 1.0.2 (2023-03-30)
```

### Comparing `django-sample-data-generator-1.0.3/LICENSE` & `django-sample-data-generator-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/PKG-INFO` & `django-sample-data-generator-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sample-data-generator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Sample data generator
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/django-django-sample-data-generator
 Project-URL: documentation, https://github.com/mireq/django-django-sample-data-generator
 Project-URL: repository, https://github.com/mireq/django-django-sample-data-generator
 Project-URL: changelog, https://github.com/mireq/django-django-sample-data-generator/blob/master/CHANGELOG.md
```

### Comparing `django-sample-data-generator-1.0.3/README.rst` & `django-sample-data-generator-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/django_sample_data_generator.egg-info/PKG-INFO` & `django-sample-data-generator-1.0.4/django_sample_data_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sample-data-generator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Sample data generator
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/django-django-sample-data-generator
 Project-URL: documentation, https://github.com/mireq/django-django-sample-data-generator
 Project-URL: repository, https://github.com/mireq/django-django-sample-data-generator
 Project-URL: changelog, https://github.com/mireq/django-django-sample-data-generator/blob/master/CHANGELOG.md
```

### Comparing `django-sample-data-generator-1.0.3/django_sample_data_generator.egg-info/SOURCES.txt` & `django-sample-data-generator-1.0.4/django_sample_data_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/django_sample_generator/__main__.py` & `django-sample-data-generator-1.0.4/django_sample_generator/__main__.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/django_sample_generator/fields.py` & `django-sample-data-generator-1.0.4/django_sample_generator/fields.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/django_sample_generator/functions.py` & `django-sample-data-generator-1.0.4/django_sample_generator/functions.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/django_sample_generator/generator.py` & `django-sample-data-generator-1.0.4/django_sample_generator/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 class ModelGeneratorBase(type):
 	def __new__(cls, name, bases, attrs):
 		new_class = super(ModelGeneratorBase, cls).__new__(cls, name, bases, attrs)
 		opts = getattr(new_class, 'Meta', None)
 		if opts is None:
 			opts = type('Meta', (MetaOpts,), {})
 		opts.model = getattr(opts, 'model', MetaOpts.model)
-		opts.unique_checks = copy(getattr(opts, 'unique_checks', MetaOpts.unique_checks))
+		opts.unique_checks = list(getattr(opts, 'unique_checks', MetaOpts.unique_checks))
 		opts.field_kwargs = copy(getattr(opts, 'field_kwargs', MetaOpts.field_kwargs))
 		opts.fields = copy(getattr(opts, 'fields', MetaOpts.fields))
 		opts.exclude = copy(getattr(opts, 'exclude', MetaOpts.exclude))
 		new_class._meta = opts
 		new_class._meta.generators = {}
 
 		if opts.model:
```

### Comparing `django-sample-data-generator-1.0.3/django_sample_generator/management/commands/create_sample_data.py` & `django-sample-data-generator-1.0.4/django_sample_generator/management/commands/create_sample_data.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/django_sample_generator/text_db` & `django-sample-data-generator-1.0.4/django_sample_generator/text_db`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/django_sample_generator/text_generator.py` & `django-sample-data-generator-1.0.4/django_sample_generator/text_generator.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/pyproject.toml` & `django-sample-data-generator-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -39,9 +39,9 @@
 where = ["."]
 include = ["django_sample_generator*"]
 
 [tool.setuptools_scm]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.3"
+version = "1.0.4"
 tag_format = "$version"
```

### Comparing `django-sample-data-generator-1.0.3/sample_project/manage.py` & `django-sample-data-generator-1.0.4/sample_project/manage.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/sample_project/web/generators.py` & `django-sample-data-generator-1.0.4/sample_project/web/generators.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/sample_project/web/migrations/0001_initial.py` & `django-sample-data-generator-1.0.4/sample_project/web/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/sample_project/web/models.py` & `django-sample-data-generator-1.0.4/sample_project/web/models.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/sample_project/web/settings.py` & `django-sample-data-generator-1.0.4/sample_project/web/settings.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/tests/generators.py` & `django-sample-data-generator-1.0.4/tests/generators.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/tests/generators_functions.py` & `django-sample-data-generator-1.0.4/tests/generators_functions.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/tests/generators_manually_defined.py` & `django-sample-data-generator-1.0.4/tests/generators_manually_defined.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/tests/generators_unique_fail.py` & `django-sample-data-generator-1.0.4/tests/generators_unique_fail.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/tests/models.py` & `django-sample-data-generator-1.0.4/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-sample-data-generator-1.0.3/tests/tests.py` & `django-sample-data-generator-1.0.4/tests/tests.py`

 * *Files identical despite different names*


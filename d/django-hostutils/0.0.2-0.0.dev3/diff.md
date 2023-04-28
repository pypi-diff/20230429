# Comparing `tmp/django-hostutils-0.0.2.tar.gz` & `tmp/django-hostutils-0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-hostutils-0.0.2.tar", last modified: Fri Apr 28 22:57:09 2023, max compression
+gzip compressed data, was "django-hostutils-0.0.dev3.tar", last modified: Tue Apr 25 00:40:22 2023, max compression
```

## Comparing `django-hostutils-0.0.2.tar` & `django-hostutils-0.0.dev3.tar`

### file list

```diff
@@ -1,52 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:57:09.609959 django-hostutils-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-28 22:57:09.609959 django-hostutils-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-28 22:57:09.609959 django-hostutils-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:57:09.605959 django-hostutils-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:57:09.605959 django-hostutils-0.0.2/src/django_hostutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-28 22:57:09.000000 django-hostutils-0.0.2/src/django_hostutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-28 22:57:09.000000 django-hostutils-0.0.2/src/django_hostutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:57:09.000000 django-hostutils-0.0.2/src/django_hostutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 22:57:09.000000 django-hostutils-0.0.2/src/django_hostutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 22:57:09.000000 django-hostutils-0.0.2/src/django_hostutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:57:09.000000 django-hostutils-0.0.2/src/django_hostutils.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:57:09.605959 django-hostutils-0.0.2/src/djangoaddicts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:57:09.605959 django-hostutils-0.0.2/src/djangoaddicts/hostutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 22:57:09.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:57:09.605959 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:57:09.605959 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:57:09.605959 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:57:09.605959 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_partition_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:57:09.609959 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html
--rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html
--rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:57:09.609959 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card_swap.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_results_timestamp.htm
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:57:09.609959 django-hostutils-0.0.2/src/djangoaddicts/hostutils/views/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/views/ajax.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/views/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-04-28 22:56:55.000000 django-hostutils-0.0.2/src/djangoaddicts/hostutils/views/htmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/bandit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/black.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/django_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   133744 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/cpu.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   131317 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/cpu.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   124420 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/disk.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   161082 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/host.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   100187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/memory.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   154714 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/network.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   122738 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/process.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/features.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   131317 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/cpu.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   124420 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/disk.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   161082 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/host.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   100187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/memory.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   154714 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/network.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   122738 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/process.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/internals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/version_history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_partition_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card_swap.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_results_timestamp.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/ajax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/htmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_cpu_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_interface_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_partition_usage.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_process_details.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_ajax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_htmx.py
```

### Comparing `django-hostutils-0.0.2/.gitignore` & `django-hostutils-0.0.dev3/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -126,9 +126,8 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 # other
 local_test
-.vscode
-src/djangoaddicts/hostutils/_version.py
+.vscode
```

### Comparing `django-hostutils-0.0.2/LICENSE` & `django-hostutils-0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/PKG-INFO` & `django-hostutils-0.0.dev3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: django-hostutils
-Version: 0.0.2
-Summary: host utilities for django projects
-Home-page: https://github.com/davidslusser/django-hostutils
-Author: David Slusser
-Author-email: dbslusser@gmail.com
-License: GNU GENERAL PUBLIC LICENSE
-Platform: any
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # django-hostutils
 Host utilities package for django projects. Bootstrap 5 templates are provided.  Host metric data includes:
 - Host OS, release, uptime
 - CPU count and utilization
 - Memory usage
 - Disk partations and utilization
 - Processes running, idle, sleeping
@@ -27,40 +14,27 @@
 |--------------|------|
 | Author       | David Slusser |
 | Description  | Host utilities package for django projects. |
 | Requirements | `Python 3.x` +<br>`Django 3.2.x` + |
 
 <br/>
 
-## Code Quality
+## Code Quality Checks
 | Workflow | Description             | Status                                                                       |
 |----------|-------------------------|------------------------------------------------------------------------------|
 |Bandit|security checks|![Bandit](https://github.com/davidslusser/workflow_tests/actions/workflows/bandit.yaml/badge.svg)|
 |Black|code formatting|![Black](https://github.com/davidslusser/workflow_tests/actions/workflows/black.yaml/badge.svg)|
 |Mypy|static type checking|![Mypy](https://github.com/davidslusser/workflow_tests/actions/workflows/mypy.yaml/badge.svg)|
 |Pylint|static code analysis|![Pylint](https://github.com/davidslusser/workflow_tests/actions/workflows/pylint.yaml/badge.svg)|
 |Pytest|unit testing|![Pytest](https://github.com/davidslusser/workflow_tests/actions/workflows/pytest.yaml/badge.svg)|
 
 <br/>
 
-## Documentation
-| Workflow | Description             | Status                                                                       |
-|----------|-------------------------|------------------------------------------------------------------------------|
-|Docs|ReadTheDocs Build|[![Documentation Status](https://readthedocs.org/projects/django-hostutils/badge/?version=latest)](https://django-hostutils.readthedocs.io/en/latest/?badge=latest)|
-
-Full documentation is available here:
-
-https://django-hostutils.readthedocs.io/en/latest/index.html 
-
-<br/>
-
 ## License
-django-hostutils is licensed under the GNU-3 license (see the LICENSE file for details).
-
-https://github.com/davidslusser/django-hostutils/blob/docs/LICENSE 
+django-userextensions is licensed under the GNU-3 license (see the LICENSE file for details).
 
 <br/>
 
 ## Installation 
 - pip install django-hostutils
 - add the following to your INSTALLED_APPS
 
@@ -69,24 +43,22 @@
     ```
 - add the following to your project-level urls.py:
    
    ```python
    path("hostutils/", include("djangoaddicts.hostutils.urls"), ),
    ```
 
-<br/>
-
 ## Usage
 Several pages are available. If you have a Bootstrap 5 nav-menu you can add the following snippet in your navbar where appropriate:
 
-```
-{% include 'hostutils/bs5/snippets/hostutils_nav_menu.htm' %}
-```
+    ```
+    {% include 'hostutils/bs5/snippets/hostutils_nav_menu.htm' %}
+    ```
 
-Individual pages can also be linked directly:
+Alternatively, individual pages can linked directly:
 
 - Host overview page: 
 
     ```
     {% url 'hostutils:host_details' %}
     ```
```

### Comparing `django-hostutils-0.0.2/README.md` & `django-hostutils-0.0.dev3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: django-hostutils
+Version: 0.0.dev3
+Summary: host utilities for django projects
+Home-page: https://github.com/davidslusser/django-hostutils
+Author: David Slusser
+Author-email: dbslusser@gmail.com
+License: GNU GENERAL PUBLIC LICENSE
+Platform: any
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # django-hostutils
 Host utilities package for django projects. Bootstrap 5 templates are provided.  Host metric data includes:
 - Host OS, release, uptime
 - CPU count and utilization
 - Memory usage
 - Disk partations and utilization
 - Processes running, idle, sleeping
@@ -14,40 +27,27 @@
 |--------------|------|
 | Author       | David Slusser |
 | Description  | Host utilities package for django projects. |
 | Requirements | `Python 3.x` +<br>`Django 3.2.x` + |
 
 <br/>
 
-## Code Quality
+## Code Quality Checks
 | Workflow | Description             | Status                                                                       |
 |----------|-------------------------|------------------------------------------------------------------------------|
 |Bandit|security checks|![Bandit](https://github.com/davidslusser/workflow_tests/actions/workflows/bandit.yaml/badge.svg)|
 |Black|code formatting|![Black](https://github.com/davidslusser/workflow_tests/actions/workflows/black.yaml/badge.svg)|
 |Mypy|static type checking|![Mypy](https://github.com/davidslusser/workflow_tests/actions/workflows/mypy.yaml/badge.svg)|
 |Pylint|static code analysis|![Pylint](https://github.com/davidslusser/workflow_tests/actions/workflows/pylint.yaml/badge.svg)|
 |Pytest|unit testing|![Pytest](https://github.com/davidslusser/workflow_tests/actions/workflows/pytest.yaml/badge.svg)|
 
 <br/>
 
-## Documentation
-| Workflow | Description             | Status                                                                       |
-|----------|-------------------------|------------------------------------------------------------------------------|
-|Docs|ReadTheDocs Build|[![Documentation Status](https://readthedocs.org/projects/django-hostutils/badge/?version=latest)](https://django-hostutils.readthedocs.io/en/latest/?badge=latest)|
-
-Full documentation is available here:
-
-https://django-hostutils.readthedocs.io/en/latest/index.html 
-
-<br/>
-
 ## License
-django-hostutils is licensed under the GNU-3 license (see the LICENSE file for details).
-
-https://github.com/davidslusser/django-hostutils/blob/docs/LICENSE 
+django-userextensions is licensed under the GNU-3 license (see the LICENSE file for details).
 
 <br/>
 
 ## Installation 
 - pip install django-hostutils
 - add the following to your INSTALLED_APPS
 
@@ -56,24 +56,22 @@
     ```
 - add the following to your project-level urls.py:
    
    ```python
    path("hostutils/", include("djangoaddicts.hostutils.urls"), ),
    ```
 
-<br/>
-
 ## Usage
 Several pages are available. If you have a Bootstrap 5 nav-menu you can add the following snippet in your navbar where appropriate:
 
-```
-{% include 'hostutils/bs5/snippets/hostutils_nav_menu.htm' %}
-```
+    ```
+    {% include 'hostutils/bs5/snippets/hostutils_nav_menu.htm' %}
+    ```
 
-Individual pages can also be linked directly:
+Alternatively, individual pages can linked directly:
 
 - Host overview page: 
 
     ```
     {% url 'hostutils:host_details' %}
     ```
```

### Comparing `django-hostutils-0.0.2/pyproject.toml` & `django-hostutils-0.0.dev3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,51 @@
-[tool.bandit]
-exclude_dirs = ["venv", "tests"]
+# https://docs.pytest.org/en/6.2.x/customize.html#pyproject-toml
+[tool.pytest.ini_options]
+addopts = "-s -v -x --strict-markers -m 'not extra' --doctest-modules --cov=."
+testpaths = ["tests"]
+filterwarnings = [
+    "ignore::UserWarning",
+]
 
 
-[tool.black]
-line-length = 120
+[tool.coverage.run]
+branch = true
+source = ["tests"]
+omit = ["*_test.py", "*/tests/*", "setup.py"]
 
 
 [tool.coverage.report]
 show_missing = true
 
 
-[tool.coverage.run]
-branch = true
-source = ["tests"]
-omit = ["*_test.py", "*/tests/*", "*_version.py", "setup.py"]
+[tool.bandit]
+exclude_dirs = ["venv", "tests"]
+
+
+[tool.black]
+line-length = 120
 
 
 [tool.flake8]
 ignore = "E203,E266,H106,H904,E133"
 max-line-length = 120
 max-complexity = 25
 hang-closing = true
 exclude = "tests"
 
 
-[tool.mypy]
-ignore_missing_imports = true
-exclude = ['venv/*']
-
-
-[tool.pylint.format]
-max-line-length = "120"
-
-
 [tool.pylint.MASTER]
 ignore-paths = ["tests"]
 exit-zero = true
 
 
 [tool.pylint.'MESSAGES CONTROL']
 disable = "R0903,R0913,R0901,W0613,W0718,C0114,C0115,C0103,R1725,R0801,R1702,R0912"
 
 
-# https://docs.pytest.org/en/6.2.x/customize.html#pyproject-toml
-[tool.pytest.ini_options]
-addopts = "-s -v -x --strict-markers -m 'not extra' --doctest-modules --cov=."
-testpaths = ["tests"]
-filterwarnings = [
-    "ignore::UserWarning",
-]
+[tool.pylint.format]
+max-line-length = "120"
+
 
-[tool.setuptools_scm]
-write_to = "src/djangoaddicts/hostutils/_version.py"
+[tool.mypy]
+ignore_missing_imports = true
+exclude = ['venv/*']
```

### Comparing `django-hostutils-0.0.2/setup.cfg` & `django-hostutils-0.0.dev3/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/django_hostutils.egg-info/PKG-INFO` & `django-hostutils-0.0.dev3/src/django_hostutils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hostutils
-Version: 0.0.2
+Version: 0.0.dev3
 Summary: host utilities for django projects
 Home-page: https://github.com/davidslusser/django-hostutils
 Author: David Slusser
 Author-email: dbslusser@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: any
 Description-Content-Type: text/markdown
@@ -27,40 +27,27 @@
 |--------------|------|
 | Author       | David Slusser |
 | Description  | Host utilities package for django projects. |
 | Requirements | `Python 3.x` +<br>`Django 3.2.x` + |
 
 <br/>
 
-## Code Quality
+## Code Quality Checks
 | Workflow | Description             | Status                                                                       |
 |----------|-------------------------|------------------------------------------------------------------------------|
 |Bandit|security checks|![Bandit](https://github.com/davidslusser/workflow_tests/actions/workflows/bandit.yaml/badge.svg)|
 |Black|code formatting|![Black](https://github.com/davidslusser/workflow_tests/actions/workflows/black.yaml/badge.svg)|
 |Mypy|static type checking|![Mypy](https://github.com/davidslusser/workflow_tests/actions/workflows/mypy.yaml/badge.svg)|
 |Pylint|static code analysis|![Pylint](https://github.com/davidslusser/workflow_tests/actions/workflows/pylint.yaml/badge.svg)|
 |Pytest|unit testing|![Pytest](https://github.com/davidslusser/workflow_tests/actions/workflows/pytest.yaml/badge.svg)|
 
 <br/>
 
-## Documentation
-| Workflow | Description             | Status                                                                       |
-|----------|-------------------------|------------------------------------------------------------------------------|
-|Docs|ReadTheDocs Build|[![Documentation Status](https://readthedocs.org/projects/django-hostutils/badge/?version=latest)](https://django-hostutils.readthedocs.io/en/latest/?badge=latest)|
-
-Full documentation is available here:
-
-https://django-hostutils.readthedocs.io/en/latest/index.html 
-
-<br/>
-
 ## License
-django-hostutils is licensed under the GNU-3 license (see the LICENSE file for details).
-
-https://github.com/davidslusser/django-hostutils/blob/docs/LICENSE 
+django-userextensions is licensed under the GNU-3 license (see the LICENSE file for details).
 
 <br/>
 
 ## Installation 
 - pip install django-hostutils
 - add the following to your INSTALLED_APPS
 
@@ -69,24 +56,22 @@
     ```
 - add the following to your project-level urls.py:
    
    ```python
    path("hostutils/", include("djangoaddicts.hostutils.urls"), ),
    ```
 
-<br/>
-
 ## Usage
 Several pages are available. If you have a Bootstrap 5 nav-menu you can add the following snippet in your navbar where appropriate:
 
-```
-{% include 'hostutils/bs5/snippets/hostutils_nav_menu.htm' %}
-```
+    ```
+    {% include 'hostutils/bs5/snippets/hostutils_nav_menu.htm' %}
+    ```
 
-Individual pages can also be linked directly:
+Alternatively, individual pages can linked directly:
 
 - Host overview page: 
 
     ```
     {% url 'hostutils:host_details' %}
     ```
```

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/forms.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/forms.py`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_partition_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_partition_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/urls.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/urls.py`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/views/__init__.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/views/ajax.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Union
+import psutil
 
 from django.http import HttpResponse
 from django.template import loader
 
 from handyhelpers.views.ajax import AjaxGetView
-
-import psutil
+from typing import Union
 
 
 class GetHostCpuStats(AjaxGetView):
     """
     Description:
         Get CPU status for a given cpu on the host machine.
     Args:
@@ -84,15 +83,15 @@
     Returns:
         HttpResponse: JSON formatted response.
     """
 
     template = loader.get_template("hostutils/bs5/ajax/get_process_stats.htm")
 
     def get(self, request, *args, **kwargs) -> HttpResponse:
-        self.data: Union[dict, psutil.Process]
+        self.data: Union[dict, psutil.Process] 
         try:
             proc = request.GET["client_response"]
             self.data = psutil.Process(int(proc))
         except psutil.AccessDenied:
             self.data = {}
         except Exception:
             return HttpResponse("Invalid request inputs", status=400)
```

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/views/gui.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/gui.py`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.2/src/djangoaddicts/hostutils/views/htmx.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/htmx.py`

 * *Files identical despite different names*

